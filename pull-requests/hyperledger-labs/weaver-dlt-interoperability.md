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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    Besu Simplestate Application Contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                SimpleState Contract for Besu network with functions: 
1. `get(key)`: returns value stored at key.
2. `set(key, value)`: sets "value" at key "key".

Added besu-cli commands to test the simplestate:
1. `./bin/besu-cli state set --network=network1 <key> <value>`
2. `./bin/besu-cli state get --network=network1 <key>`

Closes #226 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 18:31:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Docs Updated with IIN Agent instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #334 

Added one more test case for relay in `test_relay.yml` workflow, for published protos-rs.

Doc deployed here: https://sanvendev.github.io/weaver-dlt-interoperability/docs/external/getting-started/test-network/setup-local
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 09:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    create besu sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: micky <chanmickyyun@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 17:32:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    Go Mod checksum fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sandeep.nishad1 <sandeep.nishad1@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 14:00:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/338" class=".btn">#338</a>
            </td>
            <td>
                <b>
                    Bump tokio from 0.2.25 to 1.8.4 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 0.2.25 to 1.8.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.8.4</h2>
<h1>1.8.4 (November 15, 2021)</h1>
<p>This release backports a bugfix for a data race when sending and receiving on a
closed <code>oneshot</code> channel ([RUSTSEC-2021-0124]) from v1.13.1.</p>
<h3>Fixed</h3>
<ul>
<li>sync: fix a data race between <code>oneshot::Sender::send</code> and awaiting a
<code>oneshot::Receiver</code> when the oneshot has been closed (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4226">#4226</a>)</li>
</ul>
<h2>Tokio v1.8.3</h2>
<h1>1.8.3 (July 22, 2021)</h1>
<p>This release backports two fixes from 1.9.0</p>
<h3>Fixed</h3>
<ul>
<li>Fix leak if output of future panics on drop (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3967">#3967</a>)</li>
<li>Fix leak in <code>LocalSet</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3978">#3978</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3967">#3967</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3967">tokio-rs/tokio#3967</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3978">#3978</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3978">tokio-rs/tokio#3978</a></p>
<h2>Tokio 1.8.2</h2>
<p>Fixes a missed edge case from 1.8.1.</p>
<h3>Fixed</h3>
<ul>
<li>runtime: drop canceled future on next poll (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3965">#3965</a>)</li>
</ul>
<h2>Tokio 1.8.1</h2>
<p>Forward ports 1.5.1 fixes.</p>
<h3>Fixed</h3>
<ul>
<li>runtime: remotely abort tasks on <code>JoinHandle::abort</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3934">#3934</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3934">#3934</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3934">tokio-rs/tokio#3934</a></p>
<h2>tokio-1.8.0</h2>
<h1>1.8.0 (July 2, 2021)</h1>
<h3>Added</h3>
<ul>
<li>io: add <code>get_{ref,mut}</code> methods to <code>AsyncFdReadyGuard</code> and <code>AsyncFdReadyMutGuard</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3807">#3807</a>)</li>
<li>io: efficient implementation of vectored writes for <code>BufWriter</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3163">#3163</a>)</li>
<li>net: add ready/try methods to <code>NamedPipe{Client,Server}</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3866">#3866</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3899">#3899</a>)</li>
<li>sync: add <code>watch::Receiver::borrow_and_update</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3813">#3813</a>)</li>
<li>sync: implement <code>From&lt;T&gt;</code> for <code>OnceCell&lt;T&gt;</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3877">#3877</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/2273eb1a1a9c9cfa2bd998c2215239e6fe1ed57a"><code>2273eb1</code></a> chore: fix CI on master (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4008">#4008</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/249f05c0bb6694bb111b4604541e38db840cd28c"><code>249f05c</code></a> chore: fix output of macro after new rustc release (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4189">#4189</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/2bf613206a29da5a5d262e0b44bb7fac1d40fa31"><code>2bf6132</code></a> macros: fix type resolution error in #[tokio::main] (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4176">#4176</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/c9228bf7513da8b2553788195190bfa25d546ef8"><code>c9228bf</code></a> macros: make tokio-macros attributes more IDE friendly (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4162">#4162</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/441427c99356192023cf896b6f8bb747af29223c"><code>441427c</code></a> macros: fix wrong error messages (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4067">#4067</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/cc7d9e1bbf0bb71bf90759d007ca143196a81823"><code>cc7d9e1</code></a> chore: explicitly relaxed clippy lint for runtime entry macro (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4030">#4030</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/f49b7fc6da7a6e76b40a12ffebddcd6de9987196"><code>f49b7fc</code></a> tokio-macros: compat with clippy::unwrap_used (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3926">#3926</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/ea87e4ec44c5c0530d5e6c29e7d09ba818e07b5b"><code>ea87e4e</code></a> net: fix the uds_datagram tests with the latest nightly stdlib (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3952">#3952</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/e2e7b5e0ade0aa499fdb9a808b07833643457f7b"><code>e2e7b5e</code></a> examples: replace time crate with httpdate (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4169">#4169</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9a58f7fbe76c72fdd70107223410bcf8106c3635"><code>9a58f7f</code></a> tests: update Nix to 0.22.0 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3951">#3951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-0.2.25...tokio-1.8.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=0.2.25&new-version=1.8.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-02 12:44:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/336" class=".btn">#336</a>
            </td>
            <td>
                <b>
                    Automated asset lock callback
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Description**: For Byzantine Swaps. Changes to AssetManager.ts regarding same-chain implementation of automated asset lock listener and its integration into createHTLC. Since we are unable to pass the proper preimage at this current implementation, could only test unlocking for now
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 08:37:21 +0000 UTC
    </div>
</div>

