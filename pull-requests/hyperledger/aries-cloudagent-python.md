---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2991" class=".btn">#2991</a>
            </td>
            <td>
                <b>
                    Add `proof_key` issuance option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the discussions in PR #2348, here's my suggestion to add an optional field to specify a verkey to use when querying the wallet for the `didInfo` used in issuing credentials.

This would satisfy the requirements raised by @Jsyro and some of the work we are doing around binding `did:web` to a `did:indy`.

Please review and share some toughts @dbluhm @swcurran @jamshale @ianco @TimoGlastra .

This will also preserve this enabling feature from the deprecated `/jsonld/sign` endpoint, giving controllers flexibility while using other did methods.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 02:47:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2990" class=".btn">#2990</a>
            </td>
            <td>
                <b>
                    Enable `no-transport` mode as startup parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `--no-transport` startup parameter for making the agent start without requiring the `--enpoint`, `--inbound-transport` and `--outbound-transport` to be set.

The idea was shared during an aca-pug meeting and there was no objection. This can greatly simplify deployment for controllers that do no require didcomm messaging.

Currently it just overrides what is required for startup.

@dbluhm @swcurran @ianco

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 02:17:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2988" class=".btn">#2988</a>
            </td>
            <td>
                <b>
                    chore(deps): Update asyncpg requirement from ~=0.26.0 to ~=0.29.0 in /demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [asyncpg](https://github.com/MagicStack/asyncpg) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/MagicStack/asyncpg/releases">asyncpg's releases</a>.</em></p>
<blockquote>
<h2>v0.29.0</h2>
<p>Minor fixes and improvements.</p>
<h1>Improvements</h1>
<ul>
<li>
<p>Python 3.12 and PostgreSQL 16 support (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1084">#1084</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in deea86ce)</p>
</li>
<li>
<p>Add support for tuple-format custom codecs on composite types (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1061">#1061</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 922fcd10)</p>
</li>
<li>
<p>Support <code>target_session_attrs</code> in URL format, add tests (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1073">#1073</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 7cb4e70d)</p>
</li>
<li>
<p>Infinity numeric support (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1067">#1067</a>)
(by <a href="https://github.com/krokoziabla"><code>@​krokoziabla</code></a> in 0c3bf600 for <a href="https://redirect.github.com/MagicStack/asyncpg/issues/1020">#1020</a>)</p>
</li>
<li>
<p>Add support for the <code>WHERE</code> clause in <code>copy_to</code> methods (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/941">#941</a>)
(by <a href="https://github.com/kaylynn234"><code>@​kaylynn234</code></a> in b7ffab6c)</p>
</li>
<li>
<p>Add query logging callbacks and context manager (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1043">#1043</a>)
(by <a href="https://github.com/dcwatson"><code>@​dcwatson</code></a> in b2697ffd)</p>
</li>
</ul>
<h1>Fixes</h1>
<ul>
<li>
<p>When prepared statements are disabled, avoid relying on them harder (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1065">#1065</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in cbf64e18)</p>
</li>
<li>
<p>Handle environments with HOME set to a not-a-directory (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1063">#1063</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in af922bcf)</p>
</li>
<li>
<p>Fix handling of non-ASCII passwords (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1062">#1062</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 89d5bd03)</p>
</li>
<li>
<p>Disable JIT while doing type introspection (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1082">#1082</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in f21ebf64)</p>
</li>
<li>
<p>Remove connection parameter caching in <code>Pool</code> (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1053">#1053</a>)
(by <a href="https://github.com/ermakov-oleg"><code>@​ermakov-oleg</code></a> in 4ddb0397)</p>
</li>
<li>
<p>Switch to Python 3.12-style <code>wait_for</code> (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1086">#1086</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 4bdd8a7e)</p>
</li>
<li>
<p>Update automatic PostGIS type conversion for Shapely 2.0 (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1085">#1085</a>)
(by <a href="https://github.com/ChimneySwift"><code>@​ChimneySwift</code></a> in 8b45beb4)</p>
</li>
<li>
<p>Use the <code>timeout</code> context manager in the connection path (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1087">#1087</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 313b2b2b)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/MagicStack/asyncpg/commit/74f3a0031532b314d9141b6de12aa74db7726b3d"><code>74f3a00</code></a> asyncpg v0.29.0</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/d7faaff57a7a9c0029a31f09564d30ab35007907"><code>d7faaff</code></a> fix: allow host tuple (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1021">#1021</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/b2697ffdf18f7acd88a35e9a0a252c3b6fb25070"><code>b2697ff</code></a> Add query logging callbacks and context manager (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1043">#1043</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/93a6f79afb4251fa48edf6959aa87532eee91ef5"><code>93a6f79</code></a> Cut BaseProtocol circular reference on close. (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1049">#1049</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/ca9f03be3c64984311dbefbbd9e8ff0806a7f772"><code>ca9f03b</code></a> Close cursor portals once the iterator is exhausted (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1088">#1088</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/b7ffab6cb3f9bcc5d4f9c5b22398ca9c9e450af2"><code>b7ffab6</code></a> Add support for the <code>WHERE</code> clause in <code>copy_to</code> methods (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/941">#941</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/70c8bd814f9d289741845fa8dc761737f7ea4e78"><code>70c8bd8</code></a> Use cleanup_ctx in pool usage doc (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/878">#878</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/ccc7baf94cd45fc0155ae522361a6f2b2f551c44"><code>ccc7baf</code></a> Small fix for documentation on using SSL in Connection (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/995">#995</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/313b2b2bedcc10baf5871124ee915fdc48f5c4b7"><code>313b2b2</code></a> Use the <code>timeout</code> context manager in the connection path (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1087">#1087</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/8b45beb4b60e30ad6ccd19d1e925ffdad6477aa2"><code>8b45beb</code></a> Update automatic PostGIS type conversion for Shapely 2.0 (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1085">#1085</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/MagicStack/asyncpg/compare/v0.26.0...v0.29.0">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2024-05-24 21:47:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2987" class=".btn">#2987</a>
            </td>
            <td>
                <b>
                    chore(deps): Update pygments requirement from ~=2.10 to ~=2.18 in /demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pygments](https://github.com/pygments/pygments) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pygments/pygments/releases">pygments's releases</a>.</em></p>
<blockquote>
<h2>2.18.0</h2>
<ul>
<li>
<p>New lexers:</p>
<ul>
<li>Janet (<a href="https://redirect.github.com/pygments/pygments/issues/2557">#2557</a>)</li>
<li>Lean 4 (<a href="https://redirect.github.com/pygments/pygments/issues/2618">#2618</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2626">#2626</a>)</li>
<li>Luau (<a href="https://redirect.github.com/pygments/pygments/issues/2605">#2605</a>)</li>
<li>Mojo (<a href="https://redirect.github.com/pygments/pygments/issues/2691">#2691</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2515">#2515</a>)</li>
<li>org-mode (<a href="https://redirect.github.com/pygments/pygments/issues/2628">#2628</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2636">#2636</a>)</li>
<li>Promela (<a href="https://redirect.github.com/pygments/pygments/issues/2620">#2620</a>)</li>
<li>Soong / <code>Android.bp</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2659">#2659</a>)</li>
<li>Tact (<a href="https://redirect.github.com/pygments/pygments/issues/2571">#2571</a>)</li>
<li>Typst (<a href="https://redirect.github.com/pygments/pygments/issues/2596">#2596</a>)</li>
</ul>
</li>
<li>
<p>Updated lexers:</p>
<ul>
<li>Awk: recognize ternary operator (<a href="https://redirect.github.com/pygments/pygments/issues/2687">#2687</a>)</li>
<li>Bash: add <code>openrc</code> alias (<a href="https://redirect.github.com/pygments/pygments/issues/2599">#2599</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2371">#2371</a>)</li>
<li>Coq: add keywords, lex more vernacular command arguments, produce
fewer tokens on heading comments (<a href="https://redirect.github.com/pygments/pygments/issues/2678">#2678</a>)</li>
<li>DNS zone files: Fix comment parsing (<a href="https://redirect.github.com/pygments/pygments/issues/2595">#2595</a>)</li>
<li>Hy: Support unicode literals (<a href="https://redirect.github.com/pygments/pygments/issues/1126">#1126</a>)</li>
<li>Inform6: Update to Inform 6.42 (<a href="https://redirect.github.com/pygments/pygments/issues/2644">#2644</a>)</li>
<li>lean: Fix name handling (<a href="https://redirect.github.com/pygments/pygments/issues/2614">#2614</a>)</li>
<li>Logtalk: add <code>uninstantiation</code> keyword and recognize
escape sequences (<a href="https://redirect.github.com/pygments/pygments/issues/2619">#2619</a>)</li>
<li>Macaulay2: Update to 1.23 (<a href="https://redirect.github.com/pygments/pygments/issues/2655">#2655</a>)</li>
<li>Python: fix highlighting of soft keywords before <code>None</code>/<code>True</code>/<code>False</code></li>
<li>reStructuredText: use <code>Token.Comment</code> for comments instead of
<code>Comment.Preproc</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2598">#2598</a>)</li>
<li>Rust: highlight <code>:</code>, <code>::</code> and <code>-&gt;</code> as <code>Punctuation</code>
and whitespace as <code>Whitespace</code>, instead of <code>Text</code>
in both cases (<a href="https://redirect.github.com/pygments/pygments/issues/2631">#2631</a>)</li>
<li>Spice: Add keywords (<a href="https://redirect.github.com/pygments/pygments/issues/2621">#2621</a>)</li>
<li>SQL Explain: allow negative numbers (<a href="https://redirect.github.com/pygments/pygments/issues/2610">#2610</a>)</li>
<li>Swift: Support multiline strings (<a href="https://redirect.github.com/pygments/pygments/issues/2681">#2681</a>)</li>
<li>ThingsDB: add constants and new functions; support template
strings (<a href="https://redirect.github.com/pygments/pygments/issues/2624">#2624</a>)</li>
<li>UL4: support nested <code>&lt;?doc?&gt;</code> and <code>&lt;?note?&gt;</code> tags (<a href="https://redirect.github.com/pygments/pygments/issues/2597">#2597</a>)</li>
<li>VHDL: support multi-line comments of VHDL-2008 (<a href="https://redirect.github.com/pygments/pygments/issues/2622">#2622</a>)</li>
<li>Wikitext: Remove <code>kk-*</code> in <code>variant_langs</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2647">#2647</a>)</li>
<li>Xtend: Add <code>val</code> and <code>var</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2602">#2602</a>)</li>
</ul>
</li>
<li>
<p>New styles:</p>
<ul>
<li>Coffee (<a href="https://redirect.github.com/pygments/pygments/issues/2609">#2609</a>)</li>
</ul>
</li>
<li>
<p>Make background colors in the image formatter work with Pillow 10.0 (<a href="https://redirect.github.com/pygments/pygments/issues/2623">#2623</a>)</p>
</li>
<li>
<p>Require Python 3.8. As a result, the <code>importlib-metadata</code> package
is no longer needed for fast plugin discovery on Python 3.7.
The <code>plugins</code> extra (used as, e.g., <code>pip install pygments[plugins]</code>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pygments/pygments/blob/master/CHANGES">pygments's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.18.0</h2>
<p>(released May 4th, 2024)</p>
<ul>
<li>
<p>New lexers:</p>
<ul>
<li>Janet (<a href="https://redirect.github.com/pygments/pygments/issues/2557">#2557</a>)</li>
<li>Lean 4 (<a href="https://redirect.github.com/pygments/pygments/issues/2618">#2618</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2626">#2626</a>)</li>
<li>Luau (<a href="https://redirect.github.com/pygments/pygments/issues/2605">#2605</a>)</li>
<li>Mojo (<a href="https://redirect.github.com/pygments/pygments/issues/2691">#2691</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2515">#2515</a>)</li>
<li>org-mode (<a href="https://redirect.github.com/pygments/pygments/issues/2628">#2628</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2636">#2636</a>)</li>
<li>Promela (<a href="https://redirect.github.com/pygments/pygments/issues/2620">#2620</a>)</li>
<li>Soong / <code>Android.bp</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2659">#2659</a>)</li>
<li>Tact (<a href="https://redirect.github.com/pygments/pygments/issues/2571">#2571</a>)</li>
<li>Typst (<a href="https://redirect.github.com/pygments/pygments/issues/2596">#2596</a>)</li>
</ul>
</li>
<li>
<p>Updated lexers:</p>
<ul>
<li>Awk: recognize ternary operator (<a href="https://redirect.github.com/pygments/pygments/issues/2687">#2687</a>)</li>
<li>Bash: add <code>openrc</code> alias (<a href="https://redirect.github.com/pygments/pygments/issues/2599">#2599</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2371">#2371</a>)</li>
<li>Coq: add keywords, lex more vernacular command arguments, produce
fewer tokens on heading comments (<a href="https://redirect.github.com/pygments/pygments/issues/2678">#2678</a>)</li>
<li>DNS zone files: Fix comment parsing (<a href="https://redirect.github.com/pygments/pygments/issues/2595">#2595</a>)</li>
<li>Hy: Support unicode literals (<a href="https://redirect.github.com/pygments/pygments/issues/1126">#1126</a>)</li>
<li>Inform6: Update to Inform 6.42 (<a href="https://redirect.github.com/pygments/pygments/issues/2644">#2644</a>)</li>
<li>lean: Fix name handling (<a href="https://redirect.github.com/pygments/pygments/issues/2614">#2614</a>)</li>
<li>Logtalk: add <code>uninstantiation</code> keyword and recognize
escape sequences (<a href="https://redirect.github.com/pygments/pygments/issues/2619">#2619</a>)</li>
<li>Macaulay2: Update to 1.23 (<a href="https://redirect.github.com/pygments/pygments/issues/2655">#2655</a>)</li>
<li>Python: fix highlighting of soft keywords before <code>None</code>/<code>True</code>/<code>False</code></li>
<li>reStructuredText: use <code>Token.Comment</code> for comments instead of
<code>Comment.Preproc</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2598">#2598</a>)</li>
<li>Rust: highlight <code>:</code>, <code>::</code> and <code>-&gt;</code> as <code>Punctuation</code>
and whitespace as <code>Whitespace</code>, instead of <code>Text</code>
in both cases (<a href="https://redirect.github.com/pygments/pygments/issues/2631">#2631</a>)</li>
<li>Spice: Add keywords (<a href="https://redirect.github.com/pygments/pygments/issues/2621">#2621</a>)</li>
<li>SQL Explain: allow negative numbers (<a href="https://redirect.github.com/pygments/pygments/issues/2610">#2610</a>)</li>
<li>Swift: Support multiline strings (<a href="https://redirect.github.com/pygments/pygments/issues/2681">#2681</a>)</li>
<li>ThingsDB: add constants and new functions; support template
strings (<a href="https://redirect.github.com/pygments/pygments/issues/2624">#2624</a>)</li>
<li>UL4: support nested <code>&lt;?doc?&gt;</code> and <code>&lt;?note?&gt;</code> tags (<a href="https://redirect.github.com/pygments/pygments/issues/2597">#2597</a>)</li>
<li>VHDL: support multi-line comments of VHDL-2008 (<a href="https://redirect.github.com/pygments/pygments/issues/2622">#2622</a>)</li>
<li>Wikitext: Remove <code>kk-*</code> in <code>variant_langs</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2647">#2647</a>)</li>
<li>Xtend: Add <code>val</code> and <code>var</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2602">#2602</a>)</li>
</ul>
</li>
<li>
<p>New styles:</p>
<ul>
<li>Coffee (<a href="https://redirect.github.com/pygments/pygments/issues/2609">#2609</a>)</li>
</ul>
</li>
<li>
<p>Make background colors in the image formatter work with Pillow 10.0 (<a href="https://redirect.github.com/pygments/pygments/issues/2623">#2623</a>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pygments/pygments/commit/d7d11f6e6d3aa97805215c1cc833ea5f0ef1fcbb"><code>d7d11f6</code></a> Last steps for 2.18 release.</li>
<li><a href="https://github.com/pygments/pygments/commit/ec7bfd2cc91a1bb2a7200b27c2c553309d689839"><code>ec7bfd2</code></a> Fix Janet version_added.</li>
<li><a href="https://github.com/pygments/pygments/commit/ea9c8232b4edfdc7193f25f1253040e77342f878"><code>ea9c823</code></a> Update CHANGES.</li>
<li><a href="https://github.com/pygments/pygments/commit/338d36665371cd9e4193b59a267d4f576d8eb05d"><code>338d366</code></a> Merge pull request <a href="https://redirect.github.com/pygments/pygments/issues/2670">#2670</a> from Kodiologist/hylex</li>
<li><a href="https://github.com/pygments/pygments/commit/4d1371b30af2de7c6a74af6ef64673b657dfe3ea"><code>4d1371b</code></a> Lock down the pytest version.</li>
<li><a href="https://github.com/pygments/pygments/commit/8dd97e04d47437581ca2fcb19a94aeb5cbd1dba2"><code>8dd97e0</code></a> Improve docs.</li>
<li><a href="https://github.com/pygments/pygments/commit/26179d66122f2afacdc115071ce344af1984a55c"><code>26179d6</code></a> Fix deprecated variable usage in tests.</li>
<li><a href="https://github.com/pygments/pygments/commit/ad125ca614097b5b02c4603bdbe63ec79b791473"><code>ad125ca</code></a> Prepare 2.18 release.</li>
<li><a href="https://github.com/pygments/pygments/commit/24deeb9cae597db4d22496b0c2cc9e82d3e8a689"><code>24deeb9</code></a> Lock the ruff version in tox.ini.</li>
<li><a href="https://github.com/pygments/pygments/commit/c9165cf7fb18f01066222ec7d063e5e5975f2a69"><code>c9165cf</code></a> Fix format string usage.</li>
<li>Additional commits viewable in <a href="https://github.com/pygments/pygments/compare/2.10.0...2.18.0">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2024-05-24 21:47:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2986" class=".btn">#2986</a>
            </td>
            <td>
                <b>
                    chore(deps): Update prompt-toolkit requirement from ~=2.0.9 to ~=3.0.43 in /demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [prompt-toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prompt-toolkit/python-prompt-toolkit/releases">prompt-toolkit's releases</a>.</em></p>
<blockquote>
<h2>3.0.43</h2>
<p>Fixes regression from 3.0.42:</p>
<ul>
<li>Fix regression on Pypy: Don't use <code>ctypes.pythonapi</code> to restore SIGINT if not available.</li>
</ul>
<p>Other changes from 3.0.42:</p>
<ul>
<li>Fix line wrapping in <code>patch_stdout</code> on Windows.</li>
<li>Make <code>formatted_text.split_lines()</code> accept an iterable instead of lists only.</li>
<li>Disable the IPython workaround (from 3.0.41) for IPython &gt;= 8.18.</li>
<li>Restore signal.SIGINT handler between prompts</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/CHANGELOG">prompt-toolkit's changelog</a>.</em></p>
<blockquote>
<h2>3.0.43: 2023-12-13</h2>
<p>Fixes:</p>
<ul>
<li>Fix regression on Pypy: Don't use <code>ctypes.pythonapi</code> to restore SIGINT if not
available.</li>
</ul>
<h2>3.0.42: 2023-12-12</h2>
<p>Fixes:</p>
<ul>
<li>Fix line wrapping in <code>patch_stdout</code> on Windows.</li>
<li>Make <code>formatted_text.split_lines()</code> accept an iterable instead of lists only.</li>
<li>Disable the IPython workaround (from 3.0.41) for IPython &gt;= 8.18.</li>
<li>Restore signal.SIGINT handler between prompts.</li>
</ul>
<h2>3.0.41: 2023-11-14</h2>
<p>Fixes:</p>
<ul>
<li>Fix regression regarding IPython input hook (%gui) integration.</li>
</ul>
<h2>3.0.40: 2023-11-10</h2>
<p>Fixes:</p>
<ul>
<li>Improved Python 3.12 support (fixes event loop <code>DeprecationWarning</code>).</li>
</ul>
<p>New features:</p>
<ul>
<li>Vi key bindings: <code>control-t</code> and <code>control-d</code> for indent/unindent in insert
mode.</li>
<li>Insert partial suggestion when <code>control+right</code> is pressed, similar to Fish.</li>
<li>Use sphinx-nefertiti theme for the docs.</li>
</ul>
<h2>3.0.39: 2023-07-04</h2>
<p>Fixes:</p>
<ul>
<li>Fix <code>RuntimeError</code> when <code>__breakpointhook__</code> is called from another thread.</li>
<li>Fix memory leak in filters usage.</li>
<li>Ensure that key bindings are handled in the right context (when using
contextvars).</li>
</ul>
<p>New features:</p>
<ul>
<li>Accept <code>in_thread</code> keyword in <code>prompt_toolkit.shortcuts.prompt()</code>.</li>
<li>Support the <code>NO_COLOR</code> environment variable.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/4432d6233fd8e0efba5920a9650e515f54a20300"><code>4432d62</code></a> Release 3.0.43</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/6a24c99f7db0729d60d7d56f9759db617f266164"><code>6a24c99</code></a> Fix for pypy: don't use pythonapi on pypy.</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/1c6d094206045b712d795956e6ec392cf11aba93"><code>1c6d094</code></a> Use Coroutine instead of Awaitable in type annotations where possible.</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/87d01078cae7f560b241af7cc0b50cc72dfacd26"><code>87d0107</code></a> Release 3.0.42</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/6a4e6dd39e7332a30a78f3b5db94d05d4ce33007"><code>6a4e6dd</code></a> Fix example for progress bar with custom iterable</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/be4ccdfb0b738d8112e815902d2f13b53c386dd8"><code>be4ccdf</code></a> Restore signal.SIGINT handler between prompts</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/6e4ca6ee139bcd87e23e84d504e3a06856798fda"><code>6e4ca6e</code></a> Disable workaround for ipython &gt;= 8.18</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/e2e75c0dd34a57cc6523febead412b5beef85e5e"><code>e2e75c0</code></a> Make formatted_text.split_lines accept an iterable (type annotation only).</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/55cde3eb0e1be72d9232e979a708f1a792339ad9"><code>55cde3e</code></a> Fix line wrapping in <code>patch_stdout</code> on Windows.</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/857af14071162ec467a500f7028d630b2b67c11e"><code>857af14</code></a> Code formatting fixes.</li>
<li>Additional commits viewable in <a href="https://github.com/prompt-toolkit/python-prompt-toolkit/compare/2.0.9...3.0.43">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2024-05-24 21:47:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2985" class=".btn">#2985</a>
            </td>
            <td>
                <b>
                    chore(deps): Update qrcode[pil] requirement from ~=6.1 to ~=7.4 in /demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [qrcode[pil]](https://github.com/lincolnloop/python-qrcode) to permit the latest version.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/lincolnloop/python-qrcode/blob/main/CHANGES.rst">qrcode[pil]'s changelog</a>.</em></p>
<blockquote>
<h1>7.4.2 (6 February 2023)</h1>
<ul>
<li>Allow <code>pypng</code> factory to allow for saving to a string (like
<code>qr.save(&quot;some_file.png&quot;)</code>) in addition to file-like objects.</li>
</ul>
<h1>7.4.1 (3 February 2023)</h1>
<ul>
<li>Fix bad over-optimization in v7.4 that broke large QR codes. Thanks to
mattiasj-axis!</li>
</ul>
<h1>7.4 (1 February 2023)</h1>
<ul>
<li>
<p>Restructure the factory drawers, allowing different shapes in SVG image
factories as well.</p>
</li>
<li>
<p>Add a <code>--factory-drawer</code> option to the <code>qr</code> console script.</p>
</li>
<li>
<p>Optimize the output for the <code>SVGPathImage</code> factory (more than 30% reduction
in file sizes).</p>
</li>
<li>
<p>Add a <code>pypng</code> image factory as a pure Python PNG solution. If <code>pillow</code> is
<em>not</em> installed, then this becomes the default factory.</p>
</li>
<li>
<p>The <code>pymaging</code> image factory has been removed, but its factory shortcut and
the actual PymagingImage factory class now just link to the PyPNGImage
factory.</p>
</li>
</ul>
<h1>7.3.1 (1 October 2021)</h1>
<ul>
<li>Improvements for embedded image.</li>
</ul>
<h1>7.3 (19 August 2021)</h1>
<ul>
<li>Skip color mask if QR is black and white</li>
</ul>
<h1>7.2 (19 July 2021)</h1>
<ul>
<li>Add Styled PIL image factory, allowing different color masks and shapes in QR codes</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/9f4704c9285afa953702fa4303fc3ffa8cc28b26"><code>9f4704c</code></a> Preparing release 7.4.2</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/2ddbc55f5047cc3a9a8330d382f15f5a3d101aea"><code>2ddbc55</code></a> Allow png factory to save to a string path</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/8d38c156642ee4d06cdb8e1321e1eda4385fbd96"><code>8d38c15</code></a> Back to development: 7.5</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/96f8a2100fab5fc225d43599e644d75379b72216"><code>96f8a21</code></a> Preparing release 7.4.1</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/8296222ceb0c02f042da595212bbd356ab706e26"><code>8296222</code></a> Add changelog</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/7c99a2791554e828d8512bfdaa3d9e9b09f2c989"><code>7c99a27</code></a> Add section to setup.cfg so zest builds a wheel</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/14a663ce5dde0479ce01a736f97961da218a4aa7"><code>14a663c</code></a> Merge pull request <a href="https://redirect.github.com/lincolnloop/python-qrcode/issues/305">#305</a> from mattiasj-axis/fix304</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/aa485a845ddfc26a8a87d2c984ddc05a3c3d03ce"><code>aa485a8</code></a> Merge pull request <a href="https://redirect.github.com/lincolnloop/python-qrcode/issues/303">#303</a> from mgorny/wheel</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/2ab3467ba6f73d019d6b4d842281172699d37a39"><code>2ab3467</code></a> Fix create_bytes data concatenation</li>
<li><a href="https://github.com/lincolnloop/python-qrcode/commit/5b00e106a3d926a5e501bac914d0ad3eae1ae57e"><code>5b00e10</code></a> Remove redundant wheel dep from pyproject.toml</li>
<li>Additional commits viewable in <a href="https://github.com/lincolnloop/python-qrcode/compare/v6.1...v7.4.2">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2024-05-24 21:47:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2984" class=".btn">#2984</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump rlp from 4.0.0 to 4.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [rlp](https://github.com/ethereum/pyrlp) from 4.0.0 to 4.0.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/pyrlp/blob/main/docs/release_notes.rst">rlp's changelog</a>.</em></p>
<blockquote>
<h2>pyrlp v4.0.1 (2024-04-24)</h2>
<p>Internal Changes - for pyrlp Contributors</p>
<pre><code>
- Add python 3.12 support, ``rust-backend`` now works with python 3.11 and 3.12 (`[#150](https://github.com/ethereum/pyrlp/issues/150) &lt;https://github.com/ethereum/pyrlp/issues/150&gt;`__)
<p>Miscellaneous Changes</p>
<pre><code>
- `[#151](https://github.com/ethereum/pyrlp/issues/151) &amp;lt;https://github.com/ethereum/pyrlp/issues/151&amp;gt;`__
&lt;/code&gt;&lt;/pre&gt;
&lt;/blockquote&gt;
&lt;/details&gt;
&lt;details&gt;
&lt;summary&gt;Commits&lt;/summary&gt;

&lt;ul&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/f2b3f68001b43e6fb4b81151f5ab33ca29ebf5d2&quot;&gt;&lt;code&gt;f2b3f68&lt;/code&gt;&lt;/a&gt; Bump version: 4.0.0 → 4.0.1&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/a90209ad037e367326db95783968775e13be7385&quot;&gt;&lt;code&gt;a90209a&lt;/code&gt;&lt;/a&gt; Compile release notes for v4.0.1&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/496f73c2fd739429320c96a9519883aefb22959b&quot;&gt;&lt;code&gt;496f73c&lt;/code&gt;&lt;/a&gt; fix docs ci&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/9960c74ff650584a6ea8b03e3939c6bd10a8e8a7&quot;&gt;&lt;code&gt;9960c74&lt;/code&gt;&lt;/a&gt; Merge pull request &lt;a href=&quot;https://redirect.github.com/ethereum/pyrlp/issues/150&quot;&gt;#150&lt;/a&gt; from pacrob/upgrade-template&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/b88b1cefee98fdeabaee65708d1fc576baf4750f&quot;&gt;&lt;code&gt;b88b1ce&lt;/code&gt;&lt;/a&gt; Update README.md&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/ac8c476a42143ead087c64e8df36c6860c06c029&quot;&gt;&lt;code&gt;ac8c476&lt;/code&gt;&lt;/a&gt; move all tests under core, add rust backend tests for py312&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/6b331e16e8f6a078388374f1f1cb34f88c3203f7&quot;&gt;&lt;code&gt;6b331e1&lt;/code&gt;&lt;/a&gt; merge template, fill vars, lint&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/f29c8ad8f0a408ed909bf494bb1538f4c69efa8e&quot;&gt;&lt;code&gt;f29c8ad&lt;/code&gt;&lt;/a&gt; &lt;code&gt;scripts&lt;/code&gt; directory included in dist but not in wheel. (&lt;a href=&quot;https://redirect.github.com/ethereum/pyrlp/issues/130&quot;&gt;#130&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/6a869e7d24951b7ecfd4c2ce21ece92e8cb33131&quot;&gt;&lt;code&gt;6a869e7&lt;/code&gt;&lt;/a&gt; Update Makefile&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/ethereum/pyrlp/commit/74f0a2fac926aba086d2f59cfac00a4844904fce&quot;&gt;&lt;code&gt;74f0a2f&lt;/code&gt;&lt;/a&gt; &lt;code&gt;sphinx-autobuild&lt;/code&gt; for live docs updates (&lt;a href=&quot;https://redirect.github.com/ethereum/pyrlp/issues/129&quot;&gt;#129&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;Additional commits viewable in &lt;a href=&quot;https://github.com/ethereum/pyrlp/compare/v4.0.0...v4.0.1&quot;&gt;compare view&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;/details&gt;

&lt;br /&gt;
</code></pre>


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rlp&package-manager=pip&previous-version=4.0.0&new-version=4.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:43:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2983" class=".btn">#2983</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump nest-asyncio from 1.5.9 to 1.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [nest-asyncio](https://github.com/erdewit/nest_asyncio) from 1.5.9 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/erdewit/nest_asyncio/releases">nest-asyncio's releases</a>.</em></p>
<blockquote>
<p>v1.6.0</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/19f396f9396bfd34b1b0caeb9b4c631ee3d7eb21"><code>19f396f</code></a> Remove redundant blank line.</li>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/c31e7c44f063819ea2d0738e3c72c25458d3fd1b"><code>c31e7c4</code></a> Pre-empt current task before running handle, allowing unpatched tasks, fixes <a href="https://redirect.github.com/erdewit/nest_asyncio/issues/80">#80</a></li>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/35618de086e8844d24039d2fcd090b8f1647c743"><code>35618de</code></a> v1.5.9</li>
<li>See full diff in <a href="https://github.com/erdewit/nest_asyncio/compare/v1.5.9...v1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nest-asyncio&package-manager=pip&previous-version=1.5.9&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:42:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2982" class=".btn">#2982</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump portalocker from 2.7.0 to 2.8.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [portalocker](https://github.com/wolph/portalocker) from 2.7.0 to 2.8.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/wolph/portalocker/releases">portalocker's releases</a>.</em></p>
<blockquote>
<h2>v2.8.2</h2>
<p>Removed docs from build to fix <a href="https://redirect.github.com/wolph/portalocker/issues/88">#88</a> again</p>
<h2>v2.8.1</h2>
<p>Removed docs from build to fix <a href="https://redirect.github.com/wolph/portalocker/issues/88">#88</a></p>
<h2>v2.8.0</h2>
<p>Added support for Python 3.11 and 3.12 thanks to <a href="https://github.com/hugovk"><code>@​hugovk</code></a>. Made the package fully ruff, pyright and mypy compliant with automated testsing using both tox and Github actions</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/wolph/portalocker/commit/36229d2c34bcb434e112bf20d53683a960aa28db"><code>36229d2</code></a> Merge branch 'release/2.8.2'</li>
<li><a href="https://github.com/wolph/portalocker/commit/365c5f645c7d0af9c2d66c5a6520d1ee056f0a7b"><code>365c5f6</code></a> Incrementing version to v2.8.2</li>
<li><a href="https://github.com/wolph/portalocker/commit/3b43b84b23a3fcb3c99ffe09456eec66fbfa397b"><code>3b43b84</code></a> attempt <a href="https://redirect.github.com/wolph/portalocker/issues/2">#2</a> to fix <a href="https://redirect.github.com/wolph/portalocker/issues/88">#88</a></li>
<li><a href="https://github.com/wolph/portalocker/commit/f8b7c61b31296c783abef3a03bc75da6cd3879eb"><code>f8b7c61</code></a> Merge tag 'v2.8.1' into develop</li>
<li><a href="https://github.com/wolph/portalocker/commit/219cb5b30d9f210719d84d0c2259db3c6139b5a6"><code>219cb5b</code></a> Merge branch 'release/2.8.1'</li>
<li><a href="https://github.com/wolph/portalocker/commit/9b8ee01699f577be66372f064c9c86ba2542d76e"><code>9b8ee01</code></a> Incrementing version to v2.8.1</li>
<li><a href="https://github.com/wolph/portalocker/commit/17b9be50c2ec00af2bb5ce36d890e48928f0f5b5"><code>17b9be5</code></a> Removed docs from build to fix <a href="https://redirect.github.com/wolph/portalocker/issues/88">#88</a></li>
<li><a href="https://github.com/wolph/portalocker/commit/b4a0e8d1d3bb17b4cd2069f5084f25918a3338bc"><code>b4a0e8d</code></a> Merge branch 'release/2.8.0'</li>
<li><a href="https://github.com/wolph/portalocker/commit/37865042e3d146d075399f2390c253d31893242e"><code>3786504</code></a> Merge tag 'v2.8.0' into develop</li>
<li><a href="https://github.com/wolph/portalocker/commit/1bf6d4cd38b0a3898325c70aa5bef1906668b36f"><code>1bf6d4c</code></a> Incrementing version to v2.8.0</li>
<li>Additional commits viewable in <a href="https://github.com/wolph/portalocker/compare/v2.7.0...v2.8.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=portalocker&package-manager=pip&previous-version=2.7.0&new-version=2.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:41:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2981" class=".btn">#2981</a>
            </td>
            <td>
                <b>
                    chore(deps): Update asyncpg requirement from ~=0.26.0 to ~=0.29.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [asyncpg](https://github.com/MagicStack/asyncpg) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/MagicStack/asyncpg/releases">asyncpg's releases</a>.</em></p>
<blockquote>
<h2>v0.29.0</h2>
<p>Minor fixes and improvements.</p>
<h1>Improvements</h1>
<ul>
<li>
<p>Python 3.12 and PostgreSQL 16 support (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1084">#1084</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in deea86ce)</p>
</li>
<li>
<p>Add support for tuple-format custom codecs on composite types (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1061">#1061</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 922fcd10)</p>
</li>
<li>
<p>Support <code>target_session_attrs</code> in URL format, add tests (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1073">#1073</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 7cb4e70d)</p>
</li>
<li>
<p>Infinity numeric support (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1067">#1067</a>)
(by <a href="https://github.com/krokoziabla"><code>@​krokoziabla</code></a> in 0c3bf600 for <a href="https://redirect.github.com/MagicStack/asyncpg/issues/1020">#1020</a>)</p>
</li>
<li>
<p>Add support for the <code>WHERE</code> clause in <code>copy_to</code> methods (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/941">#941</a>)
(by <a href="https://github.com/kaylynn234"><code>@​kaylynn234</code></a> in b7ffab6c)</p>
</li>
<li>
<p>Add query logging callbacks and context manager (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1043">#1043</a>)
(by <a href="https://github.com/dcwatson"><code>@​dcwatson</code></a> in b2697ffd)</p>
</li>
</ul>
<h1>Fixes</h1>
<ul>
<li>
<p>When prepared statements are disabled, avoid relying on them harder (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1065">#1065</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in cbf64e18)</p>
</li>
<li>
<p>Handle environments with HOME set to a not-a-directory (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1063">#1063</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in af922bcf)</p>
</li>
<li>
<p>Fix handling of non-ASCII passwords (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1062">#1062</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 89d5bd03)</p>
</li>
<li>
<p>Disable JIT while doing type introspection (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1082">#1082</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in f21ebf64)</p>
</li>
<li>
<p>Remove connection parameter caching in <code>Pool</code> (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1053">#1053</a>)
(by <a href="https://github.com/ermakov-oleg"><code>@​ermakov-oleg</code></a> in 4ddb0397)</p>
</li>
<li>
<p>Switch to Python 3.12-style <code>wait_for</code> (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1086">#1086</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 4bdd8a7e)</p>
</li>
<li>
<p>Update automatic PostGIS type conversion for Shapely 2.0 (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1085">#1085</a>)
(by <a href="https://github.com/ChimneySwift"><code>@​ChimneySwift</code></a> in 8b45beb4)</p>
</li>
<li>
<p>Use the <code>timeout</code> context manager in the connection path (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1087">#1087</a>)
(by <a href="https://github.com/elprans"><code>@​elprans</code></a> in 313b2b2b)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/MagicStack/asyncpg/commit/74f3a0031532b314d9141b6de12aa74db7726b3d"><code>74f3a00</code></a> asyncpg v0.29.0</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/d7faaff57a7a9c0029a31f09564d30ab35007907"><code>d7faaff</code></a> fix: allow host tuple (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1021">#1021</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/b2697ffdf18f7acd88a35e9a0a252c3b6fb25070"><code>b2697ff</code></a> Add query logging callbacks and context manager (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1043">#1043</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/93a6f79afb4251fa48edf6959aa87532eee91ef5"><code>93a6f79</code></a> Cut BaseProtocol circular reference on close. (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1049">#1049</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/ca9f03be3c64984311dbefbbd9e8ff0806a7f772"><code>ca9f03b</code></a> Close cursor portals once the iterator is exhausted (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1088">#1088</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/b7ffab6cb3f9bcc5d4f9c5b22398ca9c9e450af2"><code>b7ffab6</code></a> Add support for the <code>WHERE</code> clause in <code>copy_to</code> methods (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/941">#941</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/70c8bd814f9d289741845fa8dc761737f7ea4e78"><code>70c8bd8</code></a> Use cleanup_ctx in pool usage doc (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/878">#878</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/ccc7baf94cd45fc0155ae522361a6f2b2f551c44"><code>ccc7baf</code></a> Small fix for documentation on using SSL in Connection (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/995">#995</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/313b2b2bedcc10baf5871124ee915fdc48f5c4b7"><code>313b2b2</code></a> Use the <code>timeout</code> context manager in the connection path (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1087">#1087</a>)</li>
<li><a href="https://github.com/MagicStack/asyncpg/commit/8b45beb4b60e30ad6ccd19d1e925ffdad6477aa2"><code>8b45beb</code></a> Update automatic PostGIS type conversion for Shapely 2.0 (<a href="https://redirect.github.com/MagicStack/asyncpg/issues/1085">#1085</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/MagicStack/asyncpg/compare/v0.26.0...v0.29.0">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2024-05-24 21:40:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2980" class=".btn">#2980</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump markdown from 3.5.2 to 3.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [markdown](https://github.com/Python-Markdown/markdown) from 3.5.2 to 3.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Python-Markdown/markdown/releases">markdown's releases</a>.</em></p>
<blockquote>
<h2>Release 3.6</h2>
<h3>Changed</h3>
<h4>Refactor TOC Sanitation</h4>
<ul>
<li>All postprocessors are now run on heading content.</li>
<li>Footnote references are now stripped from heading content. Fixes <a href="https://redirect.github.com/Python-Markdown/markdown/issues/660">#660</a>.</li>
<li>A more robust <code>striptags</code> is provided to convert headings to plain text.
Unlike, the <code>markupsafe</code> implementation, HTML entities are not unescaped.</li>
<li>The plain text <code>name</code>, rich <code>html</code>, and unescaped raw <code>data-toc-label</code> are
saved to <code>toc_tokens</code>, allowing users to access the full rich text content of
the headings directly from <code>toc_tokens</code>.</li>
<li>The value of <code>data-toc-label</code> is sanitized separate from heading content
before being written to <code>name</code>. This fixes a bug which allowed markup through
in certain circumstances. To access the raw unsanitized data, retrieve the
value from <code>token['data-toc-label']</code> directly.</li>
<li>An <code>html.unescape</code> call is made just prior to calling <code>slugify</code> so that
<code>slugify</code> only operates on Unicode characters. Note that <code>html.unescape</code> is
not run on <code>name</code>, <code>html</code>, or <code>data-toc-label</code>.</li>
<li>The functions <code>get_name</code> and <code>stashedHTML2text</code> defined in the <code>toc</code> extension
are both <strong>deprecated</strong>. Instead, third party extensions should use some
combination of the new functions <code>run_postprocessors</code>, <code>render_inner_html</code> and
<code>striptags</code>.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Include <code>scripts/*.py</code> in the generated source tarballs (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1430">#1430</a>).</li>
<li>Ensure lines after heading in loose list are properly detabbed (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1443">#1443</a>).</li>
<li>Give smarty tree processor higher priority than toc (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1440">#1440</a>).</li>
<li>Permit carets (<code>^</code>) and square brackets (<code>]</code>) but explicitly exclude
backslashes (<code>\</code>) from abbreviations (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1444">#1444</a>).</li>
<li>In attribute lists (<code>attr_list</code>, <code>fenced_code</code>), quoted attribute values are
now allowed to contain curly braces (<code>}</code>) (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1414">#1414</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/Python-Markdown/markdown/blob/master/docs/changelog.md">markdown's changelog</a>.</em></p>
<blockquote>
<h2>[3.6] -- 2024-03-14</h2>
<h3>Changed</h3>
<h4>Refactor TOC Sanitation</h4>
<ul>
<li>All postprocessors are now run on heading content.</li>
<li>Footnote references are now stripped from heading content. Fixes <a href="https://redirect.github.com/Python-Markdown/markdown/issues/660">#660</a>.</li>
<li>A more robust <code>striptags</code> is provided to convert headings to plain text.
Unlike, the <code>markupsafe</code> implementation, HTML entities are not unescaped.</li>
<li>The plain text <code>name</code>, rich <code>html</code>, and unescaped raw <code>data-toc-label</code> are
saved to <code>toc_tokens</code>, allowing users to access the full rich text content of
the headings directly from <code>toc_tokens</code>.</li>
<li>The value of <code>data-toc-label</code> is sanitized separate from heading content
before being written to <code>name</code>. This fixes a bug which allowed markup through
in certain circumstances. To access the raw unsanitized data, retrieve the
value from <code>token['data-toc-label']</code> directly.</li>
<li>An <code>html.unescape</code> call is made just prior to calling <code>slugify</code> so that
<code>slugify</code> only operates on Unicode characters. Note that <code>html.unescape</code> is
not run on <code>name</code>, <code>html</code>, or <code>data-toc-label</code>.</li>
<li>The functions <code>get_name</code> and <code>stashedHTML2text</code> defined in the <code>toc</code> extension
are both <strong>deprecated</strong>. Instead, third party extensions should use some
combination of the new functions <code>run_postprocessors</code>, <code>render_inner_html</code> and
<code>striptags</code>.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Include <code>scripts/*.py</code> in the generated source tarballs (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1430">#1430</a>).</li>
<li>Ensure lines after heading in loose list are properly detabbed (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1443">#1443</a>).</li>
<li>Give smarty tree processor higher priority than toc (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1440">#1440</a>).</li>
<li>Permit carets (<code>^</code>) and square brackets (<code>]</code>) but explicitly exclude
backslashes (<code>\</code>) from abbreviations (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1444">#1444</a>).</li>
<li>In attribute lists (<code>attr_list</code>, <code>fenced_code</code>), quoted attribute values are
now allowed to contain curly braces (<code>}</code>) (<a href="https://redirect.github.com/Python-Markdown/markdown/issues/1414">#1414</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Python-Markdown/markdown/commit/e524b8fe938738cb4492411a34cce89051cb9695"><code>e524b8f</code></a> Bump version to 3.6</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/3d8afc6f89e169522f44c1bbec15f66dc359eccb"><code>3d8afc6</code></a> Allow attr_list quoted values to contain curly braces</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/9edba85fc14f034b7109534220702bf60178ff15"><code>9edba85</code></a> Refactor abbr escaping</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/e4ab4a610edc6332ce81a53aa4ae6f97516ce461"><code>e4ab4a6</code></a> Refactor TOC sanitation</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/a18765c25cccab23f400edeac94d20f4be00492b"><code>a18765c</code></a> Explicitly omit carot and backslash from abbr</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/421f1e88ff4661b4433b97ec57b040a2a74e5aed"><code>421f1e8</code></a> Give smarty tree processor higher priority than toc</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/c334a3e47e6565469344154f966cf0eb9aca0de3"><code>c334a3e</code></a> Ensure lines after heading in loose list are properly detabbed</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/ea92856855a6314488acb121f21f8fa02860e008"><code>ea92856</code></a> Update the license template so GitHub can detect it</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/a2effd6d5191808c8b2e347965f6fcf4aa709e78"><code>a2effd6</code></a> Disable mkdocstrings show_symbol_type_toc option to work around searching iss...</li>
<li><a href="https://github.com/Python-Markdown/markdown/commit/91f9a1205d32f3bc6a27ca5f993409c3b97c1931"><code>91f9a12</code></a> Restore Attribute symbol type in mkdocstrings template</li>
<li>Additional commits viewable in <a href="https://github.com/Python-Markdown/markdown/compare/3.5.2...3.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=markdown&package-manager=pip&previous-version=3.5.2&new-version=3.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:40:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2979" class=".btn">#2979</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump pytest from 7.4.2 to 7.4.4 in /demo/playground/examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 7.4.2 to 7.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>pytest 7.4.4 (2023-12-31)</h2>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/11140">#11140</a>: Fix non-string constants at the top of file being detected as docstrings on Python&gt;=3.8.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/11572">#11572</a>: Handle an edge case where <code>sys.stderr</code>{.interpreted-text role=&quot;data&quot;} and <code>sys.__stderr__</code>{.interpreted-text role=&quot;data&quot;} might already be closed when <code>faulthandler</code>{.interpreted-text role=&quot;ref&quot;} is tearing down.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/11710">#11710</a>: Fixed tracebacks from collection errors not getting pruned.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/7966">#7966</a>: Removed unhelpful error message from assertion rewrite mechanism when exceptions are raised in <code>__iter__</code> methods. Now they are treated un-iterable instead.</li>
</ul>
<h2>Improved Documentation</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/11091">#11091</a>: Updated documentation to refer to hyphenated options: replaced <code>--junitxml</code> with <code>--junit-xml</code> and <code>--collectonly</code> with <code>--collect-only</code>.</li>
</ul>
<h2>pytest 7.4.3 (2023-10-24)</h2>
<h2>Bug Fixes</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/10447">#10447</a>: Markers are now considered in the reverse mro order to ensure base  class markers are considered first -- this resolves a regression.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11239">#11239</a>: Fixed <code>:=</code> in asserts impacting unrelated test cases.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11439">#11439</a>: Handled an edge case where :data:<code>sys.stderr</code> might already be closed when :ref:<code>faulthandler</code> is tearing down.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/33f694f4b30c5c502f21f81cb8ab907b12ad2f65"><code>33f694f</code></a> Prepare release version 7.4.4</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/76c107c463afcaddf74ca48252614728c6829ea7"><code>76c107c</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/11751">#11751</a> from bluetech/backport-11143-to-7.4.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/531d76daa4a871df5b2a46cae132851c29abf027"><code>531d76d</code></a> [7.4.x] Improve reporting from <strong>iter</strong> exceptions (<a href="https://redirect.github.com/pytest-dev/pytest/issues/11749">#11749</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a0f58fa9e7f9b09b212ed491464be5df9b80fc0b"><code>a0f58fa</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/11143">#11143</a> from tushar-deepsource/patch-1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/b1f3387d42571090ee4a35ec1945765b7f2ffae8"><code>b1f3387</code></a> [7.4.x] <a href="https://redirect.github.com/pytest-dev/pytest/issues/11091">#11091</a>: documentation should use hypthonated properties (<a href="https://redirect.github.com/pytest-dev/pytest/issues/11750">#11750</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2cdd619bf49ee7c5306dc70dcbf71090839ea985"><code>2cdd619</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/11747">#11747</a> from pytest-dev/backport-11711-to-7.4.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d06c05bd23ea6af8e07fd944e56c58b64375b724"><code>d06c05b</code></a> [7.4.x] nodes: fix tracebacks from collection errors are not getting pruned</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/5582bfcddf78929f7979c5023b167b333e1c2dd9"><code>5582bfc</code></a> [7.4.x] Improves clarity in Sphinx documentation for function signature. (<a href="https://redirect.github.com/pytest-dev/pytest/issues/11">#11</a>...</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/13024efd7afdbae80ce70d27295d9bbe62670cb8"><code>13024ef</code></a> [7.4.x] Fix for operation on closed file in faulthandler teardown (<a href="https://redirect.github.com/pytest-dev/pytest/issues/11631">#11631</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a40dacf6577ae990740e10572582538dfaf357b6"><code>a40dacf</code></a> [7.4.x] XFAIL TestLocalPath.test_make_numbered_dir_multiprocess_safe (<a href="https://redirect.github.com/pytest-dev/pytest/issues/11616">#11616</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/7.4.2...7.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=7.4.2&new-version=7.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:39:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2978" class=".btn">#2978</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump requests from 2.31.0 to 2.32.2 in /demo/playground/examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.31.0 to 2.32.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>v2.32.0</h2>
<h2>2.32.0 (2024-05-20)</h2>
<h2>🐍 PYCON US 2024 EDITION 🐍</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li><a href="https://github.com/psf/requests/commit/d6ebc4a2f1f68b7e355fb7e4dd5ffc0845547f9f"><code>d6ebc4a</code></a> v2.32.0</li>
<li><a href="https://github.com/psf/requests/commit/9a40d1277807f0a4f26c9a37eea8ec90faa8aadc"><code>9a40d12</code></a> Avoid reloading root certificates to improve concurrent performance (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li><a href="https://github.com/psf/requests/commit/0c030f78d24f29a459dbf39b28b4cc765e2153d7"><code>0c030f7</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a> from nateprewitt/no_char_detection</li>
<li><a href="https://github.com/psf/requests/commit/555b870eb19d497ddb67042645420083ec8efb02"><code>555b870</code></a> Allow character detection dependencies to be optional in post-packaging steps</li>
<li><a href="https://github.com/psf/requests/commit/d6dded3f00afcf56a7e866cb0732799045301eb0"><code>d6dded3</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6700">#6700</a> from franekmagiera/update-redirect-to-invalid-uri-test</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.31.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.31.0&new-version=2.32.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:38:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2977" class=".btn">#2977</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump pytest-asyncio from 0.21.1 to 0.23.7 in /demo/playground/examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.21.1 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.6</h2>
<h1>0.23.6 (2024-03-19)</h1>
<ul>
<li>Fix compatibility with pytest 8.2 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/800">#800</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5.post1</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5a0</h2>
<h1>0.23.5 (UNRELEASED)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4</h2>
<h1>0.23.4 (2024-01-28)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
<li>Addresses further issues that caused an internal pytest error during test collection</li>
<li>Declares incompatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.21.1...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.21.1&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:38:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2976" class=".btn">#2976</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump hyperledger/aries-cloudagent-python from py3.9-0.9.0 to py3.9-0.12.1 in /demo/multi-demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps [hyperledger/aries-cloudagent-python](https://github.com/hyperledger/aries-cloudagent-python) from py3.9-0.9.0 to py3.9-0.12.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/hyperledger/aries-cloudagent-python/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyperledger/aries-cloudagent-python&package-manager=docker&previous-version=py3.9-0.9.0&new-version=py3.9-0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2975" class=".btn">#2975</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump hyperledger/aries-cloudagent-python from py3.9-0.10.4 to py3.9-0.12.1 in /demo/playground
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps [hyperledger/aries-cloudagent-python](https://github.com/hyperledger/aries-cloudagent-python) from py3.9-0.10.4 to py3.9-0.12.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/hyperledger/aries-cloudagent-python/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyperledger/aries-cloudagent-python&package-manager=docker&previous-version=py3.9-0.10.4&new-version=py3.9-0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2974" class=".btn">#2974</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump python from 3.9-slim-bullseye to 3.12-slim-bullseye in /docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim-bullseye to 3.12-slim-bullseye.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim-bullseye&new-version=3.12-slim-bullseye)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2973" class=".btn">#2973</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump hyperledger/aries-cloudagent-python from py3.9-0.9.0 to py3.9-0.12.1 in /demo/docker-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps [hyperledger/aries-cloudagent-python](https://github.com/hyperledger/aries-cloudagent-python) from py3.9-0.9.0 to py3.9-0.12.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/hyperledger/aries-cloudagent-python/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyperledger/aries-cloudagent-python&package-manager=docker&previous-version=py3.9-0.9.0&new-version=py3.9-0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2972" class=".btn">#2972</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump postgres from 14 to 16 in /demo/docker-test/db
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps postgres from 14 to 16.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=postgres&package-manager=docker&previous-version=14&new-version=16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2971" class=".btn">#2971</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump python from 3.9-slim to 3.12-slim in /demo/playground/examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim to 3.12-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim&new-version=3.12-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2970" class=".btn">#2970</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump sphinx-rtd-theme from 1.1.1 to 1.3.0 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [sphinx-rtd-theme](https://github.com/readthedocs/sphinx_rtd_theme) from 1.1.1 to 1.3.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/readthedocs/sphinx_rtd_theme/blob/master/docs/changelog.rst">sphinx-rtd-theme's changelog</a>.</em></p>
<blockquote>
<h1>1.3.0</h1>
<h2>Added</h2>
<ul>
<li>Relaxed requirements to include Sphinx release <code>7.0</code></li>
</ul>
<p>.. _release-1.2.2:</p>
<h1>1.2.2</h1>
<h2>Fixes</h2>
<ul>
<li>Require <code>sphinxcontrib-jquery&gt;=4,&lt;5</code> (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1446">#1446</a>)</li>
</ul>
<h2>Added</h2>
<ul>
<li>Styling for <code>:menuselection:</code> (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1426">#1426</a>)</li>
</ul>
<p>.. _release-1.2.1:</p>
<h1>1.2.1</h1>
<h2>Fixes</h2>
<ul>
<li>Load jQuery correctly when using latest sphinxcontrib-jquery release (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1448">#1448</a>)</li>
</ul>
<p>.. _release-1.2.0:</p>
<h1>1.2.0</h1>
<h2>Dependency changes</h2>
<ul>
<li>docutils 0.18 is supported. (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1381">#1381</a>)</li>
<li>Sphinx 6 support added</li>
<li>Added <code>sphinxcontrib-jquery</code> as a dependency (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1385">#1385</a> <a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1421">#1421</a>)</li>
<li>Python 3.11 is officially supported and tested. (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1395">#1395</a>)</li>
<li>Python 3.4 and 3.5 are officially not supported (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1395">#1395</a>)</li>
</ul>
<p>Changes</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/15ed4de08de55f7066ff4f2ac39883a397db30d3"><code>15ed4de</code></a> Release 1.3.0 (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1509">#1509</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/b5833585b25358be94918f13c50530e3e9237e7e"><code>b583358</code></a> 1.3.0rc2 (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1495">#1495</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/775bca403c4d795504b1c0d7c6d41664bdcba842"><code>775bca4</code></a> Release 1.3.0rc1 (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1494">#1494</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/04f85fc42219f8148be142482b9887e64b990f4f"><code>04f85fc</code></a> Add Sphinx 7 support (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1464">#1464</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/9899ee4ee2f547f81e51297dc12317f018e62fdd"><code>9899ee4</code></a> Release 1.2.2 (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1484">#1484</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/2442ab9ffdb8910f8484362cc8dfd165ca3ffb15"><code>2442ab9</code></a> Remove version logic on sphinxcontrib-jquery, require &gt;=4,&lt;5 (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1446">#1446</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/cd6b429f875999ee48bd914da5369422aa55dd8f"><code>cd6b429</code></a> :menuselection: style (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1426">#1426</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/2107797b002848b3336694541b14ffa2367afc2c"><code>2107797</code></a> Contributing updates (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1478">#1478</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/72691f502500c8fc0c0d22422d0919bc628ddf5f"><code>72691f5</code></a> Release 1.2.1 (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1474">#1474</a>)</li>
<li><a href="https://github.com/readthedocs/sphinx_rtd_theme/commit/d836ff798cb5032b9d32eccc9a86b69bed256975"><code>d836ff7</code></a> Docs: Typo in recommended pinning (<a href="https://redirect.github.com/readthedocs/sphinx_rtd_theme/issues/1476">#1476</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/readthedocs/sphinx_rtd_theme/compare/1.1.1...1.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sphinx-rtd-theme&package-manager=pip&previous-version=1.1.1&new-version=1.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2969" class=".btn">#2969</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump untergeek/curator from 8.0.2 to 8.0.15 in /demo/elk-stack/extensions/curator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps untergeek/curator from 8.0.2 to 8.0.15.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=untergeek/curator&package-manager=docker&previous-version=8.0.2&new-version=8.0.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 21:37:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2968" class=".btn">#2968</a>
            </td>
            <td>
                <b>
                    Sonarcloud with code coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is used to get code coverage for our sonarcloud integration on PR's and when code is pushed to main. 

The complication comes with using the sonarcloud token from forked repos. I have tested using two github accounts and forking my fork. 

This works by saving the test report from the `PR Tests` workflow as an artifact and also the pr number. Then when the `PR Tests` workflow completes successfully a workflow will begin for sonarcloud witch gets information about the forked repo, and fetches the code for the scan. The code coverage is downloaded from the artifact, updated and then upload to sonarcloud.

Another workflow runs the tests on merge to main, runs the scan and uploads results. I thought about doing this as one workflow but decided separate workflows was actually much simpler.

I changed the workflow `Tests` to an action and adjusted the other workflows that used it. When calling from the push to main workflow it was having trouble as a workflow.

Requires disabling `Automatic Analysis` in the sonarcloud admin console. You can't use automatic and manage it from CI at the same time. Also won't exist until the workflows have been merged to main.

Main branch:

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/028b59c9-6977-4402-a26b-5d693305b3a3)

PR (Failing):

The required coverage can be adjusted in sonarcloud console.

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/4b30d724-da76-4187-ae6b-619e8c839568)

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/ee0efd1a-d5fb-4ffe-8c2b-5c6a0b2f0890)

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/a6ec57c1-ac31-4802-b93d-4cdddc4ada9d)

PR (Passing):

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/ff860d3b-5746-4248-8c30-b69f1334d79e)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-24 19:51:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2967" class=".btn">#2967</a>
            </td>
            <td>
                <b>
                    Add support for revocable credentials in vc_di handler
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
        Created At 2024-05-24 11:15:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2961" class=".btn">#2961</a>
            </td>
            <td>
                <b>
                    Fix Snyk sarif file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the issue with Snyk sarif file. Replace any "null" security severity values with 0. The null value is used in the case of license-related findings, which do not do not indicate a security vulnerability.

See https://github.com/github/codeql-action/issues/2187 for more context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 19:27:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2960" class=".btn">#2960</a>
            </td>
            <td>
                <b>
                    feat: VC DI proof request
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
        Created At 2024-05-21 18:09:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2959" class=".btn">#2959</a>
            </td>
            <td>
                <b>
                    DIDComm V2 Initial Implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The purpose of this PR is to add basic DIDComm V2 support to ACA-Py. It is our intention to add support gradually with small PRs, rather than one massive PR. To that end, at present, here's what we've added:

- Added `--experimental-didcomm-v2` flag to enable the DIDComm V2 code
- Added the ability to decrypt/unpack V2 messages
- When a message is received, we respond back with a DIDComm V1 problem report (there-by, providing a foundation to rely upon when adding protocols) and pack it the same way that we'd pack a DIDComm V2 message
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 14:50:00 +0000 UTC
    </div>
</div>

