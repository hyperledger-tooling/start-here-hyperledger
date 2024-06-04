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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    Bump prettier from 2.8.8 to 3.3.0 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [prettier](https://github.com/prettier/prettier) from 2.8.8 to 3.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/releases">prettier's releases</a>.</em></p>
<blockquote>
<h2>3.3.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.2.5...3.3.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/06/01/3.3.0.html">Release note</a></p>
<h2>3.2.5</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#325">Changelog</a></p>
<h2>3.2.4</h2>
<ul>
<li>Fix <code>.eslintrc.json</code> format <a href="https://redirect.github.com/prettier/prettier/issues/15947">#15947</a></li>
</ul>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#324">Changelog</a></p>
<h2>3.2.3</h2>
<ul>
<li>Format <code>tsconfig.json</code> file with <code>jsonc</code> parser <a href="https://redirect.github.com/prettier/prettier/issues/15927">#15927</a></li>
</ul>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#323">Changelog</a></p>
<h2>3.2.2</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#322">Changelog</a></p>
<h2>3.2.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#321">Changelog</a></p>
<h2>3.2.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.1.1...3.2.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/01/12/3.2.0.html">Release note</a></p>
<h2>3.1.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#311">Changelog</a></p>
<h2>3.1.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.0.3...3.1.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2023/11/13/3.1.0.html">Release note</a></p>
<h2>3.0.3</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#303">Changelog</a></p>
<h2>3.0.2</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#302">Changelog</a></p>
<h2>3.0.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#301">Changelog</a></p>
<h2>3.0.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.0.0-alpha.6...3.0.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2023/07/05/3.0.0.html">Release note</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md">prettier's changelog</a>.</em></p>
<blockquote>
<h1>3.3.0</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.2.5...3.3.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/06/01/3.3.0.html">Release Notes</a></p>
<h1>3.2.5</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.2.4...3.2.5">diff</a></p>
<h4>Support Angular inline styles as single template literal (<a href="https://redirect.github.com/prettier/prettier/pull/15968">#15968</a> by <a href="https://github.com/sosukesuzuki"><code>@​sosukesuzuki</code></a>)</h4>
<p><a href="https://blog.angular.io/introducing-angular-v17-4d7033312e4b">Angular v17</a> supports single string inline styles.</p>
<!-- raw HTML omitted -->
<pre lang="ts"><code>// Input
@Component({
  template: `&lt;div&gt;...&lt;/div&gt;`,
  styles: `h1 { color: blue; }`,
})
export class AppComponent {}
<p>// Prettier 3.2.4
<a href="https://github.com/Component"><code>@​Component</code></a>({
template: <code>&amp;lt;div&amp;gt;...&amp;lt;/div&amp;gt;</code>,
styles: <code>h1 { color: blue; }</code>,
})
export class AppComponent {}</p>
<p>// Prettier 3.2.5
<a href="https://github.com/Component"><code>@​Component</code></a>({
template: <code>&amp;lt;div&amp;gt;...&amp;lt;/div&amp;gt;</code>,
styles: <code>h1 { color: blue; }</code>,
})
export class AppComponent {}</p>
<p></code></pre></p>
<h4>Unexpected embedded formatting for Angular template (<a href="https://redirect.github.com/prettier/prettier/pull/15969">#15969</a> by <a href="https://github.com/JounQin"><code>@​JounQin</code></a>)</h4>
<p>Computed template should not be considered as Angular component template</p>
<!-- raw HTML omitted -->
<pre lang="ts"><code>// Input
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prettier/prettier/commit/c4ab460357478d2b847c60a1efb40098b1181931"><code>c4ab460</code></a> Release 3.3.0</li>
<li><a href="https://github.com/prettier/prettier/commit/8a88cdce6d4605f206305ebb9204a0cabf96a070"><code>8a88cdc</code></a> Respect <code>trailingComma</code> in angular templates (<a href="https://redirect.github.com/prettier/prettier/issues/15926">#15926</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/c2e20fbae8ce1800ac0c8242c176d9379db5c001"><code>c2e20fb</code></a> chore(deps): update babel to v7.24.6 (<a href="https://redirect.github.com/prettier/prettier/issues/16326">#16326</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/41f1dffed08b33fe6d43da1e82d798b23ba0b57c"><code>41f1dff</code></a> Add newline between markdown footnote definitions (<a href="https://redirect.github.com/prettier/prettier/issues/16063">#16063</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/da5ad84bf441afd5c157bf83840814b1deaa39b1"><code>da5ad84</code></a> chore(deps): update babel to v7.24.6 (<a href="https://redirect.github.com/prettier/prettier/issues/16325">#16325</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/f790be81319a70f08942b1e3c12d68ee392d3269"><code>f790be8</code></a> chore(deps): update dependency file-entry-cache to v9 (<a href="https://redirect.github.com/prettier/prettier/issues/16324">#16324</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/7250556e287922508d9f28c12a82165a60bab5d7"><code>7250556</code></a> chore(deps): update dependency meriyah to v4.4.3 (<a href="https://redirect.github.com/prettier/prettier/issues/16323">#16323</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/96e057a0dc1efa7247b1c50843c9422a0ed66900"><code>96e057a</code></a> chore(deps): update dependency <code>@​angular/compiler</code> to v18 (<a href="https://redirect.github.com/prettier/prettier/issues/16322">#16322</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/a4ea5a2e2fcebe72315c9c0523b35bc79fe91405"><code>a4ea5a2</code></a> chore(deps): update dependency eslint-plugin-regexp to v2.6.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16320">#16320</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/229006cd5b5178c195e5d66ce924d2b58bfde4ef"><code>229006c</code></a> chore(deps): update dependency micromatch to v4.0.7 (<a href="https://redirect.github.com/prettier/prettier/issues/16319">#16319</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/prettier/prettier/compare/2.8.8...3.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=prettier&package-manager=npm_and_yarn&previous-version=2.8.8&new-version=3.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-03 11:19:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    Bump reqwest from 0.11.14 to 0.12.4 in /aries-backchannels/aries-vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [reqwest](https://github.com/seanmonstar/reqwest) from 0.11.14 to 0.12.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/seanmonstar/reqwest/releases">reqwest's releases</a>.</em></p>
<blockquote>
<h2>v0.12.4</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>zstd</code> support, enabled with <code>zstd</code> Cargo feature (thanks <a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a>!)</li>
<li>Add <code>ClientBuilder::read_timeout(Duration)</code>, which applies the duration for each read operation. The timeout resets after a successful read.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/SamuelMarks"><code>@​SamuelMarks</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2245">seanmonstar/reqwest#2245</a></li>
</ul>
<h2>v0.12.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>FromStr</code> for <code>dns::Name</code>.</li>
<li>Add <code>ClientBuilder::built_in_webpki_certs(bool)</code> to enable them separately.</li>
<li>Add <code>ClientBuilder::built_in_native_certs(bool)</code> to enable them separately.</li>
<li>Fix sending <code>content-length: 0</code> for GET requests.</li>
<li>Fix response body <code>content_length()</code> to return value when timeout is configured.</li>
<li>Fix <code>ClientBuilder::resolve()</code> to use lowercase domain names.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/zuisong"><code>@​zuisong</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2207">seanmonstar/reqwest#2207</a></li>
<li><a href="https://github.com/djc"><code>@​djc</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2222">seanmonstar/reqwest#2222</a></li>
<li><a href="https://github.com/krant"><code>@​krant</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2226">seanmonstar/reqwest#2226</a></li>
<li><a href="https://github.com/Kriskras99"><code>@​Kriskras99</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2236">seanmonstar/reqwest#2236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/seanmonstar/reqwest/compare/v0.12.2...v0.12.3">https://github.com/seanmonstar/reqwest/compare/v0.12.2...v0.12.3</a></p>
<h2>v0.12.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix missing ALPN when connecting to socks5 proxy with rustls.</li>
<li>Fix TLS version limits with rustls.</li>
<li>Fix not detected ALPN h2 from server with native-tls.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/cxw620"><code>@​cxw620</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2165">seanmonstar/reqwest#2165</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/seanmonstar/reqwest/compare/v0.12.1...v0.12.2">https://github.com/seanmonstar/reqwest/compare/v0.12.1...v0.12.2</a></p>
<h2>v0.12.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix <code>ClientBuilder::interface()</code> when no TLS is enabled.</li>
<li>Fix <code>TlsInfo::peer_certificate()</code> being truncated with rustls.</li>
<li>Fix panic if <code>http2</code> feature disabled but TLS negotiated h2 in ALPN.</li>
<li>Fix <code>Display</code> for <code>Error</code> to not include its source error.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/atouchet"><code>@​atouchet</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2193">seanmonstar/reqwest#2193</a></li>
<li><a href="https://github.com/mbme"><code>@​mbme</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2195">seanmonstar/reqwest#2195</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/seanmonstar/reqwest/compare/v0.12.0...v0.12.1">https://github.com/seanmonstar/reqwest/compare/v0.12.0...v0.12.1</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/seanmonstar/reqwest/blob/master/CHANGELOG.md">reqwest's changelog</a>.</em></p>
<blockquote>
<h2>v0.12.4</h2>
<ul>
<li>Add <code>zstd</code> support, enabled with <code>zstd</code> Cargo feature.</li>
<li>Add <code>ClientBuilder::read_timeout(Duration)</code>, which applies the duration for each read operation. The timeout resets after a successful read.</li>
</ul>
<h2>v0.12.3</h2>
<ul>
<li>Add <code>FromStr</code> for <code>dns::Name</code>.</li>
<li>Add <code>ClientBuilder::built_in_webpki_certs(bool)</code> to enable them separately.</li>
<li>Add <code>ClientBuilder::built_in_native_certs(bool)</code> to enable them separately.</li>
<li>Fix sending <code>content-length: 0</code> for GET requests.</li>
<li>Fix response body <code>content_length()</code> to return value when timeout is configured.</li>
<li>Fix <code>ClientBuilder::resolve()</code> to use lowercase domain names.</li>
</ul>
<h2>v0.12.2</h2>
<ul>
<li>Fix missing ALPN when connecting to socks5 proxy with rustls.</li>
<li>Fix TLS version limits with rustls.</li>
<li>Fix not detected ALPN h2 from server with native-tls.</li>
</ul>
<h2>v0.12.1</h2>
<ul>
<li>Fix <code>ClientBuilder::interface()</code> when no TLS is enabled.</li>
<li>Fix <code>TlsInfo::peer_certificate()</code> being truncated with rustls.</li>
<li>Fix panic if <code>http2</code> feature disabled but TLS negotiated h2 in ALPN.</li>
<li>Fix <code>Display</code> for <code>Error</code> to not include its source error.</li>
</ul>
<h1>v0.12.0</h1>
<ul>
<li>Upgrade to <code>hyper</code>, <code>http</code>, and <code>http-body</code> v1.</li>
<li>Add better support for converting to and from <code>http::Request</code> and <code>http::Response</code>.</li>
<li>Add <code>http2</code> optional cargo feature, default on.</li>
<li>Add <code>charset</code> optional cargo feature, default on.</li>
<li>Add <code>macos-system-configuration</code> cargo feature, default on.</li>
<li>Change all optional dependencies to no longer be exposed as implicit features.</li>
<li>Add <code>ClientBuilder::interface(str)</code> to specify the local interface to bind to.</li>
<li>Experimental: disables the <code>http3</code> feature temporarily.</li>
</ul>
<h2>v0.11.27</h2>
<ul>
<li>Add <code>hickory-dns</code> feature, deprecating <code>trust-dns</code>.</li>
<li>(wasm) Fix <code>Form::text()</code> to not set octet-stream for plain text fields.</li>
</ul>
<h2>v0.11.26</h2>
<ul>
<li>Revert <code>system-configuration</code> upgrade, which broke MSRV on macOS.</li>
</ul>
<h2>v0.11.25</h2>
<ul>
<li>Fix <code>Certificate::from_pem_bundle()</code> parsing.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/seanmonstar/reqwest/commit/de5dbb1ab849cc301dcefebaeabdf4ce2e0f1e53"><code>de5dbb1</code></a> v0.12.4</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/0f126f57abd09985526dbdf86777d209afbd7cc0"><code>0f126f5</code></a> tests: fix blocking test about empty bodies and content-length</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/107388134b7c1ea684cc76ed00efe2db12194610"><code>1073881</code></a> feat: add zstd support (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/1866">#1866</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/1af8945143f0a4ba5563e2982b06fc303afea50b"><code>1af8945</code></a> feat: add ClientBuilder::read_timeout(dur) (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2241">#2241</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/e99da854a18ed6e968e0fff5bbf24a72983a0dc9"><code>e99da85</code></a> refactor: fix warnings related to mutability of <code>self</code> (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2245">#2245</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/0720159f6369f54e045a1fd315e0f24b7a0b4a39"><code>0720159</code></a> v0.12.3</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/92096952b7257af6a9eea6f94c5be04c418be0e3"><code>9209695</code></a> Remove duplicate example for ClientBuilder::default_headers (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2236">#2236</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/e3a15650d600f3ab1aa2c6f83dc7567a8677337e"><code>e3a1565</code></a> fix: use lower case domain string when using <code>resolve</code> and <code>resolve_to_addrs</code>...</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/b4c491a6ffa10418d8bfaa49fc38f2175312f90c"><code>b4c491a</code></a> feat: allow fine-grained root certs for rustls (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2232">#2232</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/cf4295d59d614b1b813cacfe97f186fba952a358"><code>cf4295d</code></a> chore: update winreg to 0.52.0 (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2226">#2226</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/seanmonstar/reqwest/compare/v0.11.14...v0.12.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=reqwest&package-manager=cargo&previous-version=0.11.14&new-version=0.12.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:49:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    Bump serde_json from 1.0.93 to 1.0.99 in /aries-backchannels/aries-vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.93 to 1.0.99.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.99</h2>
<ul>
<li>Support serializing serde's <strong>option</strong> type in a map key (<a href="https://redirect.github.com/serde-rs/json/issues/1030">#1030</a>, thanks <a href="https://github.com/LPGhatguy"><code>@​LPGhatguy</code></a>)</li>
</ul>
<h2>v1.0.98</h2>
<ul>
<li>Update indexmap dependency used by &quot;preserve_order&quot; feature to version 2</li>
</ul>
<h2>v1.0.97</h2>
<ul>
<li>Add <code>io_error_kind()</code> method to serde_json::Error: <code>fn io_error_kind(&amp;self) -&gt; Option&lt;std::io::ErrorKind&gt;</code> (<a href="https://redirect.github.com/serde-rs/json/issues/1026">#1026</a>)</li>
</ul>
<h2>v1.0.96</h2>
<ul>
<li>Guarantee that <code>to_writer</code> only writes valid UTF-8 strings (<a href="https://redirect.github.com/serde-rs/json/issues/1011">#1011</a>, thanks <a href="https://github.com/stepancheg"><code>@​stepancheg</code></a>)</li>
</ul>
<h2>v1.0.95</h2>
<ul>
<li>Preserve f32 precision when serializing f32 -&gt; serde_json::Value -&gt; JSON string in &quot;arbitrary_precision&quot; mode (<a href="https://redirect.github.com/serde-rs/json/issues/1004">#1004</a>, <a href="https://redirect.github.com/serde-rs/json/issues/1005">#1005</a>)</li>
</ul>
<h2>v1.0.94</h2>
<ul>
<li>Fix message duplication between serde_json::Error's <code>Display</code> and <code>source()</code> (<a href="https://redirect.github.com/serde-rs/json/issues/991">#991</a>, <a href="https://redirect.github.com/serde-rs/json/issues/992">#992</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/b4ec50ce7a47f1b344dd964de09a8be99fbe8300"><code>b4ec50c</code></a> Release 1.0.99</li>
<li><a href="https://github.com/serde-rs/json/commit/11530529e86a5636558bcd352b2ad4d0c5f3ae6e"><code>1153052</code></a> Merge pull request 1030 from SecondHalfGames/map-key-serialize-some</li>
<li><a href="https://github.com/serde-rs/json/commit/ba29a89a098dd5db6e889830bf1ac33837c1416e"><code>ba29a89</code></a> Release 1.0.98</li>
<li><a href="https://github.com/serde-rs/json/commit/9508e50cbcce029d36f9988da26785aa1434e3c9"><code>9508e50</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1031">#1031</a> from serde-rs/indexmap</li>
<li><a href="https://github.com/serde-rs/json/commit/706fc2b5592f415329d17df7b3777b56af909413"><code>706fc2b</code></a> Do all CI builds with old rustc using shim crate</li>
<li><a href="https://github.com/serde-rs/json/commit/d4c98d05b993de5add76feec4eb371b1035d8f77"><code>d4c98d0</code></a> Move serde_json_test crate to own workspace</li>
<li><a href="https://github.com/serde-rs/json/commit/e09d78f793b1fd189bf5ed59251ea906feb24df3"><code>e09d78f</code></a> Update indexmap dependency used for preserve_order feature to version 2</li>
<li><a href="https://github.com/serde-rs/json/commit/51459078f38c851bb750d84ab9be4d8f40dc7693"><code>5145907</code></a> Delete unneeded conditional on preserve_order steps in CI</li>
<li><a href="https://github.com/serde-rs/json/commit/b0fa9788f4f1fc03a9fc8066ea4c2aa0f26c5400"><code>b0fa978</code></a> Change MapKeySerializer::serialize_some to fall through instead of erroring</li>
<li><a href="https://github.com/serde-rs/json/commit/a0ddb25ff6b86f43912f8fc637797bcbb920c61e"><code>a0ddb25</code></a> Release 1.0.97</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/json/compare/v1.0.93...v1.0.99">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.93&new-version=1.0.99)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:49:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    Bump clap from 3.2.23 to 3.2.25 in /aries-backchannels/aries-vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [clap](https://github.com/clap-rs/clap) from 3.2.23 to 3.2.25.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/releases">clap's releases</a>.</em></p>
<blockquote>
<h2>v3.2.25</h2>
<h2>[3.2.25] - 2023-04-27</h2>
<h3>Fixes</h3>
<ul>
<li><em>(derive)</em> Resolve warnings in generated code</li>
</ul>
<h2>v3.2.24</h2>
<h2>[3.2.24] - 2023-04-25</h2>
<h3>Fixes</h3>
<ul>
<li><em>(derive)</em> Resolve warnings in generated code</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/blob/v3.2.25/CHANGELOG.md">clap's changelog</a>.</em></p>
<blockquote>
<h2>[3.2.25] - 2023-04-27</h2>
<h3>Fixes</h3>
<ul>
<li><em>(derive)</em> Resolve warnings in generated code</li>
</ul>
<h2>[3.2.24] - 2023-04-25</h2>
<h3>Fixes</h3>
<ul>
<li><em>(derive)</em> Resolve warnings in generated code</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/clap-rs/clap/commit/3bd502024e45cc9abef690f28783d76a9ce33500"><code>3bd5020</code></a> chore: Release</li>
<li><a href="https://github.com/clap-rs/clap/commit/bad2d76b75ca1de10b7a51c905f45dfb5757589d"><code>bad2d76</code></a> docs: Update changelog</li>
<li><a href="https://github.com/clap-rs/clap/commit/4b7dbfb811dbd0539b442fe8e29e325db924019d"><code>4b7dbfb</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/4866">#4866</a> from hds/v3-allow-almost-swapped</li>
<li><a href="https://github.com/clap-rs/clap/commit/b8ca7349cdf85b5736b8bccd08934a44fb3ef2ef"><code>b8ca734</code></a> fix(derive): Allow <code>clippy::almost_swapped</code></li>
<li><a href="https://github.com/clap-rs/clap/commit/f617f1328e7e389d580c6f3f2f7fd62af42f1dc4"><code>f617f13</code></a> chore: Release</li>
<li><a href="https://github.com/clap-rs/clap/commit/c29364554f59ecbd692bd2e78205286ceaef67bc"><code>c293645</code></a> docs: Update changelog</li>
<li><a href="https://github.com/clap-rs/clap/commit/b95af6419a44281ae7cc0c2ca2f252dcb2cd682f"><code>b95af64</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/4858">#4858</a> from hds/v3-no-deny-correctness</li>
<li><a href="https://github.com/clap-rs/clap/commit/f14f398bc312c96f2ec5d4c9443b7e7d9499b4f7"><code>f14f398</code></a> fix: Remove strict linting from generated code</li>
<li><a href="https://github.com/clap-rs/clap/commit/708c00bd5f07312e0347af8b3ed27e2076676449"><code>708c00b</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/4859">#4859</a> from epage/ci</li>
<li><a href="https://github.com/clap-rs/clap/commit/f95385bf36ecb935de8f988e0a75e9ccfed27291"><code>f95385b</code></a> doc: Escape literals</li>
<li>Additional commits viewable in <a href="https://github.com/clap-rs/clap/compare/v3.2.23...v3.2.25">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clap&package-manager=cargo&previous-version=3.2.23&new-version=3.2.25)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:49:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    Bump serde from 1.0.152 to 1.0.156 in /aries-backchannels/aries-vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.152 to 1.0.156.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.156</h2>
<ul>
<li>Documentation improvements</li>
</ul>
<h2>v1.0.155</h2>
<ul>
<li>Support <code>Serialize</code> and <code>Deserialize</code> impls for <code>core::ffi::CStr</code> and <code>alloc::ffi::CString</code> without &quot;std&quot; feature (<a href="https://redirect.github.com/serde-rs/serde/issues/2374">#2374</a>, thanks <a href="https://github.com/safarir"><code>@​safarir</code></a>)</li>
</ul>
<h2>v1.0.154</h2>
<ul>
<li>Fix &quot;undeclared lifetime&quot; error in generated code when deriving Deserialize for an enum with both <code>flatten</code> and <code>'static</code> fields (<a href="https://redirect.github.com/serde-rs/serde/issues/2383">#2383</a>, thanks <a href="https://github.com/Mingun"><code>@​Mingun</code></a>)</li>
</ul>
<h2>v1.0.153</h2>
<ul>
<li>Support <code>serde(alias = &quot;…&quot;)</code> attribute used inside of flattened struct (<a href="https://redirect.github.com/serde-rs/serde/issues/2387">#2387</a>, thanks <a href="https://github.com/bebecue"><code>@​bebecue</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/54671259aaaf2617b0f27dce6cc519058d4f3a90"><code>5467125</code></a> Release 1.0.156</li>
<li><a href="https://github.com/serde-rs/serde/commit/994f7c7924f7fccde5c474644f6d22115586bdee"><code>994f7c7</code></a> Format with rustfmt 1.5.2-nightly</li>
<li><a href="https://github.com/serde-rs/serde/commit/7a8e4977e230e2da45bb7e1f75d7a3175b6a7755"><code>7a8e497</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2401">#2401</a> from dtolnay/docderive</li>
<li><a href="https://github.com/serde-rs/serde/commit/fb7b6ea7ea8864a41e78378ca0555ce3f1dd8965"><code>fb7b6ea</code></a> Enable serde derive feature when built by docs.rs</li>
<li><a href="https://github.com/serde-rs/serde/commit/063dd5b93f9f0c3181de399132441668fed67029"><code>063dd5b</code></a> Show derive macros in serde's rustdoc</li>
<li><a href="https://github.com/serde-rs/serde/commit/a38aa31ade469b034dc8d04c39cc52c0e76c9e75"><code>a38aa31</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2400">#2400</a> from Nilstrieb/explicit-reexport</li>
<li><a href="https://github.com/serde-rs/serde/commit/f42b2581da2bdbb81713a93d3b7e581b81e4332e"><code>f42b258</code></a> Use explicit re-export of <code>serde_derive</code> to give rustc more info</li>
<li><a href="https://github.com/serde-rs/serde/commit/2ba406726f9f84bc3b65ce4e824ae636dfa7dc85"><code>2ba4067</code></a> Release 1.0.155</li>
<li><a href="https://github.com/serde-rs/serde/commit/7e9826e17b154b32742b71285349ec042da7ee35"><code>7e9826e</code></a> Add link to core CStr stabilization announcement</li>
<li><a href="https://github.com/serde-rs/serde/commit/f4dcc5c918a54712fbf76f50883c6c496d0b8af9"><code>f4dcc5c</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2374">#2374</a> from safarir/master</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/serde/compare/v1.0.152...v1.0.156">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.152&new-version=1.0.156)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    Bump @types/node from 14.14.28 to 14.18.63 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@types/node](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/HEAD/types/node) from 14.14.28 to 14.18.63.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/DefinitelyTyped/DefinitelyTyped/commits/HEAD/types/node">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@types/node&package-manager=npm_and_yarn&previous-version=14.14.28&new-version=14.18.63)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    Bump log from 0.4.17 to 0.4.21 in /aries-backchannels/aries-vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [log](https://github.com/rust-lang/log) from 0.4.17 to 0.4.21.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/log/blob/master/CHANGELOG.md">log's changelog</a>.</em></p>
<blockquote>
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
<h2>[0.4.20] - 2023-07-11</h2>
<ul>
<li>Remove rustversion dev-dependency by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/568">rust-lang/log#568</a></li>
<li>Remove <code>local_inner_macros</code> usage by <a href="https://github.com/EFanZh"><code>@​EFanZh</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/570">rust-lang/log#570</a></li>
</ul>
<h2>[0.4.19] - 2023-06-10</h2>
<ul>
<li>Use target_has_atomic instead of the old atomic_cas cfg by <a href="https://github.com/GuillaumeGomez"><code>@​GuillaumeGomez</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/555">rust-lang/log#555</a></li>
<li>Put MSRV into Cargo.toml by <a href="https://github.com/est31"><code>@​est31</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/557">rust-lang/log#557</a></li>
</ul>
<h2>[0.4.18] - 2023-05-28</h2>
<ul>
<li>fix markdown links (again) by <a href="https://github.com/hellow554"><code>@​hellow554</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/513">rust-lang/log#513</a></li>
<li>add cargo doc to workflow by <a href="https://github.com/hellow554"><code>@​hellow554</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/515">rust-lang/log#515</a></li>
<li>Apply Clippy lints by <a href="https://github.com/hellow554"><code>@​hellow554</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/516">rust-lang/log#516</a></li>
<li>Replace ad-hoc eq_ignore_ascii_case with slice::eq_ignore_ascii_case by <a href="https://github.com/glandium"><code>@​glandium</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/519">rust-lang/log#519</a></li>
<li>fix up windows targets by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/528">rust-lang/log#528</a></li>
<li>typo fix by <a href="https://github.com/jiangying000"><code>@​jiangying000</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/529">rust-lang/log#529</a></li>
<li>Remove dependency on cfg_if by <a href="https://github.com/EriKWDev"><code>@​EriKWDev</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/536">rust-lang/log#536</a></li>
<li>GitHub Workflows security hardening by <a href="https://github.com/sashashura"><code>@​sashashura</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/538">rust-lang/log#538</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/log/commit/3ccdc286fef3076747fe18a2a93658ea4d4ae012"><code>3ccdc28</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/617">#617</a> from rust-lang/cargo/0.4.21</li>
<li><a href="https://github.com/rust-lang/log/commit/6153cb289f0e7b80f00ae07dbe5ee41cf3d3fcb0"><code>6153cb2</code></a> prepare for 0.4.21 release</li>
<li><a href="https://github.com/rust-lang/log/commit/f0f74946a4bfb02cfc407795a3499c4b69d7a290"><code>f0f7494</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/613">#613</a> from rust-lang/feat/kv-cleanup</li>
<li><a href="https://github.com/rust-lang/log/commit/2b220bf3b705f2abc0ee591c7eb17972a979da3a"><code>2b220bf</code></a> clean up structured logging example</li>
<li><a href="https://github.com/rust-lang/log/commit/646e9ab9917fb79e44b6b36b8375106a1a09766c"><code>646e9ab</code></a> use original Visitor name for VisitValue</li>
<li><a href="https://github.com/rust-lang/log/commit/cf85c38d3519745d60e7b891c4b2025050a8389f"><code>cf85c38</code></a> add needed subfeatures to kv_unstable</li>
<li><a href="https://github.com/rust-lang/log/commit/73e953905b970ef765a86bf6cbd69bc2c5e2bac4"><code>73e9539</code></a> fix up capturing of :err</li>
<li><a href="https://github.com/rust-lang/log/commit/31bb4b0ff36e458c6bef304a336b71f6342ddcc7"><code>31bb4b0</code></a> move error macros together</li>
<li><a href="https://github.com/rust-lang/log/commit/ad917118a5e781d0dd60b3a75ba519ce9839ba70"><code>ad91711</code></a> support field shorthand in macros</li>
<li><a href="https://github.com/rust-lang/log/commit/90a347bd836873264a393a35bfd90fe478fadae2"><code>90a347b</code></a> restore removed APIs as deprecated</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/log/compare/0.4.17...0.4.21">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log&package-manager=cargo&previous-version=0.4.17&new-version=0.4.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    Bump node-fetch from 2.7.0 to 3.3.2 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.7.0 to 3.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v3.3.2</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.3.1...v3.3.2">3.3.2</a> (2023-07-25)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Remove the default connection close header. (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1736">#1736</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/8b3320d2a7c07bce4afc6b2bf6c3bbddda85b01f">8b3320d</a>), closes <a href="https://redirect.github.com/node-fetch/node-fetch/issues/1735">#1735</a> <a href="https://redirect.github.com/node-fetch/node-fetch/issues/1473">#1473</a></li>
</ul>
<h2>v3.3.1</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.3.0...v3.3.1">3.3.1</a> (2023-03-11)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>release &quot;Allow URL class object as an argument for fetch()&quot; <a href="https://redirect.github.com/node-fetch/node-fetch/issues/1696">#1696</a> (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1716">#1716</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/7b86e946b02dfdd28f4f8fca3d73a022cbb5ca1e">7b86e94</a>)</li>
</ul>
<h2>v3.3.0</h2>
<h1><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.10...v3.3.0">3.3.0</a> (2022-11-10)</h1>
<h3>Features</h3>
<ul>
<li>add static Response.json (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1670">#1670</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/55a4870ae5f805d8ff9a890ea2c652c9977e048e">55a4870</a>)</li>
</ul>
<h2>v3.2.10</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.9...v3.2.10">3.2.10</a> (2022-07-31)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS referrer (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1611">#1611</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/28802387292baee467e042e168d92597b5bbbe3d">2880238</a>)</li>
</ul>
<h2>v3.2.9</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.8...v3.2.9">3.2.9</a> (2022-07-18)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>Headers:</strong> don't forward secure headers on protocol change (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1599">#1599</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/e87b093fd678a9ea39c5b17b2a1bdfc4691eedc7">e87b093</a>)</li>
</ul>
<h2>v3.2.8</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.7...v3.2.8">3.2.8</a> (2022-07-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>possibly flaky test (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1523">#1523</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/11b703361134340a8361f591d6e3a0bcf6a261fa">11b7033</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8b3320d2a7c07bce4afc6b2bf6c3bbddda85b01f"><code>8b3320d</code></a> fix: Remove the default connection close header. (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1736">#1736</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/7b86e946b02dfdd28f4f8fca3d73a022cbb5ca1e"><code>7b86e94</code></a> fix: release &quot;Allow URL class object as an argument for fetch()&quot; <a href="https://redirect.github.com/node-fetch/node-fetch/issues/1696">#1696</a> (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1716">#1716</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8ced5b941cf36d0d7e0c1017aa2a4abcb29ecd89"><code>8ced5b9</code></a> docs: readme - non ESM example (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1707">#1707</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/71e376b0ca899a30bbda4d45f97ea87502956a62"><code>71e376b</code></a> ci(release): use latest Node LTS (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1697">#1697</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/e093030b4a6625405a331ddf48bcfd82c079f43d"><code>e093030</code></a> Allow URL class object as an argument for fetch() (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1696">#1696</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/55a4870ae5f805d8ff9a890ea2c652c9977e048e"><code>55a4870</code></a> feat: add static Response.json (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1670">#1670</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/c071406e193cce13959999982584ff27198e9e4a"><code>c071406</code></a> (1138) - Fixed HTTPResponseError with correct constructor and usage (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1666">#1666</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/6f72caa401a8ec574a22058431599ef47c222770"><code>6f72caa</code></a> docs: fix missing comma in example (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1623">#1623</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/28802387292baee467e042e168d92597b5bbbe3d"><code>2880238</code></a> fix: ReDoS referrer (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1611">#1611</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/e87b093fd678a9ea39c5b17b2a1bdfc4691eedc7"><code>e87b093</code></a> fix(Headers): don't forward secure headers on protocol change (<a href="https://redirect.github.com/node-fetch/node-fetch/issues/1599">#1599</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/node-fetch/node-fetch/compare/v2.7.0...v3.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.7.0&new-version=3.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/821" class=".btn">#821</a>
            </td>
            <td>
                <b>
                    Update prompt-toolkit requirement from ~=2.0.9 to ~=3.0.45 in /aries-backchannels/python
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
<h2>3.0.45</h2>
<p>Fixes:</p>
<ul>
<li>Improve performance of <code>GrammarCompleter</code> (faster deduplication of completions).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/CHANGELOG">prompt-toolkit's changelog</a>.</em></p>
<blockquote>
<h2>3.0.45: 2024-05-28</h2>
<p>Fixes:</p>
<ul>
<li>Improve performance of <code>GrammarCompleter</code> (faster deduplication of completions).</li>
</ul>
<h2>3.0.44: 2024-05-27</h2>
<p>New features:</p>
<ul>
<li>Accept <code>os.PathLike</code> in <code>FileHistory</code> (typing fix).</li>
</ul>
<p>Fixes:</p>
<ul>
<li>Fix memory leak in filters.</li>
<li>Improve performance of progress bar formatters.</li>
<li>Fix compatibility when a SIGINT handler is installed by non-Python (Rust, C).</li>
<li>Limit number of completions in buffer to 10k by default (for performance).</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/6a58564f6a201f1234733f726d866a64e95b6ba3"><code>6a58564</code></a> Release 3.0.45</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/a21831e7f992a014d705cc09f40a5bc5bfaf7ee1"><code>a21831e</code></a> Improve performance of GrammarCompleter (faster deduplication of completions).</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/81dcfdafb8be17bb471ce979e870bd3220844390"><code>81dcfda</code></a> Release 3.0.44.</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/386477a12c8ffca17355a55de29eb618f599261a"><code>386477a</code></a> Limit number of completions in buffer to 10k by default.</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/491b5e84cd5119a87f58cb5c88755486dd4e58f8"><code>491b5e8</code></a> Typing fix in FileHistory.</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/3c0290dff5c2d5aed4d1b1e804716ae0da391ba5"><code>3c0290d</code></a> Code style fixes for compatibility with latest Ruff.</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/85079ad4d726e64089d9e0efa9faa36a084b7d67"><code>85079ad</code></a> Fix compatibility when SIGINT handler is installed by non-Python</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/2c8430726fe02d8497ad1c8441586cf4ba4124de"><code>2c84307</code></a> Add ass</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/e0fd8fab49f43dafe17f2d873be5ecd58121cdeb"><code>e0fd8fa</code></a> fix(Docs): address some typos in the tutorial pages</li>
<li><a href="https://github.com/prompt-toolkit/python-prompt-toolkit/commit/f8cf7caed17e16c9f5327d9cccdafe5c8496acfa"><code>f8cf7ca</code></a> Fix performance issue with ProgressBar formatters</li>
<li>Additional commits viewable in <a href="https://github.com/prompt-toolkit/python-prompt-toolkit/compare/2.0.9...3.0.45">compare view</a></li>
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
        Created At 2024-05-28 14:48:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/820" class=".btn">#820</a>
            </td>
            <td>
                <b>
                    Bump python from 3.7-slim-bullseye to 3.12-slim-bullseye in /aries-backchannels/acapy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.7-slim-bullseye to 3.12-slim-bullseye.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.7-slim-bullseye&new-version=3.12-slim-bullseye)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/819" class=".btn">#819</a>
            </td>
            <td>
                <b>
                    Bump @tsed/exceptions from 6.75.4 to 6.133.1 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@tsed/exceptions](https://github.com/tsedio/tsed) from 6.75.4 to 6.133.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tsedio/tsed/commit/2d4e76268a7e17fa514af39b65d0bcc2ef84a548"><code>2d4e762</code></a> Github CI build: __run_2 v6.133.1 [ci skip]</li>
<li><a href="https://github.com/tsedio/tsed/commit/1fa19cc20ed7079422f1b2fcb29f1ce0be5ba0e9"><code>1fa19cc</code></a> fix(json-mapper): support BigInt type</li>
<li><a href="https://github.com/tsedio/tsed/commit/d5d0a9423e83653ac798257b2cb74642bafb1d22"><code>d5d0a94</code></a> docs: fix Map documentation example</li>
<li><a href="https://github.com/tsedio/tsed/commit/067bc6027f2013ffc19ce3d287dde2f43943b411"><code>067bc60</code></a> <a href="https://redirect.github.com/tsedio/tsed/issues/2096">#2096</a> Fix keycloak documentation</li>
<li><a href="https://github.com/tsedio/tsed/commit/33816667a851bb7de9028f058359d5c450c2fba5"><code>3381666</code></a> Github CI build: __run_2 v6.133.0 [ci skip]</li>
<li><a href="https://github.com/tsedio/tsed/commit/8808d6c00dafc6cabcd136900c76a21a6fe0849a"><code>8808d6c</code></a> feat(objection): add UUID PK column support</li>
<li><a href="https://github.com/tsedio/tsed/commit/346bcb29563d73aeb028312d118d0421b3ae3951"><code>346bcb2</code></a> Github CI build: __run_2 v6.132.1 [ci skip]</li>
<li><a href="https://github.com/tsedio/tsed/commit/7cdc7483a7dd05692e157f4af37712527abd6e26"><code>7cdc748</code></a> fix(terminus): fix events emitted by terminus</li>
<li><a href="https://github.com/tsedio/tsed/commit/70a88fe7e6ca50bc987ca3c67c4323e6d3ce751e"><code>70a88fe</code></a> Github CI build: __run_2 v6.132.0 [ci skip]</li>
<li><a href="https://github.com/tsedio/tsed/commit/56f34527707ff5fa34a7cd97bd9060ca52a9510d"><code>56f3452</code></a> feat(schema): add test for unsupported decorator types</li>
<li>Additional commits viewable in <a href="https://github.com/tsedio/tsed/compare/v6.75.4...v6.133.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@tsed/exceptions&package-manager=npm_and_yarn&previous-version=6.75.4&new-version=6.133.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    Bump allure-behave from 2.13.3 to 2.13.5 in /aries-test-harness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [allure-behave](https://github.com/allure-framework/allure-python) from 2.13.3 to 2.13.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/allure-framework/allure-python/releases">allure-behave's releases</a>.</em></p>
<blockquote>
<h2>2.13.5</h2>
<h2>🐞 Bug fixes</h2>
<ul>
<li>Replace version comparison with duck-style checks (fix <a href="https://redirect.github.com/allure-framework/allure-python/issues/802">#802</a>) (via <a href="https://redirect.github.com/allure-framework/allure-python/issues/803">#803</a>) - <a href="https://github.com/delatrie"><code>@​delatrie</code></a></li>
</ul>
<h2>👀 Links</h2>
<p><a href="https://github.com/allure-framework/allure-python/compare/2.13.4...master">Commits since 2.13.4</a></p>
<h2>2.13.4</h2>
<h2>🚀 New features</h2>
<ul>
<li>Add logs, stdout and stderr to the allure-pytest-bdd report  (via <a href="https://redirect.github.com/allure-framework/allure-python/issues/801">#801</a>) - <a href="https://github.com/IvanBuruyane"><code>@​IvanBuruyane</code></a></li>
<li>Make allure-behave compatible with Behave v1.2.7.dev5 (implements <a href="https://redirect.github.com/allure-framework/allure-python/issues/771">#771</a> via <a href="https://redirect.github.com/allure-framework/allure-python/issues/798">#798</a>) - <a href="https://github.com/ercaronte"><code>@​ercaronte</code></a>
<blockquote>
<p>NOTE:
Use the following syntax to install a pre-release version of Behave 1.2.7:</p>
<pre><code>pip install -U git+https://github.com/behave/behave@v1.2.7.dev5
</code></pre>
</blockquote>
</li>
</ul>
<h2>👻 Internal changes</h2>
<ul>
<li>Add run-name to release workflow (via <a href="https://redirect.github.com/allure-framework/allure-python/issues/800">#800</a>) - <a href="https://github.com/delatrie"><code>@​delatrie</code></a></li>
</ul>
<h2>👀 Links</h2>
<p><a href="https://github.com/allure-framework/allure-python/compare/2.13.3...master">Commits since 2.13.3</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/allure-framework/allure-python/commit/d85734976a3490ba1d01f859c53d4259582bac22"><code>d857349</code></a> Replace version comparison with duck-style checks (fix <a href="https://redirect.github.com/allure-framework/allure-python/issues/802">#802</a>) (<a href="https://redirect.github.com/allure-framework/allure-python/issues/803">#803</a>)</li>
<li><a href="https://github.com/allure-framework/allure-python/commit/097fcf687fe22f075dffbfcd2a0d9a44eb04195c"><code>097fcf6</code></a> Add logs, stdout and stderr to the allure-pytest-bdd report  (<a href="https://redirect.github.com/allure-framework/allure-python/issues/801">#801</a>)</li>
<li><a href="https://github.com/allure-framework/allure-python/commit/d759bc549c03c0b473457674beac350a03cba5bc"><code>d759bc5</code></a> Fixes <a href="https://redirect.github.com/allure-framework/allure-python/issues/771">#771</a> allure-behave formatter crash with behave v1.2.7.dev5 (<a href="https://redirect.github.com/allure-framework/allure-python/issues/798">#798</a>)</li>
<li><a href="https://github.com/allure-framework/allure-python/commit/2a71e7fb1d6f32ffbc34ee014e64e00cd686c248"><code>2a71e7f</code></a> add run-name to release workflow (via <a href="https://redirect.github.com/allure-framework/allure-python/issues/800">#800</a>)</li>
<li>See full diff in <a href="https://github.com/allure-framework/allure-python/compare/2.13.3...2.13.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=allure-behave&package-manager=pip&previous-version=2.13.3&new-version=2.13.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/817" class=".btn">#817</a>
            </td>
            <td>
                <b>
                    Bump python from 3.7-buster to 3.11-buster in /aries-test-harness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.7-buster to 3.11-buster.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.7-buster&new-version=3.11-buster)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    Bump @hyperledger/anoncreds-nodejs from 0.1.0 to 0.2.2 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@hyperledger/anoncreds-nodejs](https://github.com/hyperledger/anoncreds-rs/tree/HEAD/wrappers/javascript/anoncreds-nodejs) from 0.1.0 to 0.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/anoncreds-rs/releases"><code>@​hyperledger/anoncreds-nodejs</code>'s releases</a>.</em></p>
<blockquote>
<h2>v0.2.0</h2>
<h2>What's Changed</h2>
<ul>
<li>build(deps): bump semver from 5.7.1 to 5.7.2 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/222">hyperledger/anoncreds-rs#222</a></li>
<li>Update settings.yml by <a href="https://github.com/tnkhanh"><code>@​tnkhanh</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/223">hyperledger/anoncreds-rs#223</a></li>
<li>build(deps): bump word-wrap from 1.2.3 to 1.2.4 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/225">hyperledger/anoncreds-rs#225</a></li>
<li>chore: replace ursa lib with anoncreds-clsignatures-rs by <a href="https://github.com/amanji"><code>@​amanji</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/226">hyperledger/anoncreds-rs#226</a></li>
<li>Update to anoncreds-clsignatures 0.2, update tails access by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/229">hyperledger/anoncreds-rs#229</a></li>
<li>refactor: services function signatures improvements by <a href="https://github.com/bobozaur"><code>@​bobozaur</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/228">hyperledger/anoncreds-rs#228</a></li>
<li>fix: JS wrapper updates by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/231">hyperledger/anoncreds-rs#231</a></li>
<li>Revocation registry cleanups by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/233">hyperledger/anoncreds-rs#233</a></li>
<li>Remove tails path from FfiCredRevInfo by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/235">hyperledger/anoncreds-rs#235</a></li>
<li>Hashmap uniformization by <a href="https://github.com/bobozaur"><code>@​bobozaur</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/232">hyperledger/anoncreds-rs#232</a></li>
<li>fix(js): free native strings by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/238">hyperledger/anoncreds-rs#238</a></li>
<li>Simplify LinkSecret handling by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/237">hyperledger/anoncreds-rs#237</a></li>
<li>fix(js): bump patched ref-napi/ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/243">hyperledger/anoncreds-rs#243</a></li>
<li>Make zeroize not used with <code>no-default-features</code> by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/242">hyperledger/anoncreds-rs#242</a></li>
<li>Simplify create_credential parameters and remove RevocationRegistryId by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/239">hyperledger/anoncreds-rs#239</a></li>
<li>chore: update version to 0.2.0-dev.1 by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/245">hyperledger/anoncreds-rs#245</a></li>
<li>feat: add zeroize as a feature by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/244">hyperledger/anoncreds-rs#244</a></li>
<li>feat: switched to pnpm and added react native example app by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/249">hyperledger/anoncreds-rs#249</a></li>
<li>Build cleanups; verify auditwheel output by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/251">hyperledger/anoncreds-rs#251</a></li>
<li>fix: do not free string by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/253">hyperledger/anoncreds-rs#253</a></li>
<li>chore: update version to dev 2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/254">hyperledger/anoncreds-rs#254</a></li>
<li>fix leading zero bug by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/255">hyperledger/anoncreds-rs#255</a></li>
<li>lock lerna to 7.2.0 by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/256">hyperledger/anoncreds-rs#256</a></li>
<li>do not write to .npmrc for release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/257">hyperledger/anoncreds-rs#257</a></li>
<li>fixed build issue for JS wrappers by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/258">hyperledger/anoncreds-rs#258</a></li>
<li>fix js install script issue with platform by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/259">hyperledger/anoncreds-rs#259</a></li>
<li>fix minor typos in comments by <a href="https://github.com/vuittont60"><code>@​vuittont60</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/260">hyperledger/anoncreds-rs#260</a></li>
<li>update js version by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/261">hyperledger/anoncreds-rs#261</a></li>
<li>fix(js): use quotes instead of brackets for local dependencies by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/262">hyperledger/anoncreds-rs#262</a></li>
<li>use universal for darwin by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/264">hyperledger/anoncreds-rs#264</a></li>
<li>SNYK by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/280">hyperledger/anoncreds-rs#280</a></li>
<li>Address SNYK warnings by <a href="https://github.com/ryjones"><code>@​ryjones</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/277">hyperledger/anoncreds-rs#277</a></li>
<li>Design: AnonCreds Credentials using the W3C Standard by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/266">hyperledger/anoncreds-rs#266</a></li>
<li>Manual update of Snyk PRs that are not DCOd by <a href="https://github.com/swcurran"><code>@​swcurran</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/285">hyperledger/anoncreds-rs#285</a></li>
<li>AnonCreds Credentials using the W3C Standard - implementation by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/271">hyperledger/anoncreds-rs#271</a></li>
<li>Update Rust version used in CI by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/298">hyperledger/anoncreds-rs#298</a></li>
<li>Reworked w3c credentials and presentations to use DataIntegrityProof  instead of custom AnonCreds context by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/291">hyperledger/anoncreds-rs#291</a></li>
<li>ci: allow to publish wrappers separately by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/296">hyperledger/anoncreds-rs#296</a></li>
<li>AnonCreds Credentials using the W3C Standard - proof value encoding by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/276">hyperledger/anoncreds-rs#276</a></li>
<li>Do not apply prettier to pnpm lockfile by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/301">hyperledger/anoncreds-rs#301</a></li>
<li>Bump follow-redirects from 1.15.3 to 1.15.5 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/300">hyperledger/anoncreds-rs#300</a></li>
<li>AnonCreds Credentials using the W3C Standard - wrappers by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/273">hyperledger/anoncreds-rs#273</a></li>
<li>W3C: Reworked predicates representation - no mapping by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/303">hyperledger/anoncreds-rs#303</a></li>
<li>chore: update version to 0.2.0-dev.6 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/304">hyperledger/anoncreds-rs#304</a></li>
<li>Support numbers values in AnonCreds W3C VC by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/305">hyperledger/anoncreds-rs#305</a></li>
<li>chore: update version to 0.2.0-dev.7 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/306">hyperledger/anoncreds-rs#306</a></li>
<li>W3C: Removed logic connected to stripping out id property of credential attributes by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/309">hyperledger/anoncreds-rs#309</a></li>
<li>Relax validation on prover_did in a credential request by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/anoncreds-rs/pull/310">hyperledger/anoncreds-rs#310</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/hyperledger/anoncreds-rs/commits/HEAD/wrappers/javascript/anoncreds-nodejs">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@hyperledger/anoncreds-nodejs&package-manager=npm_and_yarn&previous-version=0.1.0&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:48:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/815" class=".btn">#815</a>
            </td>
            <td>
                <b>
                    Bump alpine from 3.15.4 to 3.20.0 in /aries-backchannels/aries-vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps alpine from 3.15.4 to 3.20.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=alpine&package-manager=docker&previous-version=3.15.4&new-version=3.20.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:47:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/814" class=".btn">#814</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-slim-bullseye to 3.12-slim-bullseye in /aries-backchannels/mobile
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
        Created At 2024-05-28 14:47:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/813" class=".btn">#813</a>
            </td>
            <td>
                <b>
                    Bump ubuntu from 18.04 to 24.04 in /aries-backchannels/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps ubuntu from 18.04 to 24.04.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ubuntu&package-manager=docker&previous-version=18.04&new-version=24.04)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:47:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/812" class=".btn">#812</a>
            </td>
            <td>
                <b>
                    Bump streetcred/dotnet-indy from 1.15.0 to 1.15.1 in /aries-backchannels/dotnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps streetcred/dotnet-indy from 1.15.0 to 1.15.1.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=streetcred/dotnet-indy&package-manager=docker&previous-version=1.15.0&new-version=1.15.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 14:47:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/811" class=".btn">#811</a>
            </td>
            <td>
                <b>
                    Update qrcode[pil] requirement from ~=6.1 to ~=7.4 in /aries-backchannels/mobile
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
        Created At 2024-05-28 14:47:49 +0000 UTC
    </div>
</div>

