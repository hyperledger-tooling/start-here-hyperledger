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
                    Draft pull request for Iroha all in one docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 21:02:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    fix(examples/discounted_cartrade): update the cert and private key at…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR resolves part of Issue #1181
In this PR, I update the cert and private key at default.json to activate trade process in discouted-cartrade.

Signed-off-by: Yasushi Takahashi <t-yasushi@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-02 15:11:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1179" class=".btn">#1179</a>
            </td>
            <td>
                <b>
                    ci(tools): validate bundle names packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                This script is now part of the ci.sh script which
ensures that there is no human error when defining
the webpack bundle names in the package.json files
for each package in the project.

The idea is to reduce the manual review burden on the
maintainers who can also miss these type of issues.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 05:06:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1178" class=".btn">#1178</a>
            </td>
            <td>
                <b>
                    build(tools): script to check OAS extensions #489
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Ensures that openapi.json files "x-hyperledger-cactus"
extensions do not contain common mistakes in them due to
typos or just forgetting to specify certain mandatory
properties.

Fixes #489

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 04:02:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1177" class=".btn">#1177</a>
            </td>
            <td>
                <b>
                    docs(contributing.md): do not duplicate pull requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                It's been a common problem with people erasing review history
by opening new pull requests so now it's in the CONTRIBUTING.md
specifically being called out as something that's undesired.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 01:11:42 +0000 UTC
    </div>
</div>

