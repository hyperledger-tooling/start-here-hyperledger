---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    Tutorial updates, and RFC, bug and package version fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Edited the Weaver Enablement for Fabric tutorial page, adding more context and providing explicit instructions to enable TLS among connections across relays, drivers, and IIN Agents (partly fixing #257 )
- Fixed bad links in various RFCs.
- Fixed data sharing workflow bug.
- Updated some Go module package dependencies to latest versions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 20:50:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    Bump tokio from 1.8.4 to 1.18.4 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.8.4 to 1.18.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.18.3</h2>
<h1>1.18.3 (September 27, 2022)</h1>
<p>This release removes the dependency on the <code>once_cell</code> crate to restore the MSRV of the 1.18.x LTS release. (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>)</p>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5048">tokio-rs/tokio#5048</a></p>
<h2>Tokio v1.18.2</h2>
<h1>1.18.2 (May 5, 2022)</h1>
<p>Add missing features for the <code>winapi</code> dependency. (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4663">#4663</a>)</p>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4663">#4663</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4663">tokio-rs/tokio#4663</a></p>
<h2>Tokio v1.18.1</h2>
<h1>1.18.1 (May 2, 2022)</h1>
<p>The 1.18.0 release broke the build for targets without 64-bit atomics when building with <code>tokio_unstable</code>. This release fixes that. (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4649">#4649</a>)</p>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4649">#4649</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4649">tokio-rs/tokio#4649</a></p>
<h2>Tokio v1.18.0</h2>
<h1>1.18.0 (April 27, 2022)</h1>
<p>This release adds a number of new APIs in <code>tokio::net</code>, <code>tokio::signal</code>, and
<code>tokio::sync</code>. In addition, it adds new unstable APIs to <code>tokio::task</code> (<code>Id</code>s
for uniquely identifying a task, and <code>AbortHandle</code> for remotely cancelling a
task), as well as a number of bugfixes.</p>
<h3>Fixed</h3>
<ul>
<li>blocking: add missing <code>#[track_caller]</code> for <code>spawn_blocking</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4616">#4616</a>)</li>
<li>macros: fix <code>select</code> macro to process 64 branches (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4519">#4519</a>)</li>
<li>net: fix <code>try_io</code> methods not calling Mio's <code>try_io</code> internally (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4582">#4582</a>)</li>
<li>runtime: recover when OS fails to spawn a new thread (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4485">#4485</a>)</li>
</ul>
<h3>Added</h3>
<ul>
<li>net: add <code>UdpSocket::peer_addr</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4611">#4611</a>)</li>
<li>net: add <code>try_read_buf</code> method for named pipes (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4626">#4626</a>)</li>
<li>signal: add <code>SignalKind</code> <code>Hash</code>/<code>Eq</code> impls and <code>c_int</code> conversion (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4540">#4540</a>)</li>
<li>signal: add support for signals up to <code>SIGRTMAX</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4555">#4555</a>)</li>
<li>sync: add <code>watch::Sender::send_modify</code> method (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4310">#4310</a>)</li>
<li>sync: add <code>broadcast::Receiver::len</code> method (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4542">#4542</a>)</li>
<li>sync: add <code>watch::Receiver::same_channel</code> method (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4581">#4581</a>)</li>
<li>sync: implement <code>Clone</code> for <code>RecvError</code> types (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4560">#4560</a>)</li>
</ul>
<h3>Changed</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/9241c3eddf4a6a218681b088d71f7191513e2376"><code>9241c3e</code></a> chore: prepare Tokio v1.18.4 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/699573d550fabf4bfb45d82505d6709faaae9037"><code>699573d</code></a> net: fix named pipes server configuration builder</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/5c76d070e28bd9153ec72f13d0ebe24935b9dea0"><code>5c76d07</code></a> chore: prepare Tokio v1.18.3 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5051">#5051</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/05e661490b87a3d60a8342535bdc9d213048519c"><code>05e6614</code></a> chore: don't use <code>once_cell</code> for 1.18.x LTS release (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/7aa1566cde7e04cebe60711ed6ce2f8b277158e9"><code>7aa1566</code></a> chore: prepare Tokio v1.18.2</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/7c8e552f290a7cbae21f6d3343c2ee26c418d2fb"><code>7c8e552</code></a> windows: add features for winapi (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4663">#4663</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/148bea82ee15974e64d8fc9292c2066a7278cebc"><code>148bea8</code></a> tokio: prepare Tokio v1.18.1 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4650">#4650</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/dc54aec1c785e334c23a0c8f249e71a8241f0d1d"><code>dc54aec</code></a> metrics: use mocked <code>AtomicU64</code> in IO metrics driver (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4649">#4649</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/fa665b91a8f7bbf0ab234f60f28ef25e5afac10b"><code>fa665b9</code></a> macros: always emit return statement (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4636">#4636</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/48183430fb1385c823c048af16aaea346d8e652f"><code>4818343</code></a> tokio: prepare to release v1.18.0 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4641">#4641</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.8.4...tokio-1.18.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.8.4&new-version=1.18.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 22:28:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Besu Documentation and RFC Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added `setup-local` and `ledger-initilization` for Besu network asset exchange.
- Restructured `asset-exchange` page, into multiple pages, and added Besu asset exchange instructions.
- RFC updated for Fabric-HTLC
- RFC updated for Corda data sharing
- RFC drafted for Besu data sharing and views.

Update:
- Updated Corda asset exchange in "Enable weaver in your application" document.

Update 2:
- Support an array of payloads, one from each node in Corda View.
- Updated rfc, core contracts, and SDK as per above Corda View change.
- Added 2 orgs test in Corda Interop App unit test, and fixed bug in ViewVerification when receiving view from 2 orgs.
- All modules updated to `v1.5.7` except corda modules which are updated to `v1.2.13`

Deployed new docs: https://sanvendev.github.io/weaver-dlt-interoperability/docs/external/getting-started/guide
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 12:09:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/358" class=".btn">#358</a>
            </td>
            <td>
                <b>
                    Updating Golang package versions and dependencies and Re-enabling workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fabric Interop Chaincode `libs/utils` was upgraded to `1.5.6` earlier. Other packages depending on this library required updates to their dependencies (`go.sum` files).

Re-enabled data sharing and asset transfer workflows dependent on the latest version of the Fabric Interop Chaincode.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 16:06:48 +0000 UTC
    </div>
</div>

