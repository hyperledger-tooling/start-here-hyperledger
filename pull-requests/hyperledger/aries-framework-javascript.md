---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1427" class=".btn">#1427</a>
            </td>
            <td>
                <b>
                    feat(anoncreds): issue revocable credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes some initial work done for supporting the issuance of revocable AnonCreds credentials in AFJ. 

**Brief summary of the changes:**

- Update of `AnonCredsRegistry` and `AnonCredsIssuerService` interfaces to add registration of revocation registry definitions and revocation status lists 
- AnonCreds module, through its `AnonCredsApi`, now allows to register these objects and update revocation status lists
- `AnonCredsCredentialFormatService` has been updated to handle accept revocable credential requests, retrieving an active Revocation Registry Definition and assigning an index to the credential that is going to be issued (this logic is not completely done yet though)
- Credentials module allows to send revocation notification for both `indy-anoncreds` and a potentially new `anoncreds` revocation format. This is very basic right now and needs some more work to support future formats and get information directly from the credential record to be more aligned with other modules API.
- AnonCreds module now has some new configuration items for object creation. In particular it adds the new `TailsFileService`, which is an interface for downloading and uploading tails files. The default implementation works as right now (only allows to download files), while a custom one can be used to upload files to any chosen tails server. In `samples` directory there is an example of tails server and service interface (not sure if they belong there but for the moment didn't find a better place). For the tests there is a dummy implementation that allows us to run them without the need of having an actual HTTP server

**Flow:**

For the moment, as seen in the few tests added in anoncreds-rs package, all VDR objects are managed exclusively from AnonCreds API and created/registered separately in order to have a simpler state management. For instance, if we want to create a revocable credential definition, we'd need to call:
- registerSchema
- registerCredentialDefinition
- registerRevocationRegistryDefinition
- registerRevocationStatusList

The only step that does two actions atomically is `registerRevocationRegistryDefinition`, as it will attempt to successfully uploading the tails file before registering the object in the VDR (this is mandatory because we may not know upfront what's the publicly available tails location).

To revoke a credential (or a number of credentials), `AnonCredsApi.updateRevocationStatusList()` must be called using the revocation registry definition id and credential indexes as an input.  If we want to notify the holder/s about this revocation, we must use Credentials API afterwards.

**Some notes/missing pieces**

- In this PR there is only a generic implementation using `InMemoryAnonCredsRegistry`. There is not yet any implementation for Indy VDR or Indy SDK
- It could feel more 'natural ' if we add a method called `revokeCredentials` in `CredentialsApi` that does both the revocation state update and send notification. However, this integration would need us to deal with the different credential formats and, after all, I'm not sure if it will be really useful in real world scenarios, because I think that usually an issuer would prefer to revoke multiple credentials at once (to avoid creating lots of ledger updates)
- In terms of agent storage, there are no specific changes to mark credentials as revoked and to store more information about credential revocation identification from the issuer side. I think it could be useful to find a good place to do so within AFJ model
- For the moment it depends on some fixes in anoncreds-rs (https://github.com/hyperledger/anoncreds-rs/pull/186, https://github.com/hyperledger/anoncreds-rs/pull/188 and probably something else with the timestamps that I'll need to debug more).
- Sorry for the monster PR!


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 22:51:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1422" class=".btn">#1422</a>
            </td>
            <td>
                <b>
                    fix(anoncreds-rs): revocation status list as JSON
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now that anoncreds-rs exposes revocation status list from JSON, there should not need in `AnonCredsRsVerifierService` to recreate an object, so here we pass it directly as JSON.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 13:49:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1421" class=".btn">#1421</a>
            </td>
            <td>
                <b>
                    fix: make revocation status list inline with the spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 12:15:33 +0000 UTC
    </div>
</div>

