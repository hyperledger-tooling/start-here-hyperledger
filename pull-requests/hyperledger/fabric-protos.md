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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    [WIP] Add new style binding generation for Go apiv1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 14:52:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    Bump nokogiri from 1.13.6 to 1.13.9 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.13.6 to 1.13.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>1.13.9 / 2022-10-18</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-2309">CVE-2022-2309</a>, <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-40304">CVE-2022-40304</a>, and <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-40303">CVE-2022-40303</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-2qc6-mcvw-92cw">GHSA-2qc6-mcvw-92cw</a> for more information.</li>
<li>[CRuby] Vendored zlib is updated to address <a href="https://ubuntu.com/security/CVE-2022-37434">CVE-2022-37434</a>. Nokogiri was not affected by this vulnerability, but this version of zlib was being flagged up by some vulnerability scanners, see <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2626">#2626</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.10.3">v2.10.3</a> from v2.9.14.</li>
<li>[CRuby] Vendored libxslt is updated to <a href="https://gitlab.gnome.org/GNOME/libxslt/-/releases/v1.1.37">v1.1.37</a> from v1.1.35.</li>
<li>[CRuby] Vendored zlib is updated from 1.2.12 to 1.2.13. (See <a href="https://github.com/sparklemotion/nokogiri/blob/v1.13.x/LICENSE-DEPENDENCIES.md#platform-releases">LICENSE-DEPENDENCIES.md</a> for details on which packages redistribute this library.)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>Nokogiri::XML::Namespace</code> objects, when compacted, update their internal struct's reference to the Ruby object wrapper. Previously, with GC compaction enabled, a segmentation fault was possible after compaction was triggered. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2658">#2658</a>] (Thanks, <a href="https://github.com/eightbitraptor"><code>@​eightbitraptor</code></a> and <a href="https://github.com/peterzhu2118"><code>@​peterzhu2118</code></a>!)</li>
<li>[CRuby] <code>Document#remove_namespaces!</code> now defers freeing the underlying <code>xmlNs</code> struct until the <code>Document</code> is GCed. Previously, maintaining a reference to a <code>Namespace</code> object that was removed in this way could lead to a segfault. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2658">#2658</a>]</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre><code>9b69829561d30c4461ea803baeaf3460e8b145cff7a26ce397119577a4083a02  nokogiri-1.13.9-aarch64-linux.gem
e76ebb4b7b2e02c72b2d1541289f8b0679fb5984867cf199d89b8ef485764956  nokogiri-1.13.9-arm64-darwin.gem
15bae7d08bddeaa898d8e3f558723300137c26a2dc2632a1f89c8574c4467165  nokogiri-1.13.9-java.gem
f6a1dbc7229184357f3129503530af73cc59ceba4932c700a458a561edbe04b9  nokogiri-1.13.9-x64-mingw-ucrt.gem
36d935d799baa4dc488024f71881ff0bc8b172cecdfc54781169c40ec02cbdb3  nokogiri-1.13.9-x64-mingw32.gem
ebaf82aa9a11b8fafb67873d19ee48efb565040f04c898cdce8ca0cd53ff1a12  nokogiri-1.13.9-x86-linux.gem
11789a2a11b28bc028ee111f23311461104d8c4468d5b901ab7536b282504154  nokogiri-1.13.9-x86-mingw32.gem
01830e1646803ff91c0fe94bc768ff40082c6de8cfa563dafd01b3f7d5f9d795  nokogiri-1.13.9-x86_64-darwin.gem
8e93b8adec22958013799c8690d81c2cdf8a90b6f6e8150ab22e11895844d781  nokogiri-1.13.9-x86_64-linux.gem
96f37c1baf0234d3ae54c2c89aef7220d4a8a1b03d2675ff7723565b0a095531  nokogiri-1.13.9.gem
</code></pre>
<h2>1.13.8 / 2022-07-23</h2>
<h3>Deprecated</h3>
<ul>
<li><code>XML::Reader#attribute_nodes</code> is deprecated due to incompatibility between libxml2's <code>xmlReader</code> memory semantics and Ruby's garbage collector. Although this method continues to exist for backwards compatibility, it is unsafe to call and may segfault. This method will be removed in a future version of Nokogiri, and callers should use <code>#attribute_hash</code> instead. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2598">#2598</a>]</li>
</ul>
<h3>Improvements</h3>
<ul>
<li><code>XML::Reader#attribute_hash</code> is a new method to safely retrieve the attributes of a node from <code>XML::Reader</code>. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2598">#2598</a>, <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2599">#2599</a>]</li>
</ul>
<h3>Fixed</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>1.13.9 / 2022-10-18</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-2309">CVE-2022-2309</a>, <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-40304">CVE-2022-40304</a>, and <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-40303">CVE-2022-40303</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-2qc6-mcvw-92cw">GHSA-2qc6-mcvw-92cw</a> for more information.</li>
<li>[CRuby] Vendored zlib is updated to address <a href="https://ubuntu.com/security/CVE-2022-37434">CVE-2022-37434</a>. Nokogiri was not affected by this vulnerability, but this version of zlib was being flagged up by some vulnerability scanners, see <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2626">#2626</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.10.3">v2.10.3</a> from v2.9.14.</li>
<li>[CRuby] Vendored libxslt is updated to <a href="https://gitlab.gnome.org/GNOME/libxslt/-/releases/v1.1.37">v1.1.37</a> from v1.1.35.</li>
<li>[CRuby] Vendored zlib is updated from 1.2.12 to 1.2.13. (See <a href="https://github.com/sparklemotion/nokogiri/blob/v1.13.x/LICENSE-DEPENDENCIES.md#platform-releases">LICENSE-DEPENDENCIES.md</a> for details on which packages redistribute this library.)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>Nokogiri::XML::Namespace</code> objects, when compacted, update their internal struct's reference to the Ruby object wrapper. Previously, with GC compaction enabled, a segmentation fault was possible after compaction was triggered. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2658">#2658</a>] (Thanks, <a href="https://github.com/eightbitraptor"><code>@​eightbitraptor</code></a> and <a href="https://github.com/peterzhu2118"><code>@​peterzhu2118</code></a>!)</li>
<li>[CRuby] <code>Document#remove_namespaces!</code> now defers freeing the underlying <code>xmlNs</code> struct until the <code>Document</code> is GCed. Previously, maintaining a reference to a <code>Namespace</code> object that was removed in this way could lead to a segfault. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2658">#2658</a>]</li>
</ul>
<h2>1.13.8 / 2022-07-23</h2>
<h3>Deprecated</h3>
<ul>
<li><code>XML::Reader#attribute_nodes</code> is deprecated due to incompatibility between libxml2's <code>xmlReader</code> memory semantics and Ruby's garbage collector. Although this method continues to exist for backwards compatibility, it is unsafe to call and may segfault. This method will be removed in a future version of Nokogiri, and callers should use <code>#attribute_hash</code> instead. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2598">#2598</a>]</li>
</ul>
<h3>Improvements</h3>
<ul>
<li><code>XML::Reader#attribute_hash</code> is a new method to safely retrieve the attributes of a node from <code>XML::Reader</code>. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2598">#2598</a>, <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2599">#2599</a>]</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[CRuby] Calling <code>XML::Reader#attributes</code> is now safe to call. In Nokogiri &lt;= 1.13.7 this method may segfault. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2598">#2598</a>, <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2599">#2599</a>]</li>
</ul>
<h2>1.13.7 / 2022-07-12</h2>
<h3>Fixed</h3>
<p><code>XML::Node</code> objects, when compacted, update their internal struct's reference to the Ruby object wrapper. Previously, with GC compaction enabled, a segmentation fault was possible after compaction was triggered. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2578">#2578</a>] (Thanks, <a href="https://github.com/eightbitraptor"><code>@​eightbitraptor</code></a>!)</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/897759cc25b57ebf2754897e910c86931dec7d39"><code>897759c</code></a> version bump to v1.13.9</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/aeb1ac32830a34369a46625613f21ee17e3e445e"><code>aeb1ac3</code></a> doc: update CHANGELOG</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/c663e4905a35edd23f7cc05a80126b4e446e4fd2"><code>c663e49</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2671">#2671</a> from sparklemotion/flavorjones-update-zlib-1.2.13_v1...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/212e07da28096db7d2cbda697bc2a38d71f6dc3a"><code>212e07d</code></a> ext: hack to cross-compile zlib v1.2.13 on darwin</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/76dbc8c5bef99467f3403297e29da4297fbddeb7"><code>76dbc8c</code></a> dep: update zlib to v1.2.13</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/24e3a9c41428195c66745fef8ce697101167bd08"><code>24e3a9c</code></a> doc: update CHANGELOG</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/4db3b4daa9ca8d1c1996cc9741c76ba2b8d1673b"><code>4db3b4d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2668">#2668</a> from sparklemotion/flavorjones-namespace-scopes-comp...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/73d73d6e433f17f39e188f5c03ec176b60719416"><code>73d73d6</code></a> fix: Document#remove_namespaces! use-after-free bug</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/5f58b34724a6e48c7c478cfda5fc9c4cac581e08"><code>5f58b34</code></a> fix: namespace nodes behave properly when compacted</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/b08a8586c7c34831be0f13f9147b84016d17d94b"><code>b08a858</code></a> test: repro namespace_scopes compaction issue</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.13.6...v1.13.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.13.6&new-version=1.13.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 03:31:56 +0000 UTC
    </div>
</div>

