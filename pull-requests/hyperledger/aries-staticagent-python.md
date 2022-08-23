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
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    ci: simplify workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 18:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    fix: optional parameters and seed as str or bytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 17:38:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Use async-selective-queue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor to use async-selective-queue library for the base queue implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 21:09:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump nokogiri from 1.12.5 to 1.13.8 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.12.5 to 1.13.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
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
<hr />
<p>sha256 checksums:</p>
<pre><code>d6b2c45a57738f12fe27783939fe1394e7049246288c7770d3b1fee7f49432a6  nokogiri-1.13.8-aarch64-linux.gem
00217e48a6995e81dd83014325c0ea0b015023a8922c7bdb2ef1416aa87c1f43  nokogiri-1.13.8-arm64-darwin.gem
9d04c616900e2b5118e501436ebb9bc48520d08f3695d012a314006e28082f72  nokogiri-1.13.8-java.gem
98f7dac7583f07a84ec3fcc01dc03a66fce10f412cd363fce7de749acdb2a42d  nokogiri-1.13.8-x64-mingw-ucrt.gem
117a71b37f2e1d774a9f031d393e72d5d04b92af8036e0c1a8dd509c247b2013  nokogiri-1.13.8-x64-mingw32.gem
6d04342456edfb8fbc041d0c2cf5a59baaa7aacdda414b2333100b02f85d441d  nokogiri-1.13.8-x86-linux.gem
0529d558b4280a55bc7af500d3d4d590b7c059c814a0cea52e4e18cb30c25d15  nokogiri-1.13.8-x86-mingw32.gem
8966d79e687b271df87a4b240456597c43cd98584e3f783fc35de4f066486421  nokogiri-1.13.8-x86_64-darwin.gem
344f1bc66feac787e5b2053c6e9095d1f33605083e58ddf2b8d4eef257bccc5f  nokogiri-1.13.8-x86_64-linux.gem
79c279298b2f22fd4e760f49990c7930436bac1b1cfeff7bacff192f30edea3c  nokogiri-1.13.8.gem
</code></pre>
<h2>1.13.7 / 2022-07-12</h2>
<h3>Fixed</h3>
<p><code>XML::Node</code> objects, when compacted, update their internal struct's reference to the Ruby object wrapper. Previously, with GC compaction enabled, a segmentation fault was possible after compaction was triggered. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2578">#2578</a>] (Thanks, <a href="https://github.com/eightbitraptor"><code>@​eightbitraptor</code></a>!)</p>
<hr />
<p>sha256 checksums:</p>
<pre><code>16facd06367325b75bba1575ee87ee4c695e017ab7d447106ed2c00d6211db43  nokogiri-1.13.7-aarch64-linux.gem
69a1705a1f2be838bd0a778c1ff04ea58f847a41c3b5159de012617abba53f86  nokogiri-1.13.7-arm64-darwin.gem
6f26c7ed388406541ddc10cf7ea670cebe8f08a37e69be60503687374f835e1a  nokogiri-1.13.7-java.gem
3952cb78db8d107942ec7f3096d417f4d5d77bf44ae812c488bc49269d1dde6a  nokogiri-1.13.7-x64-mingw-ucrt.gem
e836c387eae9c6c93d4870db0d50e4d9505edd28100eef80c38a70d4481c09ed  nokogiri-1.13.7-x64-mingw32.gem
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
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
<h2>1.13.6 / 2022-05-08</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-29181">CVE-2022-29181</a>, improper handling of unexpected data types, related to untrusted inputs to the SAX parsers. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-xh29-r2w5-wx8m">GHSA-xh29-r2w5-wx8m</a> for more information.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li><code>{HTML4,XML}::SAX::{Parser,ParserContext}</code> constructor methods now raise <code>TypeError</code> instead of segfaulting when an incorrect type is passed.</li>
</ul>
<h2>1.13.5 / 2022-05-04</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-29824">CVE-2022-29824</a>. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-cgx6-hpwq-fhv5">GHSA-cgx6-hpwq-fhv5</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated from v2.9.13 to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.9.14">v2.9.14</a>.</li>
</ul>
<h3>Improvements</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/21b4ac5862dba11c89255e2f0a8082bf63eac53a"><code>21b4ac5</code></a> version bump to v1.13.8</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/d6c4a2b9d81db905a5119b5a5d5d753a935dfa2d"><code>d6c4a2b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2602">#2602</a> from sparklemotion/flavorjones-fix-reader-node-gc_ba...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/80e888c4034756d25c6388fcfa03c9606576dd85"><code>80e888c</code></a> deprecate: Reader#attribute_nodes</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/8d0c4eaa6038dd3553d5e7b32e96a13172a14c3d"><code>8d0c4ea</code></a> dev: introduce NOKO_WARN_DEPRECATION macro</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/12874a7a6b43db2f75be96d9cc77fe426d5ec433"><code>12874a7</code></a> feat: Reader#attribute_hash</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/193a07d3cb2c80ab5f5739d0761479aa4fa5e807"><code>193a07d</code></a> ci: add creek to the downstream pipeline</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/0c048067f5d5993e5617fc6c0e572dfc52d5b5a6"><code>0c04806</code></a> ci: import the downstream pipeline from main</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/3f4002af60b03e1486c5aef1b2b1cc2442aed83b"><code>3f4002a</code></a> ci: update vmactions/freebsd-vm job config</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/88b4730443e9b55d14128140b1b7882f436e5e0b"><code>88b4730</code></a> version bump to v1.13.7</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/25fb3c858a90c54bfc436ed2c3f84af2b28229e5"><code>25fb3c8</code></a> doc: update CHANGELOG</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.12.5...v1.13.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.12.5&new-version=1.13.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-08-22 18:49:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    test: msg not initially present on queue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 18:49:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    chore: update black
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 18:47:43 +0000 UTC
    </div>
</div>

