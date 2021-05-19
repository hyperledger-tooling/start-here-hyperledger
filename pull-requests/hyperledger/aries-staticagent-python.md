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
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Bump nokogiri from 1.11.1 to 1.11.4 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.11.1 to 1.11.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>1.11.4 / 2021-05-14</h2>
<h3>Security</h3>
<p>[CRuby] Vendored libxml2 upgraded to v2.9.12 which addresses:</p>
<ul>
<li><a href="https://security.archlinux.org/CVE-2019-20388">CVE-2019-20388</a></li>
<li><a href="https://security.archlinux.org/CVE-2020-24977">CVE-2020-24977</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3517">CVE-2021-3517</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3518">CVE-2021-3518</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3537">CVE-2021-3537</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3541">CVE-2021-3541</a></li>
</ul>
<p>Note that two additional CVEs were addressed upstream but are not relevant to this release. <a href="https://security.archlinux.org/CVE-2021-3516">CVE-2021-3516</a> via <code>xmllint</code> is not present in Nokogiri, and <a href="https://security.archlinux.org/CVE-2020-7595">CVE-2020-7595</a> has been patched in Nokogiri since v1.10.8 (see <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1992">#1992</a>).</p>
<p>Please see <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-7rrm-v45f-jp64">nokogiri/GHSA-7rrm-v45f-jp64 </a> or <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2233">#2233</a> for a more complete analysis of these CVEs and patches.</p>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] vendored libxml2 is updated from 2.9.10 to 2.9.12. (Note that 2.9.11 was skipped because it was superseded by 2.9.12 a few hours after its release.)</li>
</ul>
<h2>1.11.3 / 2021-04-07</h2>
<h3>Fixed</h3>
<ul>
<li>[CRuby] Passing non-<code>Node</code> objects to <code>Document#root=</code> now raises an <code>ArgumentError</code> exception. Previously this likely segfaulted. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1900">#1900</a>]</li>
<li>[JRuby] Passing non-<code>Node</code> objects to <code>Document#root=</code> now raises an <code>ArgumentError</code> exception. Previously this raised a <code>TypeError</code> exception.</li>
<li>[CRuby] arm64/aarch64 systems (like Apple's M1) can now compile libxml2 and libxslt from source (though we continue to strongly advise users to install the native gems for the best possible experience)</li>
</ul>
<h2>1.11.2 / 2021-03-11</h2>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>NodeSet</code> may now safely contain <code>Node</code> objects from multiple documents. Previously the GC lifecycle of the parent <code>Document</code> objects could lead to nodes being GCed while still in scope. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1952#issuecomment-770856928">#1952</a>]</li>
<li>[CRuby] Patch libxml2 to avoid &quot;huge input lookup&quot; errors on large CDATA elements. (See upstream <a href="https://gitlab.gnome.org/GNOME/libxml2/-/issues/200">GNOME/libxml2#200</a> and <a href="https://gitlab.gnome.org/GNOME/libxml2/-/merge_requests/100">GNOME/libxml2!100</a>.) [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2132">#2132</a>].</li>
<li>[CRuby+Windows] Enable Nokogumbo (and other downstream gems) to compile and link against <code>nokogiri.so</code> by including <code>LDFLAGS</code> in <code>Nokogiri::VERSION_INFO</code>. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2167">#2167</a>]</li>
<li>[CRuby] <code>{XML,HTML}::Document.parse</code> now invokes <code>#initialize</code> exactly once. Previously <code>#initialize</code> was invoked twice on each object.</li>
<li>[JRuby] <code>{XML,HTML}::Document.parse</code> now invokes <code>#initialize</code> exactly once. Previously <code>#initialize</code> was not called, which was a problem for subclassing such as done by <code>Loofah</code>.</li>
</ul>
<h3>Improved</h3>
<ul>
<li>Reduce the number of object allocations needed when parsing an HTML::DocumentFragment. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2087">#2087</a>] (Thanks, <a href="https://github.com/ashmaroli"><code>@​ashmaroli</code></a>!)</li>
<li>[JRuby] Update the algorithm used to calculate <code>Node#line</code> to be wrong less-often. The underlying parser, Xerces, does not track line numbers, and so we've always used a hacky solution for this method. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1223">#1223</a>, <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2177">#2177</a>]</li>
<li>Introduce <code>--enable-system-libraries</code> and <code>--disable-system-libraries</code> flags to <code>extconf.rb</code>. These flags provide the same functionality as <code>--use-system-libraries</code> and the <code>NOKOGIRI_USE_SYSTEM_LIBRARIES</code> environment variable, but are more idiomatic. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2193">#2193</a>] (Thanks, <a href="https://github.com/eregon"><code>@​eregon</code></a>!)</li>
<li>[TruffleRuby] <code>--disable-static</code> is now the default on TruffleRuby when the packaged libraries are used. This is more flexible and compiles faster. (Note, though, that the default on TR is still to use system libraries.) [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2191#issuecomment-780724627">#2191</a>, <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2193">#2193</a>] (Thanks, <a href="https://github.com/eregon"><code>@​eregon</code></a>!)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>1.11.4 / 2021-05-14</h2>
<h3>Security</h3>
<p>[CRuby] Vendored libxml2 upgraded to v2.9.12 which addresses:</p>
<ul>
<li><a href="https://security.archlinux.org/CVE-2019-20388">CVE-2019-20388</a></li>
<li><a href="https://security.archlinux.org/CVE-2020-24977">CVE-2020-24977</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3517">CVE-2021-3517</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3518">CVE-2021-3518</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3537">CVE-2021-3537</a></li>
<li><a href="https://security.archlinux.org/CVE-2021-3541">CVE-2021-3541</a></li>
</ul>
<p>Note that two additional CVEs were addressed upstream but are not relevant to this release. <a href="https://security.archlinux.org/CVE-2021-3516">CVE-2021-3516</a> via <code>xmllint</code> is not present in Nokogiri, and <a href="https://security.archlinux.org/CVE-2020-7595">CVE-2020-7595</a> has been patched in Nokogiri since v1.10.8 (see <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1992">#1992</a>).</p>
<p>Please see <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-7rrm-v45f-jp64">nokogiri/GHSA-7rrm-v45f-jp64 </a> or <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2233">#2233</a> for a more complete analysis of these CVEs and patches.</p>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] vendored libxml2 is updated from 2.9.10 to 2.9.12. (Note that 2.9.11 was skipped because it was superseded by 2.9.12 a few hours after its release.)</li>
</ul>
<h2>1.11.3 / 2021-04-07</h2>
<h3>Fixed</h3>
<ul>
<li>[CRuby] Passing non-<code>Node</code> objects to <code>Document#root=</code> now raises an <code>ArgumentError</code> exception. Previously this likely segfaulted. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1900">#1900</a>]</li>
<li>[JRuby] Passing non-<code>Node</code> objects to <code>Document#root=</code> now raises an <code>ArgumentError</code> exception. Previously this raised a <code>TypeError</code> exception.</li>
<li>[CRuby] arm64/aarch64 systems (like Apple's M1) can now compile libxml2 and libxslt from source (though we continue to strongly advise users to install the native gems for the best possible experience)</li>
</ul>
<h2>1.11.2 / 2021-03-11</h2>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>NodeSet</code> may now safely contain <code>Node</code> objects from multiple documents. Previously the GC lifecycle of the parent <code>Document</code> objects could lead to nodes being GCed while still in scope. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1952#issuecomment-770856928">#1952</a>]</li>
<li>[CRuby] Patch libxml2 to avoid &quot;huge input lookup&quot; errors on large CDATA elements. (See upstream <a href="https://gitlab.gnome.org/GNOME/libxml2/-/issues/200">GNOME/libxml2#200</a> and <a href="https://gitlab.gnome.org/GNOME/libxml2/-/merge_requests/100">GNOME/libxml2!100</a>.) [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2132">#2132</a>].</li>
<li>[CRuby+Windows] Enable Nokogumbo (and other downstream gems) to compile and link against <code>nokogiri.so</code> by including <code>LDFLAGS</code> in <code>Nokogiri::VERSION_INFO</code>. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2167">#2167</a>]</li>
<li>[CRuby] <code>{XML,HTML}::Document.parse</code> now invokes <code>#initialize</code> exactly once. Previously <code>#initialize</code> was invoked twice on each object.</li>
<li>[JRuby] <code>{XML,HTML}::Document.parse</code> now invokes <code>#initialize</code> exactly once. Previously <code>#initialize</code> was not called, which was a problem for subclassing such as done by <code>Loofah</code>.</li>
</ul>
<h3>Improved</h3>
<ul>
<li>Reduce the number of object allocations needed when parsing an <code>HTML::DocumentFragment</code>. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2087">#2087</a>] (Thanks, <a href="https://github.com/ashmaroli"><code>@​ashmaroli</code></a>!)</li>
<li>[JRuby] Update the algorithm used to calculate <code>Node#line</code> to be wrong less-often. The underlying parser, Xerces, does not track line numbers, and so we've always used a hacky solution for this method. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/1223">#1223</a>, <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2177">#2177</a>]</li>
<li>Introduce <code>--enable-system-libraries</code> and <code>--disable-system-libraries</code> flags to <code>extconf.rb</code>. These flags provide the same functionality as <code>--use-system-libraries</code> and the <code>NOKOGIRI_USE_SYSTEM_LIBRARIES</code> environment variable, but are more idiomatic. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2193">#2193</a>] (Thanks, <a href="https://github.com/eregon"><code>@​eregon</code></a>!)</li>
<li>[TruffleRuby] <code>--disable-static</code> is now the default on TruffleRuby when the packaged libraries are used. This is more flexible and compiles faster. (Note, though, that the default on TR is still to use system libraries.) [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2191#issuecomment-780724627">#2191</a>, <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2193">#2193</a>] (Thanks, <a href="https://github.com/eregon"><code>@​eregon</code></a>!)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/9d69b44ed3357b8069856083d39ee418cd10109b"><code>9d69b44</code></a> version bump to v1.11.4</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/058e87fdfda2cc2f309df098d18fe8856e785fcc"><code>058e87f</code></a> update CHANGELOG with complete CVE information</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/92852514a0d4621961deb6ce249441ff5140358f"><code>9285251</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2234">#2234</a> from sparklemotion/2233-upgrade-to-libxml-2-9-12</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/5436f6120f883e9f185d48b992f39118a4897760"><code>5436f61</code></a> update CHANGELOG</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/761d320af2872c61b91f7b147cf57481566e3c67"><code>761d320</code></a> patch: renumber libxml2 patches</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/889ee2a9cb1e190bfa664cbf3552585f4d0a09a7"><code>889ee2a</code></a> test: update behavior of namespaces in HTML</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/9751d852c005606447dac7bb17f1a56593014583"><code>9751d85</code></a> test: remove low-value HTML::SAX::PushParser encoding test</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/9fcb7d25eabfab5e701d882e72ecab3b2ea6b13c"><code>9fcb7d2</code></a> test: adjust xpath gc test to libxml2's max recursion depth</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/1c99019f5f1bee23e4bff6cf72871f470097f7b2"><code>1c99019</code></a> patch: backport libxslt configure.ac change for libxml2 config</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/82a253fe7c5bdfab5fbe4c1b0c536b5ce4c72ac3"><code>82a253f</code></a> patch: fix isnan/isinf patch to apply cleanly to libxml 2.9.12</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.11.1...v1.11.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.11.1&new-version=1.11.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-19 17:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Add files required by repolint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-15 00:25:12 +0000 UTC
    </div>
</div>

