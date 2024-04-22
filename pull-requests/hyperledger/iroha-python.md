---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    [ci]: Update branches triggers names
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
        Created At 2024-04-22 09:55:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    [fix] #172: Query Block Headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 07:38:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Bump eyre from 0.6.9 to 0.6.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [eyre](https://github.com/eyre-rs/eyre) from 0.6.9 to 0.6.12.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/eyre-rs/eyre/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=eyre&package-manager=cargo&previous-version=0.6.9&new-version=0.6.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 07:20:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Bump h2 from 0.3.22 to 0.3.26
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.22 to 0.3.26.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/releases">h2's releases</a>.</em></p>
<blockquote>
<h2>v0.3.26</h2>
<h2>What's Changed</h2>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<p>See <a href="https://seanmonstar.com/blog/hyper-http2-continuation-flood/">https://seanmonstar.com/blog/hyper-http2-continuation-flood/</a> for more info.</p>
<h2>v0.3.25</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: optimize header list size calculations by <a href="https://github.com/Noah-Kennedy"><code>@​Noah-Kennedy</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/750">hyperium/h2#750</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25">https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25</a></p>
<h2>v0.3.24</h2>
<h2>Fixed</h2>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h2>v0.3.23</h2>
<h2>What's Changed</h2>
<ul>
<li>cherry-pick fix: streams awaiting capacity lockout in <a href="https://redirect.github.com/hyperium/h2/pull/734">hyperium/h2#734</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/blob/v0.3.26/CHANGELOG.md">h2's changelog</a>.</em></p>
<blockquote>
<h1>0.3.26 (April 3, 2024)</h1>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<h1>0.3.25 (March 15, 2024)</h1>
<ul>
<li>Improve performance decoding many headers.</li>
</ul>
<h1>0.3.24 (January 17, 2024)</h1>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h1>0.3.23 (January 10, 2024)</h1>
<ul>
<li>Backport fix from 0.4.1 for stream capacity assignment.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/h2/commit/357127e279c06935830fe2140378312eac801494"><code>357127e</code></a> v0.3.26</li>
<li><a href="https://github.com/hyperium/h2/commit/1a357aaefc7243fdfa9442f45d90be17794a4004"><code>1a357aa</code></a> fix: limit number of CONTINUATION frames allowed</li>
<li><a href="https://github.com/hyperium/h2/commit/5b6c9e0da092728d702dff3607626aafb7809d77"><code>5b6c9e0</code></a> refactor: cleanup new unused warnings (<a href="https://redirect.github.com/hyperium/h2/issues/757">#757</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/3a798327211345b9b2bf797e2e4f3aca4e0ddfee"><code>3a79832</code></a> v0.3.25</li>
<li><a href="https://github.com/hyperium/h2/commit/94e80b1c72bec282bb5d13596803e6fb341fec4c"><code>94e80b1</code></a> perf: optimize header list size calculations (<a href="https://redirect.github.com/hyperium/h2/issues/750">#750</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/7243ab5854b2375213a5a2cdfd543f1d669661e2"><code>7243ab5</code></a> Prepare v0.3.24</li>
<li><a href="https://github.com/hyperium/h2/commit/d919cd6fd8e0f4f5d1f6282fab0b38a1b4bf999c"><code>d919cd6</code></a> streams: limit error resets for misbehaving connections</li>
<li><a href="https://github.com/hyperium/h2/commit/a7eb14a487c0094187314fca63cfe4de4d3d78ef"><code>a7eb14a</code></a> v0.3.23</li>
<li><a href="https://github.com/hyperium/h2/commit/b668c7fbe22e0cb4a76b0a67498cbb4d0aacbc75"><code>b668c7f</code></a> fix: streams awaiting capacity lockout (<a href="https://redirect.github.com/hyperium/h2/issues/730">#730</a>) (<a href="https://redirect.github.com/hyperium/h2/issues/734">#734</a>)</li>
<li>See full diff in <a href="https://github.com/hyperium/h2/compare/v0.3.22...v0.3.26">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.22&new-version=0.3.26)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 07:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    Bump zerocopy from 0.7.26 to 0.7.32
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [zerocopy](https://github.com/google/zerocopy) from 0.7.26 to 0.7.32.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/google/zerocopy/releases">zerocopy's releases</a>.</em></p>
<blockquote>
<h2>v0.7.32</h2>
<h2>What's Changed</h2>
<ul>
<li>[derive] Exclude large test files when publishing by <a href="https://github.com/joshlf"><code>@​joshlf</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/744">google/zerocopy#744</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/google/zerocopy/compare/v0.7.31...v0.7.32">https://github.com/google/zerocopy/compare/v0.7.31...v0.7.32</a></p>
<h2>v0.7.31</h2>
<p>This release fixes the soundness issue described in <a href="https://redirect.github.com/google/zerocopy/issues/716">#716</a>. The affected versions will soon be yanked.</p>
<p>This release is also described in security advisories <a href="https://rustsec.org/advisories/RUSTSEC-2023-0074.html">RUSTSEC-2023-0074</a> and <a href="https://github.com/google/zerocopy/security/advisories/GHSA-3mv5-343c-w2qg">GHSA-3mv5-343c-w2qg</a>.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix soundness hole in Ref::into_ref and into_mut by <a href="https://github.com/joshlf"><code>@​joshlf</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/721">google/zerocopy#721</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/google/zerocopy/compare/v0.7.30...v0.7.31">https://github.com/google/zerocopy/compare/v0.7.30...v0.7.31</a></p>
<h2>v0.7.30</h2>
<h2>What's Changed</h2>
<ul>
<li>[policies] Document yanking policy by <a href="https://github.com/joshlf"><code>@​joshlf</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/677">google/zerocopy#677</a></li>
<li>[ci] Roll pinned nightly toolchain by <a href="https://github.com/google-pr-creation-bot"><code>@​google-pr-creation-bot</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/680">google/zerocopy#680</a></li>
<li>[readme] Link to GitHub Releases (<a href="https://redirect.github.com/google/zerocopy/issues/692">#692</a>) by <a href="https://github.com/joshlf"><code>@​joshlf</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/693">google/zerocopy#693</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/google/zerocopy/compare/v0.7.29...v0.7.30">https://github.com/google/zerocopy/compare/v0.7.29...v0.7.30</a></p>
<h2>v0.7.29</h2>
<h2>What's Changed</h2>
<ul>
<li>[ci] Roll pinned nightly toolchain by <a href="https://github.com/google-pr-creation-bot"><code>@​google-pr-creation-bot</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/664">google/zerocopy#664</a></li>
<li>[ci] Roll pinned nightly toolchain by <a href="https://github.com/google-pr-creation-bot"><code>@​google-pr-creation-bot</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/668">google/zerocopy#668</a></li>
<li>[ci] Roll pinned nightly toolchain by <a href="https://github.com/google-pr-creation-bot"><code>@​google-pr-creation-bot</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/669">google/zerocopy#669</a></li>
<li>[ci] Roll pinned nightly toolchain by <a href="https://github.com/google-pr-creation-bot"><code>@​google-pr-creation-bot</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/670">google/zerocopy#670</a></li>
<li>Implement <code>TryFromBytes</code> for <code>[T]</code> by <a href="https://github.com/jswrenn"><code>@​jswrenn</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/666">google/zerocopy#666</a></li>
<li>[ci] Roll pinned nightly toolchain by <a href="https://github.com/google-pr-creation-bot"><code>@​google-pr-creation-bot</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/673">google/zerocopy#673</a></li>
<li>[derive] Fix AsBytes for <code>#[repr(C, packed(N))]</code> by <a href="https://github.com/maurer"><code>@​maurer</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/672">google/zerocopy#672</a></li>
<li>Release 0.7.29 by <a href="https://github.com/joshlf"><code>@​joshlf</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/676">google/zerocopy#676</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/google/zerocopy/compare/v0.7.28...v0.7.29">https://github.com/google/zerocopy/compare/v0.7.28...v0.7.29</a></p>
<h2>v0.7.28</h2>
<h2>What's Changed</h2>
<ul>
<li>Improve <code>transmute*!</code> documentation by <a href="https://github.com/jswrenn"><code>@​jswrenn</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/661">google/zerocopy#661</a></li>
<li>Improve <code>AsBytes</code> documentation by <a href="https://github.com/jswrenn"><code>@​jswrenn</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/660">google/zerocopy#660</a></li>
<li>[docs] Fix typo in include_value! doc comment by <a href="https://github.com/joshlf"><code>@​joshlf</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/662">google/zerocopy#662</a></li>
<li>Release 0.7.28 by <a href="https://github.com/joshlf"><code>@​joshlf</code></a> in <a href="https://redirect.github.com/google/zerocopy/pull/663">google/zerocopy#663</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/google/zerocopy/blob/main/CHANGELOG.md">zerocopy's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>Releases</h2>
<p>We track releases and release notes using <a href="https://github.com/google/zerocopy/releases">GitHub
Releases</a>.</p>
<h2>Yanks and Regressions</h2>
<h3>0.2.2 through 0.2.8, 0.3.0 through 0.3.1, 0.4.0, 0.5.0, 0.6.0 through 0.6.5, 0.7.0 through 0.7.30</h3>
<p><em>Security advisories for this bug have been published as
<a href="https://rustsec.org/advisories/RUSTSEC-2023-0074.html">RUSTSEC-2023-0074</a> and <a href="https://github.com/google/zerocopy/security/advisories/GHSA-3mv5-343c-w2qg">GHSA-3mv5-343c-w2qg</a>.</em></p>
<p>In these versions, the <code>Ref</code> methods <code>into_ref</code>, <code>into_mut</code>, <code>into_slice</code>, and
<code>into_mut_slice</code> were permitted in combination with the standard library
<code>cell::Ref</code> and <code>cell::RefMut</code> types for <code>Ref&lt;B, T&gt;</code>'s <code>B</code> type parameter. These
combinations are unsound, and may permit safe code to exhibit undefined
behavior. Fixes have been published to each affected minor version which do not
permit this code to compile.</p>
<p>See <a href="https://redirect.github.com/google/zerocopy/issues/716">#716</a><a href="https://redirect.github.com/google/zerocopy/issues/716">issue-716</a> for more details.</p>
<h3>0.7.27, 0.7.28</h3>
<p>These versions were briefly yanked due to a non-soundness regression reported in
<a href="https://redirect.github.com/google/zerocopy/issues/672">#672</a><a href="https://redirect.github.com/google/zerocopy/pull/672">pull-672</a>. After reconsidering our yanking policy in <a href="https://redirect.github.com/google/zerocopy/issues/679">#679</a><a href="https://redirect.github.com/google/zerocopy/issues/679">issue-679</a>,
we un-yanked these versions.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/google/zerocopy/commit/94b7e0a44d4e0a3d9ce8f6f56f901a4cf50fe4b6"><code>94b7e0a</code></a> [derive] Exclude large test files when publishing (<a href="https://redirect.github.com/google/zerocopy/issues/744">#744</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/7d3a8f9ea6bcf982ecd77db39a8be410b098232e"><code>7d3a8f9</code></a> Fix soundness hole in Ref::into_ref and into_mut (<a href="https://redirect.github.com/google/zerocopy/issues/721">#721</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/961612f110ca313eea06ca2563c88c83b51da492"><code>961612f</code></a> [readme] Link to GitHub Releases (<a href="https://redirect.github.com/google/zerocopy/issues/692">#692</a>) (<a href="https://redirect.github.com/google/zerocopy/issues/693">#693</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/449b78c67f20639d7dbe5d7b5a49c6dd7e9d175e"><code>449b78c</code></a> [ci] Roll pinned nightly toolchain (<a href="https://redirect.github.com/google/zerocopy/issues/680">#680</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/8f7d88b90ebdb1c644c58100a9953bf54f438ec5"><code>8f7d88b</code></a> [policies] Document yanking policy (<a href="https://redirect.github.com/google/zerocopy/issues/677">#677</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/5b76223e0eddea87e0f81429e218d12de94cd954"><code>5b76223</code></a> Release 0.7.29 (<a href="https://redirect.github.com/google/zerocopy/issues/676">#676</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/941c83fb4cea49dfac025a749653c6c3ea3fc019"><code>941c83f</code></a> [derive] Fix AsBytes for <code>#[repr(C, packed(N))]</code> (<a href="https://redirect.github.com/google/zerocopy/issues/672">#672</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/d18d233cf4e49d6abe15730eadb0e73a96f26ce2"><code>d18d233</code></a> [ci] Roll pinned nightly toolchain (<a href="https://redirect.github.com/google/zerocopy/issues/673">#673</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/ac0c27e77557779a9d1c79542a7cff7b29c59c69"><code>ac0c27e</code></a> implement <code>TryFromBytes</code> for <code>[T]</code> (<a href="https://redirect.github.com/google/zerocopy/issues/666">#666</a>)</li>
<li><a href="https://github.com/google/zerocopy/commit/122828ed8a360d9347ecd18989324020e79b81af"><code>122828e</code></a> [ci] Roll pinned nightly toolchain (<a href="https://redirect.github.com/google/zerocopy/issues/670">#670</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/google/zerocopy/compare/v0.7.26...v0.7.32">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zerocopy&package-manager=cargo&previous-version=0.7.26&new-version=0.7.32)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 07:20:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Bump mio from 0.8.9 to 0.8.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [mio](https://github.com/tokio-rs/mio) from 0.8.9 to 0.8.11.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/mio/blob/master/CHANGELOG.md">mio's changelog</a>.</em></p>
<blockquote>
<h1>0.8.11</h1>
<ul>
<li>Fix receiving IOCP events after deregistering a Windows named pipe
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1760">tokio-rs/mio#1760</a>, backport pr:
<a href="https://redirect.github.com/tokio-rs/mio/pull/1761">tokio-rs/mio#1761</a>).</li>
</ul>
<h1>0.8.10</h1>
<h2>Added</h2>
<ul>
<li>Solaris support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1724">tokio-rs/mio#1724</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/mio/commit/0328bdef900b6396b8d00d33c825cd8af748553d"><code>0328bde</code></a> Release v0.8.11</li>
<li><a href="https://github.com/tokio-rs/mio/commit/708449851283b57eb6f514c8f289b66e982720b3"><code>7084498</code></a> Fix warnings</li>
<li><a href="https://github.com/tokio-rs/mio/commit/90d4fe00df870acd3d38f3dc4face9aacab8fbb9"><code>90d4fe0</code></a> named-pipes: fix receiving IOCP events after deregister</li>
<li><a href="https://github.com/tokio-rs/mio/commit/c710a307f8627c4d63ac1003252aa45175e08399"><code>c710a30</code></a> Add v0.8.x to the CI</li>
<li><a href="https://github.com/tokio-rs/mio/commit/c29e21c244b2b835e8b3e015b92c708c33c7d70a"><code>c29e21c</code></a> Release v0.8.10</li>
<li><a href="https://github.com/tokio-rs/mio/commit/f6a20da1c81c2d56a78bc6f6832b9904b9215914"><code>f6a20da</code></a> Add Solaris operating system support (<a href="https://redirect.github.com/tokio-rs/mio/issues/1724">#1724</a>)</li>
<li>See full diff in <a href="https://github.com/tokio-rs/mio/compare/v0.8.9...v0.8.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mio&package-manager=cargo&previous-version=0.8.9&new-version=0.8.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 07:20:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/174" class=".btn">#174</a>
            </td>
            <td>
                <b>
                    [fix] Fix malformed link in README
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
        Created At 2024-04-17 14:20:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    [chore] Update Iroha version to 1.6 in README
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
        Created At 2024-04-17 06:23:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/171" class=".btn">#171</a>
            </td>
            <td>
                <b>
                    [refactor] add query_all_asset_definitions and more tests
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
        Created At 2024-04-15 19:01:05 +0000 UTC
    </div>
</div>

