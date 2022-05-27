---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2048" class=".btn">#2048</a>
            </td>
            <td>
                <b>
                    feat(iroha-connector): implement validator interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(iroha-connector): implement validator interface

Add monitoring and sending async/sync requests to ledger via SocketIO.

Closes: https://github.com/hyperledger/cactus/issues/1941

Author: stepniowskip <piotr.stepniowski@fujitsu.com>

Original PR: #1966
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 11:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2047" class=".btn">#2047</a>
            </td>
            <td>
                <b>
                    refactor(cmd-socketio-server): remove code duplication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Moved verifyValidatorJwt to `cactus-common` to keep encrypt/decrypt logic
  of socketio-based validators in one, common location.
- Move config-reading and signMessageJwt helper functions from validators to cmd-socketio-server
  to remove code duplication.
  Refactor validators to use these common instead of own implementation.
- Remove ValidatorAuthentication.ts that is not used anymore
  (not part of public interface, it was copied by validators during before couple commits ago).
- Create jwt-message-authentication.test.ts from old, similar one in cactus-api-client.
- Updated readme with instructions of how to start asset-trade and electricity-trade samples
  without docker-compose (to be used during development).
  Added helper script for patching the config.

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

-----------------

This PR is for the last commit only - [refactor(cmd-socketio-server): remove code duplication](https://github.com/hyperledger/cactus/commit/200a7da23d68a38eb2c1af8869175e172c1d3b62). Please ignore previous one (dependencies) which will be removed before the merge.

Depends on #2033
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 10:56:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2046" class=".btn">#2046</a>
            </td>
            <td>
                <b>
                    build(deps): bump convict from 6.2.2 to 6.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [convict](https://github.com/mozilla/node-convict) from 6.2.2 to 6.2.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mozilla/node-convict/blob/master/CHANGELOG.md">convict's changelog</a>.</em></p>
<blockquote>
<h2>[6.2.3] - 2022-05-07</h2>
<h3>Fixed</h3>
<ul>
<li>More more complete fix for prototype pollution vulnerability first addressed
in <a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/384">#384</a> (Marc-Aurèle Darche <a href="https://github.com/madarche"><code>@​madarche</code></a>, Snyk Security team)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mozilla/node-convict/commit/deef5d77f4f6a714579387c2d67a051396477415"><code>deef5d7</code></a> v6.2.3</li>
<li><a href="https://github.com/mozilla/node-convict/commit/5e64b53082628abb9e4888838fcc8fe2851395ee"><code>5e64b53</code></a> More recent Ubuntu dist for Travis CI build</li>
<li><a href="https://github.com/mozilla/node-convict/commit/1ea0ab19c5208f66509e1c43b0d0f21c1fd29b75"><code>1ea0ab1</code></a> More more complete fix for prototype pollution</li>
<li><a href="https://github.com/mozilla/node-convict/commit/c7acb024c592652a6ad7f94ff7beed1df2d477ad"><code>c7acb02</code></a> Update info regarding publishing on NPM</li>
<li>See full diff in <a href="https://github.com/mozilla/node-convict/compare/v6.2.2...v6.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=convict&package-manager=npm_and_yarn&previous-version=6.2.2&new-version=6.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 03:00:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2044" class=".btn">#2044</a>
            </td>
            <td>
                <b>
                    build(deps): bump pyjwt from 2.1.0 to 2.4.0 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pyjwt](https://github.com/jpadilla/pyjwt) from 2.1.0 to 2.4.0.
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
&lt;li&gt;Additional commits viewable in &lt;a href=&quot;https://github.com/jpadilla/pyjwt/compare/2.1.0...2.4.0&quot;&gt;compare view&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;/details&gt;

&lt;br /&gt;
</code></pre>


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pyjwt&package-manager=pip&previous-version=2.1.0&new-version=2.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 05:47:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2043" class=".btn">#2043</a>
            </td>
            <td>
                <b>
                    test: jestify v21.4.1 invoke contract test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrate Tap to Jest

File Path:
packages/cactus-plugin-ledger-connector-quorum/
src/test/typescript/
integration/plugin-ledger-connector-quorum/
deploy-contract/
v21.4.1-invoke-contract.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 12:57:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2036" class=".btn">#2036</a>
            </td>
            <td>
                <b>
                    fix(security): close DDoS vulnerability in eth tx consistenty strategy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2001

Signed-off-by: aldousalvarez <aldousss.alvarez@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 03:25:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2035" class=".btn">#2035</a>
            </td>
            <td>
                <b>
                    test: jestify containers in test tooling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                File Path:
packages/cactus-test-
tooling/src/test/
typescript/integration/
common/
containers.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-22 23:58:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2034" class=".btn">#2034</a>
            </td>
            <td>
                <b>
                    test: jestify jvm kotlin spring server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrate Tap to Jest

File Path:
packages/cactus-plugin-ledger-connector-
corda/src/test/typescript/
integration/
jvm-kotlin-spring-server.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-22 20:46:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2033" class=".btn">#2033</a>
            </td>
            <td>
                <b>
                    feat(secret): remove Validator/Verifier secret keys from repository
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Remove validator sample CA keys hardcoded inside the repository.
- Generate fresh ECDSA keys when starting up electricity-trade
  or discounted-asset-trade sample apps.
- Add support for RSA CA keys in fabric-socketio validator.
  I couldn't find any trivial way of generating ECDSA self-signed certificate
  (without calling openssl cmdline, which seems poor from functional test perspective),
  so I've added support for RSA keys to simplify the tests.
- Allow selection of jwt algorithm in  fabric-socketio validator.
  It must correspond to the key used.
- Update the READMEs, add short description of SSL config option of fabric-socketio validator.

Closes: #2016
Closes: #2017

Depends on #1977
Depends on #2030

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

--------------

I've included commits from the dependencies to simplify the review before they're merged to main. Please review only the last commit: [feat(secret): remove Validator/Verifier secret keys from repository](https://github.com/hyperledger/cactus/commit/037100e992328cb49213b4138d9324fe419c0630)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 10:37:29 +0000 UTC
    </div>
</div>

