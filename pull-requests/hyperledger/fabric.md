---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3077" class=".btn">#3077</a>
            </td>
            <td>
                <b>
                    peers iteration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature
- Documentation update

#### Description

Another iteration on the Peers topic for new Fabric Gateway service.

#### Related issues

https://github.com/hyperledger/fabric/issues/2807


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 23:46:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3075" class=".btn">#3075</a>
            </td>
            <td>
                <b>
                    Refine Gateway gRPC error status codes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 16:34:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3074" class=".btn">#3074</a>
            </td>
            <td>
                <b>
                    EndorsementTimeout should apply to each endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently the options.EndorsementTimeout creates a context that is shared by all endorsement requests in the Endose() and Evaluate() methods.
This commit changes it so It is applied individually to each endorsing peer.
The overall timeout for Endorse/Evaluate is set in the client SDK

Resolves https://github.com/hyperledger/fabric-gateway/issues/292

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 14:15:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3070" class=".btn">#3070</a>
            </td>
            <td>
                <b>
                    goimports updates to prepare for Go 1.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run goimports to make code compatible with Go 1.17.
The changes work with both Go 1.16 and Go 1.17, therefore it can be merged now.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-21 16:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3067" class=".btn">#3067</a>
            </td>
            <td>
                <b>
                    add http proxy support to core/chaincode/platforms
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: itaru2622 <itaru2622@gmail.com>

close #3066 

#### Type of change

- New feature

#### Description

add http proxy support to chaincode container build phase when fabric-peer container run with  "-e https_proxy=... " 
for details, refer #3066 

#### Additional details

when your devenv is located behind http proxy, additional no_proxy entries may be required to pass unit-test and integration-test.
the reasons is  described in #3066 and end of docs/sources/dev-setup/devenv.rst

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-21 08:05:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3065" class=".btn">#3065</a>
            </td>
            <td>
                <b>
                    Fix Issue #257 by including additional details on Kube Service routing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Documentation update

#### Description

This PR adds a brief summary of Kubernetes Service routing as a mechanism to implement basic HA / DR / connection load balancing to the Fabric Gateway. 

#### Additional details

A sample integration of the Kube routing is available in the Kubernetes Test Network [HA GUIDE](https://github.com/hyperledger/fabric-samples/blob/main/test-network-k8s/docs/HIGH_AVAILABILITY.md)

Kube test network updates to enable gateway client load balancing are available in [fabric-samples PR #532](https://github.com/hyperledger/fabric-samples/pull/532)
#### Related issues

Additional discussion, and the original issue, is tracked at [fabric-gateway issue #257](https://github.com/hyperledger/fabric-gateway/issues/257) 

Resolves #257

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 19:15:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3064" class=".btn">#3064</a>
            </td>
            <td>
                <b>
                    Reference current application APIs in peer event service docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #2807 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 17:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3062" class=".btn">#3062</a>
            </td>
            <td>
                <b>
                    Remove redundant SDK documentation page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This page is out of date, duplicates information in sdk_chaincode.rst, and does not fit well in the architecture section.

Contributes to #2807 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 15:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3061" class=".btn">#3061</a>
            </td>
            <td>
                <b>
                    Log the transactionID in all log messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/fabric-gateway/issues/303

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 13:29:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3060" class=".btn">#3060</a>
            </td>
            <td>
                <b>
                    Updates to endorser and gateway logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update endorser and gateway log levels to improve troubleshooting.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 21:07:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3059" class=".btn">#3059</a>
            </td>
            <td>
                <b>
                    Update protobuf definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Redundant `result` fields removed from gateway.EndorseResponse and gateway.PreparedTransaction.

Contributes to hyperledger/fabric-gateway#316
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 18:23:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3056" class=".btn">#3056</a>
            </td>
            <td>
                <b>
                    docs: fixing some typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

This change fixes some typos  in the docs

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 11:38:52 +0000 UTC
    </div>
</div>

