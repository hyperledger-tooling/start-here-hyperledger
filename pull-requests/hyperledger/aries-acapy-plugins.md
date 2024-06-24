---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/640" class=".btn">#640</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /kafka_events/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events/integration with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:29:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/639" class=".btn">#639</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /firebase_push_notifications/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /firebase_push_notifications/integration with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:28:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/638" class=".btn">#638</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /rpc/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /rpc/integration with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:28:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/637" class=".btn">#637</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /multitenant_provider/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /multitenant_provider/integration with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:28:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /basicmessage_storage/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /basicmessage_storage/integration with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:28:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/635" class=".btn">#635</a>
            </td>
            <td>
                <b>
                    Bump pydantic from 1.10.15 to 1.10.16 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydantic](https://github.com/pydantic/pydantic) from 1.10.15 to 1.10.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<h2>What's Changed</h2>
<ul>
<li>Import modules/objects directly from <code>v1</code> namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Specify <code>recursive_guard</code> as kwarg in <code>FutureRef._evaluate</code> by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li><a href="https://github.com/vfazio"><code>@​vfazio</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<ul>
<li>Specify recursive_guard as kwarg in FutureRef._evaluate by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by @ cdce8p in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Import modules/objects directly from v1 namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/211910eccce116f0f25964e81c09e87fd98a351c"><code>211910e</code></a> v1.10.16 prep (<a href="https://redirect.github.com/pydantic/pydantic/issues/9630">#9630</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/464ed49b1f813103a49116476bec75a94492b338"><code>464ed49</code></a> Specify recursive_guard as kwarg in FutureRef._evaluate (<a href="https://redirect.github.com/pydantic/pydantic/issues/9612">#9612</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/9eaa67bdf8954c21195cef6128489755351046ec"><code>9eaa67b</code></a> Fix mypy v1 plugin for upcoming mypy release (<a href="https://redirect.github.com/pydantic/pydantic/issues/9586">#9586</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/5adc3815da35a8efeb7ff74418d7c0fb00b0fef7"><code>5adc381</code></a> Import modules/objects directly from v1 namespace (<a href="https://redirect.github.com/pydantic/pydantic/issues/9162">#9162</a>)</li>
<li>See full diff in <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic&package-manager=pip&previous-version=1.10.15&new-version=1.10.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 12:07:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/634" class=".btn">#634</a>
            </td>
            <td>
                <b>
                    Bump redis from 5.0.4 to 5.0.6 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [redis](https://github.com/redis/redis-py) from 5.0.4 to 5.0.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/releases">redis's releases</a>.</em></p>
<blockquote>
<h2>5.0.6</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Handle lists in the response of INFO</li>
</ul>
<h2>5.0.5</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3265">#3265</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/redis/redis-py/commit/40a90926b97593d04591f4a3a67706c2a15a2b89"><code>40a9092</code></a> Handle lists in the response of INFO (<a href="https://redirect.github.com/redis/redis-py/issues/3277">#3277</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/6f55c0286ccc444204a23e8738117f43c182bf9b"><code>6f55c02</code></a> Bump version to 5.0.5 (<a href="https://redirect.github.com/redis/redis-py/issues/3267">#3267</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/26d2d13edcf3f29a381df4850c5926cb285d3584"><code>26d2d13</code></a> Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3264">#3264</a>)</li>
<li>See full diff in <a href="https://github.com/redis/redis-py/compare/v5.0.4...v5.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=redis&package-manager=pip&previous-version=5.0.4&new-version=5.0.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 12:06:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/633" class=".btn">#633</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:58:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/632" class=".btn">#632</a>
            </td>
            <td>
                <b>
                    Bump pydantic from 1.10.15 to 1.10.16 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydantic](https://github.com/pydantic/pydantic) from 1.10.15 to 1.10.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<h2>What's Changed</h2>
<ul>
<li>Import modules/objects directly from <code>v1</code> namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Specify <code>recursive_guard</code> as kwarg in <code>FutureRef._evaluate</code> by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li><a href="https://github.com/vfazio"><code>@​vfazio</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<ul>
<li>Specify recursive_guard as kwarg in FutureRef._evaluate by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by @ cdce8p in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Import modules/objects directly from v1 namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/211910eccce116f0f25964e81c09e87fd98a351c"><code>211910e</code></a> v1.10.16 prep (<a href="https://redirect.github.com/pydantic/pydantic/issues/9630">#9630</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/464ed49b1f813103a49116476bec75a94492b338"><code>464ed49</code></a> Specify recursive_guard as kwarg in FutureRef._evaluate (<a href="https://redirect.github.com/pydantic/pydantic/issues/9612">#9612</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/9eaa67bdf8954c21195cef6128489755351046ec"><code>9eaa67b</code></a> Fix mypy v1 plugin for upcoming mypy release (<a href="https://redirect.github.com/pydantic/pydantic/issues/9586">#9586</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/5adc3815da35a8efeb7ff74418d7c0fb00b0fef7"><code>5adc381</code></a> Import modules/objects directly from v1 namespace (<a href="https://redirect.github.com/pydantic/pydantic/issues/9162">#9162</a>)</li>
<li>See full diff in <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic&package-manager=pip&previous-version=1.10.15&new-version=1.10.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/631" class=".btn">#631</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:57:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Bump redis from 5.0.4 to 5.0.6 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [redis](https://github.com/redis/redis-py) from 5.0.4 to 5.0.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/releases">redis's releases</a>.</em></p>
<blockquote>
<h2>5.0.6</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Handle lists in the response of INFO</li>
</ul>
<h2>5.0.5</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3265">#3265</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/redis/redis-py/commit/40a90926b97593d04591f4a3a67706c2a15a2b89"><code>40a9092</code></a> Handle lists in the response of INFO (<a href="https://redirect.github.com/redis/redis-py/issues/3277">#3277</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/6f55c0286ccc444204a23e8738117f43c182bf9b"><code>6f55c02</code></a> Bump version to 5.0.5 (<a href="https://redirect.github.com/redis/redis-py/issues/3267">#3267</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/26d2d13edcf3f29a381df4850c5926cb285d3584"><code>26d2d13</code></a> Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3264">#3264</a>)</li>
<li>See full diff in <a href="https://github.com/redis/redis-py/compare/v5.0.4...v5.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=redis&package-manager=pip&previous-version=5.0.4&new-version=5.0.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:56:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    Bump pydantic from 1.10.15 to 1.10.16 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydantic](https://github.com/pydantic/pydantic) from 1.10.15 to 1.10.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<h2>What's Changed</h2>
<ul>
<li>Import modules/objects directly from <code>v1</code> namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Specify <code>recursive_guard</code> as kwarg in <code>FutureRef._evaluate</code> by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li><a href="https://github.com/vfazio"><code>@​vfazio</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<ul>
<li>Specify recursive_guard as kwarg in FutureRef._evaluate by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by @ cdce8p in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Import modules/objects directly from v1 namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/211910eccce116f0f25964e81c09e87fd98a351c"><code>211910e</code></a> v1.10.16 prep (<a href="https://redirect.github.com/pydantic/pydantic/issues/9630">#9630</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/464ed49b1f813103a49116476bec75a94492b338"><code>464ed49</code></a> Specify recursive_guard as kwarg in FutureRef._evaluate (<a href="https://redirect.github.com/pydantic/pydantic/issues/9612">#9612</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/9eaa67bdf8954c21195cef6128489755351046ec"><code>9eaa67b</code></a> Fix mypy v1 plugin for upcoming mypy release (<a href="https://redirect.github.com/pydantic/pydantic/issues/9586">#9586</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/5adc3815da35a8efeb7ff74418d7c0fb00b0fef7"><code>5adc381</code></a> Import modules/objects directly from v1 namespace (<a href="https://redirect.github.com/pydantic/pydantic/issues/9162">#9162</a>)</li>
<li>See full diff in <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic&package-manager=pip&previous-version=1.10.15&new-version=1.10.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/628" class=".btn">#628</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:46:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Bump pydantic from 1.10.15 to 1.10.16 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydantic](https://github.com/pydantic/pydantic) from 1.10.15 to 1.10.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<h2>What's Changed</h2>
<ul>
<li>Import modules/objects directly from <code>v1</code> namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Specify <code>recursive_guard</code> as kwarg in <code>FutureRef._evaluate</code> by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
<li><a href="https://github.com/vfazio"><code>@​vfazio</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.16 (2024-06-11)</h2>
<ul>
<li>Specify recursive_guard as kwarg in FutureRef._evaluate by <a href="https://github.com/vfazio"><code>@​vfazio</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9612">pydantic/pydantic#9612</a></li>
<li>Fix mypy v1 plugin for upcoming mypy release by @ cdce8p in <a href="https://redirect.github.com/pydantic/pydantic/pull/9586">pydantic/pydantic#9586</a></li>
<li>Import modules/objects directly from v1 namespace by <a href="https://github.com/exs-dwoodward"><code>@​exs-dwoodward</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9162">pydantic/pydantic#9162</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/211910eccce116f0f25964e81c09e87fd98a351c"><code>211910e</code></a> v1.10.16 prep (<a href="https://redirect.github.com/pydantic/pydantic/issues/9630">#9630</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/464ed49b1f813103a49116476bec75a94492b338"><code>464ed49</code></a> Specify recursive_guard as kwarg in FutureRef._evaluate (<a href="https://redirect.github.com/pydantic/pydantic/issues/9612">#9612</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/9eaa67bdf8954c21195cef6128489755351046ec"><code>9eaa67b</code></a> Fix mypy v1 plugin for upcoming mypy release (<a href="https://redirect.github.com/pydantic/pydantic/issues/9586">#9586</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/5adc3815da35a8efeb7ff74418d7c0fb00b0fef7"><code>5adc381</code></a> Import modules/objects directly from v1 namespace (<a href="https://redirect.github.com/pydantic/pydantic/issues/9162">#9162</a>)</li>
<li>See full diff in <a href="https://github.com/pydantic/pydantic/compare/v1.10.15...v1.10.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic&package-manager=pip&previous-version=1.10.15&new-version=1.10.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Bump redis from 5.0.4 to 5.0.6 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [redis](https://github.com/redis/redis-py) from 5.0.4 to 5.0.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/releases">redis's releases</a>.</em></p>
<blockquote>
<h2>5.0.6</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Handle lists in the response of INFO</li>
</ul>
<h2>5.0.5</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3265">#3265</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/redis/redis-py/commit/40a90926b97593d04591f4a3a67706c2a15a2b89"><code>40a9092</code></a> Handle lists in the response of INFO (<a href="https://redirect.github.com/redis/redis-py/issues/3277">#3277</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/6f55c0286ccc444204a23e8738117f43c182bf9b"><code>6f55c02</code></a> Bump version to 5.0.5 (<a href="https://redirect.github.com/redis/redis-py/issues/3267">#3267</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/26d2d13edcf3f29a381df4850c5926cb285d3584"><code>26d2d13</code></a> Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3264">#3264</a>)</li>
<li>See full diff in <a href="https://github.com/redis/redis-py/compare/v5.0.4...v5.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=redis&package-manager=pip&previous-version=5.0.4&new-version=5.0.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:43:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/625" class=".btn">#625</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:43:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /oid4vci/integration/afj_runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:34:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:31:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/622" class=".btn">#622</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    Bump prettier from 3.0.3 to 3.3.2 in /oid4vci/integration/afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [prettier](https://github.com/prettier/prettier) from 3.0.3 to 3.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/releases">prettier's releases</a>.</em></p>
<blockquote>
<h2>3.3.2</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#332">Changelog</a></p>
<h2>3.3.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#331">Changelog</a></p>
<h2>3.3.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.2.5...3.3.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/06/01/3.3.0.html">Release note</a></p>
<h2>3.2.5</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#325">Changelog</a></p>
<h2>3.2.4</h2>
<ul>
<li>Fix <code>.eslintrc.json</code> format <a href="https://redirect.github.com/prettier/prettier/issues/15947">#15947</a></li>
</ul>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#324">Changelog</a></p>
<h2>3.2.3</h2>
<ul>
<li>Format <code>tsconfig.json</code> file with <code>jsonc</code> parser <a href="https://redirect.github.com/prettier/prettier/issues/15927">#15927</a></li>
</ul>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#323">Changelog</a></p>
<h2>3.2.2</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#322">Changelog</a></p>
<h2>3.2.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#321">Changelog</a></p>
<h2>3.2.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.1.1...3.2.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/01/12/3.2.0.html">Release note</a></p>
<h2>3.1.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#311">Changelog</a></p>
<h2>3.1.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.0.3...3.1.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2023/11/13/3.1.0.html">Release note</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md">prettier's changelog</a>.</em></p>
<blockquote>
<h1>3.3.2</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.3.1...3.3.2">diff</a></p>
<h4>Fix handlebars path expressions starts with <code>@</code> (<a href="https://redirect.github.com/prettier/prettier/pull/16358">#16358</a> by <a href="https://github.com/Princeyadav05"><code>@​Princeyadav05</code></a>)</h4>
<!-- raw HTML omitted -->
<pre lang="hbs"><code>{{! Input }}
&lt;div&gt;{{@x.y.z}}&lt;/div&gt;
<p>{{! Prettier 3.3.1 }}
&lt;div&gt;{{<a href="https://github.com/x"><code>@​x</code></a>}}&lt;/div&gt;</p>
<p>{{! Prettier 3.3.2 }}
&lt;div&gt;{{<a href="https://github.com/x"><code>@​x</code></a>.y.z}}&lt;/div&gt;
</code></pre></p>
<h1>3.3.1</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.3.0...3.3.1">diff</a></p>
<h4>Preserve empty lines in front matter (<a href="https://redirect.github.com/prettier/prettier/pull/16347">#16347</a> by <a href="https://github.com/fisker"><code>@​fisker</code></a>)</h4>
<!-- raw HTML omitted -->
<pre lang="markdown"><code>&lt;!-- Input --&gt;
---
foo:
  - bar1
<ul>
<li>
<p>bar2</p>
</li>
<li>
<p>bar3</p>
</li>
</ul>
<hr />
<p>Markdown</p>
<p>&lt;!-- Prettier 3.3.0 --&gt;</p>
<hr />
<p>foo:</p>
<ul>
<li>bar1</li>
<li>bar2</li>
<li>bar3</li>
</ul>
<hr />
<p>Markdown</p>
<p>&lt;!-- Prettier 3.3.1 --&gt;
&lt;/tr&gt;&lt;/table&gt;
</code></pre></p>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prettier/prettier/commit/1596a608dedac55c20bad3f1b5bfd47f961c696b"><code>1596a60</code></a> Release 3.3.2</li>
<li><a href="https://github.com/prettier/prettier/commit/aebcee5ea49ff0ee934ce39d26edb09cbd3f17db"><code>aebcee5</code></a> chore(deps): update dependency esbuild to v0.21.5 (<a href="https://redirect.github.com/prettier/prettier/issues/16379">#16379</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/57aa9287a078f0ed266e779bd00528fff2598bb2"><code>57aa928</code></a> chore(deps): update dependency c8 to v10 (<a href="https://redirect.github.com/prettier/prettier/issues/16380">#16380</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/c3d0b7f419f6f51876bbb1fc36b9755b8c9dcb8e"><code>c3d0b7f</code></a> chore(deps): update typescript-eslint to v7.13.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16376">#16376</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/27c35db5e20a121aad0cc3fff7a80658b7503ea0"><code>27c35db</code></a> chore(deps): update dependency codemirror-graphql to v2.0.12 (<a href="https://redirect.github.com/prettier/prettier/issues/16369">#16369</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/6de325866695e23269d0d217cf73c4cc0340226e"><code>6de3258</code></a> chore(deps): update dependency jest to v30.0.0-alpha.5 (<a href="https://redirect.github.com/prettier/prettier/issues/16371">#16371</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/b5f983d2bb24ae78ba560c7d57c4b1753ea32cfa"><code>b5f983d</code></a> Upgrade yarn to v4.3.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16377">#16377</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/d6f37c4109e97fdfa054d7af147e82495a18d1c7"><code>d6f37c4</code></a> chore(deps): update dependency browserslist to v4.23.1 (<a href="https://redirect.github.com/prettier/prettier/issues/16368">#16368</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/5055b7d39265fddae29917390c83ef28df497f23"><code>5055b7d</code></a> chore(deps): update dependency execa to v9.2.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16372">#16372</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/f4608cc76b097a03487f00132a904dea1312c56d"><code>f4608cc</code></a> chore(deps): update dependency cspell to v8.8.4 (<a href="https://redirect.github.com/prettier/prettier/issues/16370">#16370</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/prettier/prettier/compare/3.0.3...3.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=prettier&package-manager=npm_and_yarn&previous-version=3.0.3&new-version=3.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:26:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:14:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.9 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:13:43 +0000 UTC
    </div>
</div>

