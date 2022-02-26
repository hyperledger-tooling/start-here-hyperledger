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
                PR <a href="https://github.com/hyperledger/caliper/pull/1244" class=".btn">#1244</a>
            </td>
            <td>
                <b>
                    Update bindings to latest fabric sdks and remove old ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1200
closes #1199

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-26 10:16:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1239" class=".btn">#1239</a>
            </td>
            <td>
                <b>
                    Bump version to 0.5.0-unstable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1238
Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 09:58:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1237" class=".btn">#1237</a>
            </td>
            <td>
                <b>
                    fix the benchmarks page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1107 

Signed-off-by: D <d_kelsey@uk.ibm.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 14:29:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1236" class=".btn">#1236</a>
            </td>
            <td>
                <b>
                    fix the docs for specifying charts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1126

Signed-off-by: D <d_kelsey@uk.ibm.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 10:35:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1235" class=".btn">#1235</a>
            </td>
            <td>
                <b>
                    Remove the legacy fabric connectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is mainly a deletion exercise with the following code changes
1. simplication of which connector to load
2. only create a connector instance if required for example
flow-only-start and flow-only-end don't need to have a connector created

closes #1076 

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 18:34:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1233" class=".btn">#1233</a>
            </td>
            <td>
                <b>
                    Remove information about legacy fabric connectors
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
        Created At 2022-02-21 16:02:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1231" class=".btn">#1231</a>
            </td>
            <td>
                <b>
                    Update node versions for caliper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1125 
Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 13:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1230" class=".btn">#1230</a>
            </td>
            <td>
                <b>
                    Correct timeout defaults
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the apparent cause of a caliper run hang where it continues to
run with unfinished txns. It's actually waiting 60,000 seconds for txns
to finish which won't finish as it looks like the node sdk misses the
events.

code part of #1141 also addresses in part

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 11:18:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1229" class=".btn">#1229</a>
            </td>
            <td>
                <b>
                    update incorrect doc about timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                documentation part to #1141

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 11:12:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1228" class=".btn">#1228</a>
            </td>
            <td>
                <b>
                    Reference Discord instead of Rocket Chat
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1224

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 10:05:50 +0000 UTC
    </div>
</div>

