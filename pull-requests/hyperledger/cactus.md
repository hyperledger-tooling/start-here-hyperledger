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
                PR <a href="https://github.com/hyperledger/cactus/pull/1270" class=".btn">#1270</a>
            </td>
            <td>
                <b>
                    build(dev-container): fix yarn not found error #1269
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Primary change:
------------------

The post-create-command.sh script will now run the
install-yarn script prior to calling the configure script.
This wil lensure that yarn is installed by the time the
configure script is invoked.

Secondary change(s):
------------------------

Applied automatic formatting to the Dockerfile and the
aforementioned post-create-commands script as well.

Fixes #1269

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 17:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1268" class=".btn">#1268</a>
            </td>
            <td>
                <b>
                    refactor(cmd-server-socket,validator): [draft] refactor the directory structure of cmd-server-socket and validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolving #1233 (work-in-progress)
- status: Draft

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 14:47:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    fix(indy-validator): fixing indy validator initialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issue #1266.

- Added initialization code before pool.open_pool_ledger API call.
- Also added a key file necessary for the server.

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 14:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1244" class=".btn">#1244</a>
            </td>
            <td>
                <b>
                    feat(besu): support besu v21.1.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #982 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 12:28:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1243" class=".btn">#1243</a>
            </td>
            <td>
                <b>
                    feat(vault-keychain): add support for vault transit secret engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for following method to `PluginKeychainVault` class
- `transitSign` : sign digest using private key stored in vault server
- `transitNewKey` : create a new key
- `transitGetPub` : return `pem` encoded public key 
- `transitRotateKey` : rotate private key

For now it support `EC` (key generated from from curve p256 , p384 , p521 ) only

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 20:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1242" class=".btn">#1242</a>
            </td>
            <td>
                <b>
                    docs(tools): fix besu all-in-one docker-compose #1241
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Besu</span><span class="chip">dependencies</span>
            </td>
            <td>
                Fixes #1241

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 19:28:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1240" class=".btn">#1240</a>
            </td>
            <td>
                <b>
                    docs: update faq documentation and incorporate Quick-Start-Topics section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Structure FAQ.md into two sections:
- Quick-Start Topics
- Other Topics

Adding a new topic for API-Server 'UnauthorizedError' to the Quick-Start Topics 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 12:27:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1238" class=".btn">#1238</a>
            </td>
            <td>
                <b>
                    fix(yarn-npm-replace): replace npm with yarn in Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Improve Dockernization by replacement of npm with yarn.
This PR is a fix regarding Issue #1237
Signed-off-by: Shingo Fujimoto <shingo_fujimoto@fujitsu.com>

Update by Peter:
(this is the syntax that GitHub parses to link the issue and the PR together for automatic issue closure once the PR is merged)
Fixes #1237 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 03:28:41 +0000 UTC
    </div>
</div>

