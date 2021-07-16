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
                PR <a href="https://github.com/hyperledger/cactus/pull/1141" class=".btn">#1141</a>
            </td>
            <td>
                <b>
                    build: migrate to Yarn v1 from npm v7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                ## Dependencies

Depends on #1111 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: Thu Jul 15 2021 22:10:04 GMT-0700 (Pacific Daylight Time)
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: Thu Jul 15 2021 22:12:29 GMT-0700 (Pacific Daylight Time) 

build: migrate to Yarn v1 from npm v7

Why?
It was reported by other maintainers that yarn behaves much
better in corporate proxy/firewalled environments.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 05:18:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1139" class=".btn">#1139</a>
            </td>
            <td>
                <b>
                    chore(release): publish v0.6.0
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
        Created At 2021-07-15 23:00:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1136" class=".btn">#1136</a>
            </td>
            <td>
                <b>
                    docs(examples): supply chain- eliminate endpoint constant classes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                
Fixes #1120

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

@petermetz ping for review :) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 19:52:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1135" class=".btn">#1135</a>
            </td>
            <td>
                <b>
                    refactor(core-api): keychain plugin get/set generic type parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refactor(core-api): keychain plugin get/set generics #1135 

Fixes #1135 
Signed-off-by: Tommesha Wiggins <tommesha.wiggins@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 18:18:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): OpenAPI spec validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add missing validation from plugin REST endpoints

fixes #847

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 15:52:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    feat(connector-fabric): endorsing peers request arg #1122
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                Makes it possible to set the endorsing peers on a transaction
when submitted through the Fabric connector.

For example these values can be passed in to the new parameter
and it will set the endorsers up accordingly prior to submitting
the transaction to the ledger:
- org1.example.com
- Org1MSP
- org2.example.com
- Org2MSP

(You only need either the org domain or the msp ID, no need
to specify both of them for it to work).

For a working example, see this test case:
packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/integration/fabric-v2-2-x/run-transaction-endpoint-v1.test.ts

Depends on #1123
Depends on #1130

Fixes #1122

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 06:15:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    feat(connector-fabric): identity json signing credentials #1130
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                Introduces a new, optional (for now) parameter on the run tx
endpoint's request object called gatewayOptions which is capable
of including everything that one needs to instantiate a gateway
object of the underlying Fabric Node SDK.

This change makes it possible to not need the keychain plugin
at all when someone does not need/want it.

Fixes #1130

Depends on #1124

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 04:56:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1128" class=".btn">#1128</a>
            </td>
            <td>
                <b>
                    docs(whitepaper): add suggested reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Adds a suggested reference for people that want to cite our whitepaper
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 17:16:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1127" class=".btn">#1127</a>
            </td>
            <td>
                <b>
                    fix: fixing branch name for code cov badge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">documentation</span>
            </td>
            <td>
                Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 09:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1124" class=".btn">#1124</a>
            </td>
            <td>
                <b>
                    refactor(connector-fabric): upgrade to Fabric 2.x Node SDK #1123
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">Security</span><span class="chip">enhancement</span>
            </td>
            <td>
                The Cactus packages were relying on 1.4.x Fabric SDK dependencies
prior to this change (even when communicating with 2.x Fabric ledgers)
which is something that we needed to fix by upgrading the dependency
versions.

Fixes #1123

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 23:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1121" class=".btn">#1121</a>
            </td>
            <td>
                <b>
                    ci(github): add commit lint action to PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                This is supposed to check every single commit in a PR
for having the correct message format.

Previously the semantic PR action was only checking
the PR title or the first commit message, so you could
get in invalid commit messages by adding multiple
commits post-approval which the semantic PR action
would not check properly.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-11 01:42:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1118" class=".btn">#1118</a>
            </td>
            <td>
                <b>
                    Docs : added a badge to open cactus with vscode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1116 
Signed-off-by: shoeb <shoebsd31@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 15:21:08 +0000 UTC
    </div>
</div>

