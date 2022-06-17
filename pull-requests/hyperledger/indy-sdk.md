---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2542" class=".btn">#2542</a>
            </td>
            <td>
                <b>
                    Bump thread_local from 1.0.1 to 1.1.4 in /libindy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [thread_local](https://github.com/Amanieu/thread_local-rs) from 1.0.1 to 1.1.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/4a54e5702e0968bdda77366738ba646f646044e8"><code>4a54e57</code></a> Bump version to 1.1.4</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/ebf8b45fa2b427ede21b75d263a8c99150526dd1"><code>ebf8b45</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/34">#34</a> from ibraheemdev/patch-1</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/3d69afaab242fc1dd3a0658eb363b2df5e02fcd6"><code>3d69afa</code></a> Fix memory ordering in <code>RawIter::next</code></li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/c7d8dcdf4b93a5d80ec4075c3d8e7351c1a32012"><code>c7d8dcd</code></a> Bump version to 1.1.3</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/5e8bbf2b4f17d9c056d17de324d5a8465d20f96e"><code>5e8bbf2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/30">#30</a> from Marwes/fix_drop</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/a44b836f90e0317d256ed1dd4cff745feff285ea"><code>a44b836</code></a> fix: Drop the value in the ThreadLocal on drop</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/322cf34816a62f1519d005cc44d623741740324e"><code>322cf34</code></a> Bump version to 1.1.2</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/dca4007eafb16fe189caea4fe08a6b80223b3fb1"><code>dca4007</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/29">#29</a> from Kestrer/raw-iter</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/33ad4052309ba8b48b7436bf82d66be07103fa3f"><code>33ad405</code></a> Add #[inline] to non-generic functions</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/810c043ff71ef66b96ca5d92319df4aa7134bf44"><code>810c043</code></a> Implement iterator logic in RawIter</li>
<li>Additional commits viewable in <a href="https://github.com/Amanieu/thread_local-rs/compare/v1.0.1...1.1.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=thread_local&package-manager=cargo&previous-version=1.0.1&new-version=1.1.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:34:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2541" class=".btn">#2541</a>
            </td>
            <td>
                <b>
                    Bump thread_local from 1.0.1 to 1.1.4 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [thread_local](https://github.com/Amanieu/thread_local-rs) from 1.0.1 to 1.1.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/4a54e5702e0968bdda77366738ba646f646044e8"><code>4a54e57</code></a> Bump version to 1.1.4</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/ebf8b45fa2b427ede21b75d263a8c99150526dd1"><code>ebf8b45</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/34">#34</a> from ibraheemdev/patch-1</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/3d69afaab242fc1dd3a0658eb363b2df5e02fcd6"><code>3d69afa</code></a> Fix memory ordering in <code>RawIter::next</code></li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/c7d8dcdf4b93a5d80ec4075c3d8e7351c1a32012"><code>c7d8dcd</code></a> Bump version to 1.1.3</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/5e8bbf2b4f17d9c056d17de324d5a8465d20f96e"><code>5e8bbf2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/30">#30</a> from Marwes/fix_drop</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/a44b836f90e0317d256ed1dd4cff745feff285ea"><code>a44b836</code></a> fix: Drop the value in the ThreadLocal on drop</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/322cf34816a62f1519d005cc44d623741740324e"><code>322cf34</code></a> Bump version to 1.1.2</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/dca4007eafb16fe189caea4fe08a6b80223b3fb1"><code>dca4007</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/29">#29</a> from Kestrer/raw-iter</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/33ad4052309ba8b48b7436bf82d66be07103fa3f"><code>33ad405</code></a> Add #[inline] to non-generic functions</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/810c043ff71ef66b96ca5d92319df4aa7134bf44"><code>810c043</code></a> Implement iterator logic in RawIter</li>
<li>Additional commits viewable in <a href="https://github.com/Amanieu/thread_local-rs/compare/v1.0.1...1.1.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=thread_local&package-manager=cargo&previous-version=1.0.1&new-version=1.1.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2540" class=".btn">#2540</a>
            </td>
            <td>
                <b>
                    Bump smallvec from 0.6.13 to 0.6.14 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [smallvec](https://github.com/servo/rust-smallvec) from 0.6.13 to 0.6.14.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/servo/rust-smallvec/releases">smallvec's releases</a>.</em></p>
<blockquote>
<h2>v0.6.14</h2>
<ul>
<li>Fix a possible buffer overflow in <code>insert_many</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/252">#252</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/254">#254</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/servo/rust-smallvec/commit/5757ac500d4e544485d796b542e4e589749c291b"><code>5757ac5</code></a> Fix potential buffer overflow in <code>insert_many</code></li>
<li>See full diff in <a href="https://github.com/servo/rust-smallvec/compare/v0.6.13...v0.6.14">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smallvec&package-manager=cargo&previous-version=0.6.13&new-version=0.6.14)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:26:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2539" class=".btn">#2539</a>
            </td>
            <td>
                <b>
                    Bump smallvec from 1.0.0 to 1.8.0 in /experimental/plugins/postgres_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [smallvec](https://github.com/servo/rust-smallvec) from 1.0.0 to 1.8.0.
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
<h2>v1.4.0</h2>
<ul>
<li>Add <code>try_reserve</code>, <code>try_reserve_exact</code>, and <code>try_grow</code> methods (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/214">#214</a>).</li>
</ul>
<h2>v1.3.0</h2>
<ul>
<li>Add a new unstable <code>const_generics</code> feature (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/204">#204</a>).</li>
<li>Improve inlining of constructor functions (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/206">#206</a>).</li>
<li>Add a <code>slice.to_smallvec()</code> convenience method (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/203">#203</a>).</li>
<li>Documentation and testing improvements.</li>
</ul>
<h2>v1.2.0</h2>
<ul>
<li><code>IntoIter</code> now implements <code>Debug</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/196">#196</a>).</li>
<li><code>smallvec!</code> macro is now easier to use in <code>no_std</code> contexts where the <code>vec!</code> macro isn't automatically imported (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/198">#198</a>).</li>
</ul>
<h2>v1.1.0</h2>
<ul>
<li>Added new method <code>SmallVec::into_boxed_slice</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/190">#190</a>).</li>
<li>Added new methods <code>IntoIter::as_slice</code> and <code>as_mut_slice</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/182">#182</a>).</li>
<li><code>IntoIter</code> now implements <code>Clone</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/192">#192</a>).</li>
<li>Improved documentation and testing (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/186">#186</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/189">#189</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/193">#193</a>).</li>
<li>Minor code cleanups (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/176">#176</a>).</li>
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
<li>Additional commits viewable in <a href="https://github.com/servo/rust-smallvec/compare/v1.0.0...v1.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smallvec&package-manager=cargo&previous-version=1.0.0&new-version=1.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:25:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2538" class=".btn">#2538</a>
            </td>
            <td>
                <b>
                    Bump smallvec from 0.6.13 to 0.6.14 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [smallvec](https://github.com/servo/rust-smallvec) from 0.6.13 to 0.6.14.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/servo/rust-smallvec/releases">smallvec's releases</a>.</em></p>
<blockquote>
<h2>v0.6.14</h2>
<ul>
<li>Fix a possible buffer overflow in <code>insert_many</code> (<a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/252">#252</a>, <a href="https://github-redirect.dependabot.com/servo/rust-smallvec/issues/254">#254</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/servo/rust-smallvec/commit/5757ac500d4e544485d796b542e4e589749c291b"><code>5757ac5</code></a> Fix potential buffer overflow in <code>insert_many</code></li>
<li>See full diff in <a href="https://github.com/servo/rust-smallvec/compare/v0.6.13...v0.6.14">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smallvec&package-manager=cargo&previous-version=0.6.13&new-version=0.6.14)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2537" class=".btn">#2537</a>
            </td>
            <td>
                <b>
                    Bump crossbeam-queue from 0.2.1 to 0.2.3 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [crossbeam-queue](https://github.com/crossbeam-rs/crossbeam) from 0.2.1 to 0.2.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/149a3c93895538080fb4cc2884def30111059ffc"><code>149a3c9</code></a> Release crossbeam-queue 0.2.3</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/18363b5b3e063a940db92c54fdb6f4a0538413f4"><code>18363b5</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/476">#476</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/e32c891f376332828852fa2eb5626a831b395e28"><code>e32c891</code></a> Release new versions</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/6d6591a0e1c4d1d540d7289d27c21ec7f1689aa6"><code>6d6591a</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/474">#474</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/528c3caadb2f4f5f0d0327de35404ad077636345"><code>528c3ca</code></a> Undo bump of rand as it bumps MSRV</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/78043c7b11f7c576d5f587d4eae0798886df670d"><code>78043c7</code></a> Bump crossbeam to 0.7.4</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/640cec2f4bc29f597a15e1919225ff7716aad0fd"><code>640cec2</code></a> Bump crossbeam-deque to 0.7.3</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/e962784d97e06fcc4ea406ed0a49141c86b67a94"><code>e962784</code></a> Bump crossbeam-queue to 0.2.2</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/64ad929c5d9aac7f218f7c90ce4b8f8270ac3254"><code>64ad929</code></a> Bump crossbeam-epoch to 0.8.1</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/909edf53dacbe78bf28114e34741d06011a0c7c7"><code>909edf5</code></a> Bump crossbeam-channel to 0.4.1</li>
<li>Additional commits viewable in <a href="https://github.com/crossbeam-rs/crossbeam/compare/crossbeam-queue-0.2.1...crossbeam-queue-0.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=crossbeam-queue&package-manager=cargo&previous-version=0.2.1&new-version=0.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 00:38:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2536" class=".btn">#2536</a>
            </td>
            <td>
                <b>
                    Bump arc-swap from 0.4.4 to 0.4.8 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [arc-swap](https://github.com/vorner/arc-swap) from 0.4.4 to 0.4.8.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vorner/arc-swap/blob/v0.4.8/CHANGELOG.md">arc-swap's changelog</a>.</em></p>
<blockquote>
<h1>0.4.8</h1>
<ul>
<li>Backport of fix to soundness issue in <a href="https://github-redirect.dependabot.com/vorner/arc-swap/issues/45">#45</a> (access::Map from Constant can lead
to dangling references).</li>
</ul>
<h1>0.4.7</h1>
<ul>
<li>Rename the <code>unstable-weak</code> to <code>weak</code> feature. The support is now available on
1.45 (currently in beta).</li>
</ul>
<h1>0.4.6</h1>
<ul>
<li>Adjust to <code>Weak::as_ptr</code> from std (the weak pointer support, relying on
unstable features).</li>
<li>Support running on miri (without some optimizations), so dependencies may run
miri tests.</li>
<li>Little optimization when waiting out the contention on write operations.</li>
</ul>
<h1>0.4.5</h1>
<ul>
<li>Added <code>Guard::from_inner</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vorner/arc-swap/commit/34b809fbd0db89206ddb91afc4ee8b7fc7de3b3b"><code>34b809f</code></a> Fix soundness hole around access::Map</li>
<li><a href="https://github.com/vorner/arc-swap/commit/77b5be77687cd9431f45b09fff92312717a92cf8"><code>77b5be7</code></a> Release 0.4.7</li>
<li><a href="https://github.com/vorner/arc-swap/commit/1cd19c3b7d624778daf25e63f98f906ff40c6ea0"><code>1cd19c3</code></a> Stabilized weak support</li>
<li><a href="https://github.com/vorner/arc-swap/commit/ee8b86e71be7938aaf224ef36898ae9ef59936a1"><code>ee8b86e</code></a> Lint management</li>
<li><a href="https://github.com/vorner/arc-swap/commit/315f73bcce427c9bb2c795f28ac7807b99b4ae24"><code>315f73b</code></a> Version 0.4.6</li>
<li><a href="https://github.com/vorner/arc-swap/commit/005ec4569fde7132a0fcb669858eb5df8abee905"><code>005ec45</code></a> Merge branch 'miri'</li>
<li><a href="https://github.com/vorner/arc-swap/commit/8a93bb50a59f40042d66768e919a6e9135ec0db3"><code>8a93bb5</code></a> Update the weak ptr support for newer Rust</li>
<li><a href="https://github.com/vorner/arc-swap/commit/88fc681bced3f258f2da152abe1d49d8a9615c95"><code>88fc681</code></a> Some trivial version updates</li>
<li><a href="https://github.com/vorner/arc-swap/commit/e3f85385bb726ff371723a24ea06214a81b39753"><code>e3f8538</code></a> Get rid of the model dependency</li>
<li><a href="https://github.com/vorner/arc-swap/commit/09cb648b508226aefcadcd81a22f1cbb242194b5"><code>09cb648</code></a> Don't run pause/yield in the last iteration of wait_for_readers</li>
<li>Additional commits viewable in <a href="https://github.com/vorner/arc-swap/compare/v0.4.4...v0.4.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=arc-swap&package-manager=cargo&previous-version=0.4.4&new-version=0.4.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 23:52:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2533" class=".btn">#2533</a>
            </td>
            <td>
                <b>
                    Bump net2 from 0.2.33 to 0.2.37 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [net2](https://github.com/deprecrated/net2-rs) from 0.2.33 to 0.2.37.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/deprecrated/net2-rs/commit/a18347549413975fbbeb5567165f163e5f60a627"><code>a183475</code></a> Release v0.2.37</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/6081dff94aa3128f0742c24e3925a6f8e7f5de53"><code>6081dff</code></a> haiku: Fix sockaddr_in/sockaddr_in6; Solves <a href="https://github-redirect.dependabot.com/deprecrated/net2-rs/issues/108">#108</a></li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/71708b75d672f5f2430a1edb326d67ed14d87a51"><code>71708b7</code></a> Release v0.2.36</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/49b43f277afb1caf5104fcbe02bef581f7444686"><code>49b43f2</code></a> Do not assume memory layout of std::net::SocketAddr</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/77a6eb4d5eb36adc81ee21ab7ffebc62fdf2ab88"><code>77a6eb4</code></a> Release v0.2.35</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/eeeab131cb52790df3bedeac46e889feab8f83e3"><code>eeeab13</code></a> Add support for Haiku</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/1e915300a495b47f20e93d9b67e1740e84a339a7"><code>1e91530</code></a> Release v0.2.34</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/89945ebc27f3dbbc7782269aae40651f143bde55"><code>89945eb</code></a> Make cargo packaging explicit</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/fe62962c1b843778887970197779c11498648b7b"><code>fe62962</code></a> Clean up trailing whitespace</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/67ec2c12116d71d89f4111730c40e0f0c6e1168c"><code>67ec2c1</code></a> Update URLs in Cargo.toml</li>
<li>Additional commits viewable in <a href="https://github.com/deprecrated/net2-rs/compare/0.2.33...0.2.37">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=net2&package-manager=cargo&previous-version=0.2.33&new-version=0.2.37)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 23:47:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2532" class=".btn">#2532</a>
            </td>
            <td>
                <b>
                    Bump net2 from 0.2.34 to 0.2.37 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [net2](https://github.com/deprecrated/net2-rs) from 0.2.34 to 0.2.37.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/deprecrated/net2-rs/commit/a18347549413975fbbeb5567165f163e5f60a627"><code>a183475</code></a> Release v0.2.37</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/6081dff94aa3128f0742c24e3925a6f8e7f5de53"><code>6081dff</code></a> haiku: Fix sockaddr_in/sockaddr_in6; Solves <a href="https://github-redirect.dependabot.com/deprecrated/net2-rs/issues/108">#108</a></li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/71708b75d672f5f2430a1edb326d67ed14d87a51"><code>71708b7</code></a> Release v0.2.36</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/49b43f277afb1caf5104fcbe02bef581f7444686"><code>49b43f2</code></a> Do not assume memory layout of std::net::SocketAddr</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/77a6eb4d5eb36adc81ee21ab7ffebc62fdf2ab88"><code>77a6eb4</code></a> Release v0.2.35</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/eeeab131cb52790df3bedeac46e889feab8f83e3"><code>eeeab13</code></a> Add support for Haiku</li>
<li>See full diff in <a href="https://github.com/deprecrated/net2-rs/compare/0.2.34...0.2.37">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=net2&package-manager=cargo&previous-version=0.2.34&new-version=0.2.37)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 23:43:30 +0000 UTC
    </div>
</div>

