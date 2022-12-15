---
layout: default
title: fabric-test
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-test
---

# fabric-test <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-test){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    Revert temp pulling of binaries from 2.5-stable (main)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pull binaries from jfrog 'latest' instead of '2.5-stable' in main branch

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 17:50:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    Fix interop job publishing (main)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Don't build fabric-ca darwin binaries due to cross-compiling issues

2. Temporarily pull binaries from '2.5-stable' instead of 'latest' to get things working again. Later we'll switch the function tests to build instead of pull binaries.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 16:54:47 +0000 UTC
    </div>
</div>

