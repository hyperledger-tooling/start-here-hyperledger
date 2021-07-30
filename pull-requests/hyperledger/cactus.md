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
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
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
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
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
                <span class="chip">Developer_Experience</span><span class="chip">documentation</span>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    docs: fix naming - use API Client isntead of SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1138

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

_______________________________________
this is not done, I just wanted to push it so I can ask for what I should write for documentations. 
I'm not sure if I know enough to write the documentation !! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 17:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    feat(examples/discounted_cartrade): add preferredcustomer-jugdement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yasushi Takahashi <t-yasushi@fujitsu.com>

resolves #1148 (update by Peter)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 02:52:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    refactor(core-api): keychain plugin get/set generics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #478
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 20:15:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    Draft pull request for Iroha connector plugin
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
        Created At 2021-07-26 15:56:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    feat(besu): Support for private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Support for besu private transactions is now enabled, this is done by adding privateFor and privateFrom fields in the HTTP request.

fixes #952 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 11:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1167" class=".btn">#1167</a>
            </td>
            <td>
                <b>
                    feat(corda): support release 4.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #888 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 13:52:44 +0000 UTC
    </div>
</div>

