---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/72" class=".btn">#72</a>
            </td>
            <td>
                <b>
                    Add show modules command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-07 11:14:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Fix bin name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-07 10:38:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    develop -> main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - https://github.com/hyperledger-labs/yui-relayer/pull/68 
- https://github.com/hyperledger-labs/yui-relayer/pull/71
- https://github.com/hyperledger-labs/yui-relayer/pull/72
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 08:24:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    Remove chain modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - removes chain modules(fabric, ethereum and corda)
- update go version to v1.18
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 08:23:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    build(deps): bump shell-quote from 1.7.2 to 1.7.3 in /tests/chains/ethereum/contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/substack/node-shell-quote) from 1.7.2 to 1.7.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/substack/node-shell-quote/blob/master/CHANGELOG.md">shell-quote's changelog</a>.</em></p>
<blockquote>
<h2>1.7.3</h2>
<ul>
<li>Fix a security issue where the regex for windows drive letters allowed some shell meta-characters
to escape the quoting rules. (CVE-2021-42740)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/node-shell-quote/commit/6a8a899c62a58a30fb128a7079f02826ed4faee0"><code>6a8a899</code></a> 1.7.3</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/5799416ed454aa4ec9afafc895b4e31760ea1abe"><code>5799416</code></a> fix for security issue with windows drive letter regex</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/c7de931fa4ed0975ea9756983c88334fe4b8cde5"><code>c7de931</code></a> Add security.md</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/414853f1fd98553368ce7507cd26ebae88d71b46"><code>414853f</code></a> Update readme.markdown (<a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/43">#43</a>)</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/0fc4a978131ab68cace9c9a57cee245b6b70e595"><code>0fc4a97</code></a> use Github Actions (<a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/42">#42</a>)</li>
<li>See full diff in <a href="https://github.com/substack/node-shell-quote/compare/v1.7.2...1.7.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=shell-quote&package-manager=npm_and_yarn&previous-version=1.7.2&new-version=1.7.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-relayer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 01:59:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    build(deps): bump github.com/ethereum/go-ethereum from 1.9.25 to 1.10.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.9.25 to 1.10.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Ploitari (v1.10.17)</h2>
<p>This is a maintenance release. This release contains a lot of work in preparation for The Merge, and work for an upcoming change to the way state is stored in go-ethereum.</p>
<p>This release also adds a new tool to convert 'legacy' receipts into a newer format. During startup, geth will check the database and tell you if you need to perform the conversion. Converting receipts is only needed if geth's <code>ancients</code> database has not been resynced from scratch during the last couple of years. It is recommended to back-up your receipts freezer table (<code>ancients/receipts*</code>) before performing the conversion.</p>
<p>Compatibility note about <code>core/types</code>: For optimization purposes, <code>types.Header</code> and other types in this package now implement the <code>rlp.Encoder</code> interface. This change can cause incompatibilities because the new method is implemented with pointer receiver. Attempting to RLP-encode unadressable (i.e. non-pointer) values of type <code>Header</code> does not work anymore and will result in an error.</p>
<h3>Change Log</h3>
<ul>
<li>A lot of work towards &quot;The Merge&quot; (TM) was performed (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24574">#24574</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24569">#24569</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24550">#24550</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24548">#24548</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24506">#24506</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24545">#24545</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23982">#23982</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24522">#24522</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24364">#24364</a>)</li>
<li>A lot optimizations for RLP encoding and package trie were added (roughly 20-30% improvement) (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24126">#24126</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24425">#24425</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24420">#24420</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24251">#24251</a>)</li>
<li>Preparatory work for an upcoming for state layout change (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24460">#24460</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23954">#23954</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24486">#24486</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24391">#24391</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24392">#24392</a>)</li>
<li>GraphQL: fee history API methods were added, along with nonce for pending accounts (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24452">#24452</a>)</li>
<li>The non-cgo fallback secp256k1 crypto library was updated and is now ~25% faster (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24533">#24533</a>)</li>
<li>Support for signing nested types via <code>clef</code> (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24407">#24407</a>)</li>
<li>Receipt converter tool (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24028">#24028</a>)</li>
<li>Our builds were updated to use Go 1.18</li>
</ul>
<p>For a full rundown of the changes please consult the Geth 1.10.17 <a href="https://github.com/ethereum/go-ethereum/milestone/129?closed=1">release milestone</a>.</p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
<li>OSX packages in our <a href="https://github.com/ethereum/homebrew-ethereum">Homebrew Tap repository</a>.</li>
</ul>
<h2>Osun (v1.10.16)</h2>
<p>The focus of this release is bugfixes.</p>
<h4>Bugfixes</h4>
<ul>
<li>Block tracing via <code>debug.traceBlockByHash</code> has sometimes produced inconsistent/corrupt results. Fixed via (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24286">#24286</a>).</li>
<li>The <code>--whitelist</code> CLI parameter functionality was broken in <code>v1.10.14</code>, and is fixed in this release (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24210">#24210</a>).</li>
<li>A bug was introduced, and subsequently fixed, which could cause data corruption during mining (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24349">#24349</a>).</li>
<li>When signing complex datatypes in EIP712-type data, the signing-hash was incorrect. Fixed via (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24220">#24220</a>).</li>
<li>Evm execution times exported via <code>metrics</code>, were sometimes incorrect. Fixed in (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24304">#24304</a>).</li>
<li>Range prover edgecases found and fixed (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24266">#24266</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24257">#24257</a>).</li>
<li>Fix an error related to <code>HTTP2</code> handling (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24292">#24292</a>).</li>
<li>A lot of spleling-mistkaes and issues related to correctness were fixed (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24194">#24194</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24196">#24196</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24198">#24198</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24205">#24205</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24207">#24207</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24244">#24244</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24270">#24270</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24271">#24271</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24224">#24224</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24372">#24372</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24323">#24323</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24289">#24289</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24263">#24263</a> and <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24211">#24211</a>).</li>
</ul>
<h4>New features</h4>
<ul>
<li>Work on The Merge includes support for <code>RANDOM</code> opcode (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24141">#24141</a>) and various other internal refactorings (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24328">#24328</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24280">#24280</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24236">#24236</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23256">#23256</a>).</li>
<li>The <code>devp2p</code> binary now supports doing <code>snap/v1</code> protocol testing against a remote node, which can be used for Hive-testing (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24276">#24276</a>).</li>
<li>New diagnostic command to show database metadata (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23900">#23900</a>)</li>
<li><code>ethclient</code> support for <code>CallContractAtHash</code> (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24355">#24355</a>).</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/25c9b49fdb74931137431c24cf28d3c65f9420d2"><code>25c9b49</code></a> params: go-ethereum v1.10.17 stable</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/de6a113f843822165b7fb26eb4147e493ce5d8b2"><code>de6a113</code></a> eth/catalyst: only apply block if we actually have the state (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/24598">#24598</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/b502b6ac977a4e13e4255b5b71bdbd3aef608f4b"><code>b502b6a</code></a> cmd/geth: change to non-fatal error message when legacy receipt storage is no...</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/1027cb52c4068931ef67d7ad8c9ebd4c7a766112"><code>1027cb5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/24605">#24605</a> from karalabe/revert-setting-ttd</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/b06e8c4a8a12a9cdfa7ac8dc7fd5f6d15cf089d1"><code>b06e8c4</code></a> core/vm: fix sstore gas comment type (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/24583">#24583</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/b45d82e94ad2695831d63a11a64c2bcc8d5a8576"><code>b45d82e</code></a> core: set ttd override on all chain variations</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/0fffd3acbdc5c8f83a27b001623769cb73c5d231"><code>0fffd3a</code></a> build: close sftp connection when done (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/24593">#24593</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/eb3ebceaa112dc62bbe5751e721c1d6c90bc50fb"><code>eb3ebce</code></a> internal/build: exit sftp upload (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/24590">#24590</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/d1c243f84100f7d5e2291ec0e731c54b0ec9d2be"><code>d1c243f</code></a> internal/build: prevent travis timeout during ppa upload (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/24589">#24589</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/19b9cf714ff1aeb044e67e8eb8f1e3cb4f965e7d"><code>19b9cf7</code></a> internal/build: show ppa upload process stdout on stdout (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/24588">#24588</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.9.25...v1.10.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.9.25&new-version=1.10.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-relayer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 01:59:54 +0000 UTC
    </div>
</div>

