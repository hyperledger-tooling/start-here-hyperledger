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
                PR <a href="https://github.com/hyperledger/fabric/pull/3080" class=".btn">#3080</a>
            </td>
            <td>
                <b>
                    Other key concepts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature
- Documentation update

#### Description

Other Key Concepts - Network and Ordering Service topics for gateway

#### Related issues

https://github.com/hyperledger/fabric/issues/2807 
- Other Key Concepts items


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-27 23:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3079" class=".btn">#3079</a>
            </td>
            <td>
                <b>
                    Peers for Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

Final review of Peers page/topic for Fabric Gateway GA

#### Type of change

- New feature
- Documentation update

#### Description

Fabric Gateway service - new model for peers and apps for transaction proposals and endorsements.

#### Related issues

https://github.com/hyperledger/fabric/issues/2807

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-27 20:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3078" class=".btn">#3078</a>
            </td>
            <td>
                <b>
                    What's New for v2.4.0 doc topic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add What's New for v2.4.0

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 15:37:29 +0000 UTC
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

