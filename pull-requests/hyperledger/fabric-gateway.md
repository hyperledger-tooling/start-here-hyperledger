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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/163" class=".btn">#163</a>
            </td>
            <td>
                <b>
                    Remove references to tech preview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove references to gateway "tech preview", as well as
references to "alpha" and "beta" where possible, since
we expect gateway to work with all Fabric v2.4 releases and later.

Also cleanup duplicate sample content in the hsm sample page.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 14:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/162" class=".btn">#162</a>
            </td>
            <td>
                <b>
                    Update gateway sample readme with additional information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clean up instructions for v2.4.0-beta.
Add a description of the scenarios demonstrated in the sample client applications.
Minor cleanups to the scenario fixtures.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 05:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    Fix bad unit test for CommitStatus error in Go client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The error handling is also wrong and wasn't picked up because of the bad unit test.

Resolves #158
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 08:15:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/159" class=".btn">#159</a>
            </td>
            <td>
                <b>
                    Return gRPC errors directly in Go client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Avoid wrapping errors to allow client applications to interrogate gRPC status and additional details associated with the error.

Resolves #158
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 17:42:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    go hsm signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 09:37:58 +0000 UTC
    </div>
</div>

