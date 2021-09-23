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
                PR <a href="https://github.com/hyperledger/cactus/pull/1377" class=".btn">#1377</a>
            </td>
            <td>
                <b>
                    docs(reading-list): update BAFT DLPC doc to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also added latest business best practices doc link
Previous link was to an an announcement of the doc rather than the doc itself, and was also an outdated version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 18:11:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1376" class=".btn">#1376</a>
            </td>
            <td>
                <b>
                    ci: drop Node v12 from matrix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Why though?
Because Node v12 will soon be EOL'd once 16 becomes the stable LTS
next month and testing only 2 versions in our matrix will help ease
the pain (at least temporarily) caused by the docker hub rate limits.

Also upgraded the versions for 14 and 16 to the latest as of 2021-09-22

Also set the max parallel to 2 in order to closer match reallity
instead of 1024 which if we actually used the dockerhub rate limits
would fail all the tests anyway.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 16:43:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1349" class=".btn">#1349</a>
            </td>
            <td>
                <b>
                    refactor (core-api): make schema names consistent in openapi spec 
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
        Created At 2021-09-17 16:24:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    docs(api-table): update API table and description
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - updated API table for socket.io verifier and validator.
- names are changed for consistency

This PR corresponds to issue #1320

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 14:02:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1347" class=".btn">#1347</a>
            </td>
            <td>
                <b>
                    fix: endpoints implementation in corda plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1346

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 08:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1345" class=".btn">#1345</a>
            </td>
            <td>
                <b>
                    build(deps): upgrade axios to latest to fix CVE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span>
            </td>
            <td>
                Depends on #1344


Details
CVE-2021-3749
high severity
Vulnerable versions: <= 0.21.1
Patched version: 0.21.2
axios is vulnerable to Inefficient Regular Expression Complexity

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com> 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 00:45:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1344" class=".btn">#1344</a>
            </td>
            <td>
                <b>
                    build: downgrade to yarn v1.18.0 due to upgrade-interactive bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #1343

See: https://github.com/yarnpkg/yarn/issues/7807 for the root cause
and https://classic.yarnpkg.com/en/docs/cli/upgrade-interactive/
for more information about what yarn upgrade-interactive does.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 00:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1343" class=".btn">#1343</a>
            </td>
            <td>
                <b>
                    build(yarn): reset script now wipes node modules, yarn lock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Found myself in need of this when strange errors started occurring
between branch switches where the gRPC tooling was not installed
properly despite the configure script running successfully.
Now the reset is script is much more robust and it closer
resembles the outcome of a fresh clone.

Also: Ran the reset script and it updated the lock file, including
that in the commit as well to see if in the future othe reset runs
will also generate these/similar changes to the lock file or not.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 23:32:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1342" class=".btn">#1342</a>
            </td>
            <td>
                <b>
                    ci: set the swap file size to 10 GB for GitHub runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                This will hopefully alleviate the issue of some tests causing
out of memory crashes on the 7.5GB RAM GitHub Action Runners.

Could of course have a domino effect where the swap kicks in
and slows everything down so much that the tests just start
timing out instead of crashing with OOM ¯\_(ツ)_/¯

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 23:21:55 +0000 UTC
    </div>
</div>

