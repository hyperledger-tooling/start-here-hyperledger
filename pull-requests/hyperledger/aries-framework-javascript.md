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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/561" class=".btn">#561</a>
            </td>
            <td>
                <b>
                    style: non-null assertions and newline import
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
        Created At 2021-12-02 15:16:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/560" class=".btn">#560</a>
            </td>
            <td>
                <b>
                    feat: add problem report protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Summary of Changes
Implemented the problem report [RFC-0035](https://github.com/hyperledger/aries-rfcs/blob/main/features/0035-report-problem/README.md)

Problem Report RFC effective for reporting of errors and warnings to other agents. Once this PR is merged agent will be able to report problems occurred in `Connection`, `Issue Credential`  & `Present Proof`

### Related Issue 
#58 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 13:43:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/559" class=".btn">#559</a>
            </td>
            <td>
                <b>
                    ci: create non-annotated tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

The ci created annotated tags which clashes with lerna. This PR makes sure we create non-annotated tags
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 11:06:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/558" class=".btn">#558</a>
            </td>
            <td>
                <b>
                    ci: create tag on alpha release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

@JamesKEbert I think this should do it. It will create a tag names `alpha.<number>` on each release. I think lerna search for the default `vX.X.X` prefix so should not cause any issues. 

Let's try!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 18:24:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/557" class=".btn">#557</a>
            </td>
            <td>
                <b>
                    feat: add question answer protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Added a question answer module (https://github.com/hyperledger/aries-rfcs/blob/main/features/0113-question-answer/README.md) to send and receive question messages and to send and receive answer messages with a valid response. 

# Pull Request Checklist

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Added **tests** for changed code (run `scripts/preflight` to run tests and check code style).
- [x] Prefixed code comments with GitHub nick and an appropriate prefix.
- [x] Coding style is consistent with the rest of the framework.
- [x] Updated **documentation** for changed code and new or modified features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 17:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    fix(core): expose record metadata types
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
        Created At 2021-12-01 08:57:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    fix: removed check for senderkey for connectionless exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Trinsic doesn't send the senderVerkey on a connectionless exchange.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 13:32:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/554" class=".btn">#554</a>
            </td>
            <td>
                <b>
                    feat: add generic did resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add generic did resolver. Implementation is based on the `did-resolver` library, but uses its own did method registry for a bit more flexiblity. Parsing logic is used from the `did-resolver` library and it is also possible to wrap `did-resolver` plugins (we do that for `web-did-resolver`.

Supports `did:sov`, `did:web`, `did:key`.

Usage:

```ts
// Module
const did = await agent.dids.resolve('did:web:trinsic.id')

// or service (need to have instance of the service, class is for example)
const did = await DidResolverService.resolve('did:web:trinsic.id')
```

The `did:key` implementation comes with a `DidKey` class that makes it easy to use for encoding public keys as `did:key` string.

```ts
const publicKeyBase58 = "xxxx" // publicKeyBase58 is same as verkey
const didKey = DidKey.fromPublicKeyBase58(publicKeyBase58, KeyType.ED25519)

const did = didKey.did // get did:key string
```


TODO: more tests and documentation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 16:03:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    ci: add continuous deployment scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds continuous deployment scripts for stable releases. We can now run a manual `workflow_dispatch` action on the `Continuous Integration` pipeline and it will create a PR for the next release. 

Once that PR is merged it will automatically tag, create a github release and release to NPM. This is in preparation for the 0.1.0 release I want to do.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-27 18:39:58 +0000 UTC
    </div>
</div>

