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
                PR <a href="https://github.com/hyperledger/cello/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Updated the dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As titled.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 03:30:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    Bump the pip group across 2 directories with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [requests](https://github.com/psf/requests) and [urllib3](https://github.com/urllib3/urllib3) to permit the latest version.
Updates `requests` to 2.32.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.3</h2>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/0e322af87745eff34caffe4df68456ebc20d9068"><code>0e322af</code></a> v2.32.3</li>
<li><a href="https://github.com/psf/requests/commit/e18879932287c2bf4bcee4ddf6ccb8a69b6fc656"><code>e188799</code></a> Don't create default SSLContext if ssl module isn't present (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
<li><a href="https://github.com/psf/requests/commit/145b5399486b56e00250204f033441f3fdf2f3c9"><code>145b539</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a> from sigmavirus24/bug/6715</li>
<li><a href="https://github.com/psf/requests/commit/b1d73ddb509a3a2d3e10744e85f9cdebdbde90f0"><code>b1d73dd</code></a> Don't use default SSLContext with custom poolmanager kwargs</li>
<li><a href="https://github.com/psf/requests/commit/6badbac6e0d6b5a53872f26401761ad37a9002b8"><code>6badbac</code></a> Update HISTORY.md</li>
<li><a href="https://github.com/psf/requests/commit/a62a2d35d918baa8e793f7aa4fb41527644dfca5"><code>a62a2d3</code></a> Allow for overriding of specific pool key params</li>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v0.2.0...v2.32.3">compare view</a></li>
</ul>
</details>
<br />

Updates `requests` from 2.31.0 to 2.32.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.3</h2>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/0e322af87745eff34caffe4df68456ebc20d9068"><code>0e322af</code></a> v2.32.3</li>
<li><a href="https://github.com/psf/requests/commit/e18879932287c2bf4bcee4ddf6ccb8a69b6fc656"><code>e188799</code></a> Don't create default SSLContext if ssl module isn't present (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
<li><a href="https://github.com/psf/requests/commit/145b5399486b56e00250204f033441f3fdf2f3c9"><code>145b539</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a> from sigmavirus24/bug/6715</li>
<li><a href="https://github.com/psf/requests/commit/b1d73ddb509a3a2d3e10744e85f9cdebdbde90f0"><code>b1d73dd</code></a> Don't use default SSLContext with custom poolmanager kwargs</li>
<li><a href="https://github.com/psf/requests/commit/6badbac6e0d6b5a53872f26401761ad37a9002b8"><code>6badbac</code></a> Update HISTORY.md</li>
<li><a href="https://github.com/psf/requests/commit/a62a2d35d918baa8e793f7aa4fb41527644dfca5"><code>a62a2d3</code></a> Allow for overriding of specific pool key params</li>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v0.2.0...v2.32.3">compare view</a></li>
</ul>
</details>
<br />

Updates `urllib3` from 1.26.18 to 1.26.19
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.19</h2>
<h2>🚀 urllib3 is fundraising for HTTP/2 support</h2>
<p><a href="https://sethmlarson.dev/urllib3-is-fundraising-for-http2-support">urllib3 is raising ~$40,000 USD</a> to release HTTP/2 support and ensure long-term sustainable maintenance of the project after a sharp decline in financial support for 2023. If your company or organization uses Python and would benefit from HTTP/2 support in Requests, pip, cloud SDKs, and thousands of other projects <a href="https://opencollective.com/urllib3">please consider contributing financially</a> to ensure HTTP/2 support is developed sustainably and maintained for the long-haul.</p>
<p>Thank you for your support.</p>
<h2>Changes</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/urllib3/urllib3/compare/1.26.18...1.26.19">https://github.com/urllib3/urllib3/compare/1.26.18...1.26.19</a></p>
<p>Note that due to an issue with our release automation, no <code> multiple.intoto.jsonl</code> file is available for this release.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/1.26.19/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h2>1.26.19 (2024-06-17)</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Fixed handling of OpenSSL 3.2.0 new error message for misconfiguring an HTTP proxy as HTTPS. (<code>[#3405](https://github.com/urllib3/urllib3/issues/3405) &lt;https://github.com/urllib3/urllib3/issues/3405&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/d9d85c88aa644af56d5e129634e750ce76e1a765"><code>d9d85c8</code></a> Release 1.26.19</li>
<li><a href="https://github.com/urllib3/urllib3/commit/8528b63b6fe5cfd7b21942cf988670de68fcd8c0"><code>8528b63</code></a> [1.26] Fix downstream tests (<a href="https://redirect.github.com/urllib3/urllib3/issues/3409">#3409</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/40b6d1605814dd1db0a46e202d6e56f2e4c9a468"><code>40b6d16</code></a> Merge pull request from GHSA-34jh-p97f-mpxf</li>
<li><a href="https://github.com/urllib3/urllib3/commit/29cfd02f66376c61bd20f1725477925106321f68"><code>29cfd02</code></a> Fix handling of OpenSSL 3.2.0 new error message &quot;record layer failure&quot; (<a href="https://redirect.github.com/urllib3/urllib3/issues/3405">#3405</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b60064388302f54a3455259ddab121618650a154"><code>b600643</code></a> [1.26] Bump RECENT_DATE (<a href="https://redirect.github.com/urllib3/urllib3/issues/3404">#3404</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/7e2d3890926d4788e219f63e2e36fbeb8714827f"><code>7e2d389</code></a> [1.26] Fix running CPython 2.7 tests in CI (<a href="https://redirect.github.com/urllib3/urllib3/issues/3137">#3137</a>)</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/1.26.18...1.26.19">compare view</a></li>
</ul>
</details>
<br />


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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 01:28:01 +0000 UTC
    </div>
</div>

