---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2589" class=".btn">#2589</a>
            </td>
            <td>
                <b>
                    build(openapi): license presence check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Adds a custom check that ensures that all the properties of the
license object are specified (name, identifier, url).
2. Optimized the custom-check that verifies the opan API json specs so
that it ignores **/node_modules/ not just node_modules (meaning that it
was only excluding the root dir not all sub-dirs of the packages as well)

Fixes #490

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 00:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2588" class=".btn">#2588</a>
            </td>
            <td>
                <b>
                    test(test-geth-ledger): add test for test-geth-ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add tests for geth-test-ledger
- fix small errors in GethTestLedger class
    
Closes: #2579 
Depends on: #2577
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 15:41:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2587" class=".btn">#2587</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in example-carbon-accounting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2062
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 06:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2586" class=".btn">#2586</a>
            </td>
            <td>
                <b>
                    build(cmd-api-server): upgrade to Artillery v2.x or migrate to loadtest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2234
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 04:40:51 +0000 UTC
    </div>
</div>

