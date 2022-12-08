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
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump nokogiri from 1.13.8 to 1.13.10 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.13.8 to 1.13.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>1.13.10 / 2022-12-07</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Address CVE-2022-23476, unchecked return value from <code>xmlTextReaderExpand</code>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-qv4q-mr5r-qprj">GHSA-qv4q-mr5r-qprj</a> for more information.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>[CRuby] <code>XML::Reader#attribute_hash</code> now returns <code>nil</code> on parse errors. This restores the behavior of <code>#attributes</code> from v1.13.7 and earlier. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2715">#2715</a>]</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre><code>777ce2e80f64772e91459b943e531dfef387e768f2255f9bc7a1655f254bbaa1  nokogiri-1.13.10-aarch64-linux.gem
b432ff47c51386e07f7e275374fe031c1349e37eaef2216759063bc5fa5624aa  nokogiri-1.13.10-arm64-darwin.gem
73ac581ddcb680a912e92da928ffdbac7b36afd3368418f2cee861b96e8c830b  nokogiri-1.13.10-java.gem
916aa17e624611dddbf2976ecce1b4a80633c6378f8465cff0efab022ebc2900  nokogiri-1.13.10-x64-mingw-ucrt.gem
0f85a1ad8c2b02c166a6637237133505b71a05f1bb41b91447005449769bced0  nokogiri-1.13.10-x64-mingw32.gem
91fa3a8724a1ce20fccbd718dafd9acbde099258183ac486992a61b00bb17020  nokogiri-1.13.10-x86-linux.gem
d6663f5900ccd8f72d43660d7f082565b7ffcaade0b9a59a74b3ef8791034168  nokogiri-1.13.10-x86-mingw32.gem
81755fc4b8130ef9678c76a2e5af3db7a0a6664b3cba7d9fe8ef75e7d979e91b  nokogiri-1.13.10-x86_64-darwin.gem
51d5246705dedad0a09b374d09cc193e7383a5dd32136a690a3cd56e95adf0a3  nokogiri-1.13.10-x86_64-linux.gem
d3ee00f26c151763da1691c7fc6871ddd03e532f74f85101f5acedc2d099e958  nokogiri-1.13.10.gem
</code></pre>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/v1.13.10/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>1.13.10 / 2022-12-07</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Address CVE-2022-23476, unchecked return value from <code>xmlTextReaderExpand</code>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-qv4q-mr5r-qprj">GHSA-qv4q-mr5r-qprj</a> for more information.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>[CRuby] <code>XML::Reader#attribute_hash</code> now returns <code>nil</code> on parse errors. This restores the behavior of <code>#attributes</code> from v1.13.7 and earlier. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2715">#2715</a>]</li>
</ul>
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
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/4c80121dc309e67fa3d9f66a00516bad39b42c31"><code>4c80121</code></a> version bump to v1.13.10</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/85410e38410f670cbbc8c5b00d07b843caee88ce"><code>85410e3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2715">#2715</a> from sparklemotion/flavorjones-fix-reader-error-hand...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/9fe0761c47c0d4270d1a5220cfd25de080350d50"><code>9fe0761</code></a> fix(cruby): XML::Reader#attribute_hash returns nil on error</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/3b9c736bee91f95514da309eef28b06c0c29ce3a"><code>3b9c736</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2717">#2717</a> from sparklemotion/flavorjones-lock-psych-to-fix-bui...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/2efa87b49a26d1e961c2a0c143ecf28a67033677"><code>2efa87b</code></a> test: skip large cdata test on system libxml2</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/3187d6739c90864a7bb59cf8276facb1a47ca85d"><code>3187d67</code></a> dep(dev): pin psych to v4 until v5 builds in CI</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/a16b4bf14cec72e1a396c28a85135cd9abb08d9b"><code>a16b4bf</code></a> style(rubocop): disable Minitest/EmptyLineBeforeAssertionMethods</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/897759cc25b57ebf2754897e910c86931dec7d39"><code>897759c</code></a> version bump to v1.13.9</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/aeb1ac32830a34369a46625613f21ee17e3e445e"><code>aeb1ac3</code></a> doc: update CHANGELOG</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/c663e4905a35edd23f7cc05a80126b4e446e4fd2"><code>c663e49</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2671">#2671</a> from sparklemotion/flavorjones-update-zlib-1.2.13_v1...</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.13.8...v1.13.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.13.8&new-version=1.13.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-08 03:17:40 +0000 UTC
    </div>
</div>

