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
                PR <a href="https://github.com/hyperledger/cactus/pull/1193" class=".btn">#1193</a>
            </td>
            <td>
                <b>
                    refactor: remap ts typings from types to lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was necessary because if we import JSON files and
then re-use their schema as types, then the d.ts files
will need to have access to said JSON file which does
not happen if the typings and the actual .js code are
in separate directories because then the relative paths
are not working as they should.

Moving the lib and the types together means that now
the d.ts files can import with the same relative paths
that the orignial source code (.ts files) can as well.

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 21:03:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    feat(connector-quorum): remove hard dependency on keychain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(quorum): remove hard dependency on keychain

Removed hard dependency on keychain for Quorum plugin.

Updated old test cases and added new test cases.

resolves #1161 

Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 12:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    feat(cmd-api-server): support grpc web services #1189
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">API_Server</span>
            </td>
            <td>
                # WORK IN PROGRESS

Fixes #1189
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 06:38:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1188" class=".btn">#1188</a>
            </td>
            <td>
                <b>
                    feat(keychain-google-sm): complete request handler and endpoints #1097
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1097 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 19:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1187" class=".btn">#1187</a>
            </td>
            <td>
                <b>
                    fix(example): send http request to discounted-cartrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This resolve Issue #1181 
I create req_discounted_cartrade.py in example/discounted-cartrade.
This sends http request to discounted-cartrade after resistors indy data.

Signed-off-by: Yasushi Takahashi <t-yasushi@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 06:46:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    chore(release): publish v0.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 21:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    build(package.json): add reset script that git cleans prior to configure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Why though?
This is designed to eliminate possible build issues that arise because of leftover code files
somehow lurking around the project directory structure that are being ignored by git and
therefore lulling a contributor to thinking that since VSCode shows no index/staged changes
the project is in a clean slate and the build should pass all the same.
The reset script in essence is a softer version of going all out, deleting your entire
project directory and cloning it from scratch which is a lot more effort than just running
the reset script added here that has a good chance of fixing the same problems as the hard
resetting if re-clone would fix.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 19:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    build: yarnrc --ignore-engines true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Specifies the --ignore-engines true parameter to be the default for
every yarn command contributors run within the project. This makes it
sligthly more convenient to work with yarn since now you can just say
"yarn install" instead of having to go with the much longer "yarn
install --ignore-engines". 

Of course in an ideal world we would not need
the --ignore-engines parameter but the Fabric Node SDK (and some other
dependencies probably) do not declare NodeJS v16 as a supported engine
(despite our tests succeeding on these) so we just do not have a choice
with this if we want to support NodeJS 16 (which we very much
do)

Also removes --ignore-engines parameter from the yarn install
command that the configure script runs so that the CI also verifies this
to be working fine.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 05:10:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1183" class=".btn">#1183</a>
            </td>
            <td>
                <b>
                    feat(iroha): add Iroha AIO image and Iroha test ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Provides port randomization
2. Possibility to launch from within test cases, no need for docker-compose
3. Can be linked to postgres container via the default host network interface instead of being forced to deal with docker networks and all the statefulness they bring into the picture
4. Contains a workaround to the FILE -> ENV configuration precedence of Iroha (opened an issue about this - PR is dropping soon but in the meantime we needed it to work anyway so that's why the entrypoint script has the jq trickery in there to update the configuration file based on what's in the environment variables for postgres credentials)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 21:02:40 +0000 UTC
    </div>
</div>

