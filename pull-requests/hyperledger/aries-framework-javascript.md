---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1629" class=".btn">#1629</a>
            </td>
            <td>
                <b>
                    refactor(indy-sdk)!: remove indy-sdk package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still WIP.

Removes the indy-sdk package and updates all code to now use only the new shared components. Still some work to do related to removing the usage of indy-sdk and making sure all tests work. But this is an initial step.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 05:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1624" class=".btn">#1624</a>
            </td>
            <td>
                <b>
                    build(deps): bump actions/setup-node from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>In scope of this release we changed version of node runtime for action from node16 to node20 and updated dependencies in <a href="https://redirect.github.com/actions/setup-node/pull/866">actions/setup-node#866</a></p>
<p>Besides, release contains such changes as:</p>
<ul>
<li>Upgrade actions/checkout to v4 by <a href="https://github.com/gmembre-zenika"><code>@​gmembre-zenika</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/868">actions/setup-node#868</a></li>
<li>Update actions/checkout for documentation and yaml by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/876">actions/setup-node#876</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/gmembre-zenika"><code>@​gmembre-zenika</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-node/pull/868">actions/setup-node#868</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-node/compare/v3...v4.0.0">https://github.com/actions/setup-node/compare/v3...v4.0.0</a></p>
<h2>v3.8.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Update semver by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/861">actions/setup-node#861</a></li>
<li>Update temp directory creation by <a href="https://github.com/nikolai-laevskii"><code>@​nikolai-laevskii</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/859">actions/setup-node#859</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.15.4 to 7.23.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/870">actions/setup-node#870</a></li>
<li>Add notice about binaries not being updated yet by <a href="https://github.com/nikolai-laevskii"><code>@​nikolai-laevskii</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/872">actions/setup-node#872</a></li>
<li>Update toolkit cache and core by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> and <a href="https://github.com/seongwon-privatenote"><code>@​seongwon-privatenote</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/875">actions/setup-node#875</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-node/compare/v3...v3.8.2">https://github.com/actions/setup-node/compare/v3...v3.8.2</a></p>
<h2>v3.8.1</h2>
<h2>What's Changed</h2>
<p>In scope of this release, the filter was removed within the cache-save step by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/831">actions/setup-node#831</a>. It is filtered and checked in the toolkit/cache library.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-node/compare/v3...v3.8.1">https://github.com/actions/setup-node/compare/v3...v3.8.1</a></p>
<h2>v3.8.0</h2>
<h2>What's Changed</h2>
<h3>Bug fixes:</h3>
<ul>
<li>Add check for existing paths by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/803">actions/setup-node#803</a></li>
<li>Resolve SymbolicLink by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/809">actions/setup-node#809</a></li>
<li>Change passing logic for cache input by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/816">actions/setup-node#816</a></li>
<li>Fix armv7 cache issue by <a href="https://github.com/louislam"><code>@​louislam</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/794">actions/setup-node#794</a></li>
<li>Update check-dist workflow name by <a href="https://github.com/sinchang"><code>@​sinchang</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/710">actions/setup-node#710</a></li>
</ul>
<h3>Feature implementations:</h3>
<ul>
<li>feat: handling the case where &quot;node&quot; is used for tool-versions file. by <a href="https://github.com/xytis"><code>@​xytis</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/812">actions/setup-node#812</a></li>
</ul>
<h3>Documentation changes:</h3>
<ul>
<li>Refer to semver package name in README.md by <a href="https://github.com/olleolleolle"><code>@​olleolleolle</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/808">actions/setup-node#808</a></li>
</ul>
<h3>Update dependencies:</h3>
<ul>
<li>Update toolkit cache to fix zstd by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/804">actions/setup-node#804</a></li>
<li>Bump tough-cookie and <code>@​azure/ms-rest-js</code> by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/802">actions/setup-node#802</a></li>
<li>Bump semver from 6.1.2 to 6.3.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-node/pull/807">actions/setup-node#807</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/8f152de45cc393bb48ce5d89d36b731f54556e65"><code>8f152de</code></a> Update actions/checkout for documentation and yaml (<a href="https://redirect.github.com/actions/setup-node/issues/876">#876</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/23755b521f87533c8ed7f8fb13674f9021579e34"><code>23755b5</code></a> upgrade actions/checkout to v4 (<a href="https://redirect.github.com/actions/setup-node/issues/868">#868</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/54534a2a9ba7308e8a8995af3104899e6a95b681"><code>54534a2</code></a> Change node version for action to node20 (<a href="https://redirect.github.com/actions/setup-node/issues/866">#866</a>)</li>
<li>See full diff in <a href="https://github.com/actions/setup-node/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-01 10:05:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1623" class=".btn">#1623</a>
            </td>
            <td>
                <b>
                    feat: added ability to refresh the pool manually
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously AFJ wouldn't call refresh on genesis files, this meant that the pool could be out of date and contain dead nodes. This change adds a function to the pool service that allows an afj user to manually refresh the pool as needed. Example:
```typescript
const poolService = newAgent.dependencyManager.resolve(IndyVdrPoolService)
await poolService.refreshPoolConnections()
```
all the pools are refreshed asynchronously so it doesn't take more than 1 - 2 seconds on BC Wallet.

Note: I tried returning the transactions too so that we could cache them, however when I was playing around with the yarn patch I made, whenever I called `this._pool.transactions` in the `IndyCdrPool.js` file I would get a JSON parse error. I was unclear what was causing the error, it seems to be coming from the indy-vdr-shared library

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 20:15:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1622" class=".btn">#1622</a>
            </td>
            <td>
                <b>
                    feat: update dockerfile to node 18 and sample mediator to askar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Intermediate solution until we finally remove `indy-sdk` dependency: current Dockerfile won't work because it install node 16 and we now require at least 18, so here we are updating it. Also upgraded sample mediator to use Aries Askar, which now works properly due to the patched `ref-napi` library.

Resolves #1621 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 19:57:15 +0000 UTC
    </div>
</div>

