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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Addressed lint warnings in Blockattestation service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addressed protobuf lint wanring in Blockattestation proto file.


Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 10:57:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Publish generated API documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previous attempt failed with…

ssh: Could not resolve hostname publish-pages: Temporary failure in name resolution
Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 10:13:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Add comment to buf.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Linting rules should not be ingnored in new files

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 09:21:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    New service and messages for block attestation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New block attestation service for BFT block replication and verification feature. 

Issue: https://github.com/hyperledger/fabric/issues/3413

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 07:25:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Publish generated API documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previous attempt failed with…

fatal: could not read Password for 'https://***@github.com': No such device or address
Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 16:37:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/90" class=".btn">#90</a>
            </td>
            <td>
                <b>
                    Bump nokogiri from 1.13.3 to 1.13.6 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [nokogiri](https://github.com/sparklemotion/nokogiri) from 1.13.3 to 1.13.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>1.13.6 / 2022-05-08</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Address <a href="https://nvd.nist.gov/vuln/detail/CVE-2022-29181">CVE-2022-29181</a>, improper handling of unexpected data types, related to untrusted inputs to the SAX parsers. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-xh29-r2w5-wx8m">GHSA-xh29-r2w5-wx8m</a> for more information.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li><code>{HTML4,XML}::SAX::{Parser,ParserContext}</code> constructor methods now raise <code>TypeError</code> instead of segfaulting when an incorrect type is passed.</li>
</ul>
<hr />
<p>sha256:</p>
<pre><code>58417c7c10f78cd1c0e1984f81538300d4ea98962cfd3f46f725efee48f9757a  nokogiri-1.13.6-aarch64-linux.gem
a2b04ec3b1b73ecc6fac619b41e9fdc70808b7a653b96ec97d04b7a23f158dbc  nokogiri-1.13.6-arm64-darwin.gem
4437f2d03bc7da8854f4aaae89e24a98cf5c8b0212ae2bc003af7e65c7ee8e27  nokogiri-1.13.6-java.gem
99d3e212bbd5e80aa602a1f52d583e4f6e917ec594e6aa580f6aacc253eff984  nokogiri-1.13.6-x64-mingw-ucrt.gem
a04f6154a75b6ed4fe2d0d0ff3ac02f094b54e150b50330448f834fa5726fbba  nokogiri-1.13.6-x64-mingw32.gem
a13f30c2863ef9e5e11240dd6d69ef114229d471018b44f2ff60bab28327de4d  nokogiri-1.13.6-x86-linux.gem
63a2ca2f7a4f6bd9126e1695037f66c8eb72ed1e1740ef162b4480c57cc17dc6  nokogiri-1.13.6-x86-mingw32.gem
2b266e0eb18030763277b30dc3d64337f440191e2bd157027441ac56a59d9dfe  nokogiri-1.13.6-x86_64-darwin.gem
3fa37b0c3b5744af45f9da3e4ae9cbd89480b35e12ae36b5e87a0452e0b38335  nokogiri-1.13.6-x86_64-linux.gem
b1512fdc0aba446e1ee30de3e0671518eb363e75fab53486e99e8891d44b8587  nokogiri-1.13.6.gem
</code></pre>
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
<ul>
<li>[CRuby] The libxml2 HTML4 parser no longer exhibits quadratic behavior when recovering some broken markup related to start-of-tag and bare <code>&lt;</code> characters.</li>
</ul>
<h3>Changed</h3>
<ul>
<li>[CRuby] The libxml2 HTML4 parser in v2.9.14 recovers from some broken markup differently. Notably, the XML CDATA escape sequence <code>&lt;![CDATA[</code> and incorrectly-opened comments will result in HTML text nodes starting with <code>&amp;lt;!</code> instead of skipping the invalid tag. This behavior is a direct result of the <a href="https://gitlab.gnome.org/GNOME/libxml2/-/commit/798bdf1">quadratic-behavior fix</a> noted above. The behavior of downstream sanitizers relying on this behavior will also change. Some tests describing the changed behavior are in <a href="https://github.com/sparklemotion/nokogiri/blob/3ed5bf2b5a367cb9dc6e329c5a1c512e1dd4565d/test/html4/test_comments.rb#L187-L204"><code>test/html4/test_comments.rb</code></a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
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
<ul>
<li>[CRuby] The libxml2 HTML parser no longer exhibits quadratic behavior when recovering some broken markup related to start-of-tag and bare <code>&lt;</code> characters.</li>
</ul>
<h3>Changed</h3>
<ul>
<li>[CRuby] The libxml2 HTML parser in v2.9.14 recovers from some broken markup differently. Notably, the XML CDATA escape sequence <code>&lt;![CDATA[</code> and incorrectly-opened comments will result in HTML text nodes starting with <code>&amp;lt;!</code> instead of skipping the invalid tag. This behavior is a direct result of the <a href="https://gitlab.gnome.org/GNOME/libxml2/-/commit/798bdf1">quadratic-behavior fix</a> noted above. The behavior of downstream sanitizers relying on this behavior will also change. Some tests describing the changed behavior are in <a href="https://github.com/sparklemotion/nokogiri/blob/3ed5bf2b5a367cb9dc6e329c5a1c512e1dd4565d/test/html4/test_comments.rb#L187-L204"><code>test/html4/test_comments.rb</code></a>.</li>
</ul>
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
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/b7817b6a62ac210203a451d1a691a824288e9eab"><code>b7817b6</code></a> version bump to v1.13.6</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/61b1a395cd512af2e0595a8e369465415e574fe8"><code>61b1a39</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2530">#2530</a> from sparklemotion/flavorjones-check-parse-memory-ty...</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/83cc451c3f29df397caa890afc3b714eae6ab8f7"><code>83cc451</code></a> fix: {HTML4,XML}::SAX::{Parser,ParserContext} check arg types</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/22c9e5b300c27a377fdde37c17eb9d07dd7322d0"><code>22c9e5b</code></a> version bump to v1.13.5</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/615588192572f7cfcb43eabbb070a6e07bf9e731"><code>6155881</code></a> doc: update CHANGELOG for v1.13.5</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/c519a47ab11f5e8fce77328fcb01a7b3befc2b9e"><code>c519a47</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sparklemotion/nokogiri/issues/2527">#2527</a> from sparklemotion/2525-update-libxml-2_9_14-v1_13_x</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/66c2886e78f6801def83a549c3e6581ac48e61e8"><code>66c2886</code></a> dep: update libxml2 to v2.9.14</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/b7c4cc35de38fcfdde4da1203d79ae38bc4324bf"><code>b7c4cc3</code></a> test: unpend the LIBXML_LOADED_VERSION test on freebsd</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/eac793487183a5e72464e53cccd260971d5f29b5"><code>eac7934</code></a> dev: require yaml</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/f3521ba3d38922d76dd5ed59705eab3988213712"><code>f3521ba</code></a> style(rubocop): pend Style/FetchEnvVar for now</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.13.3...v1.13.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nokogiri&package-manager=bundler&previous-version=1.13.3&new-version=1.13.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-05-13 15:11:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    Fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 06:50:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    [WIP] Release Java bindings to Maven Central Repository
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
        Created At 2022-05-10 15:34:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    Fix Mavan publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix missing working directory in publish step

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 10:39:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    Publish Java bindings
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
        Created At 2022-05-10 10:13:41 +0000 UTC
    </div>
</div>

