---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    Basic implementation of did:web resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ci</span>
            </td>
            <td>
                Implementation of the `did:web` DID method resolver.

https://w3c-ccg.github.io/did-method-web
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 14:41:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    Do not run libvcx publishing from fork PRs
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
        Created At 2023-05-03 14:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                     move common stuff from the messages crate to shared_vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #821 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 13:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    Cleanup/ffi leftovers
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
        Created At 2023-05-02 15:31:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    Fix setting txn author agreement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - 0.55.0 release contained bug that transaction author agreement doesn't get set up in global settings state of aries-vcx-core, therefore ledger writes doesn't work for indy ledgers which require transaction author agreement
- this fixes the issue
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 14:58:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    Refactor of the iOS CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This refactor aims to improve the CI speed of the iOS build by removing unnecessary targets and vendoring our own build scripts for the libsodium and zeromq libraries (to avoid some unnecessary operations from the previous scripts).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 12:34:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    remove all feature flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to implement changes suggested here:
https://github.com/hyperledger/aries-vcx/pull/797#pullrequestreview-1379809296.
Fixes #799 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 15:53:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/817" class=".btn">#817</a>
            </td>
            <td>
                <b>
                    Unit test for enum SerializableObjectWithState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: https://github.com/hyperledger/aries-vcx/issues/774
Add unit test for serialization and deserialization of enum SerializeableObjectWithState.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-30 16:45:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    Fix README for deprecated link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `libvcx` is deprecated, the docs need to reflect that. The link in the docs to the deprecation notice seems to be broken. This PR fixes that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 12:47:09 +0000 UTC
    </div>
</div>

