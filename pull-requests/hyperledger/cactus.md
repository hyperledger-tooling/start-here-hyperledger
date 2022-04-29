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
                PR <a href="https://github.com/hyperledger/cactus/pull/1996" class=".btn">#1996</a>
            </td>
            <td>
                <b>
                    refactor(cmd-api-server): clean up configuration parameters #720
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: #720

Parameters that are cleaned up are: cactusNodeId, consortiumId, keychainSuffixKeyPairPem
Parameter keyPairPem cannot be remove as it results to an error in running the api server.

Cleaning the three mentioned parameter are backwards compatible with tags versions:
v1.0.0-rc.3 and v1.0.0
The latest tag being used as of this change is v1.0.0-25-gdda3f00c

Signed-off-by: ruzell22 <ruzell.vince.aquino@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 10:05:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1994" class=".btn">#1994</a>
            </td>
            <td>
                <b>
                    feat(cmd-api-server): swagger.json endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span>
            </td>
            <td>
                fixes: #1877
Signed-off-by: charellesandig <charelle.wrk@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 04:25:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1993" class=".btn">#1993</a>
            </td>
            <td>
                <b>
                    ci: add container scanning to default checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: aldousalvarez <aldousss.alvarez@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 03:02:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1992" class=".btn">#1992</a>
            </td>
            <td>
                <b>
                    ci(connector-besu): include endpoints in fuzzer tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed

ci(connector-besu): include endpoints in fuzzer tests 


    Primary Changes
    --------------
    1. Updated the git workflow to include the besu connector plugin endpoint
    2. Added the task to run Besu all-in-one image
       as a valid ws endpoint is required for connector to initialize
    3. Updated the besu connector plugin README.md for minor fixes

Fixes #1949

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 10:03:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1991" class=".btn">#1991</a>
            </td>
            <td>
                <b>
                    docs(maintainers): add Rama and Sandeep
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
        Created At 2022-04-26 03:05:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1990" class=".btn">#1990</a>
            </td>
            <td>
                <b>
                    ci: bump NodeJS v14 and v16 minor versions to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Fixes #1980

Signed-off-by: aldousalvarez <aldousss.alvarez@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 02:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1989" class=".btn">#1989</a>
            </td>
            <td>
                <b>
                    ci: add yaml workflow file for semantic-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1987

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 21:03:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1988" class=".btn">#1988</a>
            </td>
            <td>
                <b>
                    test: jestify jwt socketio endpoint authorization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                packages/cactus-cmd-api-server/src/test/typescript/integration/jwt-socketio-endpoint-authorization.test.ts; WIP
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 12:45:53 +0000 UTC
    </div>
</div>

