---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/660" class=".btn">#660</a>
            </td>
            <td>
                <b>
                    Fix configuration path for case-sensitive fs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">comp/samples</span>
            </td>
            <td>
                The client SDK needs to load the configuration file from the file
system. In this sample app we use the configurations provided in
fabric-samples/test-network. On a case-sensitive fs (Linux), the
constructed path (ccpPath) in this demo app is not correct. We fix
this by demo by using strings.ToLower as we know the path already.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>



**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
The problem is described in #656. This PR fixes the problem with simple-go.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 12:39:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    fabric-private-chaincode/samples/deployment/test-network/Readme.md bugs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">comp/samples</span>
            </td>
            <td>
                **What this PR does / why we need it**:
Fixes the test-network README so it works again ;)

**Which issue(s) this PR fixes**:
see [issue](https://github.com/hyperledger/fabric-private-chaincode/issues/656)

**Special notes for your reviewer**:
Thanks to  Marcus and Koshi for helping me solve my issues.

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:
I do not expect that to happen.

However, please whoever knows how the simple-go client works. Check out why it is breaking with the test-network.
I was not able to figure that out.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 15:57:17 +0000 UTC
    </div>
</div>

