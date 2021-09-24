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

