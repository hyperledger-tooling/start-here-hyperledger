---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1302" class=".btn">#1302</a>
            </td>
            <td>
                <b>
                    vNext: Added documentation for the new Peer Gateway connector in the Fabric configuration and Runtime configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added documentation in the Fabric and Runtime configuration of vNext for the new Peer Gateway connector and Fabric 2.4 binding + some required fixes for the existings connectors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 16:58:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1301" class=".btn">#1301</a>
            </td>
            <td>
                <b>
                    [Doc] Mainly address install docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. replace reference to rocketchat with discord
2. Tweak the 0.4.2 install docs to reference 0.4.2 and remove references
to fabric 1.4 (replace with 2.2 as appropriate)
3. Redo the vNext docs incorporating the 0.4.2 tweaks but also move
installing caliper source to contribution guide
4. remove IBM Plex Mono for code examples as it doesn't appear to align
properly
5. remove the documented latest options for bindings as this could be
confusing especially as besu is at 22.x.x release now and we only
support 1.4 as the latest

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 12:55:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1298" class=".btn">#1298</a>
            </td>
            <td>
                <b>
                    Peer Gateway: Added Connector Selector implementation modifications to support the new Peer Gateway Connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added logic to pick new Peer Gateway connector in the connector selector in FabriConnectorFactory.js 
- added 2.4 fabric SUT version with binding packages in .config.yaml
- added last fixes for the Peer Gateway connector implementation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 10:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1297" class=".btn">#1297</a>
            </td>
            <td>
                <b>
                    Update the usage examples to more appropriate versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The documentation in vNext will also be updated in line with this
change.

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 09:41:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1295" class=".btn">#1295</a>
            </td>
            <td>
                <b>
                    address fabric tutorial not working with newer docker-compose
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                newer docker-compose versions don't work with the specific git checkout
in the tutorial.

I've fixed the bug in fabric-samples but as it hasn't been tagged as a
release yet we need to use another specific git commit but updates to
test-network now means it works with newer docker-compose versions.

closes #1291

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 13:14:49 +0000 UTC
    </div>
</div>

