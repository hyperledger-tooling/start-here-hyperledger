---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Allow interopcc to run in K8s as external service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added Dockerfile to build the image for interopcc.
2. Also moved protos build command in a script, which can be called by makefile as well as Dockerfile.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 16:11:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    app cc wrapper code implementing the interface functions in base class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 22:55:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    wrapper functions for fungible assets and base-class for non-fungible assets 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes consist of the following:

- Added non-fungible asset operations using contractId into base-class (i.e., asset_locks.go) and base-class contract (i.e., asset_locks_contract.go)
- Test cases for the changes of non-fungible asset operations (i.e., changes into asset_locks_test.go)
- Wrapper functions for the fungible/token assets (i.e., changes into assetmgmt.go)
- Refactoring of the base class code
- Minor edits to few other files

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-23 20:55:43 +0000 UTC
    </div>
</div>

