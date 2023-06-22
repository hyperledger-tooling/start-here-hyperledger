---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2276" class=".btn">#2276</a>
            </td>
            <td>
                <b>
                    feat: add anoncreds interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                And use it in Issue Credential v2 and Present Proof v2.

This PR supersedes #2191. As compared to #2191, this PR includes the required changes to use revocation with the generic anoncreds interface. Additionally, I've cleaned up this branch quite a bit. We had some unsuccessful detours (led by me lol) that resulted in both a messy history and changes in places that didn't need changes in the end.

Due to the need to clean up history, the contributions of my collaborators have unfortunately been obscured. Thank you @burdettadam and @cjhowland for all of your work on this!

As discussed with @swcurran, the intent of this PR is to have it merged to a feature branch (as in not merged to main) and for work to continue on the feature branch. I will create a number of issues reflecting things we hadn't gotten to yet or explicitly set aside for later as well as calling out discoveries that warrant further discussion.

Here is a brief summary of the changes that are included in this PR:

## Changes
### Added AnonCreds Registry and plugin interface
- This is a generic AnonCreds registry interface. It defines a registrar and resolver abstract base class which are to be implemented by plugins. The plugged in resolvers and registrars are then registered with the main registry interface which selects the appropriate resolver/registrar for a given identifier and operation.
- Interface found in `aries_cloudagent.anoncreds.registry`
- ABCs found in `aries_cloudagent.anoncreds.base`
- Associated models for generic representations of schemas, cred defs, and revocation artifacts found in `aries_cloudagent.anoncreds.models`

### Added default registry for "legacy indy"
- Found in `aries_cloudagent.anoncreds.default.legacy_indy`
- Uses the `aries_cloudagent.ledger` to send transactions to indy networks.
- Does NOT support endorsement protocol flow.

### Added stubs for did:web and did:indy
- These reside alongside the `legacy_indy` registry but are just stubbed out for now.

### Added AnonCreds Issuer, Verifier, and Holder interfaces
- Found in `aries_cloudagent.anoncreds.{issuer,verifier,holder}`
- These are very similar to but different from the original `IndyIssuer`, `IndyVerifier` and `IndyHolder` interfaces that existed previously.
- The role of these interfaces has expanded slightly, especially for Issuer, to better abstract the details of credential artifact registration and creation when using the generic anoncreds interface.

### Added AnonCreds Revocation interface
- Found in `aries_cloudagent.anoncreds.revocation`
- This is intended to replace several components: `IssuerRevRegRecord`, `RevocationRegistry`, and `IndyRevocation`.
- The components it replaces remain in place until all responsibilities have been moved.
- There was an unfortunate amount of conceptual overlap between these components. On top of this, their responsibilities were confused over time, resulting in models/records doing more than the probably should have.
- Implements a `create_credential` method similar to `AnonCredsIssuer.create_credential`. The issuer version supports credentials for cred defs that do not support revocation. The revocation version supports credentials for cred defs that do support revocation. The separation results in a cleaner implementation on both sides and cleaner split in responsibilities.

### Update Issue Credential v2 indy format handler to use AnonCreds interface
- Generally only minor tweaks with the exception of a cleaned up `issue_credential`; previously, this method made calls directly to the ledger with Indy specific revocation details being handled at this layer. These details have been moved down the stack to `AnonCredsRevocation.create_credential`.

### Update Present Proof v2 indy format handler to use AnonCreds interface
- Generally minor tweaks.

### Update Revocation Manager
- This component bridges the gap between protocol records and `IssuerCredRevRecord`s and AnonCreds details.
- Updated revoke and publish methods to use the generic interface.
- There remains some Indy-isms in `update_rev_reg_revoked_state`. I believe this can be translated to a more generic operation but I haven't had a chance to take a closer look at the revocation recovery pieces yet.

### Added AnonCredsTailsServer and updated BaseTailsServer
- In order to publish a tails file to the tails server, we have to take a different tactic due to when rev reg def ids are available and opportunities for invalid URL values to be in the rev reg def id. Now, we upload by hash instead of rev reg id.
- We have a branch on our fork of indy tails server that implements the new endpoint: https://github.com/Indicio-tech/indy-tails-server/tree/fix/put-get-file-backwards-compat

### Added Admin endpoints for AnonCreds operations
```
post /anoncreds/schema
get /anoncreds/schema/{schemaId}
get /anoncreds/schemas
post /anoncreds/credential-definition
get /anoncreds/credential-definition/{cred_def_id}
get /anoncreds/credential-definitions
post /anoncreds/revocation-registry-definition
post /anoncreds/revocation-list
put /anoncreds/registry/{rev_reg_id}/tails-file
put /anoncreds/registry/{rev_reg_id}/active
post /anoncreds/revoke
post /anoncreds/publish-revocations
```
- These behave more or less as expected when compared to `/schemas`, `/credential-definitions`, `/revocation/*`, etc.
- This is currently the only flow supported. Automated setup flow is in the works.

### Updated `BaseLedger` to behave as needed for the legacy indy registry
- The ledger implementation previously did some funky stuff with passed in `IndyIssuer` to both create and publish anoncreds artifacts. The responsibility of the ledger has been reduced to only publishing.
- These changes were implemented destructively but don't have to be if we want to better support backwards compatibility of Indy specific components.
- Some improvements were made to error handling to clean up the flow of some methods (see `aries_cloudagent.ledger.error`)

### Updates to Dockerfiles, requirements, setup to add anoncreds dep
- Currently pulling directly from git repo since no package is published to PyPI yet
- Binary also pulled from github releases page

## Notably missing changes
- Issue Credential v1 and Present Proof v1 implementation has not been updated
- Old endpoints are still present but are in various states of functional; these will either need to be deprecated or adapted
- Removal of deprecated components like `IssuerRevRegRecord`; we need a migration plan here, too
- There are some shortcomings in link secret handling as caused by the anoncreds library not accepting a memory view (see https://github.com/hyperledger/anoncreds-rs/issues/202#issuecomment-1581415680)
- Additional rearranging of components like `aries_cloudagent.ledger`; several should be moved to somewhere in `anoncreds.default.indy` or similar
- Models for portions of AnonCreds credentials are still defined in `aries_cloudagent.indy` -- moving these components was omitted for a cleaner set of changes in this PR (not moving these reduced the number of lines changed by half)
- In general, backwards compatibility with previously created anoncreds objects. Holder and verifier roles are likely fine but Issuer will need a migration plan.
- Updates to tests. Sorry :grimacing: -- we have been testing using an integration style test that calls the added admin API endpoints. I have not included these tests in this PR for the sake of cleanliness. I uploaded the test as a gist here: https://gist.github.com/dbluhm/4d33d8946d23dbaced9be825c49a9d5c
- Automated setup of revocation artifacts -- I have some WIP but opted to hurry up and open this PR rather than wait for me to finish.
- did:indy and did:web implementations
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 17:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2273" class=".btn">#2273</a>
            </td>
            <td>
                <b>
                    Add replacement_id to API.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                create/create-offer, send/send-offer now have replacement_id in the POST body to set the id

Addresses #2218

`replacement_id` for [RFC-0453](https://github.com/hyperledger/aries-rfcs/tree/main/features/0453-issue-credential-v2) was half implemented, just needed to expose it to the API for the issuer to set the value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 00:46:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2272" class=".btn">#2272</a>
            </td>
            <td>
                <b>
                    Minor revisions to the README.md and DevReadMe.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 19:22:56 +0000 UTC
    </div>
</div>

