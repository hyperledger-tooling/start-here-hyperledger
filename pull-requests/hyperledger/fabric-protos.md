---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Bump nokogiri from 1.13.6 to 1.14.3 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.13.6 to 1.14.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>1.14.3 / 2023-04-11</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address CVE-2023-29469, CVE-2023-28484, and one other security-related issue. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-pxvg-2qj5-37jq">GHSA-pxvg-2qj5-37jqGHSA-pxvg-2qj5-37jq</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.10.4">v2.10.4</a> from v2.10.3.</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre><code>9cc53dd8d92868a0f5bcee44396357a19f95e32d8b9754092622a25bc954c60c  nokogiri-1.14.3-aarch64-linux.gem
320fa1836b8e59e86a804baee534893bcf3b901cc255bbec6d87f3dd3e431610  nokogiri-1.14.3-arm-linux.gem
67dd4ac33a8cf0967c521fa57e5a5422db39da8a9d131aaa2cd53deaa12be4cd  nokogiri-1.14.3-arm64-darwin.gem
13969ec7f41d9cff46fc7707224c55490a519feef7cfea727c6945c5b444caa2  nokogiri-1.14.3-java.gem
9885085249303461ee08f9a9b161d0a570391b8f5be0316b3ac5a6d9a947e1e2  nokogiri-1.14.3-x64-mingw-ucrt.gem
997943d7582a23ad6e7a0abe081d0d40d2c1319a6b2749f9b30fd18037f0c38a  nokogiri-1.14.3-x64-mingw32.gem
58c30b763aebd62dc4222385509d7f83ac398ee520490fadc4b6d7877e29895a  nokogiri-1.14.3-x86-linux.gem
e1d58a5c56c34aab71b00901a969e19bf9f7322ee459b4e9380f433213887c04  nokogiri-1.14.3-x86-mingw32.gem
f0a1ed1460a91fd2daf558357f4c0ceac6d994899da1bf98431aeda301e4dc74  nokogiri-1.14.3-x86_64-darwin.gem
e323a7c654ef846e64582fb6e26f6fed869a96753f8e048ff723e74d8005cb11  nokogiri-1.14.3-x86_64-linux.gem
3b1cee0eb8879e9e25b6dd431be597ca68f20283b0d4f4ca986521fad107dc3a  nokogiri-1.14.3.gem
</code></pre>
<h2>1.14.2 / 2023-02-13</h2>
<h3>Fixed</h3>
<ul>
<li>Calling <code>NodeSet#to_html</code> on an empty node set no longer raises an encoding-related exception. This bug was introduced in v1.14.0 while fixing <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2649">#2649</a>. [<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2784">#2784</a>]</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre lang="text"><code>966acf4f6c1fba10518f86498141cf44265564ac5a65dcc8496b65f8c354f776  nokogiri-1.14.2-aarch64-linux.gem
8a3a35cadae4a800ddc0b967394257343d62196d9d059b54e38cf067981db428  nokogiri-1.14.2-arm-linux.gem
81404cd014ecb597725c3847523c2ee365191a968d0b5f7d857e03f388c57631  nokogiri-1.14.2-arm64-darwin.gem
0a39222af14e75eb0243e8d969345e03b90c0e02b0f33c61f1ebb6ae53538bb5  nokogiri-1.14.2-java.gem
62a18f9213a0ceeaf563d1bc7ccfd93273323c4356ded58a5617c59bc4635bc5  nokogiri-1.14.2-x64-mingw-ucrt.gem
54f6ac2c15a7a88f431bb5e23f4616aa8fc97a92eb63336bcf65b7050f2d3be0  nokogiri-1.14.2-x64-mingw32.gem
c42fa0856f01f901954898e28c3c2b4dce0e843056b1b126f441d06e887e1b77  nokogiri-1.14.2-x86-linux.gem
f940d9c8e47b0f19875465376f2d1c8911bc9489ac9a48c124579819dc4a7f19  nokogiri-1.14.2-x86-mingw32.gem
2508978f5ca28944919973f6300f0a7355fbe72604ab6a6913f1630be1030265  nokogiri-1.14.2-x86_64-darwin.gem
bc6405e1f3ddac6e401f82d775f1c0c24c6e58c371b3fadaca0596d5d511e476  nokogiri-1.14.2-x86_64-linux.gem
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>1.14.3 / 2023-04-11</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address CVE-2023-29469, CVE-2023-28484, and one other security-related issue. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-pxvg-2qj5-37jq">GHSA-pxvg-2qj5-37jqGHSA-pxvg-2qj5-37jq</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.10.4">v2.10.4</a> from v2.10.3.</li>
</ul>
<h2>1.14.2 / 2023-02-13</h2>
<h3>Fixed</h3>
<ul>
<li>Calling <code>NodeSet#to_html</code> on an empty node set no longer raises an encoding-related exception. This bug was introduced in v1.14.0 while fixing <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2649">#2649</a>. [<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2784">#2784</a>]</li>
</ul>
<h2>1.14.1 / 2023-01-30</h2>
<h3>Fixed</h3>
<ul>
<li>Serializing documents now works again with pseudo-IO objects that don't support IO's encoding API (like rubyzip's <code>Zip::OutputStream</code>). This was a regression in v1.14.0 due to the fix for <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/752">#752</a> in <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2434">#2434</a>, and was not completely fixed by <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2753">#2753</a>. [<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2773">#2773</a>]</li>
<li>[CRuby] Address compiler warnings about <code>void*</code> casting and old-style C function definitions.</li>
</ul>
<h2>1.14.0 / 2023-01-12</h2>
<h3>Notable Changes</h3>
<h4>Ruby</h4>
<p>This release introduces native gem support for Ruby 3.2. (Also see &quot;Technical note&quot; under &quot;Changed&quot; below.)</p>
<p>This release ends support for:</p>
<ul>
<li>Ruby 2.6, for which <a href="https://www.ruby-lang.org/en/downloads/branches/">upstream support ended 2022-04-12</a>.</li>
<li>JRuby 9.3, which is not fully compatible with Ruby 2.7+</li>
</ul>
<h4>Faster, more reliable installation: Native Gem for <code>aarch64-linux</code> (aka <code>linux/arm64/v8</code>)</h4>
<p>This version of Nokogiri ships <em>official</em> native gem support for the <code>aarch64-linux</code> platform, which should support AWS Graviton and other ARM64 Linux platforms. Please note that glibc &gt;= 2.29 is required for aarch64-linux systems, see <a href="https://nokogiri.org/#supported-platforms">Supported Platforms</a> for more information.</p>
<h4>Faster, more reliable installation: Native Gem for <code>arm-linux</code> (aka <code>linux/arm/v7</code>)</h4>
<p>This version of Nokogiri ships <em>experimental</em> native gem support for the <code>arm-linux</code> platform. Please note that glibc &gt;= 2.29 is required for arm-linux systems, see <a href="https://nokogiri.org/#supported-platforms">Supported Platforms</a> for more information.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/e8d2f4a829c50e6ad4ccd1625cd094e3a24acf36"><code>e8d2f4a</code></a> version bump to v1.14.3</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/59fbc7b6d5cecad921cc24daa34d69bbda8713fb"><code>59fbc7b</code></a> doc: update CHANGELOG for v1.14.3</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/347eacbeeacd2be0140faede75395bd1ed01073f"><code>347eacb</code></a> Merge pull request <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2852">#2852</a> from sparklemotion/flavorjones-libxml2-2.10.4-backport</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/36b0b3355d6d0d45bfdf1b55012bccfb348a6b4f"><code>36b0b33</code></a> dep: update libxml2 to 2.10.4 from 2.10.3</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/ac83e6ee7011ce9fec24399c759a73fb924a0de6"><code>ac83e6e</code></a> test: update behavior of namespaces in HTML4</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/2cf4996c5280f93e1ea66b2aceeed848d57fbe01"><code>2cf4996</code></a> test: make default GC behavior &quot;normal&quot;</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/1580121eeae3c1f266c4012d22d61314aa3202b7"><code>1580121</code></a> version bump to v1.14.2</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/530947753e3074d551217ea6bce7b4bbbc1234a9"><code>5309477</code></a> Merge pull request <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2791">#2791</a> from sparklemotion/2784-encoding-empty-strings-v1.14.x</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/975ae491c4993ff47e36262dc8e305fa2d651bf4"><code>975ae49</code></a> doc: update CHANGELOG</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/f13cdb46406c9b119a368cf506d831865dd95163"><code>f13cdb4</code></a> fix: empty node set serialization when document encoding is nil</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.13.6...v1.14.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.13.6&new-version=1.14.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 06:09:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    Bump commonmarker from 0.23.6 to 0.23.9 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [commonmarker](https://github.com/gjtorikian/commonmarker) from 0.23.6 to 0.23.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gjtorikian/commonmarker/releases">commonmarker's releases</a>.</em></p>
<blockquote>
<h2>v0.23.9</h2>
<h2>What's Changed</h2>
<ul>
<li>Update to 0.29.0.gfm.11 by <a href="https://github.com/anticomputer"><code>@​anticomputer</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/236">gjtorikian/commonmarker#236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.8...v0.23.9">https://github.com/gjtorikian/commonmarker/compare/v0.23.8...v0.23.9</a></p>
<h2>v0.23.8</h2>
<h2>What's Changed</h2>
<ul>
<li>Update cmark-upstream to <code>0.29.0.gfm.9</code> by <a href="https://github.com/smockle"><code>@​smockle</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/227">gjtorikian/commonmarker#227</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/smockle"><code>@​smockle</code></a> made their first contribution in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/227">gjtorikian/commonmarker#227</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.7...v0.23.8">https://github.com/gjtorikian/commonmarker/compare/v0.23.7...v0.23.8</a></p>
<h2>v0.23.7</h2>
<h2>What's Changed</h2>
<ul>
<li>C API stable test by <a href="https://github.com/gjtorikian"><code>@​gjtorikian</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/201">gjtorikian/commonmarker#201</a></li>
<li>Update to 29.0.gfm.7 by <a href="https://github.com/anticomputer"><code>@​anticomputer</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/224">gjtorikian/commonmarker#224</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7">https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7</a></p>
<h2>v0.23.7.pre1</h2>
<h2>What's Changed</h2>
<ul>
<li>C API stable test by <a href="https://github.com/gjtorikian"><code>@​gjtorikian</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/201">gjtorikian/commonmarker#201</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7.pre1">https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7.pre1</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/gjtorikian/commonmarker/blob/main/CHANGELOG.md">commonmarker's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v1.0.0.pre9">v1.0.0.pre9</a> (2023-03-28)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v1.0.0.pre8...v1.0.0.pre9">Full Changelog</a></p>
<p><strong>Merged pull requests:</strong></p>
<ul>
<li>Updates from upstream <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/235">#235</a> (<a href="https://github.com/gjtorikian">gjtorikian</a>)</li>
<li>Bump comrak from 0.16.0 to 0.17.1 <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/234">#234</a> (<a href="https://github.com/apps/dependabot">dependabot[bot]</a>)</li>
<li>Bump magnus from 0.5.1 to 0.5.2 <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/233">#233</a> (<a href="https://github.com/apps/dependabot">dependabot[bot]</a>)</li>
<li>Add ability to load <code>tmtheme</code>s from a folder <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/232">#232</a> (<a href="https://github.com/gjtorikian">gjtorikian</a>)</li>
<li>Bump magnus from 0.5.0 to 0.5.1 <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/231">#231</a> (<a href="https://github.com/apps/dependabot">dependabot[bot]</a>)</li>
<li>Bump magnus from 0.4.4 to 0.5.0 <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/230">#230</a> (<a href="https://github.com/apps/dependabot">dependabot[bot]</a>)</li>
<li>Test the new integrated rb-sys <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/228">#228</a> (<a href="https://github.com/gjtorikian">gjtorikian</a>)</li>
</ul>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v1.0.0.pre8">v1.0.0.pre8</a> (2023-03-09)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.8...v1.0.0.pre8">Full Changelog</a></p>
<p><strong>Closed issues:</strong></p>
<ul>
<li>Something changed in how header anchors are named in the output HTML <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/229">#229</a></li>
<li>Problem with CommonMarker on an Azure VM <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/226">#226</a></li>
</ul>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v0.23.8">v0.23.8</a> (2023-01-31)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v1.0.0.pre7...v0.23.8">Full Changelog</a></p>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v1.0.0.pre7">v1.0.0.pre7</a> (2023-01-26)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.7...v1.0.0.pre7">Full Changelog</a></p>
<p><strong>Merged pull requests:</strong></p>
<ul>
<li>Bump comrak from 0.15.0 to 0.16.0 <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/225">#225</a> (<a href="https://github.com/apps/dependabot">dependabot[bot]</a>)</li>
<li>Change <code>unsafe_</code> to <code>unsafe</code> <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/220">#220</a> (<a href="https://github.com/gjtorikian">gjtorikian</a>)</li>
<li>Clarify syntax highlighter plugin usage in README <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/218">#218</a> (<a href="https://github.com/DannyBen">DannyBen</a>)</li>
<li>Fix a couple of misleading README points <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/215">#215</a> (<a href="https://github.com/DannyBen">DannyBen</a>)</li>
<li>remove gemspec <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/214">#214</a> (<a href="https://github.com/gjtorikian">gjtorikian</a>)</li>
<li>Add shortcodes/emoji <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/210">#210</a> (<a href="https://github.com/gjtorikian">gjtorikian</a>)</li>
</ul>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v0.23.7">v0.23.7</a> (2023-01-24)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v1.0.0.pre6...v0.23.7">Full Changelog</a></p>
<p><strong>Closed issues:</strong></p>
<ul>
<li>Ruby 3.1 required? <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/222">#222</a></li>
<li>README #extensions link has broken <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/221">#221</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/42cfc90251353f9fceda91b884d0ded8d3da0bcf"><code>42cfc90</code></a> Merge pull request <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/236">#236</a> from anticomputer/update-to-0.29.0.gfm.10</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/d793fbf45106f17c1eb721293bcc8d098bd999dc"><code>d793fbf</code></a> Update cmark-upstream to <a href="https://github.com/github/cmark-gfm/commit/1e230827a">https://github.com/github/cmark-gfm/commit/1e230827a</a>...</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/4e4588f2e0d34a21eeb79ec53459d248fdf56b39"><code>4e4588f</code></a> Update Makefile for export header consolidation</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/2eb8ca8f2f4463448806663d72218cdcc0a9f38c"><code>2eb8ca8</code></a> Update cmark-upstream to <a href="https://github.com/github/cmark-gfm/commit/c8dcdc71c">https://github.com/github/cmark-gfm/commit/c8dcdc71c</a>...</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/bbb49db7223d71ad9366309c358c7c09a4e1c5a8"><code>bbb49db</code></a> HtmlRenderer: don't nest &lt;strong&gt;</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/f303e6bae7d83c76f3a929fa9e59ae2e3ac27081"><code>f303e6b</code></a> :gem: release 0.23.9</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/d6fe4c8be4febe86f68c68884b08d21a66a2aff4"><code>d6fe4c8</code></a> Update cmark-upstream to <a href="https://github.com/github/cmark-gfm/commit/dcf6b3862">https://github.com/github/cmark-gfm/commit/dcf6b3862</a>...</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/94c0af96f0bea7dad5a2f2e906cdc5ca457e025b"><code>94c0af9</code></a> Merge pull request <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/227">#227</a> from gjtorikian/update-to-0.29.0.gfm.9</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/5249f70a97f426d487bbead52f7d0ce03ab658af"><code>5249f70</code></a> :gem: release 0.23.8</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/85c205798f7e7078a2abfdb9c1723616facffabf"><code>85c2057</code></a> Added aria-label changes to test-footnotes.rb</li>
<li>Additional commits viewable in <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=commonmarker&package-manager=bundler&previous-version=0.23.6&new-version=0.23.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 05:27:31 +0000 UTC
    </div>
</div>

