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
                PR <a href="https://github.com/hyperledger/caliper/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    remove latency values if no successful txns in final report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1065

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 11:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Caliper terminates if prometheus is not available
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is due to the error event not being correctly captured when a
request is made to prometheus

Also added some extra code to output a warning and stop trying to do any
more queries for the round.

It won't stop it for all rounds but checks on every round.

closes #1267

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 14:30:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    change web3js-eea to web3js-quorum
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
        Created At 2022-03-24 09:17:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1281" class=".btn">#1281</a>
            </td>
            <td>
                <b>
                    [Docs] Remove fabric operations doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes details from the network configuration docs of fabric (ie
how to create channels, install/instantiate chaincodes) as it shouldn't
be used.

The code will remain for now as the integration tests still require it.

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 13:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1280" class=".btn">#1280</a>
            </td>
            <td>
                <b>
                    rename certain terms in code base
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - also fix some links as well

Signed-off-by: D <d_kelsey@uk.ibm.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 09:23:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1279" class=".btn">#1279</a>
            </td>
            <td>
                <b>
                    [Docs] Remove certain terms from docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - removed some terms where possible
- fixed a couple more links

can't change previous release docs around master as that's how it was
coded.

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 09:15:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1277" class=".btn">#1277</a>
            </td>
            <td>
                <b>
                    Remove countqueryasload option from docs
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
        Created At 2022-03-22 14:54:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1276" class=".btn">#1276</a>
            </td>
            <td>
                <b>
                    Remove CountQueryAsLoad Option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also fixes
1. unused timeout property in fabric gateway connectors
2. ignore license check in generator tests for downloaded files

Doc update to follow

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 14:48:56 +0000 UTC
    </div>
</div>

