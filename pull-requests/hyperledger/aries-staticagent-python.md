---
layout: default
title: aries-staticagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-staticagent-python
---

# aries-staticagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-staticagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump nokogiri from 1.12.5 to 1.13.4 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.12.5 to 1.13.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>1.13.4 / 2022-04-11</h2>
<h3>Security</h3>
<ul>
<li>Address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-24836">CVE-2022-24836</a>, a regular expression denial-of-service vulnerability. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-crjr-9rc5-ghw8">GHSA-crjr-9rc5-ghw8</a> for more information.</li>
<li>[CRuby] Vendored zlib is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2018-25032">CVE-2018-25032</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-v6gp-9mmm-c6p5">GHSA-v6gp-9mmm-c6p5</a> for more information.</li>
<li>[JRuby] Vendored Xerces-J (<code>xerces:xercesImpl</code>) is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-23437">CVE-2022-23437</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-xxx9-3xcr-gjj3">GHSA-xxx9-3xcr-gjj3</a> for more information.</li>
<li>[JRuby] Vendored nekohtml (<code>org.cyberneko.html</code>) is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-24839">CVE-2022-24839</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-gx8x-g87m-h5q6">GHSA-gx8x-g87m-h5q6</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored zlib is updated from 1.2.11 to 1.2.12. (See <a href="https://github.com/sparklemotion/nokogiri/blob/v1.13.x/LICENSE-DEPENDENCIES.md#platform-releases">LICENSE-DEPENDENCIES.md</a> for details on which packages redistribute this library.)</li>
<li>[JRuby] Vendored Xerces-J (<code>xerces:xercesImpl</code>) is updated from 2.12.0 to 2.12.2.</li>
<li>[JRuby] Vendored nekohtml (<code>org.cyberneko.html</code>) is updated from a fork of 1.9.21 to 1.9.22.noko2. This fork is now publicly developed at <a href="https://github.com/sparklemotion/nekohtml">https://github.com/sparklemotion/nekohtml</a></li>
</ul>
<hr />
<p>sha256sum:</p>
<pre><code>095ff1995ed3dda3ea98a5f08bdc54bef02be1ce4e7c81034c4812e5e7c6e7e3  nokogiri-1.13.4-aarch64-linux.gem
7ebfc7415c819bcd4e849627e879cef2fb328bec90e802e50d74ccd13a60ec75  nokogiri-1.13.4-arm64-darwin.gem
41efd87c121991de26ef0393ac713d687e539813c3b79e454a2e3ffeecd107ea  nokogiri-1.13.4-java.gem
ab547504692ada0cec9d2e4e15afab659677c3f4c1ac3ea639bf5212b65246a1  nokogiri-1.13.4-x64-mingw-ucrt.gem
fa5c64cfdb71642ed647428e4d0d75ee0f4d189cfb63560c66fd8bdf99eb146b  nokogiri-1.13.4-x64-mingw32.gem
d6f07cbcbc28b75e8ac5d6e729ffba3602dffa0ad16ffac2322c9b4eb9b971fc  nokogiri-1.13.4-x86-linux.gem
0f7a4fd13e25abe3f98663fef0d115d58fdeff62cf23fef12d368e42adad2ce6  nokogiri-1.13.4-x86-mingw32.gem
3eef282f00ad360304fbcd5d72eb1710ff41138efda9513bb49eec832db5fa3e  nokogiri-1.13.4-x86_64-darwin.gem
3978610354ec67b59c128d23259c87b18374ee1f61cb9ed99de7143a88e70204  nokogiri-1.13.4-x86_64-linux.gem
0d46044eb39271e3360dae95ed6061ce17bc0028d475651dc48db393488c83bc  nokogiri-1.13.4.gem
</code></pre>
<h2>1.13.3 / 2022-02-21</h2>
<h3>Fixed</h3>
<ul>
<li>[CRuby] Revert a HTML4 parser bug in libxml 2.9.13 (introduced in Nokogiri v1.13.2). The bug causes libxml2's HTML4 parser to fail to recover when encountering a bare <code>&lt;</code> character in some contexts. This version of Nokogiri restores the earlier behavior, which is to recover from the parse error and treat the <code>&lt;</code> as normal character data (which will be serialized as <code>&amp;lt;</code> in a text node). The bug (and the fix) is only relevant when the <code>RECOVER</code> parse option is set, as it is by default. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2461">#2461</a>]</li>
</ul>
<hr />
<p>SHA256 checksums:</p>
<pre><code>025a4e333f6f903072a919f5f75b03a8f70e4969dab4280375b73f9d8ff8d2c0  nokogiri-1.13.3-aarch64-linux.gem
b9cb59c6a6da8cf4dbee5dbb569c7cc95a6741392e69053544e0f40b15ab9ad5  nokogiri-1.13.3-arm64-darwin.gem
e55d18cee64c19d51d35ad80634e465dbcdd46ac4233cb42c1e410307244ebae  nokogiri-1.13.3-java.gem
53e2d68116cd00a873406b8bdb90c78a6f10e00df7ddf917a639ac137719b67b  nokogiri-1.13.3-x64-mingw-ucrt.gem
b5f39ebb662a1be7d1c61f8f0a2a683f1bb11690a6f00a99a1aa23a071f80145  nokogiri-1.13.3-x64-mingw32.gem
7c0de5863aace4bbbc73c4766cf084d1f0b7a495591e46d1666200cede404432  nokogiri-1.13.3-x86-linux.gem
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/v1.13.4/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>1.13.4 / 2022-04-11</h2>
<h3>Security</h3>
<ul>
<li>Address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-24836">CVE-2022-24836</a>, a regular expression denial-of-service vulnerability. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-crjr-9rc5-ghw8">GHSA-crjr-9rc5-ghw8</a> for more information.</li>
<li>[CRuby] Vendored zlib is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2018-25032">CVE-2018-25032</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-v6gp-9mmm-c6p5">GHSA-v6gp-9mmm-c6p5</a> for more information.</li>
<li>[JRuby] Vendored Xerces-J (<code>xerces:xercesImpl</code>) is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-23437">CVE-2022-23437</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-xxx9-3xcr-gjj3">GHSA-xxx9-3xcr-gjj3</a> for more information.</li>
<li>[JRuby] Vendored nekohtml (<code>org.cyberneko.html</code>) is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-24839">CVE-2022-24839</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-gx8x-g87m-h5q6">GHSA-gx8x-g87m-h5q6</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored zlib is updated from 1.2.11 to 1.2.12. (See <a href="https://github.com/sparklemotion/nokogiri/blob/v1.13.x/LICENSE-DEPENDENCIES.md#platform-releases">LICENSE-DEPENDENCIES.md</a> for details on which packages redistribute this library.)</li>
<li>[JRuby] Vendored Xerces-J (<code>xerces:xercesImpl</code>) is updated from 2.12.0 to 2.12.2.</li>
<li>[JRuby] Vendored nekohtml (<code>org.cyberneko.html</code>) is updated from a fork of 1.9.21 to 1.9.22.noko2. This fork is now publicly developed at <a href="https://github.com/sparklemotion/nekohtml">https://github.com/sparklemotion/nekohtml</a></li>
</ul>
<h2>1.13.3 / 2022-02-21</h2>
<h3>Fixed</h3>
<ul>
<li>[CRuby] Revert a HTML4 parser bug in libxml 2.9.13 (introduced in Nokogiri v1.13.2). The bug causes libxml2's HTML4 parser to fail to recover when encountering a bare <code>&lt;</code> character in some contexts. This version of Nokogiri restores the earlier behavior, which is to recover from the parse error and treat the <code>&lt;</code> as normal character data (which will be serialized as <code>&amp;lt;</code> in a text node). The bug (and the fix) is only relevant when the <code>RECOVER</code> parse option is set, as it is by default. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2461">#2461</a>]</li>
</ul>
<h2>1.13.2 / 2022-02-21</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated from 2.9.12 to 2.9.13. This update addresses <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-23308">CVE-2022-23308</a>.</li>
<li>[CRuby] Vendored libxslt is updated from 1.1.34 to 1.1.35. This update addresses <a href="https://nvd.nist.gov/vuln/detail/CVE-2021-30560">CVE-2021-30560</a>.</li>
</ul>
<p>Please see <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-fq42-c5rg-92c2">GHSA-fq42-c5rg-92c2</a> for more information about these CVEs.</p>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated from 2.9.12 to 2.9.13. Full changelog is available at <a href="https://download.gnome.org/sources/libxml2/2.9/libxml2-2.9.13.news">https://download.gnome.org/sources/libxml2/2.9/libxml2-2.9.13.news</a></li>
<li>[CRuby] Vendored libxslt is updated from 1.1.34 to 1.1.35. Full changelog is available at <a href="https://download.gnome.org/sources/libxslt/1.1/libxslt-1.1.35.news">https://download.gnome.org/sources/libxslt/1.1/libxslt-1.1.35.news</a></li>
</ul>
<h2>1.13.1 / 2022-01-13</h2>
<h3>Fixed</h3>
<ul>
<li>Fix <code>Nokogiri::XSLT.quote_params</code> regression in v1.13.0 that raised an exception when non-string stylesheet parameters were passed. Non-string parameters (e.g., integers and symbols) are now explicitly supported and both keys and values will be stringified with <code>#to_s</code>. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2418">#2418</a>]</li>
<li>Fix CSS selector query regression in v1.13.0 that raised an <code>Nokogiri::XML::XPath::SyntaxError</code> when parsing XPath attributes mixed into the CSS query. Although this mash-up of XPath and CSS syntax previously worked unintentionally, it is now an officially supported feature and is documented as such. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2419">#2419</a>]</li>
</ul>
<h2>1.13.0 / 2022-01-06</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/4e2c4b2571dc58af294f61e6fd923f0d1698c036"><code>4e2c4b2</code></a> version bump to v1.13.4</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/6a20ee4d5d203d7d43096ec4d133e06cc3ba2339"><code>6a20ee4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2510">#2510</a> from sparklemotion/flavorjones-encoding-reader-perfo...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/b848031a598545f3383e282596349ee0d42db99b"><code>b848031</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2509">#2509</a> from sparklemotion/flavorjones-parse-processing-inst...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/c0ecf3b6ef90fd0032b348988b7111026c0dd060"><code>c0ecf3b</code></a> test: pend the LIBXML_LOADED_VERSION test on freebsd</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/e444525ef1634b675cd1cf52d39f4320ef0aecfd"><code>e444525</code></a> fix(perf): HTML4::EncodingReader detection</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/1eb5580666187fdde82966f7937dd12f44cc5637"><code>1eb5580</code></a> style(rubocop): allow intentional use of empty initializer</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/0feac5af685dc2fccfbafc33350bf49aab9423ba"><code>0feac5a</code></a> fix(dep): HTML parsing of processing instructions</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/db72b906c5ae9c08920a6ef73db07d55f6da2951"><code>db72b90</code></a> test: recent nekohtml versions do not consider 'a' to be inline</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/2af2a87985290673e4aeb93746a0d638f417060b"><code>2af2a87</code></a> style(rubocop): allow intentional use of empty initializer</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/ba7a28c9a2f150b87fe3a48d58f2cd93d810a5a0"><code>ba7a28c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2499">#2499</a> from sparklemotion/2441-xerces-2.12.2-backport-v1.13.x</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.12.5...v1.13.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.12.5&new-version=1.13.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-staticagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 08:53:47 +0000 UTC
    </div>
</div>

