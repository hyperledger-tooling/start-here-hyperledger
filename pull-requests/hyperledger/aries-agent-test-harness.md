---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    Increase timeout for restarting agents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Increased the timeout for restarting agents mid feature run. This happens in the DIDTransport tests. This is an attempt to fix the failures in the ACA-Py and AFJ runset where sometimes running in the context of the interop test pipeline most tests will fail. It looks as if at some point in the DIDTransport tests the acapy agent either fails to start or the test is not waiting long enough for it to be started and make the `status` api call then continue the tests. This increases the wait time to check the status to see if it is just ACA-py taking a little more time to startup in that environment. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 20:10:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/845" class=".btn">#845</a>
            </td>
            <td>
                <b>
                    Bump log from 0.4.17 to 0.4.22 in /aries-backchannels/aries-vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [log](https://github.com/rust-lang/log) from 0.4.17 to 0.4.22.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/log/blob/master/CHANGELOG.md">log's changelog</a>.</em></p>
<blockquote>
<h2>[0.4.22] - 2024-06-27</h2>
<h2>What's Changed</h2>
<ul>
<li>Add some clarifications to the library docs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/620">rust-lang/log#620</a></li>
<li>Add links to <code>colog</code> crate by <a href="https://github.com/chrivers"><code>@​chrivers</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/621">rust-lang/log#621</a></li>
<li>adding line_number test + updating some testing infrastructure by <a href="https://github.com/DIvkov575"><code>@​DIvkov575</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/619">rust-lang/log#619</a></li>
<li>Clarify the actual set of functions that can race in _racy variants by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/623">rust-lang/log#623</a></li>
<li>Replace deprecated std::sync::atomic::spin_loop_hint() by <a href="https://github.com/Catamantaloedis"><code>@​Catamantaloedis</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/625">rust-lang/log#625</a></li>
<li>Check usage of max_level features by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/627">rust-lang/log#627</a></li>
<li>Remove unneeded import by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/628">rust-lang/log#628</a></li>
<li>Loosen orderings for logger initialization in <a href="https://redirect.github.com/rust-lang/log/pull/632">rust-lang/log#632</a>. Originally by <a href="https://github.com/pwoolcoc"><code>@​pwoolcoc</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/599">rust-lang/log#599</a></li>
<li>Use Location::caller() for file and line info in <a href="https://redirect.github.com/rust-lang/log/pull/633">rust-lang/log#633</a>. Originally by <a href="https://github.com/Cassy343"><code>@​Cassy343</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/520">rust-lang/log#520</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/chrivers"><code>@​chrivers</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/621">rust-lang/log#621</a></li>
<li><a href="https://github.com/DIvkov575"><code>@​DIvkov575</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/619">rust-lang/log#619</a></li>
<li><a href="https://github.com/Catamantaloedis"><code>@​Catamantaloedis</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/625">rust-lang/log#625</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/rust-lang/log/compare/0.4.21...0.4.22">https://github.com/rust-lang/log/compare/0.4.21...0.4.22</a></p>
<h2>[0.4.21] - 2024-02-27</h2>
<h2>What's Changed</h2>
<ul>
<li>Minor clippy nits by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/578">rust-lang/log#578</a></li>
<li>Simplify Display impl by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/579">rust-lang/log#579</a></li>
<li>Set all crates to 2021 edition by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/580">rust-lang/log#580</a></li>
<li>Various changes based on review by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/583">rust-lang/log#583</a></li>
<li>Fix typo in file_static() method doc by <a href="https://github.com/dimo414"><code>@​dimo414</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/590">rust-lang/log#590</a></li>
<li>Specialize empty key value pairs by <a href="https://github.com/EFanZh"><code>@​EFanZh</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/576">rust-lang/log#576</a></li>
<li>Fix incorrect lifetime in Value::to_str() by <a href="https://github.com/peterjoel"><code>@​peterjoel</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/587">rust-lang/log#587</a></li>
<li>Remove some API of the key-value feature by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/585">rust-lang/log#585</a></li>
<li>Add logcontrol-log and log-reload by <a href="https://github.com/swsnr"><code>@​swsnr</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/595">rust-lang/log#595</a></li>
<li>Add Serialization section to kv::Value docs by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/593">rust-lang/log#593</a></li>
<li>Rename Value::to_str to to_cow_str by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/592">rust-lang/log#592</a></li>
<li>Clarify documentation and simplify initialization of <code>STATIC_MAX_LEVEL</code> by <a href="https://github.com/ptosi"><code>@​ptosi</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/594">rust-lang/log#594</a></li>
<li>Update docs to 2021 edition, test by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/577">rust-lang/log#577</a></li>
<li>Add &quot;alterable_logger&quot; link to README.md by <a href="https://github.com/brummer-simon"><code>@​brummer-simon</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/589">rust-lang/log#589</a></li>
<li>Normalize line ending by <a href="https://github.com/EFanZh"><code>@​EFanZh</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/602">rust-lang/log#602</a></li>
<li>Remove <code>ok_or</code> in favor of <code>Option::ok_or</code> by <a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/607">rust-lang/log#607</a></li>
<li>Use <code>Acquire</code> ordering for initialization check by <a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/610">rust-lang/log#610</a></li>
<li>Get structured logging API ready for stabilization by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/613">rust-lang/log#613</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/nyurik"><code>@​nyurik</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/578">rust-lang/log#578</a></li>
<li><a href="https://github.com/dimo414"><code>@​dimo414</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/590">rust-lang/log#590</a></li>
<li><a href="https://github.com/peterjoel"><code>@​peterjoel</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/587">rust-lang/log#587</a></li>
<li><a href="https://github.com/ptosi"><code>@​ptosi</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/594">rust-lang/log#594</a></li>
<li><a href="https://github.com/brummer-simon"><code>@​brummer-simon</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/589">rust-lang/log#589</a></li>
<li><a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/607">rust-lang/log#607</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/log/commit/d5ba2cfee9b3b4ca1fcad911b7f59dc79eeee022"><code>d5ba2cf</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/634">#634</a> from rust-lang/cargo/0.4.22</li>
<li><a href="https://github.com/rust-lang/log/commit/d1a8306aadb88d56b74c73cdce4ef0153fb549cb"><code>d1a8306</code></a> prepare for 0.4.22 release</li>
<li><a href="https://github.com/rust-lang/log/commit/46894ef229483bbabd30a806c474417fc034559c"><code>46894ef</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/633">#633</a> from rust-lang/feat/panic-info</li>
<li><a href="https://github.com/rust-lang/log/commit/e0d389c9cadd91363f2fec52bd30f9585168a89f"><code>e0d389c</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/632">#632</a> from rust-lang/feat/loosen-atomics</li>
<li><a href="https://github.com/rust-lang/log/commit/c9e5e13e9b02ec80e784c6fe4deacdc8f3194fca"><code>c9e5e13</code></a> use Location::caller() for file and line info</li>
<li><a href="https://github.com/rust-lang/log/commit/507b672660288f0223edb6353d34f8733fa0a2f4"><code>507b672</code></a> loosen orderings for logger initialization</li>
<li><a href="https://github.com/rust-lang/log/commit/c879b011a8ac662545adf9484d9a668ebcf9b814"><code>c879b01</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/628">#628</a> from Thomasdezeeuw/fix-warnings</li>
<li><a href="https://github.com/rust-lang/log/commit/405fdb4d9f847c93c0133469ea808f09320714ba"><code>405fdb4</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/627">#627</a> from Thomasdezeeuw/check-features</li>
<li><a href="https://github.com/rust-lang/log/commit/1307ade1122549badf2b8fdd10c11e519eaa029a"><code>1307ade</code></a> Remove unneeded import</li>
<li><a href="https://github.com/rust-lang/log/commit/710560ecb7035a6baf1fd9d97d7f09d0cc075006"><code>710560e</code></a> Don't use --all-features in CI</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/log/compare/0.4.17...0.4.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log&package-manager=cargo&previous-version=0.4.17&new-version=0.4.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 11:49:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-29 05:19:07 +0000 UTC
    </div>
</div>

