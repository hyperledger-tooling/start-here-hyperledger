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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    Use maven central for gateway client dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the release-1.4 commercial paper client applications to pull the gateway jars from Maven central.

This PR supersedes PR #585 (abandoned / closed) 
    
Signed-off-by: lyd <luoyaodong98@gmail.com>

Co-authored-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 14:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Remove kubectl binary (again)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since kubectl binary is mistakenly added again in PR #714, this patch removes it.

It seems that the following commit was mixed up with another PR commits, including PR #713.
https://github.com/hyperledger/fabric-samples/pull/714/commits/24c296c8a8e6966595c6395bcc4ba9948217176a
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 02:15:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Remove kubectl binary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR#713, I mistakenly added kubectl binary, so this patch removes it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 08:35:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Some minor improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch includes some minor improvements, such as:
- Fix typos and broken links
- Correct chaincode type of asset-transfer-basic-debug
  (seems it should be ccaas)

Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 07:38:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Can implement a simple CURD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Leave the serialization of parameters to the upper level

Signed-off-by: D <gvssimux@qq.com>

Co-authored-by: D <gvssimux@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 02:43:35 +0000 UTC
    </div>
</div>

