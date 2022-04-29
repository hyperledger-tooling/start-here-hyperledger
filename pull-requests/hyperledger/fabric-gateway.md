---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    Looser checks for required Node engines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Specify only the minimum required Node version, below which the code will not run. Allows more flexibility for consumers to pick a preferred Node runtime versions, including non-LTS versions. The documented supported versions still specify the Node versions tested and for which bugs will be addressed.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 12:38:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Use engine-strict to ensure compatibility with tested Node versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add an .npmrc so that `npm install` will fail during testing if any dependencies do not support the Node version used to run tests.

Also modify the Makefile so that targets executed in sub-directories correctly fail-fast rather than continuing to execute subsequent commands.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 10:00:34 +0000 UTC
    </div>
</div>

