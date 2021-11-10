---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    Solve replicator close deadlock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                When closing the replicator, in one case, the replicator's event-loop go-routine breaks out
of the loop without broadcasting to the propose-loop sync.Cond, and the propose loop remains
waiting on it and does not exit.

The solution is to broadcast to the sync.Cond when the event-loop go-routine exits, not only
when it detects the stop signal.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 07:15:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Check TxId is a URL segment-nz
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 20:10:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/240" class=".btn">#240</a>
            </td>
            <td>
                <b>
                    Unit test flake
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">testing</span>
            </td>
            <td>
                Eliminate flake by removing sleep, use zap.Hooks instead.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 16:22:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    Allow zap.Options in logger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allowing zap.Options in the logger will allow us to insert zap.Hooks.
This will allow us to catch log messages during unit testing, and test
events that are difficult to observer otherwise.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 09:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    Intro page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 07:22:15 +0000 UTC
    </div>
</div>

