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
                PR <a href="https://github.com/hyperledger/cactus/pull/1806" class=".btn">#1806</a>
            </td>
            <td>
                <b>
                    refactor(cartrade): dockerize catrade and fabric validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Cartrade example will be setup in docker-compose, updated the readme with new instructions.
- Fabric validator runs in container as well.
- Removed obsolete scripts, changed them where needed.
- Build artifacts are not put directly in root `dist/` dir anymore (it's still used by apps not dockerized yet, though, but will be changed in future commits).
- Validator configuration is made cartrade-specific, this will be done in the same way for other sample apps in future commits.
- Some setup changes were necessary in other samples as well, all should work like before.
- Added small patch in fabric-all-in-one to support cartrade scenario (endorsment from peer from single org).
- Updated indy clientbase base image because it didn't work with `ppa:deadsnakes` anymore.

Closes: #1805
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

### TODO (in future PR)
- Clean exports from `@hyperledger/cactus-cmd-socket-server` (will not use this long fragile path in the future)

Depends on #1800
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 09:24:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1802" class=".btn">#1802</a>
            </td>
            <td>
                <b>
                    Upgrade to grpc@1.24.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                grpc is a gRPC Library for Node

Affected versions of this package are vulnerable to Prototype Pollution via loadPackageDefinition.

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I have the right to submit it under the open source license indicated in the file; or

(b) The contribution is based upon previous work that, to the best of my knowledge, is covered under an appropriate open source license and I have the right under that license to submit that work with modifications, whether created in whole or in part by me, under the same open source license (unless I am permitted to submit under a different license), as indicated in the file; or

(c) The contribution was provided directly to me by some other person who certified (a), (b) or (c) and I have not modified it.

(d) I understand and agree that this project and the contribution are public and that a record of the contribution (including all personal information I submit with it, including my sign-off) is maintained indefinitely and may be redistributed consistent with this project or the open source license(s) involved.

Signed-off-by: Bhaskar Ram <bhaskar@parrotsec.in>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 17:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1801" class=".btn">#1801</a>
            </td>
            <td>
                <b>
                    feat: add jwt authorization to supply chain example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1579

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 15:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1800" class=".btn">#1800</a>
            </td>
            <td>
                <b>
                    fix(plugin-ledger-connector-fabric-socketio): upgrade Fabric due to jsrsasign
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">Fabric</span><span class="chip">Security</span>
            </td>
            <td>
                Revert fabric sdk package change from PR #1754

Closes: #1799
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

After change:
```
@hyperledger/cactus@ /home/outsh/cactus
├─┬ @hyperledger/cactus-cmd-socket-server@1.0.0-rc.3 -> ./packages/cactus-cmd-socketio-server
│ └─┬ fabric-ca-client@1.4.19
│   └── jsrsasign@10.5.0
├─┬ @hyperledger/cactus-example-carbon-accounting-backend@1.0.0-rc.3 -> ./examples/cactus-example-carbon-accounting-backend
│ └─┬ fabric-network@2.2.10
│   └─┬ fabric-common@2.2.10
│     └── jsrsasign@10.5.0 deduped
├─┬ @hyperledger/cactus-plugin-ledger-connector-fabric-socketio@1.0.0-rc.3 -> ./packages/cactus-plugin-ledger-connector-fabric-socketio
│ └─┬ fabric-client@1.4.19
│   └── jsrsasign@10.5.0 deduped
├─┬ @hyperledger/cactus-plugin-ledger-connector-fabric@1.0.0-rc.3 -> ./packages/cactus-plugin-ledger-connector-fabric
│ ├─┬ fabric-ca-client@2.3.0-snapshot.62
│ │ └── jsrsasign@10.5.0
│ ├─┬ fabric-common@2.3.0-snapshot.63
│ │ └── jsrsasign@10.5.0 deduped
│ ├── jsrsasign@10.4.0
│ └─┬ ws-wallet@1.1.5
│   └── jsrsasign@10.4.1
└─┬ @hyperledger/cactus-test-tooling@1.0.0-rc.3 -> ./packages/cactus-test-tooling
  └─┬ fabric-ca-client@2.2.10
    ├─┬ fabric-common@2.2.10
    │ └── jsrsasign@10.5.0 deduped
    └── jsrsasign@10.5.0 deduped
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 13:18:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1798" class=".btn">#1798</a>
            </td>
            <td>
                <b>
                    docs(examples): cover different levels of immersion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently just a draft, elephant shrew is a stand-in picture for now


Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 18:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1797" class=".btn">#1797</a>
            </td>
            <td>
                <b>
                    test: enhancement to check connection eth validator blp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add tests for sync (read and write) requests to validator. 
- Add tests for async (read and write) requests to validator. 
- Add handling for Monitor Mode in blp. 
- Add tests for config files. Add automatization tools for tests and setup of blp.
-  Updated readme.

Depends on: #1629 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 12:55:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1796" class=".btn">#1796</a>
            </td>
            <td>
                <b>
                    fix(security): address CVE-2019-5413
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #1777 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 06:07:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1795" class=".btn">#1795</a>
            </td>
            <td>
                <b>
                    docs: changes to BUILD.md and CONTRIBUTING.md #1792
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document updates for issue #1792 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 05:32:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1794" class=".btn">#1794</a>
            </td>
            <td>
                <b>
                    docs(cactus-core-api): add README file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Developer_Experience</span><span class="chip">dependent</span><span class="chip">Core_API</span>
            </td>
            <td>
                Depends on #1556 - feat(core-api): add weaver protobuf codegen

Fixes #833

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 22:39:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1793" class=".btn">#1793</a>
            </td>
            <td>
                <b>
                    style: 2021-09-20 linter warnings batch 20 / 26 #1369
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                style: 2021-09-20 linter warnings batch 20 / 26 

 changes made in assigned lines 191-200
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 08:05:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1791" class=".btn">#1791</a>
            </td>
            <td>
                <b>
                    build(deps): bump engine.io from 4.1.1 to 4.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span>
            </td>
            <td>
                Bumps [engine.io](https://github.com/socketio/engine.io) from 4.1.1 to 4.1.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/releases">engine.io's releases</a>.</em></p>
<blockquote>
<h2>4.1.2</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<blockquote>
<p>RangeError: Invalid WebSocket frame: RSV2 and RSV3 must be clear
at Receiver.getInfo (/.../node_modules/ws/lib/receiver.js:176:14)
at Receiver.startLoop (/.../node_modules/ws/lib/receiver.js:136:22)
at Receiver._write (/.../node_modules/ws/lib/receiver.js:83:10)
at writeOrBuffer (internal/streams/writable.js:358:12)</p>
</blockquote>
<p>This bug was introduced by <a href="https://github.com/socketio/engine.io/commit/f3c291fa613a9d50c924d74293035737fdace4f2">this commit</a>, included in <code>engine.io@4.0.0</code>, so previous releases are not impacted.</p>
<p>Thanks to Marcus Wejderot from Mevisio for the responsible disclosure.</p>
<h3>Bug Fixes</h3>
<ul>
<li>properly handle invalid data sent by a malicious websocket client (<a href="https://github.com/socketio/engine.io/commit/a70800d7e96da32f6e6622804ef659ebc58659db">a70800d</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/engine.io/compare/4.1.1...4.1.2">https://github.com/socketio/engine.io/compare/4.1.1...4.1.2</a></li>
<li>Client release: -</li>
<li>ws version: <a href="https://github.com/websockets/ws/releases/tag/7.4.2">~7.4.2</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/blob/4.1.2/CHANGELOG.md">engine.io's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/engine.io/compare/4.1.1...4.1.2">4.1.2</a> (2022-01-11)</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<blockquote>
<p>RangeError: Invalid WebSocket frame: RSV2 and RSV3 must be clear
at Receiver.getInfo (/.../node_modules/ws/lib/receiver.js:176:14)
at Receiver.startLoop (/.../node_modules/ws/lib/receiver.js:136:22)
at Receiver._write (/.../node_modules/ws/lib/receiver.js:83:10)
at writeOrBuffer (internal/streams/writable.js:358:12)</p>
</blockquote>
<p>This bug was introduced by <a href="https://github.com/socketio/engine.io/commit/f3c291fa613a9d50c924d74293035737fdace4f2">this commit</a>, included in <code>engine.io@4.0.0</code>, so previous releases are not impacted.</p>
<p>Thanks to Marcus Wejderot from Mevisio for the responsible disclosure.</p>
<h3>Bug Fixes</h3>
<ul>
<li>properly handle invalid data sent by a malicious websocket client (<a href="https://github.com/socketio/engine.io/commit/a70800d7e96da32f6e6622804ef659ebc58659db">a70800d</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/engine.io/commit/c6315af44826b87f6802574f1ef79dfa63777fab"><code>c6315af</code></a> chore(release): 4.1.2</li>
<li><a href="https://github.com/socketio/engine.io/commit/a70800d7e96da32f6e6622804ef659ebc58659db"><code>a70800d</code></a> fix: properly handle invalid data sent by a malicious websocket client</li>
<li>See full diff in <a href="https://github.com/socketio/engine.io/compare/4.1.1...4.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=engine.io&package-manager=npm_and_yarn&previous-version=4.1.1&new-version=4.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 00:36:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1790" class=".btn">#1790</a>
            </td>
            <td>
                <b>
                    ci: fix Could not get resource https://jcenter.bintray.com/
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">Corda</span><span class="chip">dependencies</span>
            </td>
            <td>
                Stopped using jcenter altogether. The build appears to be working
fine with the alternative repositories afterwards so it
looks like this is all we'll need to fix this problem (knock on wood).

Fixes #1789

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 19:53:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1787" class=".btn">#1787</a>
            </td>
            <td>
                <b>
                    build(deps): bump shelljs from 0.8.4 to 0.8.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shelljs](https://github.com/shelljs/shelljs) from 0.8.4 to 0.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/shelljs/shelljs/releases">shelljs's releases</a>.</em></p>
<blockquote>
<h2>v0.8.5</h2>
<p>This was a small security fix for <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1058">#1058</a>.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/shelljs/shelljs/commit/70668a4555c7d49c4f67d53ea063b899be4d6d40"><code>70668a4</code></a> 0.8.5</li>
<li><a href="https://github.com/shelljs/shelljs/commit/d919d22dd6de385edaa9d90313075a77f74b338c"><code>d919d22</code></a> fix(exec): lockdown file permissions (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1060">#1060</a>)</li>
<li>See full diff in <a href="https://github.com/shelljs/shelljs/compare/v0.8.4...v0.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=shelljs&package-manager=npm_and_yarn&previous-version=0.8.4&new-version=0.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 07:26:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1784" class=".btn">#1784</a>
            </td>
            <td>
                <b>
                    test(test-plugin-htlc-eth-besu): fix negative test case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Negative test case of `new-contract-endpoint-invalid.test.ts` fixed

Fixes #1698

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 20:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1782" class=".btn">#1782</a>
            </td>
            <td>
                <b>
                    Cactus test plugin htlc eth besu erc20/refund endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/
test/typescript/integration/plugin-htlc-eth-besu-erc20/
refund-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 18:07:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1781" class=".btn">#1781</a>
            </td>
            <td>
                <b>
                    build(deps): bump node-forge from 0.10.0 to 1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span>
            </td>
            <td>
                Bumps [node-forge](https://github.com/digitalbazaar/forge) from 0.10.0 to 1.0.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/digitalbazaar/forge/blob/main/CHANGELOG.md">node-forge's changelog</a>.</em></p>
<blockquote>
<h2>1.0.0 - 2022-01-04</h2>
<h3>Notes</h3>
<ul>
<li><strong>1.0.0</strong>!</li>
<li>This project is over a decade old! Time for a 1.0.0 release.</li>
<li>The URL related changes may expose bugs in some of the networking related
code (unrelated to the much wider used cryptography code). The automated and
manual test coverage for this code is weak at best. Issues or patches to
update the code or tests would be appreciated.</li>
</ul>
<h3>Removed</h3>
<ul>
<li><strong>SECURITY</strong>, <strong>BREAKING</strong>: Remove <code>forge.debug</code> API. The API has the
potential for prototype pollution. This API was only briefly used by the
maintainers for internal project debug purposes and was never intended to be
used with untrusted user inputs. This API was not documented or advertised
and is being removed rather than fixed.</li>
<li><strong>SECURITY</strong>, <strong>BREAKING</strong>: Remove <code>forge.util.parseUrl()</code> (and
<code>forge.http.parseUrl</code> alias) and use the <a href="https://url.spec.whatwg.org/">WHATWG URL
Standard</a>. <code>URL</code> is supported by modern browers
and modern Node.js. This change is needed to address URL parsing security
issues. If <code>forge.util.parseUrl()</code> is used directly or through <code>forge.xhr</code> or
<code>forge.http</code> APIs, and support is needed for environments without <code>URL</code>
support, then a polyfill must be used.</li>
<li><strong>BREAKING</strong>: Remove <code>forge.task</code> API. This API was never used, documented,
or advertised by the maintainers. If anyone was using this API and wishes to
continue development it in other project, please let the maintainers know.
Due to use in the test suite, a modified version is located in
<code>tests/support/</code>.</li>
<li><strong>BREAKING</strong>: Remove <code>forge.util.makeLink</code>, <code>forge.util.makeRequest</code>,
<code>forge.util.parseFragment</code>, <code>forge.util.getQueryVariables</code>. Replace with
<code>URL</code>, <code>URLSearchParams</code>, and custom code as needed.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><strong>BREAKING</strong>: Increase supported Node.js version to 6.13.0 for URL support.</li>
<li><strong>BREAKING</strong>: Renamed <code>master</code> branch to <code>main</code>.</li>
<li><strong>BREAKING</strong>: Release process updated to use tooling that prefixes versions
with <code>v</code>. Other tools, scripts, or scanners may need to adapt.</li>
<li><strong>BREAKING</strong>: Remove docs related to Bower and
<a href="https://github.com/digitalbazaar/forge-dist">forge-dist</a>. Install using
<a href="https://github.com/digitalbazaar/forge/blob/main/README.md#installation">another method</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>OIDs for <code>surname</code>, <code>title</code>, and <code>givenName</code>.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li><strong>BREAKING</strong>: OID 2.5.4.5 name fixed from <code>serialName</code> to <code>serialNumber</code>.
Depending on how applications used this id to name association it could cause
compatibility issues.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/digitalbazaar/forge/commit/bc1a8d8837ef29672dbd320c5d03f06068ae4116"><code>bc1a8d8</code></a> Release 1.0.0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/9055d6f6099e5199d7e62027e8eb0f5860d33938"><code>9055d6f</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/69395d0684eb56ee0cdd9a0ea0e541a4013dafd2"><code>69395d0</code></a> Fix install note.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/5f8d5c215f157faf8d2e1d8061c4d6086363f871"><code>5f8d5c2</code></a> Update docs.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/27286feec0f9ac0094a6b7a3041e5c1a412ad7a5"><code>27286fe</code></a> Fix style.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/a3f48e4078211ec0176b6e387d83bbc3f8470b0a"><code>a3f48e4</code></a> Fix spelling.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/aea85c5cb9e7a1a180298cb4fd84e39cea254e03"><code>aea85c5</code></a> Remove URL related APIs.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/db8016c805371e72b06d8e2edfe0ace0df934a5e"><code>db8016c</code></a> Remove forge.util.parseUrl.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/e1a740d0be6c773af1840e0f0620994b8beeb020"><code>e1a740d</code></a> 🔒 change CSR examples to use 2048 bits</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/6a10f7c5bad32286fd2a02eac350109f2333a272"><code>6a10f7c</code></a> Fix OID <code>serialName</code> to <code>serialNumber</code>.</li>
<li>Additional commits viewable in <a href="https://github.com/digitalbazaar/forge/compare/0.10.0...v1.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-forge&package-manager=npm_and_yarn&previous-version=0.10.0&new-version=1.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 17:29:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1780" class=".btn">#1780</a>
            </td>
            <td>
                <b>
                    build(deps): bump follow-redirects from 1.14.5 to 1.14.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.5 to 1.14.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ede36d7c60d3acdcd324dcd99a9dbd52e4fb3a6"><code>2ede36d</code></a> Release version 1.14.7 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8b347cbcef7c7b72a6e9be20f5710c17d6163c22"><code>8b347cb</code></a> Drop Cookie header across domains.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/6f5029ae1a0fdab4dc25f6379a5ee303c2319070"><code>6f5029a</code></a> Release version 1.14.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/af706bee57de954414c0bde0a9f33e62beea3e52"><code>af706be</code></a> Ignore null headers.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.5...v1.14.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.5&new-version=1.14.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 17:27:54 +0000 UTC
    </div>
</div>

