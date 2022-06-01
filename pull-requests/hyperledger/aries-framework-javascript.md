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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    feat: present proof v2 Indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Worked on Present Proof V2 to work with Indy credentials
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 11:49:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    docs: add ios ledger troubleshooting information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These docs address issues found with multiple ledgers in iOS release environments found in #647. The solutions present in the docs have been tested in Bifold [PR #336](https://github.com/hyperledger/aries-mobile-agent-react-native/pull/336).


Other contributors who assisted: @reflectivedevelopment, @TheTreek, @amanji
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 19:35:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/803" class=".btn">#803</a>
            </td>
            <td>
                <b>
                    fix(indy): async ledger connection issues on iOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Waiting on Author</span>
            </td>
            <td>
                Change `connectToPools` function to sequentially connect to pools. Previously there were [issues on iOS](https://github.com/hyperledger/aries-framework-javascript/issues/647) because of too many open sockets on this function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 19:25:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/801" class=".btn">#801</a>
            </td>
            <td>
                <b>
                    refactor: move signatures suites to vc module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the signature suites, the jsonld util and other files to the vc module. This will help with the separation of credential formats we're going to look at soon. It also fixes an issue with type files being places outside of the src directory causing build issues. We didn't catch this because CI was not enabled on the 0.3.0 branch. CI is now enabled which gives us more assurance when merging PRs.

This doesn't change anything about the functionality. It's just relocation, and fixing of type issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 09:51:48 +0000 UTC
    </div>
</div>

