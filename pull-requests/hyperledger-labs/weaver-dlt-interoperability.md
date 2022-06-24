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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    Base Structure for Identity Services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Build the skeleton folder structure for the various decentralized identity components needed for interoperation.
Built the base server logic for IIN Agents with build scripts.
Minor updates to documentation and minor typo fixes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 14:42:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Bump smallvec from 1.4.0 to 1.8.0 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [smallvec](https://github.com/servo/rust-smallvec) from 1.4.0 to 1.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/servo/rust-smallvec/releases">smallvec's releases</a>.</em></p>
<blockquote>
<h2>v1.8.0</h2>
<ul>
<li>Add optional support for the <code>arbitrary</code> crate (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/275">#275</a>).</li>
</ul>
<h2>v1.7.0</h2>
<ul>
<li><code>new_const</code> and <code>from_const</code> constructors for creating a SmallVec in <code>const</code> contexts.  Requires Rust 1.51 and the optional <code>const_new</code> feature.  (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/265">#265</a>)</li>
</ul>
<h2>v1.6.1</h2>
<ul>
<li>Fix a possible buffer overflow in <code>insert_many</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/252">#252</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/254">#254</a>).</li>
</ul>
<h2>v1.6.0</h2>
<ul>
<li>The <code>&quot;union&quot;</code> feature is now compatible with stable Rust 1.49 (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/248">#248</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/247">#247</a>).</li>
<li>Fixed warnings when compiling with Rust 1.51 nightly (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/242">#242</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/246">#246</a>).</li>
</ul>
<h2>v1.5.1</h2>
<ul>
<li>Improve performance of <code>push</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/241">#241</a>).</li>
</ul>
<h2>v1.5.0</h2>
<ul>
<li>Add the <code>append</code> method (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/237">#237</a>).</li>
<li>Add support for more array sizes between 17 and 31 (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/234">#234</a>).</li>
<li>Don't panic on deserialization errors (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/238">#238</a>).</li>
</ul>
<h2>v1.4.2</h2>
<ul>
<li><code>insert_many</code> no longer leaks elements if the provided iterator panics (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/213">#213</a>).</li>
<li>The unstable <code>const_generics</code> and <code>specialization</code> features are updated to work with the most recent nightly Rust toolchain (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/232">#232</a>).</li>
<li>Internal code cleanup (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/229">#229</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/231">#231</a>).</li>
</ul>
<h2>v1.4.1</h2>
<ul>
<li>Don't allocate when the size of the element type is zero. Allocating zero bytes is undefined behavior. (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/228">#228</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/servo/rust-smallvec/commit/0a4fdff3b012ed4d4b603800bf971239e5a966ba"><code>0a4fdff</code></a> Version 1.8.0</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/6d0dea5bc4e26dad163ce5d92a387f5a13f8d4b5"><code>6d0dea5</code></a> Auto merge of <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/275">#275</a> - as-com:arbitrary-support, r=mbrubeck</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/9bcd950f253d8eaed9173bee77cb46caee171460"><code>9bcd950</code></a> Add support for arbitrary</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/7cbb3b1fa1c45b008fded551d47b51101ae7ff14"><code>7cbb3b1</code></a> Auto merge of <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/271">#271</a> - saethlin:drain-aliasing-test, r=jdm</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/0fced9d92e61c91a3f8b33bc7cdf0dc67137ce2d"><code>0fced9d</code></a> Test for drains that shift the tail, when inline</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/218e0bb00548050146adea58f2a96aab32bc4e54"><code>218e0bb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/270">#270</a> from servo/github-actions</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/52c50af7dae393f325bdcb4f63e7a2be92ba49cd"><code>52c50af</code></a> Replace TravisCI with Github Actions.</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/5ae217a899b82ee0d7c190bfe722e2c68e4539a9"><code>5ae217a</code></a> Include the cost of shifts in insert/remove benchmarks (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/268">#268</a>)</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/58edc0e53876c35d160acf99a60de8a564eeec2b"><code>58edc0e</code></a> Version 1.7.0</li>
<li><a href="https://github.com/servo/rust-smallvec/commit/1e4b15181037584bbb273d74f30bf47ac37d042d"><code>1e4b151</code></a> Added feature <code>const_new</code> which enables <code>SmallVec::new_const()</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/265">#265</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/servo/rust-smallvec/compare/v1.4.0...v1.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smallvec&package-manager=cargo&previous-version=1.4.0&new-version=1.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-17 01:34:26 +0000 UTC
    </div>
</div>

