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
                PR <a href="https://github.com/hyperledger/fabric/pull/2978" class=".btn">#2978</a>
            </td>
            <td>
                <b>
                    Improve health checker docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add more details about health checkers, including ability
to not register Docker health checker if using
external chaincode builders.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 14:34:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2977" class=".btn">#2977</a>
            </td>
            <td>
                <b>
                    Update developer environment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

Improve the setting up dev environment section

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 09:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2975" class=".btn">#2975</a>
            </td>
            <td>
                <b>
                    Limit TestBlockPullerBadBlocks pullblock time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

#### Description
Testcase times out after 20 minutes as the client is not able
to connect to the server.  The rootcause for the server connection
failure is not known yet.  

BlockPuller provides an option to limit the retries to get the blocks
This will help here when the client failed to connect & fail the testcase
fast. This PR set the retries to 5 times. 

#### Related issues
#2835 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 12:45:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2974" class=".btn">#2974</a>
            </td>
            <td>
                <b>
                    Rename EndpointError to ErrorDetail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the gateway.proto, the EndpointError message has been renamed ErrorDetail.
This commit updates the proto dependency and renames the type in the gateway code.

Contributes to #2971 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 08:09:00 +0000 UTC
    </div>
</div>

