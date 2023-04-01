---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/423" class=".btn">#423</a>
            </td>
            <td>
                <b>
                    Remove all remaining mentions and code related to AoT wasm contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR completely removes any remaining documentation and code related to supporting AoT compiled wasm contracts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 00:51:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    Clean up 18.04 references
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses #381 .

A couple of references still persist in the proxy yaml files.
As detailed in those comments, once we improve the proxy handling, those files should become obsolete and be removed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 18:36:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    Overhaul Python package build and install
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does three things:
- [ ] Switches the build for the SWIG Python bindings to use the updated cmake build infra (WIP)
- [ ] Updates how the Python wheel is built
- [ ] Ships the built wheel and updates documentation for installation

**NOT TESTED YET**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 01:38:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    Split test scripts into a local unit test and one for services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Splits the test into two parts:
* unit test that requires no running services
* services test that verifies correct operation of eservice/pservice/sservice

The services test need not be run from the same host where the services are running.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 16:32:39 +0000 UTC
    </div>
</div>

