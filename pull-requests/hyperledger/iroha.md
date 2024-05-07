---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4566" class=".btn">#4566</a>
            </td>
            <td>
                <b>
                    chore(deps): bump trybuild from 1.0.91 to 1.0.94
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [trybuild](https://github.com/dtolnay/trybuild) from 1.0.91 to 1.0.94.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/trybuild/releases">trybuild's releases</a>.</em></p>
<blockquote>
<h2>1.0.94</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/dtolnay/trybuild/issues/268">#268</a>)</li>
</ul>
<h2>1.0.93</h2>
<ul>
<li>Remove dependency on <code>once_cell</code> crate (<a href="https://redirect.github.com/dtolnay/trybuild/issues/266">#266</a>, thanks <a href="https://github.com/taiki-e"><code>@​taiki-e</code></a>)</li>
</ul>
<h2>1.0.92</h2>
<ul>
<li>Update normalization of verbose type paths to accommodate error message changes in rust 1.78 (<a href="https://redirect.github.com/dtolnay/trybuild/issues/265">#265</a>, thanks <a href="https://github.com/weiznich"><code>@​weiznich</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/trybuild/commit/9ed763b56f204ecc2624657016c12aeae3d26920"><code>9ed763b</code></a> Release 1.0.94</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/b3c948124251872bc3111d2cf2938ae044e9e9d1"><code>b3c9481</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/268">#268</a> from dtolnay/checkcfg</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/7bb6f2fb22f39744771fa229740d8e023c67e424"><code>7bb6f2f</code></a> Resolve unexpected_cfgs warning</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/8a57d8c2eb84241a5986f11cb99621d8a59ce65e"><code>8a57d8c</code></a> Release 1.0.93</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/b9888357069e2cbc24a752ad5c7c125f60d178ac"><code>b988835</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/267">#267</a> from dtolnay/constmutex</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/95f8cdbd329c1c46d1a413faf3622053838eaa4d"><code>95f8cdb</code></a> Remove OnceLock around intra-process lock's mutex</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/62b1543732bb61ac0cba28d90cc5b17826ebe780"><code>62b1543</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/266">#266</a> from taiki-e/once_cell</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/f8795cf667dec726e3884eccf1b3a3d401726b8d"><code>f8795cf</code></a> Remove dependency on once_cell</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/5fb7caeccc5a1fea9b834659f84658cfa4bfa551"><code>5fb7cae</code></a> Release 1.0.92</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/bbe5be02f83ede9aa2ac096689837ba5b12601fd"><code>bbe5be0</code></a> Merge pull request 265 from weiznich/fix/paths_with_rust_1.78</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/trybuild/compare/1.0.91...1.0.94">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=trybuild&package-manager=cargo&previous-version=1.0.91&new-version=1.0.94)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 16:39:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4565" class=".btn">#4565</a>
            </td>
            <td>
                <b>
                    chore(deps): bump anyhow from 1.0.82 to 1.0.83
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [anyhow](https://github.com/dtolnay/anyhow) from 1.0.82 to 1.0.83.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/anyhow/releases">anyhow's releases</a>.</em></p>
<blockquote>
<h2>1.0.83</h2>
<ul>
<li>Integrate compile-time checking of cfgs (<a href="https://redirect.github.com/dtolnay/anyhow/issues/363">#363</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/anyhow/commit/96f039226221ce615fabda347efaecd66bd441aa"><code>96f0392</code></a> Release 1.0.83</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/17bbd1e2adb003fa0cba5be66e1f1c3874d15a5e"><code>17bbd1e</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/anyhow/issues/363">#363</a> from dtolnay/checkcfg</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/3ab3c3bca258c4e86ddedf1c33bd8f06f6e2db27"><code>3ab3c3b</code></a> Resolve unexpected_cfgs warning</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/8e62244b25b99cca2c00ece065a719438ca55e87"><code>8e62244</code></a> Discard CI coverage of backtrace feature on toolchains older than 1.63</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/e77374f1edff6f133e912400bbafa09dc7c64db4"><code>e77374f</code></a> Mirror PR 343 changes from readme to rustdoc</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/cb47d7c31a3f28eaa08fe936d0bd58b7a7ab738a"><code>cb47d7c</code></a> Reword no-std documentation change from PR 343</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/6b5bdb17b6df2816ddf7d525dd583f6c968e7f7f"><code>6b5bdb1</code></a> Wrap PR 343 to 80 columns</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/f01080beafaccb1f293db41f7ae8e5688723afe8"><code>f01080b</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/anyhow/issues/343">#343</a> from Arthur-Milchior/readme1</li>
<li>See full diff in <a href="https://github.com/dtolnay/anyhow/compare/1.0.82...1.0.83">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=anyhow&package-manager=cargo&previous-version=1.0.82&new-version=1.0.83)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 16:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4564" class=".btn">#4564</a>
            </td>
            <td>
                <b>
                    test: Add torii api tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 14:32:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4560" class=".btn">#4560</a>
            </td>
            <td>
                <b>
                    chore(deps): bump cryptography from 42.0.3 to 42.0.7 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.3 to 42.0.7.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.7 - 2024-05-06</p>
<pre><code>
* Restored Windows 7 compatibility for our pre-built wheels. Note that we do
  not test on Windows 7 and wheels for our next release will not support it.
  Microsoft no longer provides support for Windows 7 and users are encouraged
  to upgrade.
<p>.. _v42-0-6:</p>
<p>42.0.6 - 2024-05-04
</code></pre></p>
<ul>
<li>Fixed compilation when using LibreSSL 3.9.1.</li>
</ul>
<p>.. _v42-0-5:</p>
<p>42.0.5 - 2024-02-23</p>
<pre><code>
* Limit the number of name constraint checks that will be performed in
  :mod:`X.509 path validation &lt;cryptography.x509.verification&gt;` to protect
  against denial of service attacks.
* Upgrade ``pyo3`` version, which fixes building on PowerPC.
<p>.. _v42-0-4:</p>
<p>42.0.4 - 2024-02-20
</code></pre></p>
<ul>
<li>Fixed a null-pointer-dereference and segfault that could occur when creating
a PKCS#12 bundle. Credit to <strong>Alexander-Programming</strong> for reporting the
issue. <strong>CVE-2024-26130</strong></li>
<li>Fixed ASN.1 encoding for PKCS7/SMIME signed messages. The fields <code>SMIMECapabilities</code>
and <code>SignatureAlgorithmIdentifier</code> should now be correctly encoded according to the
definitions in :rfc:<code>2633</code> :rfc:<code>3370</code>.</li>
</ul>
<p>.. _v42-0-3:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/0cc7fc384381ea09eea5f031d31b1417f9f40fdf"><code>0cc7fc3</code></a> Prepare for 42.0.7 release (<a href="https://redirect.github.com/pyca/cryptography/issues/10949">#10949</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/cfad00478a0cc035ad722e68411bac7b6602e195"><code>cfad004</code></a> Prepare backports for 42.0.6 release (<a href="https://redirect.github.com/pyca/cryptography/issues/10929">#10929</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/33833f031d9d36234e11d9671be150d53b9e598d"><code>33833f0</code></a> Release 42.0.5 (<a href="https://redirect.github.com/pyca/cryptography/issues/10470">#10470</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/4be53bf20cc90cbac01f5f94c5d1aecc5289ba1f"><code>4be53bf</code></a> Added a budget for NC checks to protect against DoS (<a href="https://redirect.github.com/pyca/cryptography/issues/10467">#10467</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10468">#10468</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/8e9de309f850a17409da5de39cfcd9296c25ea36"><code>8e9de30</code></a> Bump pyo3 from 0.20.2 to 0.20.3 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/10462">#10462</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10465">#10465</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/fe18470f7d05f963e7267e34fdf985d81ea6ceea"><code>fe18470</code></a> Bump for 42.0.4 release (<a href="https://redirect.github.com/pyca/cryptography/issues/10445">#10445</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/aaa2dd06ed470695de818405a982d4c459869803"><code>aaa2dd0</code></a> Fix ASN.1 issues in PKCS#7 and S/MIME signing (<a href="https://redirect.github.com/pyca/cryptography/issues/10373">#10373</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10442">#10442</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/7a4d012991061974da5d9cb7614de65eac94f49b"><code>7a4d012</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10422">#10422</a> -- don't crash when a PKCS#12 key and cert don't match (<a href="https://redirect.github.com/pyca/cryptography/issues/10423">#10423</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/df314bb182bdfd661333969a94325e4680d785f6"><code>df314bb</code></a> backport actions m1 switch to 42.0.x (<a href="https://redirect.github.com/pyca/cryptography/issues/10415">#10415</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.3...42.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.3&new-version=42.0.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 17:01:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4559" class=".btn">#4559</a>
            </td>
            <td>
                <b>
                    chore(deps): bump prometheus from 0.13.3 to 0.13.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [prometheus](https://github.com/tikv/rust-prometheus) from 0.13.3 to 0.13.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tikv/rust-prometheus/blob/master/CHANGELOG.md">prometheus's changelog</a>.</em></p>
<blockquote>
<h2>0.13.4</h2>
<ul>
<li>
<p>Improvement: Add PullingGauge (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/405">#405</a>)</p>
</li>
<li>
<p>Improvement: Let cargo know which example requires which features (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/511">#511</a>)</p>
</li>
<li>
<p>Bug fix: Prevent <code>clippy::ignored_unit_patterns</code> in macro expansions (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/497">#497</a>)</p>
</li>
<li>
<p>Internal change: Add CI job for minimum toolchain (MSRV) (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/467">#467</a>)</p>
</li>
<li>
<p>Internal change: Update CI to <code>actions/checkout@v4</code> (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/499">#499</a>)</p>
</li>
<li>
<p>Internal change: Update dependencies</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tikv/rust-prometheus/commit/04fce2f3bf81920c2607e6572dd9eba309969d22"><code>04fce2f</code></a> prometheus: release 0.13.4 (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/520">#520</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/6e435db331f7e269ae1a7498d5ef5b4787e71636"><code>6e435db</code></a> build(deps): update reqwest requirement from ^0.11 to ^0.12 (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/516">#516</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/439e3b8c14938a66352df4228ec32a9b707d1888"><code>439e3b8</code></a> Prevent <code>clippy::ignored_unit_patterns</code> in macro expansions (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/497">#497</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/bf696d642c7ede1c694f93f9b088371e30dd96ab"><code>bf696d6</code></a> ci: bump MSRV to fix test jobs (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/519">#519</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/b7e874524f2b0580a28853e2042656a55b6484f0"><code>b7e8745</code></a> Let the cargo.toml know which example requires which features (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/511">#511</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/f49c724df0e123520554664436da68e555593af0"><code>f49c724</code></a> cargo: update all dependencies (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/504">#504</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/76a634587a95340db56959f5808ac0a6494f6282"><code>76a6345</code></a> ci: Update to <code>actions/checkout@v4</code>. (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/499">#499</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/a72d8d7db880f57ade09dd9139c8b2c5501fbf2f"><code>a72d8d7</code></a> Bump MSRV to 1.65 to fix CI. (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/505">#505</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/7a9adcacd098128ee3017ad973afb841d1fc123e"><code>7a9adca</code></a> ci: Update badge info to not refer to Travis CI (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/500">#500</a>)</li>
<li><a href="https://github.com/tikv/rust-prometheus/commit/6e81890773ef82e3bcc6c080d406543da1fb8073"><code>6e81890</code></a> bump MSRV to 1.60.0 (<a href="https://redirect.github.com/tikv/rust-prometheus/issues/491">#491</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tikv/rust-prometheus/compare/v0.13.3...v0.13.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=prometheus&package-manager=cargo&previous-version=0.13.3&new-version=0.13.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 16:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4557" class=".btn">#4557</a>
            </td>
            <td>
                <b>
                    chore(deps): bump getrandom from 0.2.14 to 0.2.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [getrandom](https://github.com/rust-random/getrandom) from 0.2.14 to 0.2.15.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-random/getrandom/blob/master/CHANGELOG.md">getrandom's changelog</a>.</em></p>
<blockquote>
<h2>[0.2.15] - 2024-05-06</h2>
<h3>Added</h3>
<ul>
<li>Apple visionOS support <a href="https://redirect.github.com/rust-random/getrandom/issues/410">#410</a></li>
</ul>
<h3>Changed</h3>
<ul>
<li>Use <code>libc::getrandom</code> on DragonflyBSD, FreeBSD, illumos, and Solaris <a href="https://redirect.github.com/rust-random/getrandom/issues/411">#411</a> <a href="https://redirect.github.com/rust-random/getrandom/issues/416">#416</a> <a href="https://redirect.github.com/rust-random/getrandom/issues/417">#417</a> <a href="https://redirect.github.com/rust-random/getrandom/issues/420">#420</a></li>
<li>Unify <code>libc::getentropy</code>-based implementations <a href="https://redirect.github.com/rust-random/getrandom/issues/418">#418</a></li>
</ul>
<p><a href="https://redirect.github.com/rust-random/getrandom/issues/410">#410</a>: <a href="https://redirect.github.com/rust-random/getrandom/pull/410">rust-random/getrandom#410</a>
<a href="https://redirect.github.com/rust-random/getrandom/issues/411">#411</a>: <a href="https://redirect.github.com/rust-random/getrandom/pull/411">rust-random/getrandom#411</a>
<a href="https://redirect.github.com/rust-random/getrandom/issues/416">#416</a>: <a href="https://redirect.github.com/rust-random/getrandom/pull/416">rust-random/getrandom#416</a>
<a href="https://redirect.github.com/rust-random/getrandom/issues/417">#417</a>: <a href="https://redirect.github.com/rust-random/getrandom/pull/417">rust-random/getrandom#417</a>
<a href="https://redirect.github.com/rust-random/getrandom/issues/418">#418</a>: <a href="https://redirect.github.com/rust-random/getrandom/pull/418">rust-random/getrandom#418</a>
<a href="https://redirect.github.com/rust-random/getrandom/issues/420">#420</a>: <a href="https://redirect.github.com/rust-random/getrandom/pull/420">rust-random/getrandom#420</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-random/getrandom/commit/cf65e83f9df8954df101320de86f80dccfc6b68a"><code>cf65e83</code></a> Release v0.2.15 (<a href="https://redirect.github.com/rust-random/getrandom/issues/419">#419</a>)</li>
<li><a href="https://github.com/rust-random/getrandom/commit/a24538f0983d385b21f8851ce338bdc0ecb360a1"><code>a24538f</code></a> Remove .cargo/config (<a href="https://redirect.github.com/rust-random/getrandom/issues/421">#421</a>)</li>
<li><a href="https://github.com/rust-random/getrandom/commit/229d87004d33316664fd5c891f96b6b29972c080"><code>229d870</code></a> Use libc::getrandom on Solaris and update docs. (<a href="https://redirect.github.com/rust-random/getrandom/issues/420">#420</a>)</li>
<li><a href="https://github.com/rust-random/getrandom/commit/924c88d761b90d87b9fe9d15c7c8a5e15d28d8a8"><code>924c88d</code></a> Unconditionally use <code>libc::getrandom</code> on Illumos and <code>libc::geentropy</code> on Sol...</li>
<li><a href="https://github.com/rust-random/getrandom/commit/20c22138d5c48993e6d03bb3ce23f87ee3e0887f"><code>20c2213</code></a> Unify getentropy-based implementations (<a href="https://redirect.github.com/rust-random/getrandom/issues/418">#418</a>)</li>
<li><a href="https://github.com/rust-random/getrandom/commit/dca49613a00bd687e10641c22d68364aebbb7583"><code>dca4961</code></a> Unconditionally use libc::getrandom on FreeBSD (<a href="https://redirect.github.com/rust-random/getrandom/issues/416">#416</a>)</li>
<li><a href="https://github.com/rust-random/getrandom/commit/d4b0ef09dfdae5e4bb95ce2c93d75299678dd254"><code>d4b0ef0</code></a> Use libc::getrandom on DragonflyBSD (<a href="https://redirect.github.com/rust-random/getrandom/issues/411">#411</a>)</li>
<li><a href="https://github.com/rust-random/getrandom/commit/0d559231f6dee7693a7721d40da3f147264c7390"><code>0d55923</code></a> Add Apple visionOS support (<a href="https://redirect.github.com/rust-random/getrandom/issues/410">#410</a>)</li>
<li>See full diff in <a href="https://github.com/rust-random/getrandom/compare/v0.2.14...v0.2.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=getrandom&package-manager=cargo&previous-version=0.2.14&new-version=0.2.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 16:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4556" class=".btn">#4556</a>
            </td>
            <td>
                <b>
                    chore(deps): bump num-traits from 0.2.18 to 0.2.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [num-traits](https://github.com/rust-num/num-traits) from 0.2.18 to 0.2.19.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-num/num-traits/blob/master/RELEASES.md">num-traits's changelog</a>.</em></p>
<blockquote>
<h1>Release 0.2.19 (2024-05-03)</h1>
<ul>
<li><a href="https://redirect.github.com/rust-num/num-traits/pull/310">Upgrade to 2021 edition, <strong>MSRV 1.60</strong></a></li>
<li><a href="https://redirect.github.com/rust-num/num-traits/pull/305">The new <code>Float::clamp</code> limits values by minimum and maximum</a></li>
</ul>
<p><strong>Contributors</strong>: <a href="https://github.com/cuviper"><code>@​cuviper</code></a>, <a href="https://github.com/michaelciraci"><code>@​michaelciraci</code></a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-num/num-traits/commit/7ec3d41d39b28190ec1d42db38021107b3951f3a"><code>7ec3d41</code></a> Merge pull request <a href="https://redirect.github.com/rust-num/num-traits/issues/321">#321</a> from cuviper/release-0.2.19</li>
<li><a href="https://github.com/rust-num/num-traits/commit/1a8d429a2ccc763a0c4345234dbf097ca7d14c1e"><code>1a8d429</code></a> Release 0.2.19</li>
<li><a href="https://github.com/rust-num/num-traits/commit/8358949084a87873553e81493f8b52b1e3dee302"><code>8358949</code></a> Merge pull request <a href="https://redirect.github.com/rust-num/num-traits/issues/305">#305</a> from michaelciraci/implement-float-clamp</li>
<li><a href="https://github.com/rust-num/num-traits/commit/1a44ffb9deb4d76988b6ea6bc2767ed40264aac3"><code>1a44ffb</code></a> Add a default impl for <code>Float::clamp</code></li>
<li><a href="https://github.com/rust-num/num-traits/commit/295704408f524c7df8f036eb875f48e6b998d693"><code>2957044</code></a> Implementing clamp for Float trait</li>
<li><a href="https://github.com/rust-num/num-traits/commit/a90d4a62deb7946abd40e171f0ee8575bf25f96c"><code>a90d4a6</code></a> Merge pull request <a href="https://redirect.github.com/rust-num/num-traits/issues/310">#310</a> from cuviper/msrv-1.60</li>
<li><a href="https://github.com/rust-num/num-traits/commit/ca42b4e106486b8fe9b22eeabb90aa8a0452f148"><code>ca42b4e</code></a> Update the MSRV in docs</li>
<li><a href="https://github.com/rust-num/num-traits/commit/e9bea92808de77ff4d4e94c8fe0dccece542d2ce"><code>e9bea92</code></a> Upgrade to 2021 edition</li>
<li><a href="https://github.com/rust-num/num-traits/commit/4e253cdaa9948f4fb8b4136c78d655a34eac3c26"><code>4e253cd</code></a> Assume has_float_to_from_bytes</li>
<li><a href="https://github.com/rust-num/num-traits/commit/7212041f31654953ba55c7bc66e6a8440524dda4"><code>7212041</code></a> Assume has_int_to_from_bytes</li>
<li>Additional commits viewable in <a href="https://github.com/rust-num/num-traits/compare/num-traits-0.2.18...num-traits-0.2.19">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=num-traits&package-manager=cargo&previous-version=0.2.18&new-version=0.2.19)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 16:15:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4553" class=".btn">#4553</a>
            </td>
            <td>
                <b>
                    ci: Remove executor.wasm from git
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">CI</span>
            </td>
            <td>
                ## Description

Remove `executor.wasm` from git, executor is built in the CI.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4549 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 09:32:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4548" class=".btn">#4548</a>
            </td>
            <td>
                <b>
                    IGNORE: Merge to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 12:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4547" class=".btn">#4547</a>
            </td>
            <td>
                <b>
                    fix: remove serde(flatten) from SetKeyValue/RemoveKeyValue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

serde cannot flatten Strings and O::Id is always serialized as string. As a consequence it's impossible to serialize/deserialize SetKeyValue/RemoveKeyValue in genesis

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 11:25:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4546" class=".btn">#4546</a>
            </td>
            <td>
                <b>
                    fix: remove serde(flatten) from SetKeyValue/RemoveKeyValue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

serde cannot flatten `String`s and `O::Id` is always serialized as string. As a consequence it's impossible to serialize/deserialize `SetKeyValue`/`RemoveKeyValue` in genesis

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 11:15:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4545" class=".btn">#4545</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.0.0 to 25.0.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.0.0 to 25.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.0.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.0.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.0.0...v25.0.1">v25.0.1 - 2024-05-02</a></h3>
<ul>
<li>Add type stub file to <code>setup.py</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/2069bd3f57caff88fd0b7cbcd51f970890be43bd"><code>2069bd3</code></a> Bump version: 25.0.0 → 25.0.1</li>
<li><a href="https://github.com/joke2k/faker/commit/681922c11de9abfae3fd72e92becb54dc3c3c733"><code>681922c</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/106d8ba3981445bad6915a0567931416539149f7"><code>106d8ba</code></a> add stub to setup.py</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.0.0...v25.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.0.0&new-version=25.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 16:49:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4544" class=".btn">#4544</a>
            </td>
            <td>
                <b>
                    feat: filtered queries in contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

- remove `QueryWithParameters`
- move all parameters to `ClientQueryPayload` (was `QueryPayload` before, stored inside `SignedQuery`); `SignedQuery` now equivalent to `QueryWithParameters<SignedQuery>`. All the parameters are now scale-encoded and versioned instead of being passed as query parameters
- make `SmartContractQuery`, which is now equivalent to `QueryWithParameters<QueryBox>` that was used before, but has filtering support
- move all the post-processing (filterting, sorting, pagination, batching) to a single function (`LazyQueryOutput::apply_postprocessing`), introduce a new type for a post-processed query output
- add an integration test using the filtering (`ProcessedQueryOutput`)

### Linked issue

Closes #4423 

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 13:12:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4543" class=".btn">#4543</a>
            </td>
            <td>
                <b>
                    fix: Report if a request to check peer status in test_network fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Warn if a peer status request is failed. Helped me debug my misconfigured proxy failing tests when ran in IDE...

This also refactors a function a bit, because IMO it was a bit hard to read with the fold and `map_or`

### Linked issue

Closes #4542

### Benefits

`+` Easier debugging if something went wrong with requests
`-` Can introduce log noise, but shouldn't happen if the actual connection to the node is OK

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 13:04:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4541" class=".btn">#4541</a>
            </td>
            <td>
                <b>
                    refactor!: Use multihash format for private keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Added support for encoding/decoding private keys to `multihash` module, and replaced each occurence of `PRIVATE_KEY_ALGORITHM`/`PRIVATE_KEY_PAYLOAD` pair to `PRIVATE_KEY` in multihash format

### Linked issue

Closes #4412

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 12:13:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4539" class=".btn">#4539</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.199 to 1.0.200
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.199 to 1.0.200.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.200</h2>
<ul>
<li>Fix formatting of &quot;invalid type&quot; and &quot;invalid value&quot; deserialization error messages containing NaN or infinite floats (<a href="https://redirect.github.com/serde-rs/serde/issues/2733">#2733</a>, thanks <a href="https://github.com/jamessan"><code>@​jamessan</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/cc865ac5236c094275b10bff4fa41e561b3e359f"><code>cc865ac</code></a> Release 1.0.200</li>
<li><a href="https://github.com/serde-rs/serde/commit/2d973c1805dd9b613e89cc2375130a23f18ffa73"><code>2d973c1</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2733">#2733</a> from jamessan/nan-decimal</li>
<li><a href="https://github.com/serde-rs/serde/commit/6ca499b2dd3d520903095b202770eba2720ba9b5"><code>6ca499b</code></a> Only format Unexpected::Float with decimal point if it is finite</li>
<li>See full diff in <a href="https://github.com/serde-rs/serde/compare/v1.0.199...v1.0.200">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.199&new-version=1.0.200)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 16:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4538" class=".btn">#4538</a>
            </td>
            <td>
                <b>
                    fix: Remove nested option on `TransactionEventFilter::block_height`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 14:16:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4536" class=".btn">#4536</a>
            </td>
            <td>
                <b>
                    ci: trigger PR CI on lockfile updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Trigger PR CI when `.lock` files are updated. 

### Benefits

pytests will run on dependabot version updates

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 08:27:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4535" class=".btn">#4535</a>
            </td>
            <td>
                <b>
                    chore(deps): bump base64 from 0.22.0 to 0.22.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [base64](https://github.com/marshallpierce/rust-base64) from 0.22.0 to 0.22.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/marshallpierce/rust-base64/blob/master/RELEASE-NOTES.md">base64's changelog</a>.</em></p>
<blockquote>
<h1>0.22.1</h1>
<ul>
<li>Correct the symbols used for the predefined <code>alphabet::BIN_HEX</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/e14400697453bcc85997119b874bc03d9601d0af"><code>e144006</code></a> v0.22.1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/64cca59ddbb4c43244a8f38629b59960ffe36bc0"><code>64cca59</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/271">#271</a> from JobanSD/patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/838355e0ac5fb8237ec9b96be5edb011bff00275"><code>838355e</code></a> Correct BinHex 4.0 alphabet according to specifications</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/bf15ccf30af8bb6b1f326fffa025d7b0aaa3342f"><code>bf15ccf</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/270">#270</a> from marshallpierce/mp/clippy</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/fc6aabee8afaf8b2f4cfb12df4cf461bcf9b003d"><code>fc6aabe</code></a> Appease clippy</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/9a518a2d5d028068d4bf83ebf437f7a3575e640e"><code>9a518a2</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/267">#267</a> from bdura/patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/d96c80f242e3080a03fd1c079730e17373ef0eb6"><code>d96c80f</code></a> Merge branch 'marshallpierce:master' into patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/e8e4a22761614cab33d838b354c946427d136db8"><code>e8e4a22</code></a> docs: fix trailing ``` in mod.rs example</li>
<li>See full diff in <a href="https://github.com/marshallpierce/rust-base64/compare/v0.22.0...v0.22.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=base64&package-manager=cargo&previous-version=0.22.0&new-version=0.22.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 06:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4534" class=".btn">#4534</a>
            </td>
            <td>
                <b>
                    chore(dependabot): follow conventional commits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Linked issue

Related to #4502.

<!-- Link if e.g. JIRA issue or  from another repository -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 06:29:18 +0000 UTC
    </div>
</div>

