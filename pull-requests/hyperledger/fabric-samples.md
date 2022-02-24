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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    refactor folder structure to match other token samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                hey @mbwhite whenever you had a moment, this is just a refactor of folder structure request by the community so that it matches the same structure as other token samples. Thanks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-19 15:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    impl for couchdb supports in test0network8s as hardcode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                a impl for #633

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-19 12:10:15 +0000 UTC
    </div>
</div>

