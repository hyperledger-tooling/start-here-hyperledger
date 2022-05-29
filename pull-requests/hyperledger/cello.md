---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    Nominate yuanmao as new maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Yuanmao continues contributing to the Cello project after his intern for
more than 3 months. He is working mainly on the API-engine component,
and the agent. Yuanmao is also very active in proposing features and
resolving implementation issues.

Retire inactive maintainer Qiang Xu, thanks for his past contributions!

Signed-off-by: Baohua Yang <yangbaohua@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-29 14:28:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/447" class=".btn">#447</a>
            </td>
            <td>
                <b>
                    Bump pyjwt from 1.7.1 to 2.4.0 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pyjwt](https://github.com/jpadilla/pyjwt) from 1.7.1 to 2.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jpadilla/pyjwt/releases">pyjwt's releases</a>.</em></p>
<blockquote>
<h2>2.4.0</h2>
<h2>Security</h2>
<ul>
<li>[CVE-2022-29217] Prevent key confusion through non-blocklisted public key formats. <a href="https://github.com/jpadilla/pyjwt/security/advisories/GHSA-ffqj-6fqr-9h24">https://github.com/jpadilla/pyjwt/security/advisories/GHSA-ffqj-6fqr-9h24</a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Add support for Python 3.10 by <a href="https://github.com/hugovk"><code>@​hugovk</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/699">jpadilla/pyjwt#699</a></li>
<li>Don't use implicit optionals by <a href="https://github.com/rekyungmin"><code>@​rekyungmin</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/705">jpadilla/pyjwt#705</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/708">jpadilla/pyjwt#708</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/710">jpadilla/pyjwt#710</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/711">jpadilla/pyjwt#711</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/712">jpadilla/pyjwt#712</a></li>
<li>documentation fix: show correct scope for decode_complete() by <a href="https://github.com/sseering"><code>@​sseering</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/661">jpadilla/pyjwt#661</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/716">jpadilla/pyjwt#716</a></li>
<li>Explicit check the key for ECAlgorithm by <a href="https://github.com/estin"><code>@​estin</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/713">jpadilla/pyjwt#713</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/720">jpadilla/pyjwt#720</a></li>
<li>api_jwk: Add PyJWKSet.<strong>getitem</strong> by <a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/725">jpadilla/pyjwt#725</a></li>
<li>Update usage.rst by <a href="https://github.com/guneybilen"><code>@​guneybilen</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/727">jpadilla/pyjwt#727</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/728">jpadilla/pyjwt#728</a></li>
<li>fix: Update copyright information by <a href="https://github.com/kkirsche"><code>@​kkirsche</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/729">jpadilla/pyjwt#729</a></li>
<li>Docs: mention performance reasons for reusing RSAPrivateKey when encoding by <a href="https://github.com/dmahr1"><code>@​dmahr1</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/734">jpadilla/pyjwt#734</a></li>
<li>Fixed typo in usage.rst by <a href="https://github.com/israelabraham"><code>@​israelabraham</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/738">jpadilla/pyjwt#738</a></li>
<li>Add detached payload support for JWS encoding and decoding by <a href="https://github.com/fviard"><code>@​fviard</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/723">jpadilla/pyjwt#723</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/740">jpadilla/pyjwt#740</a></li>
<li>Raise DeprecationWarning for jwt.decode(verify=...) by <a href="https://github.com/akx"><code>@​akx</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/742">jpadilla/pyjwt#742</a></li>
<li>Don't mutate options dictionary in .decode_complete() by <a href="https://github.com/akx"><code>@​akx</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/743">jpadilla/pyjwt#743</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/748">jpadilla/pyjwt#748</a></li>
<li>Replace various string interpolations with f-strings by <a href="https://github.com/akx"><code>@​akx</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/744">jpadilla/pyjwt#744</a></li>
<li>Update CHANGELOG.rst by <a href="https://github.com/hipertracker"><code>@​hipertracker</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/751">jpadilla/pyjwt#751</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/hugovk"><code>@​hugovk</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/699">jpadilla/pyjwt#699</a></li>
<li><a href="https://github.com/rekyungmin"><code>@​rekyungmin</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/705">jpadilla/pyjwt#705</a></li>
<li><a href="https://github.com/sseering"><code>@​sseering</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/661">jpadilla/pyjwt#661</a></li>
<li><a href="https://github.com/estin"><code>@​estin</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/713">jpadilla/pyjwt#713</a></li>
<li><a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/725">jpadilla/pyjwt#725</a></li>
<li><a href="https://github.com/guneybilen"><code>@​guneybilen</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/727">jpadilla/pyjwt#727</a></li>
<li><a href="https://github.com/dmahr1"><code>@​dmahr1</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/734">jpadilla/pyjwt#734</a></li>
<li><a href="https://github.com/israelabraham"><code>@​israelabraham</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/738">jpadilla/pyjwt#738</a></li>
<li><a href="https://github.com/fviard"><code>@​fviard</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/723">jpadilla/pyjwt#723</a></li>
<li><a href="https://github.com/akx"><code>@​akx</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/742">jpadilla/pyjwt#742</a></li>
<li><a href="https://github.com/hipertracker"><code>@​hipertracker</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/751">jpadilla/pyjwt#751</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jpadilla/pyjwt/compare/2.3.0...2.4.0">https://github.com/jpadilla/pyjwt/compare/2.3.0...2.4.0</a></p>
<h2>2.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/700">jpadilla/pyjwt#700</a></li>
<li>Add exception chaining by <a href="https://github.com/ehdgua01"><code>@​ehdgua01</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/702">jpadilla/pyjwt#702</a></li>
<li>Revert &quot;Remove arbitrary kwargs.&quot; by <a href="https://github.com/auvipy"><code>@​auvipy</code></a> in <a href="https://github-redirect.dependabot.com/jpadilla/pyjwt/pull/701">jpadilla/pyjwt#701</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jpadilla/pyjwt/blob/master/CHANGELOG.rst">pyjwt's changelog</a>.</em></p>
<blockquote>
<h2><code>v2.4.0 &lt;https://github.com/jpadilla/pyjwt/compare/2.3.0...2.4.0&gt;</code>__</h2>
<p>Security</p>
<pre><code>
- [CVE-2022-29217] Prevent key confusion through non-blocklisted public key formats. https://github.com/jpadilla/pyjwt/security/advisories/GHSA-ffqj-6fqr-9h24
<p>Changed</p>
<pre><code>
- Explicit check the key for ECAlgorithm by @estin in https://github.com/jpadilla/pyjwt/pull/713
- Raise DeprecationWarning for jwt.decode(verify=...) by @akx in https://github.com/jpadilla/pyjwt/pull/742

Fixed
~~~~~

- Don't use implicit optionals by @rekyungmin in https://github.com/jpadilla/pyjwt/pull/705
- documentation fix: show correct scope for decode_complete() by @sseering in https://github.com/jpadilla/pyjwt/pull/661
- fix: Update copyright information by @kkirsche in https://github.com/jpadilla/pyjwt/pull/729
- Don't mutate options dictionary in .decode_complete() by @akx in https://github.com/jpadilla/pyjwt/pull/743

Added
~~~~~

- Add support for Python 3.10 by @hugovk in https://github.com/jpadilla/pyjwt/pull/699
- api_jwk: Add PyJWKSet.__getitem__ by @woodruffw in https://github.com/jpadilla/pyjwt/pull/725
- Update usage.rst by @guneybilen in https://github.com/jpadilla/pyjwt/pull/727
- Docs: mention performance reasons for reusing RSAPrivateKey when encoding by @dmahr1 in https://github.com/jpadilla/pyjwt/pull/734
- Fixed typo in usage.rst by @israelabraham in https://github.com/jpadilla/pyjwt/pull/738
- Add detached payload support for JWS encoding and decoding by @fviard in https://github.com/jpadilla/pyjwt/pull/723
- Replace various string interpolations with f-strings by @akx in https://github.com/jpadilla/pyjwt/pull/744
- Update CHANGELOG.rst by @hipertracker in https://github.com/jpadilla/pyjwt/pull/751

`v2.3.0 &amp;lt;https://github.com/jpadilla/pyjwt/compare/2.2.0...2.3.0&amp;gt;`__
-----------------------------------------------------------------------

Fixed
~~~~~

- Revert &amp;quot;Remove arbitrary kwargs.&amp;quot; `[#701](https://github.com/jpadilla/pyjwt/issues/701) &amp;lt;https://github.com/jpadilla/pyjwt/pull/701&amp;gt;`__

Added
~~~~~

- Add exception chaining `[#702](https://github.com/jpadilla/pyjwt/issues/702) &amp;lt;https://github.com/jpadilla/pyjwt/pull/702&amp;gt;`__

`v2.2.0 &amp;lt;https://github.com/jpadilla/pyjwt/compare/2.1.0...2.2.0&amp;gt;`__
-----------------------------------------------------------------------

&amp;lt;/tr&amp;gt;&amp;lt;/table&amp;gt; 
&lt;/code&gt;&lt;/pre&gt;
&lt;/blockquote&gt;
&lt;p&gt;... (truncated)&lt;/p&gt;
&lt;/details&gt;
&lt;details&gt;
&lt;summary&gt;Commits&lt;/summary&gt;

&lt;ul&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/83ff831a4d11190e3a0bed781da43f8d84352653&quot;&gt;&lt;code&gt;83ff831&lt;/code&gt;&lt;/a&gt; chore: update changelog&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/4c1ce8fd9019dd312ff257b5141cdb6d897379d9&quot;&gt;&lt;code&gt;4c1ce8f&lt;/code&gt;&lt;/a&gt; chore: update changelog&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/96f3f0275745c5a455c019a0d3476a054980e8ea&quot;&gt;&lt;code&gt;96f3f02&lt;/code&gt;&lt;/a&gt; fix: failing advisory test&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/9c528670c455b8d948aff95ed50e22940d1ad3fc&quot;&gt;&lt;code&gt;9c52867&lt;/code&gt;&lt;/a&gt; Merge pull request from GHSA-ffqj-6fqr-9h24&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/24b29adfebcb4f057a3cef5aaf35653bc0c1c8cc&quot;&gt;&lt;code&gt;24b29ad&lt;/code&gt;&lt;/a&gt; Update CHANGELOG.rst (&lt;a href=&quot;https://github-redirect.dependabot.com/jpadilla/pyjwt/issues/751&quot;&gt;#751&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/31f5acb8fb3ec6cdfe2b1b0a4a8f329b5f3ca67f&quot;&gt;&lt;code&gt;31f5acb&lt;/code&gt;&lt;/a&gt; Replace various string interpolations with f-strings (&lt;a href=&quot;https://github-redirect.dependabot.com/jpadilla/pyjwt/issues/744&quot;&gt;#744&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/5581a31c21de70444c1162bcfa29f7e0fc86edda&quot;&gt;&lt;code&gt;5581a31&lt;/code&gt;&lt;/a&gt; [pre-commit.ci] pre-commit autoupdate (&lt;a href=&quot;https://github-redirect.dependabot.com/jpadilla/pyjwt/issues/748&quot;&gt;#748&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/3d4d82248f1120c87f1f4e0e8793eaa1d54843a6&quot;&gt;&lt;code&gt;3d4d822&lt;/code&gt;&lt;/a&gt; Don't mutate options dictionary in .decode_complete() (&lt;a href=&quot;https://github-redirect.dependabot.com/jpadilla/pyjwt/issues/743&quot;&gt;#743&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/1f1fe15bb41846c602b3e106176b2c692b93a613&quot;&gt;&lt;code&gt;1f1fe15&lt;/code&gt;&lt;/a&gt; Add a deprecation warning when jwt.decode() is called with the legacy verify=...&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/jpadilla/pyjwt/commit/35fa28e59d99b99c6a780d2a029a74d6bbba8b1e&quot;&gt;&lt;code&gt;35fa28e&lt;/code&gt;&lt;/a&gt; [pre-commit.ci] pre-commit autoupdate (&lt;a href=&quot;https://github-redirect.dependabot.com/jpadilla/pyjwt/issues/740&quot;&gt;#740&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;Additional commits viewable in &lt;a href=&quot;https://github.com/jpadilla/pyjwt/compare/1.7.1...2.4.0&quot;&gt;compare view&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;/details&gt;

&lt;br /&gt;
</code></pre>


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pyjwt&package-manager=pip&previous-version=1.7.1&new-version=2.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 05:09:01 +0000 UTC
    </div>
</div>

