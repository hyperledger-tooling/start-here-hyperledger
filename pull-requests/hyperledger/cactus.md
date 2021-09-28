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
                PR <a href="https://github.com/hyperledger/cactus/pull/1385" class=".btn">#1385</a>
            </td>
            <td>
                <b>
                    chore(release): publish v0.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 00:23:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1384" class=".btn">#1384</a>
            </td>
            <td>
                <b>
                    build(deps): upgrade to Typescript v4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1129 

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-26 02:59:03 +0000 UTC
    </div>
</div>

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

