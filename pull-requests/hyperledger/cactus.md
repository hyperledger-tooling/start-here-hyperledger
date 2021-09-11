---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1318" class=".btn">#1318</a>
            </td>
            <td>
                <b>
                    docs(dev-container): fix Unable to access jarfile openapi-generator-c…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span>
            </td>
            <td>
                …li/versions/5.2.0.jar #1317

The OpenAPI generator versions were out of sync, unified it on 5.2.0 and now the dev container
does not have any issue configuring itself upon a successful boot.

Fixes #1317

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 22:03:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1316" class=".btn">#1316</a>
            </td>
            <td>
                <b>
                    docs(examples): fix supply chain app container image #1312
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Also published as a container image on ghcr.io as:
ghcr.io/hyperledger/cactus-example-supply-chain-app:2021-09-08--docs-1312

Fixes #1312

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 04:11:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1310" class=".btn">#1310</a>
            </td>
            <td>
                <b>
                    docs(ledger-support-matrix): updated releases #1279
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1279 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 12:43:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1309" class=".btn">#1309</a>
            </td>
            <td>
                <b>
                    feature(improve-indy-testnet-docker): auto-start server on container startup #1308
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modified Dockerfile so that validator program is automatically run from supervisord.

Also:
- fixed a problem found during this implementation: sandbox directory for indy_pool was not included in current version. Now startup script automatically initializes itself when it cannot find necessary files.
- lessened dependency to indy-sdk (some files are copied from indy-sdk to indy-testnet directory) by copying some files from indy-sdk to this directory. 
- Note: as of now, a container for testing server containers still depends on indy-sdk source tree. This needs to be fixed in future PR.

This PR corresponds to Issue #1308 

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 10:52:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1307" class=".btn">#1307</a>
            </td>
            <td>
                <b>
                    fix(verify-algo): fixed algorism for jwt in verifier to match algorism in validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                changed RS256  to ES256.

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 05:03:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1304" class=".btn">#1304</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): cockpit off by default #1239
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1239 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 12:46:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1303" class=".btn">#1303</a>
            </td>
            <td>
                <b>
                    docs(readme.md): add Open in VSCode badge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: shoeb <shoebsd31@gmail.com>

Added a vs code badge as described in this issue :  #1116 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-04 15:42:48 +0000 UTC
    </div>
</div>

