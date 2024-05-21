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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump @babel/traverse from 7.17.9 to 7.24.5 in /common/policy-dsl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@babel/traverse](https://github.com/babel/babel/tree/HEAD/packages/babel-traverse) from 7.17.9 to 7.24.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/traverse</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<p>Thanks <a href="https://github.com/romgrk"><code>@​romgrk</code></a> and <a href="https://github.com/sossost"><code>@​sossost</code></a> for your first PRs!</p>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 6</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>Rom Grk (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
<li>ynnsuis (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<p>Thanks <a href="https://github.com/Dunqing"><code>@​Dunqing</code></a>, <a href="https://github.com/luiscubal"><code>@​luiscubal</code></a>, and <a href="https://github.com/samualtnorman"><code>@​samualtnorman</code></a> for your first PRs!</p>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/traverse</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16402">#16402</a> fix: Correctly prints <code>{ [key in Bar]? }</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16394">#16394</a> fix: Correctly generate <code>TSMappedType</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-compat-data</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16390">#16390</a> Create bugfix plugin for classes in computed keys in Firefox (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16387">#16387</a> fix: support mutated outer decorated class binding (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16385">#16385</a> fix: Decorators when <code>super()</code> exists and <code>protoInit</code> is not needed (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-block-scoping</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16384">#16384</a> fix: Transform scoping for <code>for X</code> in loop (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16368">#16368</a> fix: Capture <code>let</code> when the <code>for</code> body is not a block (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-core</code>, <code>babel-plugin-transform-block-scoped-functions</code>, <code>babel-plugin-transform-block-scoping</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/ddbea7d4e6314f799eb371cc10e16f96ac2c96b2"><code>ddbea7d</code></a> v7.24.5</li>
<li><a href="https://github.com/babel/babel/commit/e779cad081d47bd6a91302e274dbb93f08bd1d51"><code>e779cad</code></a> fix: TypeScript annotation affects output (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16377">#16377</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ee4875443db7563b87ef8e11e1fb75582ac72ac1"><code>ee48754</code></a> Use multiple TypeScript projects (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16430">#16430</a>)</li>
<li><a href="https://github.com/babel/babel/commit/4d8b2d0fd79630aec51e2c35daca46cdb2ddd4c3"><code>4d8b2d0</code></a> Make <code>NodePath\&lt;T | U&gt;</code> distributive (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16439">#16439</a>)</li>
<li><a href="https://github.com/babel/babel/commit/a84ec282c0bea68bb184e091742ed9d996a0342f"><code>a84ec28</code></a> Enable <code>eqeqeq</code> rule (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16404">#16404</a>)</li>
<li><a href="https://github.com/babel/babel/commit/822b025fc9d43263e69aed8a9fc80e8c6b8ebf6d"><code>822b025</code></a> v7.24.1</li>
<li><a href="https://github.com/babel/babel/commit/fc0d5ad56e948f2b3d1704adb6367bbde0f25e59"><code>fc0d5ad</code></a> Update typescript and lint tools (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16351">#16351</a>)</li>
<li><a href="https://github.com/babel/babel/commit/69e792887ea7e5d1cd7375ef7f6f3254ff4f2695"><code>69e7928</code></a> Consider well-known and registered symbols as literals (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16342">#16342</a>)</li>
<li><a href="https://github.com/babel/babel/commit/40110e9d707e2b2b81f6e2b99820722a7014132a"><code>40110e9</code></a> Update source map deps (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16327">#16327</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ce59160e34e21e8f1ac2fc55ae037f7b043e8d20"><code>ce59160</code></a> v7.24.0</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.24.5/packages/babel-traverse">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@babel/traverse&package-manager=npm_and_yarn&previous-version=7.17.9&new-version=7.24.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 11:58:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/458" class=".btn">#458</a>
            </td>
            <td>
                <b>
                    build(deps): Bump mio from 0.8.6 to 0.8.11 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [mio](https://github.com/tokio-rs/mio) from 0.8.6 to 0.8.11.
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
<h1>0.8.9</h1>
<h2>Added</h2>
<ul>
<li>ESP-IDF framework support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1692">tokio-rs/mio#1692</a>).</li>
<li>AIX operating system support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1704">tokio-rs/mio#1704</a>).</li>
<li>Vita support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1721">tokio-rs/mio#1721</a>).</li>
<li><code>{UnixListener,UnixStream}:bind_addr</code>
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1630">tokio-rs/mio#1630</a>).</li>
<li><code>mio_unsupported_force_poll_poll</code> and <code>mio_unsupported_force_waker_pipe</code>
<strong>unsupported</strong> configuration flags to force a specific poll or waker
implementation
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1684">tokio-rs/mio#1684</a>,
<a href="https://redirect.github.com/tokio-rs/mio/pull/1685">tokio-rs/mio#1685</a>,
<a href="https://redirect.github.com/tokio-rs/mio/pull/1692">tokio-rs/mio#1692</a>).</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>The <code>pipe(2)</code> based waker (swapped file descriptors)
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1722">tokio-rs/mio#1722</a>).</li>
<li>The duplicate waker check to work correctly with cloned <code>Registry</code>s.
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1706">tokio-rs/mio#1706</a>).</li>
</ul>
<h1>0.8.8</h1>
<h2>Fixed</h2>
<ul>
<li>Fix compilation on WASI (<a href="https://redirect.github.com/tokio-rs/mio/pull/1676">tokio-rs/mio#1676</a>).</li>
</ul>
<h1>0.8.7</h1>
<h2>Added</h2>
<ul>
<li>Add/fix support for tvOS and watchOS, Mio should now build for tvOS and</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li><a href="https://github.com/tokio-rs/mio/commit/e80c3b21b59b92238f4c8c331fcfc4a71508d1c5"><code>e80c3b2</code></a> Release v0.8.9</li>
<li><a href="https://github.com/tokio-rs/mio/commit/862786bbbf719886be55631c0d150d4813a9a1b6"><code>862786b</code></a> Fix importing of IoSourceState</li>
<li><a href="https://github.com/tokio-rs/mio/commit/40348728e4f06f5e150783d8f1559ee974e5e834"><code>4034872</code></a> Add support for vita target</li>
<li><a href="https://github.com/tokio-rs/mio/commit/8eb4010a92bede550850e177d3dd7c4c76eb90ba"><code>8eb4010</code></a> Fix receiver and sender fd in pipe based waker</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/mio/compare/v0.8.6...v0.8.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mio&package-manager=cargo&previous-version=0.8.6&new-version=0.8.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 11:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    Update weaver dependencies and repository links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * chore: update all go module dependencies, add all go tests to workflow
* fix(weaver-go-sdk): use updated weaver protobuf for fabric and corda view
* chore: add script to generate checksums for go modules
* fix: update broken corda repository links
* ci: fix besu asset exchange workflow to use node 16
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-17 06:18:22 +0000 UTC
    </div>
</div>

