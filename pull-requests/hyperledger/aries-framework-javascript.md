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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1419" class=".btn">#1419</a>
            </td>
            <td>
                <b>
                    chore: update shared components libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 13:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1418" class=".btn">#1418</a>
            </td>
            <td>
                <b>
                    fix: remove `deleteOnFinish` and added documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix: removed deleteOnFinish
- Added small documentation to the function as well as the docs https://github.com/hyperledger/aries-javascript-docs/pull/111

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 13:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1417" class=".btn">#1417</a>
            </td>
            <td>
                <b>
                    feat: transaction endorsement draft
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 11:35:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1416" class=".btn">#1416</a>
            </td>
            <td>
                <b>
                    fix: various anoncreds revocation fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses several issues I've encountered while testing receiving and proving revocable anoncreds credentials with both the indy-sdk and the anoncreds rs libraries. 

I've moved some methods from the specific format classes anoncreds and legacy indy to util methods as the logic is quite complex and can easily be shared between the implementations. I think we should extract more logic into util methods that can be called by both format services.

There was an inconsistency with how the holder classes used timestamps. I've now updated the code to work the same and it's the responsiblity of the caller of `HolderService.createProof` to make sure it knows which timestamp of the revocation status list to use. 

Haven't tested verification of revocable credentials yes, and also haven't tested the final changes in React Native as there were enough issues to first solve in the shared AFJ code.

~~These changes are dependant on AnonCreds RS 0.1.0-dev.13, but for that we first need #1415 to be merged.~~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 13:39:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1415" class=".btn">#1415</a>
            </td>
            <td>
                <b>
                    refactor(anoncreds): master secret to link secret
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates `AnonCredsRsHolderService` according to the recent changes in `@hyperledger/anoncreds` API and applies transformations to credential request metadata (including migration script).

There is a test that is not passing, because anoncreds-rs expects the credential definition to have a `link_secret` field instead of the former/legacy `master_secret` field (this is according to this [test](https://github.com/hyperledger/anoncreds-rs/blob/1dd3f069de74b82569b0f782cfc071db8d856ace/src/data_types/cred_def.rs#L166) added recently by @blu3beri). 

From my understanding, we should still be tied to `master_secret` in this case but AnonCreds spec is not consistent about this: in [section 7.2.2](https://hyperledger.github.io/anoncreds-spec/#generating-a-credential-definition-without-revocation-support)., it first shows an example where link_secret is used (supposed to be based in an example in Sovrin MainNet which actually uses master_secret). And then, when describing all the fields within a Credential Definition, it states:

> master_secret (also known as [link secret](https://hyperledger.github.io/anoncreds-spec/#term:link-secret), but kept as master_secret for backwards compatibility)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 17:44:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1414" class=".btn">#1414</a>
            </td>
            <td>
                <b>
                    chore(askar-migration): move indy-sdk to dev deps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 14:49:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1413" class=".btn">#1413</a>
            </td>
            <td>
                <b>
                    feat: add message pickup module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR moves Message Pickup specific features into a separate module, rather than putting all together into Mediator and Recipient modules.

The idea behind this (besides making mediator/routing module more lightweight) is to start adding more advanced features to Message Pickup, for both recipient (e.g. be able to manage multiple message pickup loops) and message holder roles (e.g. support message pickup sessions in order to determine what to do with forwarded messages depending on Live mode status).

For the moment, it attempts to not introduce any breaking change at API level (other than renaming some message and handler classes that were previously exposed so somebody could have been referencing them externally).

`MessageRepository` API remains the same, although now it can be injected by using the `MessagePickupModuleConfig`, which would be the most revolutionary (?) addition from this PR from API perspective.

```typescript
new Agent({
      config,
      dependencies: agentDependencies,
      modules: {
         /* ... */
         messagePickup: new MessagePickupModule({ messageRepository: new CustomMessageRepository() }),
      }
})
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 21:14:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1412" class=".btn">#1412</a>
            </td>
            <td>
                <b>
                    fix: jsonld credential format identifier version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Fix the JSONLD_VC format string (it was missing a "v" character).

2. Remove the check credential proofType === request proofType. I believe this check is unnecessary (and always fails when testing with aca-py)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 13:47:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1411" class=".btn">#1411</a>
            </td>
            <td>
                <b>
                    chore(bbs-signatures): make module public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make @aries-framework/bbs-signatures public
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 11:14:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1409" class=".btn">#1409</a>
            </td>
            <td>
                <b>
                    fix: add reflect-metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Was causing issues if you first import anoncreds package and then core (which is the case when you order imports)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 16:23:11 +0000 UTC
    </div>
</div>

