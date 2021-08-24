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
                PR <a href="https://github.com/hyperledger/cactus/pull/1249" class=".btn">#1249</a>
            </td>
            <td>
                <b>
                    feat(keychain-azure-kv): complete request handler and endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1010 

_______________________________________
This is might be a duplicate PR that Jeff's #1206 is working on, I'm opening a new PR since I do not have collaborator rights yet. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 15:31:44 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1235" class=".btn">#1235</a>
            </td>
            <td>
                <b>
                    test: reduce artillery runtime to 1 minute from 10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1146

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

___________________________________________________________________________

Although the original issue mentioned that the artillery runtime was 10 minutes, it might have been at 5 minutes. I'm not sure if I've altered the correct code for this issue but I edited the avgLatency. Please let me know if there's something else I should have done!! 

It also looks like this testcase wasn't passing the tests (this was before I made any changes), do you want me to make a separate issue to fix the failing test cases? @petermetz 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 15:27:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1234" class=".btn">#1234</a>
            </td>
            <td>
                <b>
                    test: adding quorum multip test ledger Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This code allows for building of the a quorum multi party docker image that allows for private transactions to be tested.

Related to #951 


Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 10:23:00 +0000 UTC
    </div>
</div>

