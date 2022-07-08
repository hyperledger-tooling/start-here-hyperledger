---
layout: default
title: fabric-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operator
---

# fabric-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    bump sample network to use fabric CA v1.5.5
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
        Created At 2022-07-08 11:45:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Feature/net operator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces a new action `network operator` which will launch only the operator in the target k8s namespace. 

In addition, this bumps the k8s-builder revision to v0.6.0. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 15:23:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    upgrade test cases to ginkgo v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                upgrade test cases to ginkgo v2

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-02 11:09:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    prometheus operator support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                scope for integration fabric-operator with prometheus operator.
- [x] add unit test case for prometheus metric provider in configoverride
- [ ] add test for prometheus for use prometheus and export operator ports together
- [ ] add define in peer and orderer as prometheus operator
- [ ] implementation prometheus operator for peer and orderer
- [ ] add unit test case for service monitor? do we use service?
- [ ] add CI test case with prometheus operator

additional founding
1.  doc update
2. ginkgo update in #22 


Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 14:12:14 +0000 UTC
    </div>
</div>

