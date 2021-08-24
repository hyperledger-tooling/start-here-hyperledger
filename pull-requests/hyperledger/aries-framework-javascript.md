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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/437" class=".btn">#437</a>
            </td>
            <td>
                <b>
                    TSDoc linting + API docs for mediation module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains API doc comments with the intent they can be used in the future to generate documentation.  To keep with the code quality standards I have added TSDoc linting. I believe this aligns with AFJ code quality goals and opens up the opportunity to generate documents from source code comments, which has been a topic of discussion in the community in the past.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 19:28:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    fix: their did doc not ours
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Type: Bug</span>
            </td>
            <td>
                Was filtering based on our did doc, not theirs....
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 21:18:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/434" class=".btn">#434</a>
            </td>
            <td>
                <b>
                    Alter mediation recipient websocket transport priority
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Alters the mediationRecipient to properly indicate the priority for using Websockets when doing implicit mediation. 
Updated `@aries-framework/react-native` to include buffer as a peer dependency to allow for processing and sending of messages via websockets in React Native, updated docs to reflect this.

@burdettadam assisted on this as well :) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 01:01:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/433" class=".btn">#433</a>
            </td>
            <td>
                <b>
                    feat: add multiple inbound transports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add support for multiple inbound transports
- rename all occurrences of transporter to transport
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 09:59:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    fix: mediator updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - extract logic for implicit pickup from websocket transport to mediation module
	-  This will make it easier to move to implicit pickup of non-websocket transports
- add test for restarting recipient agent
- add timeout to return when is connected
- fix issue where services were not reassigned after sorting or filtering
- add persistence for mediator routing keys
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 08:23:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    feat: add from record method to cred preview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two api improvements
1. register credential definition doesn't require `signatureType` parameter anymore (just add bloat to the API)
2. add `fromRecord` method to credential preview to be able to create a preview from json object. this makes it a lot simpler:


Before 

```ts
const credentialPreview = new CredentialPreview({
  attributes: [
    new CredentialPreviewAttribute({
      name: 'name',
      mimeType: 'text/plain',
      value: 'John',
    }),
    new CredentialPreviewAttribute({
      name: 'age',
      mimeType: 'text/plain',
      value: '99',
    }),
  ],
})
```

After

```ts
const credentialPreview = CredentialPreview.fromRecord({
  name: 'John',
  age: '99',
})
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 15:00:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/426" class=".btn">#426</a>
            </td>
            <td>
                <b>
                    fix: date parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Added transform function for parsing dates from multiple formats. Added transform function to basic messaging.

# Related Issues

N/A

# Pull Request Checklist

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Added **tests** for changed code (run `scripts/preflight` to run tests and check code style).
- [x] Prefixed code comments with GitHub nick and an appropriate prefix.
- [x] Coding style is consistent with the rest of the framework.
- [x] Updated **documentation** for changed code and new or modified features.

_PR template adapted from the Python attrs project._
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 16:51:37 +0000 UTC
    </div>
</div>

