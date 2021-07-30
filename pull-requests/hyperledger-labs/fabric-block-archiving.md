---
layout: default
title: fabric-block-archiving
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-block-archiving
---

# fabric-block-archiving <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-block-archiving){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-block-archiving/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.25.3 to 1.26.5 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.25.3 to 1.26.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.5</h2>
<p>:warning: <strong>IMPORTANT: urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>Fixed deprecation warnings emitted in Python 3.10.</li>
<li>Updated vendored <code>six</code> library to 1.16.0.</li>
<li>Improved performance of URL parser when splitting the authority component.</li>
</ul>
<p><strong>If you or your organization rely on urllib3 consider supporting us via <a href="https://github.com/sponsors/urllib3">GitHub Sponsors</a></strong></p>
<h2>1.26.4</h2>
<p>:warning: <strong>IMPORTANT: urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>Changed behavior of the default <code>SSLContext</code> when connecting to HTTPS proxy during HTTPS requests. The default <code>SSLContext</code> now sets <code>check_hostname=True</code>.</li>
</ul>
<p><strong>If you or your organization rely on urllib3 consider supporting us via <a href="https://github.com/sponsors/urllib3">GitHub Sponsors</a></strong></p>
<h2>1.26.3</h2>
<p>:warning: <strong>IMPORTANT: urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>
<p>Fixed bytes and string comparison issue with headers (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2141">#2141</a>)</p>
</li>
<li>
<p>Changed <code>ProxySchemeUnknown</code> error message to be more actionable if the user supplies a proxy URL without a scheme (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2107">#2107</a>)</p>
</li>
</ul>
<p><strong>If you or your organization rely on urllib3 consider supporting us via <a href="https://github.com/sponsors/urllib3">GitHub Sponsors</a></strong></p>
<h2>1.26.2</h2>
<p>:warning: <strong>IMPORTANT: urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>Fixed an issue where <code>wrap_socket</code> and <code>CERT_REQUIRED</code> wouldn't be imported properly on Python 2.7.8 and earlier (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2052">#2052</a>)</li>
</ul>
<h2>1.26.1</h2>
<p>:warning: <strong>IMPORTANT: urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>Fixed an issue where two <code>User-Agent</code> headers would be sent if a <code>User-Agent</code> header key is passed as <code>bytes</code> (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2047">#2047</a>)</li>
</ul>
<h2>1.26.0</h2>
<p>:warning: <strong>IMPORTANT: urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>
<p>Added support for HTTPS proxies contacting HTTPS servers (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/1923">#1923</a>, Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/1806">#1806</a>)</p>
</li>
<li>
<p>Deprecated negotiating TLSv1 and TLSv1.1 by default. Users that
still wish to use TLS earlier than 1.2 without a deprecation warning
should opt-in explicitly by setting <code>ssl_version=ssl.PROTOCOL_TLSv1_1</code> (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2002">#2002</a>)
<strong>Starting in urllib3 v2.0: Connections that receive a <code>DeprecationWarning</code> will fail</strong></p>
</li>
<li>
<p>Deprecated <code>Retry</code> options <code>Retry.DEFAULT_METHOD_WHITELIST</code>, <code>Retry.DEFAULT_REDIRECT_HEADERS_BLACKLIST</code>
and <code>Retry(method_whitelist=...)</code> in favor of <code>Retry.DEFAULT_ALLOWED_METHODS</code>,
<code>Retry.DEFAULT_REMOVE_HEADERS_ON_REDIRECT</code>, and <code>Retry(allowed_methods=...)</code>
(Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2000">#2000</a>) <strong>Starting in urllib3 v2.0: Deprecated options will be removed</strong></p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h2>1.26.5 (2021-05-26)</h2>
<ul>
<li>Fixed deprecation warnings emitted in Python 3.10.</li>
<li>Updated vendored <code>six</code> library to 1.16.0.</li>
<li>Improved performance of URL parser when splitting
the authority component.</li>
</ul>
<h2>1.26.4 (2021-03-15)</h2>
<ul>
<li>Changed behavior of the default <code>SSLContext</code> when connecting to HTTPS proxy
during HTTPS requests. The default <code>SSLContext</code> now sets <code>check_hostname=True</code>.</li>
</ul>
<h2>1.26.3 (2021-01-26)</h2>
<ul>
<li>
<p>Fixed bytes and string comparison issue with headers (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2141">#2141</a>)</p>
</li>
<li>
<p>Changed <code>ProxySchemeUnknown</code> error message to be
more actionable if the user supplies a proxy URL without
a scheme. (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2107">#2107</a>)</p>
</li>
</ul>
<h2>1.26.2 (2020-11-12)</h2>
<ul>
<li>Fixed an issue where <code>wrap_socket</code> and <code>CERT_REQUIRED</code> wouldn't
be imported properly on Python 2.7.8 and earlier (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2052">#2052</a>)</li>
</ul>
<h2>1.26.1 (2020-11-11)</h2>
<ul>
<li>Fixed an issue where two <code>User-Agent</code> headers would be sent if a
<code>User-Agent</code> header key is passed as <code>bytes</code> (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2047">#2047</a>)</li>
</ul>
<h2>1.26.0 (2020-11-10)</h2>
<ul>
<li>
<p><strong>NOTE: urllib3 v2.0 will drop support for Python 2</strong>.
<code>Read more in the v2.0 Roadmap &lt;https://urllib3.readthedocs.io/en/latest/v2-roadmap.html&gt;</code>_.</p>
</li>
<li>
<p>Added support for HTTPS proxies contacting HTTPS servers (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/1923">#1923</a>, Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/1806">#1806</a>)</p>
</li>
<li>
<p>Deprecated negotiating TLSv1 and TLSv1.1 by default. Users that
still wish to use TLS earlier than 1.2 without a deprecation warning</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/d1616473df94b94f0f5ad19d2a6608cfe93b7cdf"><code>d161647</code></a> Release 1.26.5</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2d4a3fee6de2fa45eb82169361918f759269b4ec"><code>2d4a3fe</code></a> Improve performance of sub-authority splitting in URL</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2698537d52f8ff1f0bbb1d45cf018b118e91f637"><code>2698537</code></a> Update vendored six to 1.16.0</li>
<li><a href="https://github.com/urllib3/urllib3/commit/07bed791e9c391d8bf12950f76537dc3c6f90550"><code>07bed79</code></a> Fix deprecation warnings for Python 3.10 ssl module</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d725a9b56bb8baf87c9e6eee0e9edf010034b63b"><code>d725a9b</code></a> Add Python 3.10 to GitHub Actions</li>
<li><a href="https://github.com/urllib3/urllib3/commit/339ad34c677c98fd9ad008de1d8bbeb9dbf34381"><code>339ad34</code></a> Use pytest==6.2.4 on Python 3.10+</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f271c9c3149e20d7feffb6429b135bbb6c09ddf4"><code>f271c9c</code></a> Apply latest Black formatting</li>
<li><a href="https://github.com/urllib3/urllib3/commit/1884878aac87ef0494b282e940c32c24ee917d52"><code>1884878</code></a> [1.26] Properly proxy EOF on the SSLTransport test suite</li>
<li><a href="https://github.com/urllib3/urllib3/commit/a8913042b676c510e94fc2b097f6b514ae11a537"><code>a891304</code></a> Release 1.26.4</li>
<li><a href="https://github.com/urllib3/urllib3/commit/8d65ea1ecf6e2cdc27d42124e587c1b83a3118b0"><code>8d65ea1</code></a> Merge pull request from GHSA-5phf-pp7p-vc2r</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/1.25.3...1.26.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.25.3&new-version=1.26.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-block-archiving/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 19:52:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-block-archiving/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Bump pygments from 2.4.2 to 2.7.4 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [pygments](https://github.com/pygments/pygments) from 2.4.2 to 2.7.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pygments/pygments/releases">pygments's releases</a>.</em></p>
<blockquote>
<h2>2.7.4</h2>
<ul>
<li>
<p>Updated lexers:</p>
<ul>
<li>
<p>Apache configurations: Improve handling of malformed tags (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1656">#1656</a>)</p>
</li>
<li>
<p>CSS: Add support for variables (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1633">#1633</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1666">#1666</a>)</p>
</li>
<li>
<p>Crystal (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1650">#1650</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1670">#1670</a>)</p>
</li>
<li>
<p>Coq (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1648">#1648</a>)</p>
</li>
<li>
<p>Fortran: Add missing keywords (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1635">#1635</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1665">#1665</a>)</p>
</li>
<li>
<p>Ini (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1624">#1624</a>)</p>
</li>
<li>
<p>JavaScript and variants (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1647">#1647</a> -- missing regex flags, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1651">#1651</a>)</p>
</li>
<li>
<p>Markdown (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1623">#1623</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1617">#1617</a>)</p>
</li>
<li>
<p>Shell</p>
<ul>
<li>Lex trailing whitespace as part of the prompt (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1645">#1645</a>)</li>
<li>Add missing <code>in</code> keyword (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1652">#1652</a>)</li>
</ul>
</li>
<li>
<p>SQL - Fix keywords (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1668">#1668</a>)</p>
</li>
<li>
<p>Typescript: Fix incorrect punctuation handling (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1510">#1510</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1511">#1511</a>)</p>
</li>
</ul>
</li>
<li>
<p>Fix infinite loop in SML lexer (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1625">#1625</a>)</p>
</li>
<li>
<p>Fix backtracking string regexes in JavaScript/TypeScript, Modula2
and many other lexers (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1637">#1637</a>)</p>
</li>
<li>
<p>Limit recursion with nesting Ruby heredocs (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1638">#1638</a>)</p>
</li>
<li>
<p>Fix a few inefficient regexes for guessing lexers</p>
</li>
<li>
<p>Fix the raw token lexer handling of Unicode (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1616">#1616</a>)</p>
</li>
<li>
<p>Revert a private API change in the HTML formatter (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1655">#1655</a>) --
please note that private APIs remain subject to change!</p>
</li>
<li>
<p>Fix several exponential/cubic-complexity regexes found by
Ben Caller/Doyensec (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1675">#1675</a>)</p>
</li>
<li>
<p>Fix incorrect MATLAB example (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1582">#1582</a>)</p>
</li>
</ul>
<p>Thanks to Google's OSS-Fuzz project for finding many of these bugs.</p>
<h2>2.7.3</h2>
<ul>
<li>
<p>Updated lexers:</p>
<ul>
<li>Ada (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1581">#1581</a>)</li>
<li>HTML (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1615">#1615</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1614">#1614</a>)</li>
<li>Java (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1594">#1594</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1586">#1586</a>)</li>
<li>JavaScript (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1605">#1605</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1589">#1589</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1588">#1588</a>)</li>
<li>JSON (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1569">#1569</a> -- this is a complete rewrite)</li>
<li>Lean (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1601">#1601</a>)</li>
<li>LLVM (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1612">#1612</a>)</li>
<li>Mason (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1592">#1592</a>)</li>
<li>MySQL (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1555">#1555</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1551">#1551</a>)</li>
<li>Rust (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1608">#1608</a>)</li>
<li>Turtle (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1590">#1590</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1553">#1553</a>)</li>
</ul>
</li>
<li>
<p>Deprecated JsonBareObjectLexer, which is now identical to JsonLexer (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1600">#1600</a>)</p>
</li>
<li>
<p>The <code>ImgFormatter</code> now calculates the exact character width, which fixes some issues with overlapping text (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1213">#1213</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1611">#1611</a>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pygments/pygments/blob/master/CHANGES">pygments's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.7.4</h2>
<p>(released January 12, 2021)</p>
<ul>
<li>
<p>Updated lexers:</p>
<ul>
<li>
<p>Apache configurations: Improve handling of malformed tags (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1656">#1656</a>)</p>
</li>
<li>
<p>CSS: Add support for variables (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1633">#1633</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1666">#1666</a>)</p>
</li>
<li>
<p>Crystal (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1650">#1650</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1670">#1670</a>)</p>
</li>
<li>
<p>Coq (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1648">#1648</a>)</p>
</li>
<li>
<p>Fortran: Add missing keywords (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1635">#1635</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1665">#1665</a>)</p>
</li>
<li>
<p>Ini (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1624">#1624</a>)</p>
</li>
<li>
<p>JavaScript and variants (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1647">#1647</a> -- missing regex flags, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1651">#1651</a>)</p>
</li>
<li>
<p>Markdown (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1623">#1623</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1617">#1617</a>)</p>
</li>
<li>
<p>Shell</p>
<ul>
<li>Lex trailing whitespace as part of the prompt (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1645">#1645</a>)</li>
<li>Add missing <code>in</code> keyword (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1652">#1652</a>)</li>
</ul>
</li>
<li>
<p>SQL - Fix keywords (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1668">#1668</a>)</p>
</li>
<li>
<p>Typescript: Fix incorrect punctuation handling (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1510">#1510</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1511">#1511</a>)</p>
</li>
</ul>
</li>
<li>
<p>Fix infinite loop in SML lexer (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1625">#1625</a>)</p>
</li>
<li>
<p>Fix backtracking string regexes in JavaScript/TypeScript, Modula2
and many other lexers (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1637">#1637</a>)</p>
</li>
<li>
<p>Limit recursion with nesting Ruby heredocs (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1638">#1638</a>)</p>
</li>
<li>
<p>Fix a few inefficient regexes for guessing lexers</p>
</li>
<li>
<p>Fix the raw token lexer handling of Unicode (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1616">#1616</a>)</p>
</li>
<li>
<p>Revert a private API change in the HTML formatter (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1655">#1655</a>) --
please note that private APIs remain subject to change!</p>
</li>
<li>
<p>Fix several exponential/cubic-complexity regexes found by
Ben Caller/Doyensec (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1675">#1675</a>)</p>
</li>
<li>
<p>Fix incorrect MATLAB example (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1582">#1582</a>)</p>
</li>
</ul>
<p>Thanks to Google's OSS-Fuzz project for finding many of these bugs.</p>
<h2>Version 2.7.3</h2>
<p>(released December 6, 2020)</p>
<ul>
<li>
<p>Updated lexers:</p>
<ul>
<li>Ada (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1581">#1581</a>)</li>
<li>HTML (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1615">#1615</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1614">#1614</a>)</li>
<li>Java (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1594">#1594</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1586">#1586</a>)</li>
<li>JavaScript (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1605">#1605</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1589">#1589</a>, <a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1588">#1588</a>)</li>
<li>JSON (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1569">#1569</a> -- this is a complete rewrite)</li>
<li>Lean (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1601">#1601</a>)</li>
<li>LLVM (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1612">#1612</a>)</li>
<li>Mason (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1592">#1592</a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pygments/pygments/commit/4d555d0fffc914a2a4ac9874416cdaaf8f8c9e74"><code>4d555d0</code></a> Bump version to 2.7.4.</li>
<li><a href="https://github.com/pygments/pygments/commit/fc3b05ddf25933e45f670534f79fd1df870e142a"><code>fc3b05d</code></a> Update CHANGES.</li>
<li><a href="https://github.com/pygments/pygments/commit/ad21935815ff6402d402b036e204f0333a77031b"><code>ad21935</code></a> Revert &quot;Added dracula theme style (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1636">#1636</a>)&quot;</li>
<li><a href="https://github.com/pygments/pygments/commit/e411506a23a39f4487ecc36afb616cc4715eb571"><code>e411506</code></a> Prepare for 2.7.4 release.</li>
<li><a href="https://github.com/pygments/pygments/commit/275e34d8f0d265bd474f269471b41c635fe559ff"><code>275e34d</code></a> doc: remove Perl 6 ref</li>
<li><a href="https://github.com/pygments/pygments/commit/2e7e8c4a7b318f4032493773732754e418279a14"><code>2e7e8c4</code></a> Fix several exponential/cubic complexity regexes found by Ben Caller/Doyensec</li>
<li><a href="https://github.com/pygments/pygments/commit/eb39c43b6ef992abadb0d25f0504d0cf2f3ccd86"><code>eb39c43</code></a> xquery: fix pop from empty stack</li>
<li><a href="https://github.com/pygments/pygments/commit/2738778c0b9c615bfcae68972fc656d351d676ca"><code>2738778</code></a> fix coding style in test_analyzer_lexer</li>
<li><a href="https://github.com/pygments/pygments/commit/02e0f09d796cca5174181e7ae3971cdc010e39b0"><code>02e0f09</code></a> Added 'ERROR STOP' to fortran.py keywords. (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1665">#1665</a>)</li>
<li><a href="https://github.com/pygments/pygments/commit/c83fe4888868f79415b50f050c047dc7fe11fd3b"><code>c83fe48</code></a> support added for css variables (<a href="https://github-redirect.dependabot.com/pygments/pygments/issues/1633">#1633</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pygments/pygments/compare/2.4.2...2.7.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pygments&package-manager=pip&previous-version=2.4.2&new-version=2.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-block-archiving/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 19:52:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-block-archiving/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Bump jinja2 from 2.10.1 to 2.11.3 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jinja2](https://github.com/pallets/jinja) from 2.10.1 to 2.11.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/releases">jinja2's releases</a>.</em></p>
<blockquote>
<h2>2.11.3</h2>
<p>This contains a fix for a speed issue with the <code>urlize</code> filter. <code>urlize</code> is likely to be called on untrusted user input. For certain inputs some of the regular expressions used to parse the text could take a very long time due to backtracking. As part of the fix, the email matching became slightly stricter. The various speedups apply to <code>urlize</code> in general, not just the specific input cases.</p>
<ul>
<li>PyPI: <a href="https://pypi.org/project/Jinja2/2.11.3/">https://pypi.org/project/Jinja2/2.11.3/</a></li>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-3">https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-3</a></li>
</ul>
<h2>2.11.2</h2>
<ul>
<li>Changelog: <a href="https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-2">https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-2</a></li>
</ul>
<h2>2.11.1</h2>
<p>This fixes an issue in async environment when indexing the result of an attribute lookup, like <code>{{ data.items[1:] }}</code>.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-1">https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-1</a></li>
</ul>
<h2>2.11.0</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-0">https://jinja.palletsprojects.com/en/2.11.x/changelog/#version-2-11-0</a></li>
<li>Blog: <a href="https://palletsprojects.com/blog/jinja-2-11-0-released/">https://palletsprojects.com/blog/jinja-2-11-0-released/</a></li>
<li>Twitter: <a href="https://twitter.com/PalletsTeam/status/1221883554537230336">https://twitter.com/PalletsTeam/status/1221883554537230336</a></li>
</ul>
<p>This is the last version to support Python 2.7 and 3.5. The next version will be Jinja 3.0 and will support Python 3.6 and newer.</p>
<h2>2.10.3</h2>
<ul>
<li>Changes: <a href="http://jinja.palletsprojects.com/en/2.10.x/changelog/#version-2-10-3">http://jinja.palletsprojects.com/en/2.10.x/changelog/#version-2-10-3</a></li>
</ul>
<h2>2.10.2</h2>
<ul>
<li>Changes: <a href="http://jinja.palletsprojects.com/en/2.10.x/changelog/#version-2-10-2">http://jinja.palletsprojects.com/en/2.10.x/changelog/#version-2-10-2</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/blob/main/CHANGES.rst">jinja2's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.11.3</h2>
<p>Released 2021-01-31</p>
<ul>
<li>Improve the speed of the <code>urlize</code> filter by reducing regex
backtracking. Email matching requires a word character at the start
of the domain part, and only word characters in the TLD. :pr:<code>1343</code></li>
</ul>
<h2>Version 2.11.2</h2>
<p>Released 2020-04-13</p>
<ul>
<li>Fix a bug that caused callable objects with <code>__getattr__</code>, like
:class:<code>~unittest.mock.Mock</code> to be treated as a
:func:<code>contextfunction</code>. :issue:<code>1145</code></li>
<li>Update <code>wordcount</code> filter to trigger :class:<code>Undefined</code> methods
by wrapping the input in :func:<code>soft_str</code>. :pr:<code>1160</code></li>
<li>Fix a hang when displaying tracebacks on Python 32-bit.
:issue:<code>1162</code></li>
<li>Showing an undefined error for an object that raises
<code>AttributeError</code> on access doesn't cause a recursion error.
:issue:<code>1177</code></li>
<li>Revert changes to :class:<code>~loaders.PackageLoader</code> from 2.10 which
removed the dependency on setuptools and pkg_resources, and added
limited support for namespace packages. The changes caused issues
when using Pytest. Due to the difficulty in supporting Python 2 and
:pep:<code>451</code> simultaneously, the changes are reverted until 3.0.
:pr:<code>1182</code></li>
<li>Fix line numbers in error messages when newlines are stripped.
:pr:<code>1178</code></li>
<li>The special <code>namespace()</code> assignment object in templates works in
async environments. :issue:<code>1180</code></li>
<li>Fix whitespace being removed before tags in the middle of lines when
<code>lstrip_blocks</code> is enabled. :issue:<code>1138</code></li>
<li>:class:<code>~nativetypes.NativeEnvironment</code> doesn't evaluate
intermediate strings during rendering. This prevents early
evaluation which could change the value of an expression.
:issue:<code>1186</code></li>
</ul>
<h2>Version 2.11.1</h2>
<p>Released 2020-01-30</p>
<ul>
<li>Fix a bug that prevented looking up a key after an attribute
(<code>{{ data.items[1:] }}</code>) in an async template. :issue:<code>1141</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/jinja/commit/cf215390d4a4d6f0a4de27e2687eed176878f13d"><code>cf21539</code></a> release version 2.11.3</li>
<li><a href="https://github.com/pallets/jinja/commit/15ef8f09b659f9100610583938005a7a10472d4d"><code>15ef8f0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/pallets/jinja/issues/1343">#1343</a> from pallets/urlize-speedup</li>
<li><a href="https://github.com/pallets/jinja/commit/ef658dc3b6389b091d608e710a810ce8b87995b3"><code>ef658dc</code></a> speed up urlize matching</li>
<li><a href="https://github.com/pallets/jinja/commit/eeca0fecc3318d43f61bc340ad61db641b861ade"><code>eeca0fe</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/pallets/jinja/issues/1207">#1207</a> from mhansen/patch-1</li>
<li><a href="https://github.com/pallets/jinja/commit/2dd769111cbb1a2637f805b3b4c652ec8096d371"><code>2dd7691</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/pallets/jinja/issues/1209">#1209</a> from mhansen/patch-3</li>
<li><a href="https://github.com/pallets/jinja/commit/48929401db7228db04dfd8e88115dd5c30dc2d86"><code>4892940</code></a> do_dictsort: update example ready to copy/paste</li>
<li><a href="https://github.com/pallets/jinja/commit/7db7d336ba12574e6205fdd929386fd529e3fad4"><code>7db7d33</code></a> api.rst: bugfix in docs, import PackageLoader</li>
<li><a href="https://github.com/pallets/jinja/commit/9ec465baefe32e305bd4e61da49e6c39360c194e"><code>9ec465b</code></a> fix changelog header</li>
<li><a href="https://github.com/pallets/jinja/commit/737a4cd41d09878e7e6c584a2062f5853dc30150"><code>737a4cd</code></a> release version 2.11.2</li>
<li><a href="https://github.com/pallets/jinja/commit/179df6b54e87b3d420cabf65fc07b2605ffc05f8"><code>179df6b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/pallets/jinja/issues/1190">#1190</a> from pallets/native-eval</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/jinja/compare/2.10.1...2.11.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jinja2&package-manager=pip&previous-version=2.10.1&new-version=2.11.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-block-archiving/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 19:52:24 +0000 UTC
    </div>
</div>

