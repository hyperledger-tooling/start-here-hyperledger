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
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump nokogiri from 1.12.5 to 1.13.3 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.12.5 to 1.13.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
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
675cc3e7d7cca0d6790047a062cd3aa3eab59e3cb9b19374c34f98bade588c66  nokogiri-1.13.3-x86-mingw32.gem
f445596a5a76941a9d1980747535ab50d3399d1b46c32989bc26b7dd988ee498  nokogiri-1.13.3-x86_64-darwin.gem
3f6340661c2a283b337d227ea224f859623775b2f5c09a6bf197b786563958df  nokogiri-1.13.3-x86_64-linux.gem
bf1b1bceff910abb0b7ad825535951101a0361b859c2ad1be155c010081ecbdc  nokogiri-1.13.3.gem
</code></pre>
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
<hr />
<p>SHA256 checksums:</p>
<pre><code>63469a9bb56a21c62fbaea58d15f54f8f167ff6fde51c5c2262072f939926fdd  nokogiri-1.13.2-aarch64-linux.gem
2986617f982f645c06f22515b721e6d2613dd69493e5c41ddd03c4830c3b3065  nokogiri-1.13.2-arm64-darwin.gem
aca1d66206740b29d0d586b1d049116adcb31e6cdd7c4dd3a96eb77da215a0c4  nokogiri-1.13.2-java.gem
b9e4eea1a200d9a927a5bc7d662c427e128779cba0098ea49ddbdb3ffc3ddaec  nokogiri-1.13.2-x64-mingw-ucrt.gem
48d5493fec495867c5516a908a068c1387a1d17c5aeca6a1c98c089d9d9fdcf8  nokogiri-1.13.2-x64-mingw32.gem
62034d7aaaa83fbfcb8876273cc5551489396841a66230d3200b67919ef76cf9  nokogiri-1.13.2-x86-linux.gem
e07237b82394017c2bfec73c637317ee7dbfb56e92546151666abec551e46d1d  nokogiri-1.13.2-x86-mingw32.gem
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
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
<h3>Notes</h3>
<h4>Ruby</h4>
<p>This release introduces native gem support for Ruby 3.1. Please note that Windows users should use the <code>x64-mingw-ucrt</code> platform gem for Ruby 3.1, and <code>x64-mingw32</code> for Ruby 2.6–3.0 (see <a href="https://rubyinstaller.org/2021/12/31/rubyinstaller-3.1.0-1-released.html">RubyInstaller 3.1.0 release notes</a>).</p>
<p>This release ends support for:</p>
<ul>
<li>Ruby 2.5, for which <a href="https://www.ruby-lang.org/en/downloads/branches/">official support ended 2021-03-31</a>.</li>
<li>JRuby 9.2, which is a Ruby 2.5-compatible release.</li>
</ul>
<h4>Faster, more reliable installation: Native Gem for ARM64 Linux</h4>
<p>This version of Nokogiri ships experimental native gem support for the <code>aarch64-linux</code> platform, which should support AWS Graviton and other ARM Linux platforms. We don't yet have CI running for this platform, and so we're interested in hearing back from y'all whether this is working, and what problems you're seeing. Please send us feedback here: <a href="https://github.com/sparklemotion/nokogiri/discussions/2359">Feedback: Have you used the <code>aarch64-linux</code> native gem?</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/7d74cedf275b684d8abd0c2ee281ff6a8adde8ef"><code>7d74ced</code></a> version bump to v1.13.3</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/5970fd95c8305368da8a898490c97b36ea5fa6ba"><code>5970fd9</code></a> fix: revert libxml2 regression with HTML4 recovery</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/49b86631b7e84ec29b4b445f5a2f22fbcbf258b0"><code>49b8663</code></a> version bump to v1.13.2</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/472913378794b8cae21751b0777205e7c0606a95"><code>4729133</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2457">#2457</a> from sparklemotion/flavorjones-libxml-2.9.13-v1.13.x</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/379f757ef529feae0fafba2ae2c145c050d8a4fc"><code>379f757</code></a> dev(package): work around gnome mirrors with expired certs</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/95cf66ca9ff0fc5b85b6c74730b102afb50331c6"><code>95cf66c</code></a> dep: upgrade libxml2 2.9.12 → 2.9.13</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/d37dd02ea59d9dacf09063860007a205ef2eb82e"><code>d37dd02</code></a> dep: upgrade libxslt 1.1.34 → 1.1.35</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/59a93986ec208387e8a9bda94dbf4f89abc1c20d"><code>59a9398</code></a> dep: upgrade mini_portile 2.7 to 2.8</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/e8854632856b6641bc5439395ee8d7a3ad6b1a5c"><code>e885463</code></a> dev(package): handle either .tar.gz or .tar.xz archive names</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/7957c7b00936e282fbc93919647a3fb2502a4388"><code>7957c7b</code></a> style: rubocop</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.12.5...v1.13.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.12.5&new-version=1.13.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-02-26 09:54:54 +0000 UTC
    </div>
</div>

