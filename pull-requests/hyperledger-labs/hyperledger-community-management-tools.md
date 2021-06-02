---
layout: default
title: hyperledger-community-management-tools
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hyperledger-community-management-tools
---

# hyperledger-community-management-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hyperledger-community-management-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hyperledger-community-management-tools/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.24.2 to 1.26.5 in /project-reports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.24.2 to 1.26.5.
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
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/1.24.2...1.26.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.24.2&new-version=1.26.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/hyperledger-community-management-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 23:05:23 +0000 UTC
    </div>
</div>

