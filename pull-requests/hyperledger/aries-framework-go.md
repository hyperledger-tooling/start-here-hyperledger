---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2904" class=".btn">#2904</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.48.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.48.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.48.0</h2>
<h1>Features</h1>
<ul>
<li>enable import assertions again</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>upgrade webpack-sources for fixes regarding source maps</li>
<li>fix infinite loop in HMR runtime code</li>
</ul>
<h2>v5.47.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>upgrade webpack-sources for a bunch of bugfixes regarding source maps and missing chars in output</li>
</ul>
<h2>v5.47.0</h2>
<h1>Performance</h1>
<ul>
<li>improve source-map performance</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>avoid unnecessary <code>&quot;use strict&quot;</code>s in module mode</li>
</ul>
<h2>v5.46.0</h2>
<h1>Features</h1>
<ul>
<li>status handlers in HMR api can now return Promises to delay the HMR process</li>
<li>reasons in stats can now be grouped and collapsed
<ul>
<li>add <code>stats.reasonsSpace</code> and <code>stats.groupReasonsByOrigin</code></li>
</ul>
</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix a crash in asset modules when updating persistent cached modules from unsafe cached modules</li>
</ul>
<h1>Performance</h1>
<ul>
<li>detailed preset limits all spaces to 1000 by default</li>
<li>upgrade webpack-sources for a performance bugfix</li>
</ul>
<h2>v5.45.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>temporary revert import assertions because parser changes break the word <code>assert</code> in other places</li>
<li><code>import(/* webpackPrefetch: true */ ...)</code> no longer breaks library output</li>
<li>DataURL tries to avoid re-encoding</li>
<li>fix problems with DataURL encoding in some cases</li>
</ul>
<h2>v5.45.0</h2>
<h1>Features</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/67f3aef3c11e2a8d9e7dc1e0300350588ebd7aec"><code>67f3aef</code></a> 5.48.0</li>
<li><a href="https://github.com/webpack/webpack/commit/747c20b9c0d860052bb7952408836d00a56e8776"><code>747c20b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13815">#13815</a> from xtuc/sven/bump-acorn-import-assertions-1.7.2</li>
<li><a href="https://github.com/webpack/webpack/commit/dad2aca1365e89cc2ed029463e4436899bf75d25"><code>dad2aca</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13911">#13911</a> from webpack/bugfix/webpack-sources</li>
<li><a href="https://github.com/webpack/webpack/commit/1c1af83e12b6ed15f80396fc668efa4bda7586f7"><code>1c1af83</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13877">#13877</a> from axules/bugfix/hot-poll-infinity</li>
<li><a href="https://github.com/webpack/webpack/commit/c3a12b7bb6df0f7b6cc9a6d6fdd1dd3c9740bac0"><code>c3a12b7</code></a> upgrade webpack-sources to 3.2.0</li>
<li><a href="https://github.com/webpack/webpack/commit/551f64a59030c9250fdf97ce05b49d98efb45dab"><code>551f64a</code></a> fix empty updatedModules check</li>
<li><a href="https://github.com/webpack/webpack/commit/b573514987e53fbf248af30b0028540f411147b7"><code>b573514</code></a> fix hot/signal infinity recursion</li>
<li><a href="https://github.com/webpack/webpack/commit/3f353b6ae29ae6d96e0ab86e7233b4c785f99c60"><code>3f353b6</code></a> 5.47.1</li>
<li><a href="https://github.com/webpack/webpack/commit/6b6f4fead714a9c301c30417b49c58aba153aae6"><code>6b6f4fe</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13888">#13888</a> from webpack/bugfix/webpack-sources</li>
<li><a href="https://github.com/webpack/webpack/commit/5fc7008c3e2ade90dc7561a51eceb484ae305453"><code>5fc7008</code></a> update webpack-sources to 3.1.1</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.48.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.48.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 08:20:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2903" class=".btn">#2903</a>
            </td>
            <td>
                <b>
                    fix: presentation schema filtering respects schema IDs in contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2756

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 06:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2901" class=".btn">#2901</a>
            </td>
            <td>
                <b>
                    chore: update bdd docker dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Troy Ronda <troy@troyronda.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 14:08:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2900" class=".btn">#2900</a>
            </td>
            <td>
                <b>
                    fix: Unit tests for mobile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 13:58:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2897" class=".btn">#2897</a>
            </td>
            <td>
                <b>
                    fix: avoid a data race in eventprops.All()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Populates a fresh, local map instead of editing a map that's shared
across threads.

Fixes #2417

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 14:17:38 +0000 UTC
    </div>
</div>

