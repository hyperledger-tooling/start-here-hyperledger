---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    Fix asset-transfer-events sample Java chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - chaincode-java Gradle project name did not match the instructions or the chaincode name used by the sample application code.
- Added test of Java chaincode to CI pipeline.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 10:47:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    Update secured asset transfer sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A recent commit added the potential buyer to an asset's state based endorsement policy.
That change was problematic because if the transfer fell through, the buyer lost control of the asset,
in that they could no longer update the asset or change the sell price or sell to somebody else.

The asset state based endorsement policy is now based on the seller only, and we document
that additional parties could be added such as a trusted third party (although no
such party exists in test network at this time).

This commit also re-adds some necessary verifications, and make other minor edits and
comments to help users understand the sample.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 11:39:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/779" class=".btn">#779</a>
            </td>
            <td>
                <b>
                    Update Gateway samples for v1.1 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated build to use Go 1.18 since Go 1.16 is no longer supported.
- Use Java 11 in updated samples, and take advantage of new language features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-26 13:52:37 +0000 UTC
    </div>
</div>

