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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1302" class=".btn">#1302</a>
            </td>
            <td>
                <b>
                    feat(fabric-connector) add transact receipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: jsjs026 <jasonhack518@gmail.com>

@petermetz , @RafaelAPB 
The implementation of fabric transact receipt
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-04 05:11:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1300" class=".btn">#1300</a>
            </td>
            <td>
                <b>
                    fix(test): flaky fabric AIO container boot #876
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">Fabric</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Epic facepalm once again. Turns out the default restart try
count of supervisord is too low which leads to race conditions.
Increasing the retry count from 4 to 20 should do it, this way
the fabric-network process (see supervisord.conf file) should
be 5 times as "patient" waiting for the docker daemon to launch
within the AIO container.

What was happening before is that the fabric-network script
tried launching itself in parallel with the docker daemon, but
it would time out before the docker daemon could come online.

Published these images as
ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries
and
ghcr.io/hyperledger/cactus-fabric-all-in-one:2021-09-02--fix-876-supervisord-retries

Fixes #718
Fixes #876
Fixes #320
Fixes #319

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 01:00:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1298" class=".btn">#1298</a>
            </td>
            <td>
                <b>
                    fix: openapi-validation for consortium-manual plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add missing validation for consortium-manual plugin rest endpoints

Closes: #1297

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 16:16:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1296" class=".btn">#1296</a>
            </td>
            <td>
                <b>
                    fix: openapi-validation for fabric plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add missing validation for fabric plugin rest endpoints

Closes: #1295

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 15:26:18 +0000 UTC
    </div>
</div>

