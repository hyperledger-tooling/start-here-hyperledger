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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/661" class=".btn">#661</a>
            </td>
            <td>
                <b>
                    Add debug info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Bruno Vavala <bruno.vavala@intel.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 23:56:23 +0000 UTC
    </div>
</div>

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

