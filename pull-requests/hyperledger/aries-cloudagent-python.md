---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3048" class=".btn">#3048</a>
            </td>
            <td>
                <b>
                    :adhesive_bandage: add exception handling to wallet-upgrade check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simple fix for non-critical issue.

Currently, if something goes wrong with the `check_for_wallet_upgrades_in_progress` method, then startup will be aborted. This PR just adds a try-except block, such that the exception is logged and startup can proceed.

Relates to #3030
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 13:37:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3046" class=".btn">#3046</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 2 updates: [requests](https://github.com/psf/requests) and [urllib3](https://github.com/urllib3/urllib3).

Updates `requests` from 2.31.0 to 2.32.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
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
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>v2.32.0</h2>
<h2>2.32.0 (2024-05-20)</h2>
<h2>🐍 PYCON US 2024 EDITION 🐍</h2>
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
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
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
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li><a href="https://github.com/psf/requests/commit/d6ebc4a2f1f68b7e355fb7e4dd5ffc0845547f9f"><code>d6ebc4a</code></a> v2.32.0</li>
<li><a href="https://github.com/psf/requests/commit/9a40d1277807f0a4f26c9a37eea8ec90faa8aadc"><code>9a40d12</code></a> Avoid reloading root certificates to improve concurrent performance (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li><a href="https://github.com/psf/requests/commit/0c030f78d24f29a459dbf39b28b4cc765e2153d7"><code>0c030f7</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a> from nateprewitt/no_char_detection</li>
<li><a href="https://github.com/psf/requests/commit/555b870eb19d497ddb67042645420083ec8efb02"><code>555b870</code></a> Allow character detection dependencies to be optional in post-packaging steps</li>
<li><a href="https://github.com/psf/requests/commit/d6dded3f00afcf56a7e866cb0732799045301eb0"><code>d6dded3</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6700">#6700</a> from franekmagiera/update-redirect-to-invalid-uri-test</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.31.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />

Updates `urllib3` from 2.2.1 to 2.2.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.2.2</h2>
<h2>🚀 urllib3 is fundraising for HTTP/2 support</h2>
<p><a href="https://sethmlarson.dev/urllib3-is-fundraising-for-http2-support">urllib3 is raising ~$40,000 USD</a> to release HTTP/2 support and ensure long-term sustainable maintenance of the project after a sharp decline in financial support for 2023. If your company or organization uses Python and would benefit from HTTP/2 support in Requests, pip, cloud SDKs, and thousands of other projects <a href="https://opencollective.com/urllib3">please consider contributing financially</a> to ensure HTTP/2 support is developed sustainably and maintained for the long-haul.</p>
<p>Thank you for your support.</p>
<h2>Changes</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3122">#3122</a>)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3363">#3363</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.2.2 (2024-06-17)</h1>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<code>[#3122](https://github.com/urllib3/urllib3/issues/3122) &lt;https://github.com/urllib3/urllib3/issues/3122&gt;</code>__)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<code>[#3363](https://github.com/urllib3/urllib3/issues/3363) &lt;https://github.com/urllib3/urllib3/issues/3363&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/27e2a5c5a7ab6a517252cc8dcef3ffa6ffb8f61a"><code>27e2a5c</code></a> Release 2.2.2 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3406">#3406</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/accff72ecc2f6cf5a76d9570198a93ac7c90270e"><code>accff72</code></a> Merge pull request from GHSA-34jh-p97f-mpxf</li>
<li><a href="https://github.com/urllib3/urllib3/commit/34be4a57e59eb7365bcc37d52e9f8271b5b8d0d3"><code>34be4a5</code></a> Pin CFFI to a new release candidate instead of a Git commit (<a href="https://redirect.github.com/urllib3/urllib3/issues/3398">#3398</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/da410581b6b3df73da976b5ce5eb20a4bd030437"><code>da41058</code></a> Bump browser-actions/setup-chrome from 1.6.0 to 1.7.1 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3399">#3399</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b07a669bd970d69847801148286b726f0570b625"><code>b07a669</code></a> Bump github/codeql-action from 2.13.4 to 3.25.6 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3396">#3396</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b8589ec9f8c4da91511e601b632ac06af7e7c10e"><code>b8589ec</code></a> Measure coverage with v4 of artifact actions (<a href="https://redirect.github.com/urllib3/urllib3/issues/3394">#3394</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f3bdc5585111429e22c81b5fb26c3ec164d98b81"><code>f3bdc55</code></a> Allow triggering CI manually (<a href="https://redirect.github.com/urllib3/urllib3/issues/3391">#3391</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/52392654b30183129cf3ec06010306f517d9c146"><code>5239265</code></a> Fix HTTP version in debug log (<a href="https://redirect.github.com/urllib3/urllib3/issues/3316">#3316</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b34619f94ece0c40e691a5aaf1304953d88089de"><code>b34619f</code></a> Bump actions/checkout to 4.1.4 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3387">#3387</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/9961d14de7c920091d42d42ed76d5d479b80064d"><code>9961d14</code></a> Bump browser-actions/setup-chrome from 1.5.0 to 1.6.0 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3386">#3386</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3045" class=".btn">#3045</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.2.1 to 2.2.2 in /demo/playground/examples in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /demo/playground/examples with 1 update: [urllib3](https://github.com/urllib3/urllib3).

Updates `urllib3` from 2.2.1 to 2.2.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.2.2</h2>
<h2>🚀 urllib3 is fundraising for HTTP/2 support</h2>
<p><a href="https://sethmlarson.dev/urllib3-is-fundraising-for-http2-support">urllib3 is raising ~$40,000 USD</a> to release HTTP/2 support and ensure long-term sustainable maintenance of the project after a sharp decline in financial support for 2023. If your company or organization uses Python and would benefit from HTTP/2 support in Requests, pip, cloud SDKs, and thousands of other projects <a href="https://opencollective.com/urllib3">please consider contributing financially</a> to ensure HTTP/2 support is developed sustainably and maintained for the long-haul.</p>
<p>Thank you for your support.</p>
<h2>Changes</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3122">#3122</a>)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3363">#3363</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.2.2 (2024-06-17)</h1>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<code>[#3122](https://github.com/urllib3/urllib3/issues/3122) &lt;https://github.com/urllib3/urllib3/issues/3122&gt;</code>__)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<code>[#3363](https://github.com/urllib3/urllib3/issues/3363) &lt;https://github.com/urllib3/urllib3/issues/3363&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/27e2a5c5a7ab6a517252cc8dcef3ffa6ffb8f61a"><code>27e2a5c</code></a> Release 2.2.2 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3406">#3406</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/accff72ecc2f6cf5a76d9570198a93ac7c90270e"><code>accff72</code></a> Merge pull request from GHSA-34jh-p97f-mpxf</li>
<li><a href="https://github.com/urllib3/urllib3/commit/34be4a57e59eb7365bcc37d52e9f8271b5b8d0d3"><code>34be4a5</code></a> Pin CFFI to a new release candidate instead of a Git commit (<a href="https://redirect.github.com/urllib3/urllib3/issues/3398">#3398</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/da410581b6b3df73da976b5ce5eb20a4bd030437"><code>da41058</code></a> Bump browser-actions/setup-chrome from 1.6.0 to 1.7.1 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3399">#3399</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b07a669bd970d69847801148286b726f0570b625"><code>b07a669</code></a> Bump github/codeql-action from 2.13.4 to 3.25.6 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3396">#3396</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b8589ec9f8c4da91511e601b632ac06af7e7c10e"><code>b8589ec</code></a> Measure coverage with v4 of artifact actions (<a href="https://redirect.github.com/urllib3/urllib3/issues/3394">#3394</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f3bdc5585111429e22c81b5fb26c3ec164d98b81"><code>f3bdc55</code></a> Allow triggering CI manually (<a href="https://redirect.github.com/urllib3/urllib3/issues/3391">#3391</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/52392654b30183129cf3ec06010306f517d9c146"><code>5239265</code></a> Fix HTTP version in debug log (<a href="https://redirect.github.com/urllib3/urllib3/issues/3316">#3316</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b34619f94ece0c40e691a5aaf1304953d88089de"><code>b34619f</code></a> Bump actions/checkout to 4.1.4 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3387">#3387</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/9961d14de7c920091d42d42ed76d5d479b80064d"><code>9961d14</code></a> Bump browser-actions/setup-chrome from 1.5.0 to 1.6.0 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3386">#3386</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.2.1&new-version=2.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3042" class=".btn">#3042</a>
            </td>
            <td>
                <b>
                    Fix - only run integration tests on opened PR's
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This check to only run integration tests was added recently on the unrelated PR https://github.com/hyperledger/aries-cloudagent-python/pull/3000. The problem is it didn't run the integration tests after a draft was converted to open. 

This seems to fix it. By adding the pull request types.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 17:05:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3038" class=".btn">#3038</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump marshmallow from 3.20.2 to 3.21.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [marshmallow](https://github.com/marshmallow-code/marshmallow) from 3.20.2 to 3.21.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/marshmallow-code/marshmallow/blob/dev/CHANGELOG.rst">marshmallow's changelog</a>.</em></p>
<blockquote>
<p>3.21.3 (2024-06-05)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Fix memory leak that prevented schema instances from getting GC'd (:pr:<code>2277</code>).
Thanks :user:<code>mrcljx</code> for the PR.</li>
</ul>
<p>3.21.2 (2024-05-01)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Allow timestamp 0 in <code>fields.DateTime</code> (:issue:<code>2133</code>).
Thanks :user:<code>flydzen</code> for reporting.</li>
</ul>
<p>3.21.1 (2024-03-04)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Fix error message when field is declared as a class and not an instance (:issue:<code>2245</code>).
Thanks :user:<code>travnick</code> for reporting.</li>
</ul>
<p>3.21.0 (2024-02-26)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Fix validation of <code>URL</code> fields to allow missing user field,
per NWG RFC 3986 (:issue:<code>2232</code>). Thanks :user:<code>ddennerline3</code> for reporting
and :user:<code>deckar01</code> for the PR.</li>
</ul>
<p>Other changes:</p>
<ul>
<li><em>Backwards-incompatible</em>: <code>__version__</code>, <code>__parsed_version__</code>, and <code>__version_info__</code>
attributes are deprecated (:issue:<code>2227</code>). Use feature detection or
<code>importlib.metadata.version(&quot;marshmallow&quot;)</code> instead.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/b9646e326c511c11fc07aef4aa0004c14a5d454c"><code>b9646e3</code></a> Bump version and update changelog</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/99103a675fa469c05ea93c4cbc91d47fd5556eee"><code>99103a6</code></a> Remove leaky lru_cache (<a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2277">#2277</a>)</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/47205b5c4f89794341eebbbbd0e39b765c4c8bbe"><code>47205b5</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2276">#2276</a>)</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/aaecd5b02dc46b068e30964edbfb8d91d1eab3db"><code>aaecd5b</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/c592536b649fab0bbfb4bc3f84b65577a13b8ca2"><code>c592536</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2269">#2269</a>)</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/ee0c903c3c1ea6ee4e00b9565ab2556da996b6de"><code>ee0c903</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/d4fd5a4abbb556e337afde6b46bf3a37ab7100f9"><code>d4fd5a4</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/511b8c5354929b78b63d57578556443e41f8293f"><code>511b8c5</code></a> Bump version and update changelog</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/03f56a4f0fae9e650028227be265b5786b0575a9"><code>03f56a4</code></a> Merge pull request <a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2264">#2264</a> from marshmallow-code/allow_timestamp_0</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/58fbbcd3446ade39ea3be83ce9ee9170acf0230b"><code>58fbbcd</code></a> Encapsulate timestamp boolean check in utils</li>
<li>Additional commits viewable in <a href="https://github.com/marshmallow-code/marshmallow/compare/3.20.2...3.21.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=marshmallow&package-manager=pip&previous-version=3.20.2&new-version=3.21.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 12:07:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3037" class=".btn">#3037</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump packaging from 23.1 to 23.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [packaging](https://github.com/pypa/packaging) from 23.1 to 23.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pypa/packaging/releases">packaging's releases</a>.</em></p>
<blockquote>
<h2>23.2</h2>
<h2>What's Changed</h2>
<ul>
<li>parse_marker should consume the entire source string by <a href="https://github.com/mwerschy"><code>@​mwerschy</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/687">pypa/packaging#687</a></li>
<li>Create a Security Policy file  by <a href="https://github.com/joycebrum"><code>@​joycebrum</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/695">pypa/packaging#695</a></li>
<li>Add python 3.12 to CI by <a href="https://github.com/mayeut"><code>@​mayeut</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/689">pypa/packaging#689</a></li>
<li>Remove URL validation from requirement parsing by <a href="https://github.com/uranusjr"><code>@​uranusjr</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/684">pypa/packaging#684</a></li>
<li>Add types for packaging.version._Version by <a href="https://github.com/hauntsaninja"><code>@​hauntsaninja</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/665">pypa/packaging#665</a></li>
<li>Add PyPy 3.10 to CI by <a href="https://github.com/mayeut"><code>@​mayeut</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/699">pypa/packaging#699</a></li>
<li>Remove unused argument in <code>_manylinux._is_compatible</code> by <a href="https://github.com/mayeut"><code>@​mayeut</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/700">pypa/packaging#700</a></li>
<li>Canonicalize names for requirements comparison by <a href="https://github.com/astrojuanlu"><code>@​astrojuanlu</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/696">pypa/packaging#696</a></li>
<li>Add platform tag support for LoongArch by <a href="https://github.com/loongson-zn"><code>@​loongson-zn</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/693">pypa/packaging#693</a></li>
<li>Ability to install <code>armv7l manylinux/musllinux</code> wheels on <code>armv8l</code> by <a href="https://github.com/mayeut"><code>@​mayeut</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/690">pypa/packaging#690</a></li>
<li>Include CHANGELOG.rst in sdist by <a href="https://github.com/astrojuanlu"><code>@​astrojuanlu</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/704">pypa/packaging#704</a></li>
<li>Update pyupgrade to Python 3.7+ by <a href="https://github.com/fangchenli"><code>@​fangchenli</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/580">pypa/packaging#580</a></li>
<li>Fix version pattern pre-releases by <a href="https://github.com/deathaxe"><code>@​deathaxe</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/705">pypa/packaging#705</a></li>
<li>Fix typos found by codespell by <a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/706">pypa/packaging#706</a></li>
<li>Support enriched metadata by <a href="https://github.com/brettcannon"><code>@​brettcannon</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/686">pypa/packaging#686</a></li>
<li>Correct rST syntax in CHANGELOG.rst by <a href="https://github.com/atugushev"><code>@​atugushev</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/709">pypa/packaging#709</a></li>
<li>fix: platform tag for GraalPy by <a href="https://github.com/mayeut"><code>@​mayeut</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/711">pypa/packaging#711</a></li>
<li>Document that this library uses a calendar-based versioning scheme by <a href="https://github.com/faph"><code>@​faph</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/717">pypa/packaging#717</a></li>
<li>fix: Update copyright date for docs by <a href="https://github.com/garrypolley"><code>@​garrypolley</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/713">pypa/packaging#713</a></li>
<li>Bump pip version to avoid known vulnerabilities by <a href="https://github.com/joycebrum"><code>@​joycebrum</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/720">pypa/packaging#720</a></li>
<li>Typing annotations fixed in version.py by <a href="https://github.com/jolaf"><code>@​jolaf</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/723">pypa/packaging#723</a></li>
<li>parse_{sdist,wheel}_filename: don't raise InvalidVersion by <a href="https://github.com/SpecLad"><code>@​SpecLad</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/721">pypa/packaging#721</a></li>
<li>Fix code blocks in CHANGELOG.md by <a href="https://github.com/edmorley"><code>@​edmorley</code></a> in <a href="https://redirect.github.com/pypa/packaging/pull/724">pypa/packaging#724</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mwerschy"><code>@​mwerschy</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/687">pypa/packaging#687</a></li>
<li><a href="https://github.com/joycebrum"><code>@​joycebrum</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/695">pypa/packaging#695</a></li>
<li><a href="https://github.com/astrojuanlu"><code>@​astrojuanlu</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/696">pypa/packaging#696</a></li>
<li><a href="https://github.com/loongson-zn"><code>@​loongson-zn</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/693">pypa/packaging#693</a></li>
<li><a href="https://github.com/fangchenli"><code>@​fangchenli</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/580">pypa/packaging#580</a></li>
<li><a href="https://github.com/deathaxe"><code>@​deathaxe</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/705">pypa/packaging#705</a></li>
<li><a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/706">pypa/packaging#706</a></li>
<li><a href="https://github.com/atugushev"><code>@​atugushev</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/709">pypa/packaging#709</a></li>
<li><a href="https://github.com/faph"><code>@​faph</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/717">pypa/packaging#717</a></li>
<li><a href="https://github.com/garrypolley"><code>@​garrypolley</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/713">pypa/packaging#713</a></li>
<li><a href="https://github.com/jolaf"><code>@​jolaf</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/723">pypa/packaging#723</a></li>
<li><a href="https://github.com/SpecLad"><code>@​SpecLad</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/721">pypa/packaging#721</a></li>
<li><a href="https://github.com/edmorley"><code>@​edmorley</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/packaging/pull/724">pypa/packaging#724</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/packaging/compare/23.1...23.2">https://github.com/pypa/packaging/compare/23.1...23.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pypa/packaging/blob/main/CHANGELOG.rst">packaging's changelog</a>.</em></p>
<blockquote>
<p>23.2 - 2023-10-01</p>
<pre><code>
* Document calendar-based versioning scheme (:issue:`716`)
* Enforce that the entire marker string is parsed (:issue:`687`)
* Requirement parsing no longer automatically validates the URL (:issue:`120`)
* Canonicalize names for requirements comparison (:issue:`644`)
* Introduce ``metadata.Metadata`` (along with ``metadata.ExceptionGroup`` and ``metadata.InvalidMetadata``; :issue:`570`)
* Introduce the ``validate`` keyword parameter to ``utils.normalize_name()`` (:issue:`570`)
* Introduce ``utils.is_normalized_name()`` (:issue:`570`)
* Make ``utils.parse_sdist_filename()`` and ``utils.parse_wheel_filename()``
  raise ``InvalidSdistFilename`` and ``InvalidWheelFilename``, respectively,
  when the version component of the name is invalid
</code></pre>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pypa/packaging/commit/b3a5d7d68991c040615d5345bb55f61de53ba176"><code>b3a5d7d</code></a> Bump for release</li>
<li><a href="https://github.com/pypa/packaging/commit/d7ce40d8cc005a6b83f4abb33ae7d48d0428a4f6"><code>d7ce40d</code></a> Fix code blocks in CHANGELOG.md (<a href="https://redirect.github.com/pypa/packaging/issues/724">#724</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/524b701c6e30fc4da9355117367273f591c6de72"><code>524b701</code></a> parse_{sdist,wheel}_filename: don't raise InvalidVersion (<a href="https://redirect.github.com/pypa/packaging/issues/721">#721</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/b509bef6a4573595b23a97ecbfe569000918157f"><code>b509bef</code></a> Typing annotations fixed (<a href="https://redirect.github.com/pypa/packaging/issues/723">#723</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/0206c394cebce1b261299032edcb33f842b65d10"><code>0206c39</code></a> Bump pip version to avoid known vulnerabilities (<a href="https://redirect.github.com/pypa/packaging/issues/720">#720</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/702353715de375a65e49d1ae4af21c35dce838b8"><code>7023537</code></a> fix: Update copyright date for docs (<a href="https://redirect.github.com/pypa/packaging/issues/713">#713</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/39786bb4bf661bdb5137b8db8bd38d8e838dd67f"><code>39786bb</code></a> Document use of calendar-based versioning scheme (<a href="https://redirect.github.com/pypa/packaging/issues/717">#717</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/c1346dfdafecffc30ca777ac004ed2898e60e34e"><code>c1346df</code></a> fix: Detect when a platform is 32-bit more accurately (<a href="https://redirect.github.com/pypa/packaging/issues/711">#711</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/7e68d828f265ef05cf4cd3b5def9baffef8c2968"><code>7e68d82</code></a> Correct rST syntax in CHANGELOG.rst (<a href="https://redirect.github.com/pypa/packaging/issues/709">#709</a>)</li>
<li><a href="https://github.com/pypa/packaging/commit/61e6efb6b6ee99e445f575bc522b716daeaa37cf"><code>61e6efb</code></a> Support enriched metadata in <code>packaging.metadata</code> (<a href="https://redirect.github.com/pypa/packaging/issues/686">#686</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pypa/packaging/compare/23.1...23.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=packaging&package-manager=pip&previous-version=23.1&new-version=23.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 12:07:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump mkdocs-material from 9.5.10 to 9.5.27
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.5.10 to 9.5.27.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.5.27</h2>
<ul>
<li>Updated Estonian translations</li>
</ul>
<p>Thanks to <a href="https://github.com/Eilyre"><code>@​Eilyre</code></a> for their contributions</p>
<h2>mkdocs-material-9.5.26</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7232">#7232</a>: Tab switches on scroll when linking tabs (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7230">#7230</a>: Blog author avatar broken when referring to local file</li>
</ul>
<h2>mkdocs-material-9.5.25</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7209">#7209</a>: Tags plugin crashing on numeric tags</li>
</ul>
<h2>mkdocs-material-9.5.24</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7187">#7187</a>: Version selector title rendering issue</li>
</ul>
<h2>mkdocs-material-9.5.23</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7183">#7183</a>: Edge case in anchor navigation when using instant navigation</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6436">#6436</a>: Version selector not showing version alias</li>
</ul>
<h2>mkdocs-material-9.5.22</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7170">#7170</a>: Copy button adds empty lines for line spans (9.5.18 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7160">#7160</a>: Version switching doesn't stay on page (9.5.5 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5619">#5619</a>: Links in Mermaid.js diagrams not discernible</li>
</ul>
<h2>mkdocs-material-9.5.21</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7133">#7133</a>: Ensure latest version of Mermaid.js is used</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7125">#7125</a>: Added warning for dotfiles in info plugin</li>
</ul>
<p>Thanks to <a href="https://github.com/kamilkrzyskow"><code>@​kamilkrzyskow</code></a> for their contributions</p>
<h2>mkdocs-material-9.5.20</h2>
<ul>
<li>Fixed deprecation warning in privacy plugin (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7119">#7119</a>: Tags plugin emits deprecation warning (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7118">#7118</a>: Social plugin crashes if fonts are disabled (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7085">#7085</a>: Social plugin crashes on Windows when downloading fonts</li>
</ul>
<h2>mkdocs-material-9.5.19</h2>
<ul>
<li>Updated MkDocs to 1.6 and limited version to &lt; 2</li>
<li>Updated Docker image to latest Alpine Linux</li>
<li>Removed <code>setup.py</code>, now that GitHub fully understands <code>pyproject.toml</code></li>
<li>Improved interop of social plugin with third-party MkDocs themes</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7099">#7099</a>: Blog reading time not rendered correctly for Japanese</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7097">#7097</a>: Improved resilience of tags plugin when no tags are given</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7090">#7090</a>: Active tab indicator in nested content tabs rendering bug</li>
</ul>
<h2>mkdocs-material-9.5.18</h2>
<ul>
<li>Refactored tooltips implementation to fix positioning issues</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7044">#7044</a>: Rendering glitch when hovering contributor avatar in Chrome</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7043">#7043</a>: Highlighted lines in code blocks cutoff on mobile</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6910">#6910</a>: Incorrect position of tooltip for page status in sidebar</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.5.27 (2024-06-16)</p>
<ul>
<li>Updated Estonian translations</li>
</ul>
<p>mkdocs-material-9.5.26 (2024-06-06)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7232">#7232</a>: Tab switches on scroll when linking tabs (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7230">#7230</a>: Blog author avatar broken when referring to local file</li>
</ul>
<p>mkdocs-material-9.5.25+insiders-4.53.11 (2024-05-27)</p>
<ul>
<li>Fixed projects plugin crashing when serving before building subprojects</li>
</ul>
<p>mkdocs-material-9.5.25 (2024-05-27)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7209">#7209</a>: Tags plugin crashing on numeric tags</li>
</ul>
<p>mkdocs-material-9.5.24+insiders-4.53.10 (2024-05-20)</p>
<ul>
<li>Fixed projects plugin crashing in serve mode when disabled</li>
<li>Fixed projects plugin crashing when building nested projects</li>
</ul>
<p>mkdocs-material-9.5.24+insiders-4.53.9 (2024-05-20)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7191">#7191</a>: Tags listings not rendering when toc_depth is changed</li>
</ul>
<p>mkdocs-material-9.5.24 (2024-05-20)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7187">#7187</a>: Version selector title rendering issue</li>
</ul>
<p>mkdocs-material-9.5.23 (2024-05-15)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7183">#7183</a>: Edge case in anchor navigation when using instant navigation</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6436">#6436</a>: Version selector not showing version alias</li>
</ul>
<p>mkdocs-material-9.5.22 (2024-05-12)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7170">#7170</a>: Copy button adds empty lines for line spans (9.5.18 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7160">#7160</a>: Version switching doesn't stay on page (9.5.5 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5619">#5619</a>: Links in Mermaid.js diagrams not discernible</li>
</ul>
<p>mkdocs-material-9.5.21 (2024-05-03)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7133">#7133</a>: Ensure latest version of Mermaid.js is used</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7125">#7125</a>: Added warning for dotfiles in info plugin</li>
</ul>
<p>mkdocs-material-9.5.20 (2024-04-29)</p>
<ul>
<li>Fixed deprecation warning in privacy plugin (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7119">#7119</a>: Tags plugin emits deprecation warning (9.5.19 regression)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f4adebd7587ed7d38a09062ca9af29283ad3d13f"><code>f4adebd</code></a> Prepare 9.5.27 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/9e1f527e57eae44656ea86e3553e9bc29144da0f"><code>9e1f527</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f4db9de0f018427ceb6bc28d5fb095d6c1468b13"><code>f4db9de</code></a> Updated Estonian translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/b45c51dee43472b4164f703b5ee1db775a99a5a6"><code>b45c51d</code></a> Changed Twitter to X (<a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7266">#7266</a>)</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/4ba7a6db51029b346f7ac1fecc1c99e46654cade"><code>4ba7a6d</code></a> Add reference to PlantUML Markdown schema (<a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7260">#7260</a>)</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/ccc8d8491f35a9b37ff2ea4a60503304fab1cf9b"><code>ccc8d84</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0c54a880d27803cb57aa4c5ca20ed70347e82aeb"><code>0c54a88</code></a> Updated Premium sponsors</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f8871975babb2928ef5d797ddcc659ddf8aa19ff"><code>f887197</code></a> Updated changelog</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0d5a08ca9de9f97cb2302490b8ef9d451dfd17f3"><code>0d5a08c</code></a> Prepare 9.5.26 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/1cc45d50d077c8c27d58b71dcc11b941779ec9b2"><code>1cc45d5</code></a> Fixed active tab stolen on scroll with linked content tabs</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.5.10...9.5.27">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.5.10&new-version=9.5.27)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 12:06:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump configargparse from 1.5.5 to 1.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [configargparse](https://github.com/bw2/ConfigArgParse) from 1.5.5 to 1.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/ee77f44d03415f2afe73c82096bae2293db29a3b"><code>ee77f44</code></a> added several missed global variables from the argparse module</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/9f73219735abff20751523b5250875a7839daa1e"><code>9f73219</code></a> Merge pull request <a href="https://redirect.github.com/bw2/ConfigArgParse/issues/279">#279</a> from shadchin/drop_py2</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/6acc381513c2289a8301e8643742af91fecbb454"><code>6acc381</code></a> remove 2.7 since github doesn't have a test environment for it</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/959c190571f3762dcf6c883e5181a5a3b18153b5"><code>959c190</code></a> try adding tests for 2.7</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/c1a08f418c43ee55890c213a870429e05f48665b"><code>c1a08f4</code></a> Remove Python 2 support</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/bca2c2fb8f13f45dea0f06d4b4c3f0b4336c2d54"><code>bca2c2f</code></a> updated README</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/82fd623a01879368dfd4f44195e153917f4d924b"><code>82fd623</code></a> re-ordered badges</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/15c4c05657992de04a610b61b7d103c009d815dc"><code>15c4c05</code></a> added downloads per week stat</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/64637827bbcb70b341c3a79fe0828dbd76f71b1c"><code>6463782</code></a> attempt to fix apidocs</li>
<li><a href="https://github.com/bw2/ConfigArgParse/commit/6d8b8494d30148ee2040b5f11f39beb444d363aa"><code>6d8b849</code></a> attempt to fix apidocs</li>
<li>Additional commits viewable in <a href="https://github.com/bw2/ConfigArgParse/compare/1.5.5...1.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=configargparse&package-manager=pip&previous-version=1.5.5&new-version=1.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 12:06:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3034" class=".btn">#3034</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump uuid-utils from 0.7.0 to 0.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [uuid-utils](https://github.com/aminalaee/uuid-utils) from 0.7.0 to 0.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aminalaee/uuid-utils/releases">uuid-utils's releases</a>.</em></p>
<blockquote>
<h2>Version 0.8.0</h2>
<h3>Added</h3>
<ul>
<li>Add optional <code>nanos</code> argument to <code>uuid6</code> and <code>uuid7</code> by <a href="https://github.com/cstruct"><code>@​cstruct</code></a> in <a href="https://redirect.github.com/aminalaee/uuid-utils/pull/51">aminalaee/uuid-utils#51</a></li>
<li>Make <code>uuid3</code> and <code>uuid5</code> compatible with Python 3.12 by <a href="https://github.com/aminalaee"><code>@​aminalaee</code></a> in <a href="https://redirect.github.com/aminalaee/uuid-utils/pull/56">aminalaee/uuid-utils#56</a></li>
<li>Improve <code>compat</code> typings by <a href="https://github.com/aminalaee"><code>@​aminalaee</code></a> in <a href="https://redirect.github.com/aminalaee/uuid-utils/pull/55">aminalaee/uuid-utils#55</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/moritzwilksch"><code>@​moritzwilksch</code></a> made their first contribution in <a href="https://redirect.github.com/aminalaee/uuid-utils/pull/48">aminalaee/uuid-utils#48</a></li>
<li><a href="https://github.com/cstruct"><code>@​cstruct</code></a> made their first contribution in <a href="https://redirect.github.com/aminalaee/uuid-utils/pull/51">aminalaee/uuid-utils#51</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/aminalaee/uuid-utils/compare/0.7.0...0.8.0">https://github.com/aminalaee/uuid-utils/compare/0.7.0...0.8.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/43ca15c2e620ff0c3a823685d6dc4e64b772b01e"><code>43ca15c</code></a> Update release Action</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/1e9284887ac340d19477d361dca4fd110d3b0964"><code>1e92848</code></a> Version 0.8.0 (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/57">#57</a>)</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/2c2161fa753439ed953e4fa50893454e268a170a"><code>2c2161f</code></a> Make <code>uuid3</code> and <code>uuid5</code> compatible with Python 3.12 (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/56">#56</a>)</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/063eec8dd8e96a751eebb75d65d0073970c9159d"><code>063eec8</code></a> Improve compat typings (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/55">#55</a>)</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/88739a3f39a78d00d282332452df1d34bcc5420c"><code>88739a3</code></a> Add docs (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/53">#53</a>)</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/d4902b310364468680c6eae2a41d1a2f713acae6"><code>d4902b3</code></a> Remove <code>black</code> and <code>isort</code> (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/52">#52</a>)</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/8c9391bd9c56116c1054ad75b9c7d9bc3c4cfe1e"><code>8c9391b</code></a> Add optional <code>nanos</code> argument to <code>uuid6</code> and <code>uuid7</code> (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/51">#51</a>)</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/4838dddc1c773907d455c77eef38735237518c79"><code>4838ddd</code></a> Add conda install to Readme (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/48">#48</a>)</li>
<li>See full diff in <a href="https://github.com/aminalaee/uuid-utils/compare/0.7.0...0.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uuid-utils&package-manager=pip&previous-version=0.7.0&new-version=0.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 12:06:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3033" class=".btn">#3033</a>
            </td>
            <td>
                <b>
                    :sparkles: Add pagination support for listing Connection, Cred Ex, and Pres Ex records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Marking as draft to first confirm functionality works as expected

Edit: Success! I've written a local test to assert that limit/offset does indeed work as expected, and that unique records are returned across pages. 
___

This adds `limit` and `offset` query parameters to:
- listing connection records (in v1 connections API)
- listing credential exchange records (in v1 and v2 issue_credentials API)
- listing presentation exchange records (in v1 and v2 present_proof API)

As with #3000: the default behavior is now changed to no longer attempt to fetch all records for these endpoints. A default page size of 100 is used, with a maximum allowable page size of 10'000.

As you can see, adding the functionality is as simple as extending `PaginatedQuerySchema` for the query parameter schemas, and then to read limit and offset, and passing it to the Records.query method.

There are probably more endpoints where this functionality can be added, so I'm open for suggestions to apply the same elsewhere, but it should be straight forward enough for other contributors to add too.

These are just what I believe to be the essential endpoints, such that issuers/verifiers listing connections or exchange records won't try to read potentially millions of records.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 12:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3032" class=".btn">#3032</a>
            </td>
            <td>
                <b>
                    Prevent getting stuck with no active registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a problem where it was possible to get stuck in a state where a new registry wouldn't become active or created after rotating occurred when the tails server was unavailable.

Refactored some code in the revocation/indy module.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 18:58:49 +0000 UTC
    </div>
</div>

