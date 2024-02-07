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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Bump nokogiri from 1.13.6 to 1.16.2 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.13.6 to 1.16.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>v1.16.2 / 2024-02-04</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address CVE-2024-25062. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-xc9x-jj77-9p9j">GHSA-xc9x-jj77-9p9j</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.12.5">v2.12.5</a> from v2.12.4. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre><code>69ba15d2a2498324489ed63850997f0b8f684260114ea81116d3082f16551d2d  nokogiri-1.16.2-aarch64-linux.gem
6a05ce42e3587a40cf8936ece0beaa5d32922254215d2e8cf9ad40588bb42e57  nokogiri-1.16.2-arm-linux.gem
c957226c8e36b31be6a3afb8602e2128282bf8b40ea51016c4cd21aa2608d3f8  nokogiri-1.16.2-arm64-darwin.gem
122652bfc338cd8a54a692ac035e245e41fd3b8283299202ca26e7a7d50db310  nokogiri-1.16.2-java.gem
7344b5072ca69fc5bedb61cb01a3b765b93a27aae5a2a845c2ba7200e4345074  nokogiri-1.16.2-x64-mingw-ucrt.gem
a2a5e184a424111a0d5b77947986484920ad708009c667f061e8d02035c562dd  nokogiri-1.16.2-x64-mingw32.gem
833efddeb51a6c2c9f6356295623c2b2e0d50050d468695c59bd929162953323  nokogiri-1.16.2-x86-linux.gem
e67fc0418dffaff9dc8b1dc65f0605282c3fee9488832d0223b620b4319e0b53  nokogiri-1.16.2-x86-mingw32.gem
5def799e5f139f21a79d7cf71172313a7b6fb0e4b2a31ab9bd5d4ad305994539  nokogiri-1.16.2-x86_64-darwin.gem
5b146240ac6ec6c40fd4367623e74442bca45a542bd3282b1d4d18b07b8e5dfe  nokogiri-1.16.2-x86_64-linux.gem
68922ee5cde27497d995c46f2821957bae961947644eed2822d173daf7567f9c  nokogiri-1.16.2.gem
</code></pre>
<h2>v1.16.1 / 2024-02-03</h2>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.12.4">v2.12.4</a> from v2.12.3. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>XML::Reader</code> defaults the encoding to UTF-8 if it's not specified in either the document or as a method parameter. Previously non-ASCII characters were serialized as NCRs in this case. <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2891">#2891</a> (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
<li>[CRuby] Restored support for compilation by GCC versions earlier than 4.6, which was broken in v1.15.0 (540e9aee). <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3090">#3090</a> (<a href="https://github.com/adfoster-r7"><code>@​adfoster-r7</code></a>)</li>
<li>[CRuby] Patched upstream libxml2 to allow parsing HTML5 in the context of a namespaced node (e.g., foreign content like MathML). [#3112, <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3116">#3116</a>] (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
<li>[CRuby] Fixed a small memory leak in libgumbo (HTML5 parser) when the maximum tree depth limit is hit. [#3098, <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3100">#3100</a>] (<a href="https://github.com/stevecheckoway"><code>@​stevecheckoway</code></a>)</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre><code>a541f35e5b9798a0c97300f9ee18f4217da2a2945a6d5499e4123b9018f9cafc  nokogiri-1.16.1-aarch64-linux.gem
6b82affd195000ab2f9c36cc08744ec2d2fcf6d8da88d59a2db67e83211f7c69  nokogiri-1.16.1-arm-linux.gem
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>v1.16.2 / 2024-02-04</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address CVE-2024-25062. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-xc9x-jj77-9p9j">GHSA-xc9x-jj77-9p9j</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.12.5">v2.12.5</a> from v2.12.4. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
</ul>
<h2>v1.16.1 / 2024-02-03</h2>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.12.4">v2.12.4</a> from v2.12.3. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>XML::Reader</code> defaults the encoding to UTF-8 if it's not specified in either the document or as a method parameter. Previously non-ASCII characters were serialized as NCRs in this case. <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/2891">#2891</a> (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
<li>[CRuby] Restored support for compilation by GCC versions earlier than 4.6, which was broken in v1.15.0 (540e9aee). <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3090">#3090</a> (<a href="https://github.com/adfoster-r7"><code>@​adfoster-r7</code></a>)</li>
<li>[CRuby] Patched upstream libxml2 to allow parsing HTML5 in the context of a namespaced node (e.g., foreign content like MathML). [#3112, <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3116">#3116</a>] (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
<li>[CRuby] Fixed a small memory leak in libgumbo (HTML5 parser) when the maximum tree depth limit is hit. [#3098, <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3100">#3100</a>] (<a href="https://github.com/stevecheckoway"><code>@​stevecheckoway</code></a>)</li>
</ul>
<h2>v1.16.0 / 2023-12-27</h2>
<h3>Notable Changes</h3>
<h4>Ruby</h4>
<p>This release introduces native gem support for Ruby 3.3.</p>
<p>This release ends support for Ruby 2.7, for which <a href="https://www.ruby-lang.org/en/downloads/branches/">upstream support ended 2023-03-31</a>.</p>
<h4>Pattern matching</h4>
<p>This version marks <em>official support</em> for the pattern matching API in <code>XML::Attr</code>, <code>XML::Document</code>, <code>XML::DocumentFragment</code>, <code>XML::Namespace</code>, <code>XML::Node</code>, and <code>XML::NodeSet</code> (and their subclasses), originally introduced as an experimental feature in v1.14.0. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</p>
<p>Documentation on what can be matched:</p>
<ul>
<li><a href="https://nokogiri.org/rdoc/Nokogiri/XML/Attr.html?h=deconstruct#method-i-deconstruct_keys"><code>XML::Attr#deconstruct_keys</code></a></li>
<li><a href="https://nokogiri.org/rdoc/Nokogiri/XML/Document.html?h=deconstruct#method-i-deconstruct_keys"><code>XML::Document#deconstruct_keys</code></a></li>
<li><a href="https://nokogiri.org/rdoc/Nokogiri/XML/Namespace.html?h=deconstruct+namespace#method-i-deconstruct_keys"><code>XML::Namespace#deconstruct_keys</code></a></li>
<li><a href="https://nokogiri.org/rdoc/Nokogiri/XML/Node.html?h=deconstruct#method-i-deconstruct_keys"><code>XML::Node#deconstruct_keys</code></a></li>
<li><a href="https://nokogiri.org/rdoc/Nokogiri/XML/DocumentFragment.html?h=deconstruct#method-i-deconstruct"><code>XML::DocumentFragment#deconstruct</code></a></li>
<li><a href="https://nokogiri.org/rdoc/Nokogiri/XML/NodeSet.html?h=deconstruct#method-i-deconstruct"><code>XML::NodeSet#deconstruct</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/673756fdd69d1036874b7d7250cc38a51fd4d7b8"><code>673756f</code></a> version bump to v1.16.2</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/74ffd67a8efb9972657e5c4625fd8419bbccbe06"><code>74ffd67</code></a> dep: update libxml to 2.12.5 (branch v1.16.x) (<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3122">#3122</a>)</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/0d4018dc7009580659c101fc41efb3babcfec229"><code>0d4018d</code></a> dep: update libxml2 to v2.12.5</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/f33a25f4378df33912ebc6b4ebc0f9e8e80ddfa8"><code>f33a25f</code></a> dep: remove patch from <a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3112">#3112</a> which has been released upstream</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/e99416896a182bc520a7940bbe286ec33597ab2b"><code>e994168</code></a> version bump to v1.16.1</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/77ea2f228c20e79c848ca2906813ea5b5010281b"><code>77ea2f2</code></a> dev: add files to manifest ignore list</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/756f27c6b7a23294d84bdcca5e03a639d0dd7421"><code>756f27c</code></a> build(deps): bump actions/{download,upload}-artifact from 3 to 4</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/464f8d41eb73ca9c6dae0b366afcf5f4e8bff342"><code>464f8d4</code></a> .gitignore: clangd-related files</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/2beeb960691df28dd5ebf828192c65b60250670f"><code>2beeb96</code></a> doc: update CHANGELOG</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/a26536d7a41fd40c52940e165bb5a4f6b4c39662"><code>a26536d</code></a> fix: apply upstream patch for in-context parsing (<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3116">#3116</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.13.6...v1.16.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.13.6&new-version=1.16.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 02:26:02 +0000 UTC
    </div>
</div>

