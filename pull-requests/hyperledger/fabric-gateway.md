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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Reinstate nightly publishing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Old node module has been deprecated so can remove that step from ci and
switch back to nightly publishing

Signed-off-by: James Taylor <jamest@uk.ibm.com>

Contributes to #209 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 18:06:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Deprecate old node module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previous deprecation failed with `422 Unprocessable Entity` which should be
fixed in npm v7

Signed-off-by: James Taylor <jamest@uk.ibm.com>

Contributes to #209 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 17:14:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Rename node module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename fabric-gateway module to scoped @hyperledger/fabric-gateway

Also deprecates existing published fabric-gateway module

Signed-off-by: James Taylor <jamest@uk.ibm.com>

Contributes to #209 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 16:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    Default gRPC call timeouts for Go API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated samples to demonstrate setting default timeouts.
- Removed async submit example for HSM samples since this duplicates main samples and keeping them simple makes it easier to see the HSM-specific aspects.

Contributes to #198 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 15:52:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Fix scenario tests for latest fabric updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes in fabric gateway relating to evaluate retry logic and error message text have broken some of the error scenario tests.  This commit fixes them.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 14:43:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Timeouts for Go API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed chaincode events default call options from samples since it makes little sense to set an arbitrary timeout on a streaming call.

Contributes to #198 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 12:22:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    Node API documentation improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Examples of default call timeouts.
- Simplify Node gRPC client constructor examples.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 13:01:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    Dynamic load of optional pkcs11js dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevents this dependency being loaded unless an HSM signer is actually created, avoiding runtime issues on systems that do not have the optional pkcs11js dependency available.

Resolves #252 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 09:54:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    Allow setting default call options for Node client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also update samples to demonstrate default timeouts.

Contributes to #198 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 10:58:34 +0000 UTC
    </div>
</div>

