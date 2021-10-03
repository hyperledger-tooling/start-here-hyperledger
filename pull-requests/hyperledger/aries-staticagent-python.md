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
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    Update CONTRIBUTING.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 16:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/73" class=".btn">#73</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump nokogiri from 1.11.4 to 1.12.5 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.11.4 to 1.12.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>1.12.5 / 2021-09-27</h2>
<h3>Security</h3>
<p>[JRuby] Address CVE-2021-41098 (<a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-2rr5-8q37-2w7h">GHSA-2rr5-8q37-2w7h</a>).</p>
<p>In Nokogiri v1.12.4 and earlier, on JRuby only, the SAX parsers resolve external entities (XXE) by default. This fix turns off entity-resolution-by-default in the JRuby SAX parsers to match the CRuby SAX parsers' behavior.</p>
<p>CRuby users are not affected by this CVE.</p>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>Document#to_xhtml</code> properly serializes self-closing tags in libxml &gt; 2.9.10. A behavior change introduced in libxml 2.9.11 resulted in emitting start and and tags (e.g., <code>&lt;br&gt;&lt;/br&gt;</code>) instead of a self-closing tag (e.g., <code>&lt;br/&gt;</code>) in previous Nokogiri versions. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2324">#2324</a>]</li>
</ul>
<hr />
<p>SHA256 checksums:</p>
<pre><code>36bfa3a07aced069b3f3c9b39d9fb62cb0728d284d02b079404cd55780beaeff  nokogiri-1.12.5-arm64-darwin.gem
16b1a9ddbb70a9c998462912a5972097cbc79c3e01eb373906886ef8a469f589  nokogiri-1.12.5-java.gem
218dcc6edd1b49cc6244b5f88afb978739bb2f3f166c271557fe5f51e4bc713c  nokogiri-1.12.5-x64-mingw32.gem
e33bb919d64c16d931a5f26dc880969e587d225cfa97e6b56e790fb52179f527  nokogiri-1.12.5-x86-linux.gem
e13c2ed011b8346fbd589e96fe3542d763158bc2c7ad0f4f55f6d801afd1d9ff  nokogiri-1.12.5-x86-mingw32.gem
1ed64f7db7c1414b87fce28029f2a10128611d2037e0871ba298d00f9a00edd6  nokogiri-1.12.5-x86_64-darwin.gem
0868c8d0a147904d4dedaaa05af5f06656f2d3c67e4432601718559bf69d6cea  nokogiri-1.12.5-x86_64-linux.gem
2b20905942acc580697c8c496d0d1672ab617facb9d30d156b3c7676e67902ec  nokogiri-1.12.5.gem
</code></pre>
<h2>1.12.4 / 2021-08-29</h2>
<h3>Notable fix: Namespace inheritance</h3>
<p>Namespace behavior when reparenting nodes has historically been poorly specified and the behavior diverged between CRuby and JRuby. As a result, making this behavior consistent in v1.12.0 introduced a breaking change.</p>
<p>This patch release reverts the Builder behavior present in v1.12.0..v1.12.3 but keeps the Document behavior. This release also introduces a Document attribute to allow affected users to easily change this behavior for their legacy code without invasive changes.</p>
<h4>Compensating Feature in XML::Document</h4>
<p>This release of Nokogiri introduces a new <code>Document</code> boolean attribute, <code>namespace_inheritance</code>, which controls whether children should inherit a namespace when they are reparented. <code>Nokogiri::XML:Document</code> defaults this attribute to <code>false</code> meaning &quot;do not inherit,&quot; thereby making explicit the behavior change introduced in v1.12.0.</p>
<p>CRuby users who desire the pre-v1.12.0 behavior may set <code>document.namespace_inheritance = true</code> before reparenting nodes.</p>
<p>See <a href="https://nokogiri.org/rdoc/Nokogiri/XML/Document.html#namespace_inheritance-instance_method">https://nokogiri.org/rdoc/Nokogiri/XML/Document.html#namespace_inheritance-instance_method</a> for example usage.</p>
<h4>Fix for XML::Builder</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>1.12.5 / 2021-09-27</h2>
<h3>Security</h3>
<p>[JRuby] Address CVE-2021-41098 (<a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-2rr5-8q37-2w7h">GHSA-2rr5-8q37-2w7h</a>).</p>
<p>In Nokogiri v1.12.4 and earlier, on JRuby only, the SAX parsers resolve external entities (XXE) by default. This fix turns off entity-resolution-by-default in the JRuby SAX parsers to match the CRuby SAX parsers' behavior.</p>
<p>CRuby users are not affected by this CVE.</p>
<h3>Fixed</h3>
<ul>
<li>[CRuby] <code>Document#to_xhtml</code> properly serializes self-closing tags in libxml &gt; 2.9.10. A behavior change introduced in libxml 2.9.11 resulted in emitting start and and tags (e.g., <code>&lt;br&gt;&lt;/br&gt;</code>) instead of a self-closing tag (e.g., <code>&lt;br/&gt;</code>) in previous Nokogiri versions. [<a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2324">#2324</a>]</li>
</ul>
<h2>1.12.4 / 2021-08-29</h2>
<h3>Notable fix: Namespace inheritance</h3>
<p>Namespace behavior when reparenting nodes has historically been poorly specified and the behavior diverged between CRuby and JRuby. As a result, making this behavior consistent in v1.12.0 introduced a breaking change.</p>
<p>This patch release reverts the Builder behavior present in v1.12.0..v1.12.3 but keeps the Document behavior. This release also introduces a Document attribute to allow affected users to easily change this behavior for their legacy code without invasive changes.</p>
<h4>Compensating Feature in XML::Document</h4>
<p>This release of Nokogiri introduces a new <code>Document</code> boolean attribute, <code>namespace_inheritance</code>, which controls whether children should inherit a namespace when they are reparented. <code>Nokogiri::XML:Document</code> defaults this attribute to <code>false</code> meaning &quot;do not inherit,&quot; thereby making explicit the behavior change introduced in v1.12.0.</p>
<p>CRuby users who desire the pre-v1.12.0 behavior may set <code>document.namespace_inheritance = true</code> before reparenting nodes.</p>
<p>See <a href="https://nokogiri.org/rdoc/Nokogiri/XML/Document.html#namespace_inheritance-instance_method">https://nokogiri.org/rdoc/Nokogiri/XML/Document.html#namespace_inheritance-instance_method</a> for example usage.</p>
<h4>Fix for XML::Builder</h4>
<p>However, recognizing that we want <code>Builder</code>-created children to inherit namespaces, Builder now will set <code>namespace_inheritance=true</code> on the underlying document for both JRuby and CRuby. This means that, on CRuby, the pre-v1.12.0 behavior is restored.</p>
<p>Users who want to turn this behavior off may pass a keyword argument to the Builder constructor like so:</p>
<pre lang="ruby"><code>Nokogiri::XML::Builder.new(namespace_inheritance: false)
</code></pre>
<p>See <a href="https://nokogiri.org/rdoc/Nokogiri/XML/Builder.html#label-Namespace+inheritance">https://nokogiri.org/rdoc/Nokogiri/XML/Builder.html#label-Namespace+inheritance</a> for example usage.</p>
<h4>Downstream gem maintainers</h4>
<p>Note that any downstream gems may want to specifically omit Nokogiri v1.12.0--v1.12.3 from their dependency specification if they rely on child namespace inheritance:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/47f6a461fdc3e375b30522259e48569fb578dece"><code>47f6a46</code></a> version bump to v1.12.5</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/2a0ac88518fdd1509d14c4cbdb9784c73dd8a839"><code>2a0ac88</code></a> update CHANGELOG</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/6b6063782cefc42e527dc967c6119125cae0042d"><code>6b60637</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2329">#2329</a> from sparklemotion/flavorjones-GHSA-2rr5-8q37-2w7h_1...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/4bd943cae3039c51c3f54de9cd76abbfb647666b"><code>4bd943c</code></a> fix(jruby): SAX parser uses an entity resolver</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/f943ee4108b007d225e00c3ac7da00df17b81b1a"><code>f943ee4</code></a> refactor(jruby): handle errors more consistently</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/27901227488ea7e439777cfc907e52c68622e6a3"><code>2790122</code></a> format: test files</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/01e1618f7551ae3c32c1a5790c1004c18a46b316"><code>01e1618</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2327">#2327</a> from sparklemotion/2324-xhtml-self-closing-tags_v1.12.x</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/a0180c72c55c44b8e0db3a98040bd5f115742817"><code>a0180c7</code></a> fix: HTML4::Document.to_xhtml self-closing tags</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/564ac1787303332e0b2b92311ff6f1b30a893eae"><code>564ac17</code></a> release v1.12.4</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/4d5754baede4fc98cd4f12754f479bd228b6b55b"><code>4d5754b</code></a> backport <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2320">#2320</a></li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.11.4...v1.12.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.11.4&new-version=1.12.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-28 05:32:38 +0000 UTC
    </div>
</div>

