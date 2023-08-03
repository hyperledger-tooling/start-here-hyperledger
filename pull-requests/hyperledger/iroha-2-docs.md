---
layout: default
title: iroha-2-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-2-docs
---

# iroha-2-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-2-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/365" class=".btn">#365</a>
            </td>
            <td>
                <b>
                    Bump vite from 4.3.2 to 4.3.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite) from 4.3.2 to 4.3.9.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/main/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->4.3.9 (2023-05-26)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: fs.deny with leading double slash (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13348">#13348</a>) (<a href="https://github.com/vitejs/vite/commit/813ddd6">813ddd6</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13348">#13348</a></li>
<li>fix: optimizeDeps during build and external ids (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13274">#13274</a>) (<a href="https://github.com/vitejs/vite/commit/e3db771">e3db771</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13274">#13274</a></li>
<li>fix(css): return deps if have no postcss plugins (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13344">#13344</a>) (<a href="https://github.com/vitejs/vite/commit/28923fb">28923fb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13344">#13344</a></li>
<li>fix(legacy): style insert order (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13266">#13266</a>) (<a href="https://github.com/vitejs/vite/commit/e444375">e444375</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13266">#13266</a></li>
<li>chore: revert prev release commit (<a href="https://github.com/vitejs/vite/commit/2a30a07">2a30a07</a>)</li>
<li>release: v4.3.9 (<a href="https://github.com/vitejs/vite/commit/5c9abf7">5c9abf7</a>)</li>
<li>docs: optimizeDeps.needsInterop (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13323">#13323</a>) (<a href="https://github.com/vitejs/vite/commit/b34e79c">b34e79c</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13323">#13323</a></li>
<li>test: respect commonjs options in playgrounds (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13273">#13273</a>) (<a href="https://github.com/vitejs/vite/commit/19e8c68">19e8c68</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13273">#13273</a></li>
<li>refactor: simplify SSR options' if statement (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13254">#13254</a>) (<a href="https://github.com/vitejs/vite/commit/8013a66">8013a66</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13254">#13254</a></li>
<li>perf(ssr): calculate stacktrace offset lazily (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13256">#13256</a>) (<a href="https://github.com/vitejs/vite/commit/906c4c1">906c4c1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13256">#13256</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.3.8 (2023-05-18)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: avoid outdated module to crash in importAnalysis after restart (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13231">#13231</a>) (<a href="https://github.com/vitejs/vite/commit/3609e79">3609e79</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13231">#13231</a></li>
<li>fix(ssr): skip updateCjsSsrExternals if legacy flag disabled (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13230">#13230</a>) (<a href="https://github.com/vitejs/vite/commit/13fc345">13fc345</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13230">#13230</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.3.7 (2023-05-16)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: revert only watch .env files in envDir (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/12587">#12587</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13217">#13217</a>) (<a href="https://github.com/vitejs/vite/commit/0fd4616">0fd4616</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/12587">#12587</a> <a href="https://redirect.github.com/vitejs/vite/issues/13217">#13217</a></li>
<li>fix(assetImportMetaUrl): allow ternary operator in template literal urls (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13121">#13121</a>) (<a href="https://github.com/vitejs/vite/commit/d5d9a31">d5d9a31</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13121">#13121</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.3.6 (2023-05-15)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: avoid dev-server crash when ws proxy error (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/12829">#12829</a>) (<a href="https://github.com/vitejs/vite/commit/87e1f58">87e1f58</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/12829">#12829</a></li>
<li>fix: call <code>tryFsResolve</code> for relative <code>new URL(foo, import.meta.url)</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13142">#13142</a>) (<a href="https://github.com/vitejs/vite/commit/eeb0617">eeb0617</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13142">#13142</a></li>
<li>fix: don't inject CSS sourcemap for direct requests (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13115">#13115</a>) (<a href="https://github.com/vitejs/vite/commit/7d80a47">7d80a47</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13115">#13115</a></li>
<li>fix: handle more yarn pnp load errors (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13160">#13160</a>) (<a href="https://github.com/vitejs/vite/commit/adf61d9">adf61d9</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13160">#13160</a></li>
<li>fix(build): declare moduleSideEffects for vite:modulepreload-polyfill (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13099">#13099</a>) (<a href="https://github.com/vitejs/vite/commit/d63129b">d63129b</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13099">#13099</a></li>
<li>fix(css): respect <code>esbuild.charset</code> when minify (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13190">#13190</a>) (<a href="https://github.com/vitejs/vite/commit/4fd35ed">4fd35ed</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13190">#13190</a></li>
<li>fix(server): intercept ping requests (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13117">#13117</a>) (<a href="https://github.com/vitejs/vite/commit/d06cc42">d06cc42</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13117">#13117</a></li>
<li>fix(ssr): stacktrace uses abs path with or without sourcemap (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/12902">#12902</a>) (<a href="https://github.com/vitejs/vite/commit/88c855e">88c855e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/12902">#12902</a></li>
<li>perf: skip windows absolute paths for node resolve (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13162">#13162</a>) (<a href="https://github.com/vitejs/vite/commit/e640939">e640939</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13162">#13162</a></li>
<li>chore: remove useless dep (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13165">#13165</a>) (<a href="https://github.com/vitejs/vite/commit/9a7ec98">9a7ec98</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13165">#13165</a></li>
<li>chore(reporter): reuse clearLine (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13156">#13156</a>) (<a href="https://github.com/vitejs/vite/commit/535795a">535795a</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13156">#13156</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.3.5 (2023-05-05)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: location is not defined error in cleanScssBugUrl (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13100">#13100</a>) (<a href="https://github.com/vitejs/vite/commit/91d7b67">91d7b67</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13100">#13100</a></li>
<li>fix: unwrapId and pass ssr flag when adding to moduleGraph in this.load (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13083">#13083</a>) (<a href="https://github.com/vitejs/vite/commit/9041e19">9041e19</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13083">#13083</a></li>
<li>fix(assetImportMetaUrl): reserve dynamic template literal query params (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/13034">#13034</a>) (<a href="https://github.com/vitejs/vite/commit/7089528">7089528</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/13034">#13034</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/vitejs/vite/commits/v4.3.9/packages/vite">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=vite&package-manager=npm_and_yarn&previous-version=4.3.2&new-version=4.3.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-2-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 05:26:32 +0000 UTC
    </div>
</div>

