---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/560" class=".btn">#560</a>
            </td>
            <td>
                <b>
                    Edited the gitignore.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added the Django setting to the `.gitignore`.
2. Added the cello folder to the `.gitignore`.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-08 19:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/559" class=".btn">#559</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.26.5 to 1.26.17 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.26.5 to 1.26.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.17</h2>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (GHSA-v845-jxx5-vc9f)</li>
</ul>
<h2>1.26.16</h2>
<ul>
<li>Fixed thread-safety issue where accessing a <code>PoolManager</code> with many distinct origins would cause connection pools to be closed while requests are in progress (<a href="https://redirect.github.com/urllib3/urllib3/issues/2954">#2954</a>)</li>
</ul>
<h2>1.26.15</h2>
<ul>
<li>Fix socket timeout value when HTTPConnection is reused (<a href="https://redirect.github.com/urllib3/urllib3/issues/2645">urllib3/urllib3#2645</a>)</li>
<li>Remove &quot;!&quot; character from the unreserved characters in IPv6 Zone ID parsing (<a href="https://redirect.github.com/urllib3/urllib3/issues/2899">urllib3/urllib3#2899</a>)</li>
<li>Fix IDNA handling of 'x80' byte (<a href="https://redirect.github.com/urllib3/urllib3/issues/2901">urllib3/urllib3#2901</a>)</li>
</ul>
<h2>1.26.14</h2>
<ul>
<li>Fixed parsing of port 0 (zero) returning None, instead of 0 (<a href="https://redirect.github.com/urllib3/urllib3/issues/2850">#2850</a>)</li>
<li>Removed deprecated <code>HTTPResponse.getheaders()</code> calls in <code>urllib3.contrib</code> module.</li>
</ul>
<h2>1.26.13</h2>
<ul>
<li>Deprecated the <code>HTTPResponse.getheaders()</code> and <code>HTTPResponse.getheader()</code> methods.</li>
<li>Fixed an issue where parsing a URL with leading zeroes in the port would be rejected even when the port number after removing the zeroes was valid.</li>
<li>Fixed a deprecation warning when using cryptography v39.0.0.</li>
<li>Removed the <code>&lt;4</code> in the <code>Requires-Python</code> packaging metadata field.</li>
</ul>
<h2>1.26.12</h2>
<ul>
<li>Deprecated the <code>urllib3[secure]</code> extra and the <code>urllib3.contrib.pyopenssl</code> module. Both will be removed in v2.x. See this <a href="https://redirect.github.com/urllib3/urllib3/issues/2680">GitHub issue</a> for justification and info on how to migrate.</li>
</ul>
<h2>1.26.11</h2>
<p><strong>If you or your organization rely on urllib3 consider supporting us via <a href="https://github.com/sponsors/urllib3">GitHub Sponsors</a>.</strong></p>
<p>:warning: <strong>urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>Fixed an issue where reading more than 2 GiB in a call to HTTPResponse.read would raise an OverflowError on Python 3.9 and earlier.</li>
</ul>
<h2>1.26.10</h2>
<p><strong>If you or your organization rely on urllib3 consider supporting us via <a href="https://github.com/sponsors/urllib3">GitHub Sponsors</a>.</strong></p>
<p>:warning: <strong>urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<p>:closed_lock_with_key: <strong>This is the first release to be signed with Sigstore!</strong> You can verify the distributables using the <code>.sig</code> and <code>.crt</code> files included on this release.</p>
<ul>
<li>Removed support for Python 3.5</li>
<li>Fixed an issue where a <code>ProxyError</code> recommending configuring the proxy as HTTP instead of HTTPS could appear even when an HTTPS proxy wasn't configured.</li>
</ul>
<h2>1.26.9</h2>
<p><strong>If you or your organization rely on urllib3 consider supporting us via <a href="https://github.com/sponsors/urllib3">GitHub Sponsors</a>.</strong></p>
<p>:warning: <strong>urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>1.26.17 (2023-10-02)</h1>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (<code>[#3139](https://github.com/urllib3/urllib3/issues/3139) &lt;https://github.com/urllib3/urllib3/pull/3139&gt;</code>_)</li>
</ul>
<h1>1.26.16 (2023-05-23)</h1>
<ul>
<li>Fixed thread-safety issue where accessing a <code>PoolManager</code> with many distinct origins
would cause connection pools to be closed while requests are in progress (<code>[#2954](https://github.com/urllib3/urllib3/issues/2954) &lt;https://github.com/urllib3/urllib3/pull/2954&gt;</code>_)</li>
</ul>
<h1>1.26.15 (2023-03-10)</h1>
<ul>
<li>Fix socket timeout value when <code>HTTPConnection</code> is reused (<code>[#2645](https://github.com/urllib3/urllib3/issues/2645) &lt;https://github.com/urllib3/urllib3/issues/2645&gt;</code>__)</li>
<li>Remove &quot;!&quot; character from the unreserved characters in IPv6 Zone ID parsing
(<code>[#2899](https://github.com/urllib3/urllib3/issues/2899) &lt;https://github.com/urllib3/urllib3/issues/2899&gt;</code>__)</li>
<li>Fix IDNA handling of '\x80' byte (<code>[#2901](https://github.com/urllib3/urllib3/issues/2901) &lt;https://github.com/urllib3/urllib3/issues/2901&gt;</code>__)</li>
</ul>
<h1>1.26.14 (2023-01-11)</h1>
<ul>
<li>Fixed parsing of port 0 (zero) returning None, instead of 0. (<code>[#2850](https://github.com/urllib3/urllib3/issues/2850) &lt;https://github.com/urllib3/urllib3/issues/2850&gt;</code>__)</li>
<li>Removed deprecated getheaders() calls in contrib module. Fixed the type hint of <code>PoolKey.key_retries</code> by adding <code>bool</code> to the union. (<code>[#2865](https://github.com/urllib3/urllib3/issues/2865) &lt;https://github.com/urllib3/urllib3/issues/2865&gt;</code>__)</li>
</ul>
<h1>1.26.13 (2022-11-23)</h1>
<ul>
<li>Deprecated the <code>HTTPResponse.getheaders()</code> and <code>HTTPResponse.getheader()</code> methods.</li>
<li>Fixed an issue where parsing a URL with leading zeroes in the port would be rejected
even when the port number after removing the zeroes was valid.</li>
<li>Fixed a deprecation warning when using cryptography v39.0.0.</li>
<li>Removed the <code>&lt;4</code> in the <code>Requires-Python</code> packaging metadata field.</li>
</ul>
<h1>1.26.12 (2022-08-22)</h1>
<ul>
<li>Deprecated the <code>urllib3[secure]</code> extra and the <code>urllib3.contrib.pyopenssl</code> module.
Both will be removed in v2.x. See this <code>GitHub issue &lt;https://github.com/urllib3/urllib3/issues/2680&gt;</code>_
for justification and info on how to migrate.</li>
</ul>
<h1>1.26.11 (2022-07-25)</h1>
<ul>
<li>Fixed an issue where reading more than 2 GiB in a call to <code>HTTPResponse.read</code> would
raise an <code>OverflowError</code> on Python 3.9 and earlier.</li>
</ul>
<h1>1.26.10 (2022-07-07)</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/c9016bf464751a02b7e46f8b86504f47d4238784"><code>c9016bf</code></a> Release 1.26.17</li>
<li><a href="https://github.com/urllib3/urllib3/commit/01220354d389cd05474713f8c982d05c9b17aafb"><code>0122035</code></a> Backport GHSA-v845-jxx5-vc9f (<a href="https://redirect.github.com/urllib3/urllib3/issues/3139">#3139</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/e63989f97d206e839ab9170c8a76e3e097cc60e8"><code>e63989f</code></a> Fix installing <code>brotli</code> extra on Python 2.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2e7a24d08713a0131f0b3c7197889466d645cc49"><code>2e7a24d</code></a> [1.26] Configure OS for RTD to fix building docs</li>
<li><a href="https://github.com/urllib3/urllib3/commit/57181d6ea910ac7cb2ff83345d9e5e0eb816a0d0"><code>57181d6</code></a> [1.26] Improve error message when calling urllib3.request() (<a href="https://redirect.github.com/urllib3/urllib3/issues/3058">#3058</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/3c0148048a523325819377b23fc67f8d46afc3aa"><code>3c01480</code></a> [1.26] Run coverage even with failed jobs</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d94029b7e2193ff47b627906a70e06377a09aae8"><code>d94029b</code></a> Release 1.26.16</li>
<li><a href="https://github.com/urllib3/urllib3/commit/18e92145e9cddbabdf51c98f54202aa37fd5d4c8"><code>18e9214</code></a> Use trusted publishing for PyPI</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d25cf83bbae850a290fe34ed1610ae55c0558b36"><code>d25cf83</code></a> [1.26] Fix invalid test_ssl_failure_midway_through_conn</li>
<li><a href="https://github.com/urllib3/urllib3/commit/25cca389496b86ee809c21e5b641aeaa74809263"><code>25cca38</code></a> [1.26] Fix test_ssl_object_attributes</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/1.26.5...1.26.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.26.5&new-version=1.26.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 04:43:26 +0000 UTC
    </div>
</div>

