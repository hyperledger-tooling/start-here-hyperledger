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
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Bump fabric and fabric-ca version in integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump fabric and fabric-ca version in integration tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 17:02:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    Bump fabric, fabric-ca, fabric-lib-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update to the latest fabric (v2.5.9), fabric-ca, and fabric-lib-go.
These versions all depend on the same version of github.com/IBM/idemix and
resolves issues related to breaking changes in github.com/IBM/idemix.
    
Note that the fabric dependency is now on the release-2.5 branch rather than main branch,
which is why one of the function calls needed to be updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 16:39:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.22.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.22.5.
Latest Go also requires an update to controller-gen (otherwise it panics with a nil pointer).
The controller-gen update in turn improves formatting of the generated CRD yaml files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 16:11:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/198" class=".btn">#198</a>
            </td>
            <td>
                <b>
                    Use ubi-minimal image instead of ubi go-toolset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                go-toolset doesn't have the latest versions of Go.
Therefore use the ubi minimal image and install our preferred version of Go when building operator.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 03:40:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.21.11.
Note that starting with Go 1.21, the version in go.mod should be 3 digits.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 19:17:21 +0000 UTC
    </div>
</div>

