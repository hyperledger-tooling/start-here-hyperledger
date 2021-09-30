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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    Documentation and code readability improvements for HSM signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #227 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 09:44:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    Synchronize access to session in HSM signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PKCS#11 sessions cannot be used concurrently.

Resolves #227 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 16:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    Interfaces for ChaincodeEvent and Status in Java API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exposing concrete implementation classes that could not be instantiated by client code would make unit testing for client application code harder.

Resolves #224 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 15:59:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    Update Go API documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Async submit example
- Chaincode events example
- Modified off-line signing examples to demonstrate end-to-end flow
- Added examples of equivalent calls using alternative Contract methods
- Renamed some code examples to ensure they are associated with the correct methods
- Minor corrections to Java equivalent call examples
- Removed Node submit/submitAsync equivalent call examples as they are unnecessarily complex and used for different use-cases

Resolves #219 
Resolves #218 
Resolves #179 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 14:01:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Java API documentation updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Async submit example in Contract class doc
- Add equivalent call examples to Contract methods to help relate different API methods
- Chaincode events example in Network class doc
- Tidy-up of package-level code example
- Consistency of top-level description between Node and Java documentation

Resolves #215 
Resolves #216 
Contributes to #179 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 17:11:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/222" class=".btn">#222</a>
            </td>
            <td>
                <b>
                    Node API documentation updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Show printing of transaction results in top-level example
- Update async submit example to match current API
- Extended off-line signing example to cover complete flow
- Add equivalent call examples to Contract methods to help relate different API methods

Resolves #220 
Resolves #221 
Contributes to #179 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 13:14:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    Refactor commit status API to improve usability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minimise the number of potential error points that application code need to handle. Also minimise mutability within implementation.

Updated samples to reflect API change, which required samples to use the current development code.

Resolves #212
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 12:28:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Add tag to node module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Temporarily add the latest tag to nightly build publishing

This should be reverted when there are release builds!

Resolves #208

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 13:27:24 +0000 UTC
    </div>
</div>

