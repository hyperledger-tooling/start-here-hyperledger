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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/834" class=".btn">#834</a>
            </td>
            <td>
                <b>
                    fix(oob): expose parseinvitation publicly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Quite a nice function to have outside of the framework for parsing qrcodes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-03 11:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/833" class=".btn">#833</a>
            </td>
            <td>
                <b>
                    fix: clone record before emitting event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clone records before emitting them in events to avoid mutation later on. 

Fixes #832 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 19:02:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    feat: support advanced wallet query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for some of the most important wallet query features as defined by the indy-sdk (and aries-askar). https://hyperledger-indy.readthedocs.io/projects/sdk/en/latest/docs/design/011-wallet-query-language/README.html

Currently only added support for `$and`, `$or` and `$not`, which is enough for most use cases. We need this in particular for querying credentials based on a DIF presentation definition. 

Fixes https://github.com/hyperledger/aries-framework-javascript/issues/739

@blu3beri I just used the default syntax for this, so you'd use it like this:

```ts
const query: Query<TheRecord> = {
  $and: [
	{ $or: [{ expandedTypes: 'https://url1.com' }, { context: 'https://url1.com' }] },
	{ $or: [{ expandedTypes: 'https://url2.com' }, { context: 'https://url2.com' }] },
  ]
}
```

We can look at a builder, but not sure what that would look like exactly? 

@NB-PrasadKatkar this should unblock you for the presentation exchange work
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 16:30:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    WIP: feat: wip add validation to JSON transformer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP

closes #742 
Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 13:23:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    refactor: Reuse cred def id and attributes from Proposal message in Indy Format Service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See Issue #837 https://github.com/hyperledger/aries-framework-javascript/issues/827
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 12:27:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    fix(oob): export messages in oob
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed that the `OutofBandInvitation` was not exported to the public and it can be quite useful to have

- Exported the `messages` folder inside the `oob` module
- There might be more items we want to export from here, but I am not too sure about which.

Signed-off-by: Berend Sliedrecht <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 12:25:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    fix: process ws return route messages serially
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We were already processing messages serially for pickup v1 and v2. This pr updates to also use this for websocket inbound transport. This can help prevent some race conditions and is consistent with the other pickup approaches
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 15:53:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    fix(oob): legacy invitation with multiple endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                more issues with interop testing in AATH.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 15:00:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    docs: using postgres storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added documentation for usage and setup of Postgres plugin setup
- [x] Linux
- [x] Mac
- [ ] Windows (Not able to build Postgres plugin on windows yet, getting an error regarding **libsodium-sys 0.0.16** )

#758 #771 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 13:37:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    fix(connections): didexchange to connection state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                small issue I discovered in updating AATH
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 13:20:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/819" class=".btn">#819</a>
            </td>
            <td>
                <b>
                    refactor(credentials): separate offer interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to avoid having connection and connection id in the same object and be able to remove protocol version
from the accept proposal / create offer functionality
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 09:32:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    merge main into 0.3.0-pre
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
        Created At 2022-05-31 05:55:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    fix(credentials): default for credentials in exchange record
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
        Created At 2022-05-31 05:48:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/815" class=".btn">#815</a>
            </td>
            <td>
                <b>
                    docs: add ontario copyright license
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mostafa <mostafa.youssef@ontario.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 02:55:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/814" class=".btn">#814</a>
            </td>
            <td>
                <b>
                    fix(oob): check service is string instance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Adds a check whether the service is instanceof String as mentioned in  #812. this is needed due to the class-validator logic sadly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-30 11:15:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/813" class=".btn">#813</a>
            </td>
            <td>
                <b>
                    fix(core): allow JSON as input for indy attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Right now, you have to create an instance of the class `CredentialPreviewAttribute` in the public API, like so:

```typescript
const attribute = new CredentialPreview({name: 'foo', value: 'bar'})
```

This PR will still allow for this but it is extended to also include:

```typescript
const attribute = { name: 'foo', value: 'bar' }
```

And it will tranform this into a class instance.

The reason for this PR is that is very weird for a public API to accept a class that only adds a `toJSON` method.

(I did not pickup the proofs module, as V2 is not merged and we can include it in there or I will pick it up after the merge).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-30 11:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/808" class=".btn">#808</a>
            </td>
            <td>
                <b>
                    fix(routing): also use pickup strategy from config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes #807 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 14:11:46 +0000 UTC
    </div>
</div>

