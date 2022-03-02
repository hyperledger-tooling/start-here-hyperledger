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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/663" class=".btn">#663</a>
            </td>
            <td>
                <b>
                    fix docs: Chaincode-as-a-service tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the followings to run the tutorial.
- Add an instruction to set PATH to call the `peer` command.
- Correct an option for `deployCCAAS` to debug Chaincode.

Signed-off-by: Yuki Kondo <yuki.kondo.ob@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 06:01:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/660" class=".btn">#660</a>
            </td>
            <td>
                <b>
                    Update test network to fabric 2.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 11:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    Remove duplicate erc-721 Go chaincode sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                erc-721 Go chaincode was delivered to both /go and /chaincode-go directories.
This commit removes the /go implementation.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 07:29:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    Fix ledger queries sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                -Go chaincode - Paginated range query should return the bookmark so that next page can be requested
-Javascript chaincode - Make query return JSON consistent with Go chaincode
-Javascript app was broken at bookmark query due to invalid JSON parsing from inconsistent chaincode responses
-Javascript and Java app had incorrect comments

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 06:46:15 +0000 UTC
    </div>
</div>

