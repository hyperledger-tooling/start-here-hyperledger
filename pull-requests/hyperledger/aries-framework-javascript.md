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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/849" class=".btn">#849</a>
            </td>
            <td>
                <b>
                    feat: wip add choice for taa mechanism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                todos:
* tests
* ensure this is complete and correct

Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 11:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/848" class=".btn">#848</a>
            </td>
            <td>
                <b>
                    fix(proof): allow duplicates in proof attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a partial fix for https://github.com/hyperledger/aries-framework-javascript/issues/837
The check is limited to duplicates between predicates and attributes only. Duplicit attributes should be allowed as they don't cause any error during proof creation.
Still todo: Either
* parse and validate based on `restrictions`, whether the items collide or not
or
* completely rethink the check and validate only at the point of `ProofsModule.acceptRequest` (which is the actual problem)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 13:58:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    docs(samples): fix extension module sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 10:51:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    docs: remove signed off by lines from changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 09:36:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/845" class=".btn">#845</a>
            </td>
            <td>
                <b>
                    refactor: adds custom rxjs operator to filter record events by record type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds custom rxjs operator to filter record events by record type. To be used in hooks extension.

Signed-off-by: Akiff Manji <akiff.manji@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 21:52:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    chore(migration): add credentials migration script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds migration script for updating credential records to 0.2.0 structure. 

Fixes #738
Supersedes #843 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 20:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    feat(core): generic repository events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #723 

Added generic `RecordSavedEvent`, `RecordUpdatedEvent`, and `RecordDeletedEvent` emitted from `Repository`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 15:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/841" class=".btn">#841</a>
            </td>
            <td>
                <b>
                    refactor(credentials): generic credentials module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR overhauls the credentials module to make it ready for modularization. This PR became a lot bigger than anticipated, but it are mostly consistency and cosmetic changes that don't change the behaviour. It also doesn't change the public api of the agent, except for a few interface fixes (e.g. removing a property that shouldn't have been exposed in the first place)

Main item addressed in this PR:

### Dynamic Interfaces for credential formats

Instead of creating interfaces for each method defining the supported credential formats.

```ts
interface ProposeCredentialOptions {
  credentialFormats: {
    indy: IndyProposePayload
  }
}
```

We can now dynamically configure the services and credential formats. This will make it possible to extract the formats and services out of core while still keeping a fully typed interface.

You can declare which services and formats you use like this (currently not needed as it has defaults, this will later be automatically detected based on your agent configuration):


```ts
// v1 and v2 for indy
CredentialsModule<[IndyCredentialFormatService], [V1CredentialService, V2CredentialService]>
```

Now when I use the agent it will restrict which protocol versions I can use and which credentialFormats

```ts
agent.credentials.proposeCredentials({
  /* other options */
  protocolVersion: 'v3' // will error
  credentialFormats: {
    // indy is allowed and will have typing because we registered the interface.
    indy: {
    }
  }
})
```

So even though everything is still in core, it's fullly decoupled now.

You define a format like this:

```ts
export interface IndyCredentialFormat extends CredentialFormat {
  formatKey: 'indy'
  credentialRecordType: 'indy'
  credentialFormats: {
    createProposal: IndyProposeCredentialFormat
    acceptProposal: IndyAcceptProposalFormat
    createOffer: IndyOfferCredentialFormat
    acceptOffer: IndyAcceptOfferFormat
    createRequest: never // cannot start from createRequest
    acceptRequest: Record<string, never> // empty object
    createCredential: IndyIssueCredentialFormat
  }
}
```

To make sure this won't cause issues with extensions later on I've extended the api a bit to make a bit more generic and less focused on the indy use case (adding interface method we don't need right now).

In addition I made some smaller changes:
- Remove `CredentialProtocolVersion`. You now need to use string values. Because we can dynamically register new versions, an enum doesn't really work.
- move all indy related models to the indy format directory
- create separate interfaces for each method in the module, service and format service. The interfaces were reused between layers, which helps with duplication, but makes consistency and overview harder. This will also help with separating into multiple packages and will keep us sharper on responsiblity of each layer.
- order all methods in the module,service,format service based on the public/private interface order and the topic order (group all proposal methods at top, then all offer methods, etc..).
- removed requirement to pass values to accept methods (this should 
- removed all places where we modify the input options object to pass to a lower serivce. Options are now always unique.
- move all tests to the correct folder (v1 and v2 tests were being mixed in the v1 and v2 directories)
- extract revocation notification into separate revocation-notification protocol directory.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 22:02:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/840" class=".btn">#840</a>
            </td>
            <td>
                <b>
                    Feature/shortenedUrl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for attempting to parse a URL as a shortened URL after failing to parse a URL normally, This follows the most recent changes to the [`out-of-band` rfc](https://github.com/hyperledger/aries-rfcs/tree/main/features/0434-outofband) with the known caveats involved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 18:16:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/839" class=".btn">#839</a>
            </td>
            <td>
                <b>
                    fix(oob): expose oob record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Berend Sliedrecht <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 14:43:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    fix: send message to service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed issue where message sender would incorrectly return early from loop (inside `sendMessage`) even if service was unable to be satisfied by outbound transports.

Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 15:24:47 +0000 UTC
    </div>
</div>

