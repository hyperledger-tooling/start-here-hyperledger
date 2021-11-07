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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    build doc on pull request but don't deploy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                For pull-request, build the documentation. This will catch all errors before merging the PR.

For push-request, build and deploy the documentation. This will deploy the pages on `gh-pages` channel. 

Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 05:43:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    Create docker workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Trigger docker build on each PR and tag push to main branch.
Push docker image with latest repository tag to docker hub only on tag push.

Signed-off-by: Gennady Laventman <gennady@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 16:09:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    Integration test: basic cluster
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span><span class="chip">testing</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 09:20:06 +0000 UTC
    </div>
</div>

