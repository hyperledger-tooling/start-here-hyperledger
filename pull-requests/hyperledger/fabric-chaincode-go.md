---
layout: default
title: fabric-chaincode-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-go
---

# fabric-chaincode-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Remove azure pipelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 15:26:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Add GHA support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add gh-actions workflow

Update the one formatting, two lint and failing tests assertion that prevents the build from completing

The assertion (assert.Equal) fixes should be a temporary solution as I believe we need to change the assertion library.
To the one used by the main fabric repo - as that seems to be able to cope with equality of TLSConfig structures.   The current one here doesn't cope with objects with functions.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 10:42:09 +0000 UTC
    </div>
</div>

