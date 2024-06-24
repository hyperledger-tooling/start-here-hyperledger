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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    Upgrade all nested poetry lock files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This just improves the script a bit by searching for and upgrading the nested projects like integration tests and others.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 23:36:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    General upgrade of ruff
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
        Created At 2024-06-17 23:33:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/654" class=".btn">#654</a>
            </td>
            <td>
                <b>
                    General upgrade urllib3
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
        Created At 2024-06-17 23:31:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/653" class=".btn">#653</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /firebase_push_notifications in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /firebase_push_notifications with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:31:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /multitenant_provider in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /multitenant_provider with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:31:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    Bump the npm_and_yarn group in /oid4vci/integration/afj with 7 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group in /oid4vci/integration/afj with 7 updates:

| Package | From | To |
| --- | --- | --- |
| [semver](https://github.com/npm/node-semver) | `5.7.2` | `7.5.4` |
| [expo](https://github.com/expo/expo/tree/HEAD/packages/expo) | `49.0.17` | `51.0.14` |
| [ws](https://github.com/websockets/ws) | `6.2.2` | `6.2.3` |
| [braces](https://github.com/micromatch/braces) | `3.0.2` | `3.0.3` |
| [express](https://github.com/expressjs/express) | `4.18.2` | `4.19.2` |
| [ip](https://github.com/indutny/node-ip) | `1.1.9` | `removed` |
| [react-native](https://github.com/facebook/react-native/tree/HEAD/packages/react-native) | `0.72.6` | `0.74.2` |

Updates `semver` from 5.7.2 to 7.5.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.5.4</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.1</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2>v7.5.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2>v7.4.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/113f51312a1a6b6aa50d4f9486b4fde21782c1f5"><code>113f513</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/532">#532</a> identifierBase parameter for .inc (<a href="https://redirect.github.com/npm/node-semver/issues/532">#532</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/b-bly"><code>@​b-bly</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/48d8f8fa63bf6e35db70ff840b6da1a51596a5a8"><code>48d8f8f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/530">#530</a> export new RELEASE_TYPES constant (<a href="https://github.com/hcharley"><code>@​hcharley</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/36cd334708ec1f85a71445622fb1864bceee0f4e"><code>36cd334</code></a> chore: release 7.5.4</li>
<li><a href="https://github.com/npm/node-semver/commit/8456d87971a447ce295d9f1a396b37b29a972a63"><code>8456d87</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dde1f002baadf7b4cc45504c4046d13586de11b7"><code>dde1f00</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dffcd1b07ec6a192bc0fb405d30d19da46fdc690"><code>dffcd1b</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.16.0 to 4.17.0</li>
<li><a href="https://github.com/npm/node-semver/commit/d619f66513a0fa953177882ecee2c365a65efe97"><code>d619f66</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/3bc42477d1a69361eb79978851be090e5fb4bc2a"><code>3bc4247</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.15.1 to 4.16.0</li>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> fix: trim each range set before parsing</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> fix: correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/4f0f6b19a54b1ba7e1c62af2dfba61f7a4fa68d5"><code>4f0f6b1</code></a> chore: fix arguments in whitespace test (<a href="https://redirect.github.com/npm/node-semver/issues/574">#574</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6bd1a37f95904512015353a3a5dd726f785c9eb8"><code>6bd1a37</code></a> chore: remove duplicate test in semver class (<a href="https://redirect.github.com/npm/node-semver/issues/575">#575</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v5.7.2...v7.5.4">compare view</a></li>
</ul>
</details>
<br />

Updates `expo` from 49.0.17 to 51.0.14
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expo/expo/blob/main/CHANGELOG.md">expo's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<p>This is the log of notable changes to the Expo client that are developer-facing.
Package-specific changes not released in any SDK will be added here just before the release. Until then, you can find them in changelogs of the individual packages (see <a href="https://github.com/expo/expo/blob/main/packages">packages</a> directory).</p>
<h2>Unpublished</h2>
<h3>📚 3rd party library updates</h3>
<h3>🛠 Breaking changes</h3>
<h3>🎉 New features</h3>
<h3>🐛 Bug fixes</h3>
<h2>51.0.0 — 2024-05-07</h2>
<h3>🛠 Breaking changes</h3>
<ul>
<li><strong><code>expo-auth-session</code></strong>
<ul>
<li>Drop deprecated <code>expoClientId</code> field from auth proxy. (<a href="https://redirect.github.com/expo/expo/pull/28590">#28590</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-barcode-scanner</code></strong>
<ul>
<li><code>expo-barcode-scanner</code> is now deprecated. Please use <code>expo-camera</code> instead. (<a href="https://redirect.github.com/expo/expo/pull/26025">#26025</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-constants</code></strong>
<ul>
<li>Remove deprecated installationId, isDevice, nativeAppVersion, nativeBuildVersion, platform.platform, platform.systemVersion, platform.userInterfaceIdiom properties. (<a href="https://redirect.github.com/expo/expo/pull/26329">#26329</a> by <a href="https://github.com/aleqsio"><code>@​aleqsio</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-face-detector</code></strong>
<ul>
<li><code>expo-face-detector</code> is now deprecated. We recommed using <a href="https://github.com/mrousavy/react-native-vision-camera">react-native-vision-camera</a> instead. (<a href="https://redirect.github.com/expo/expo/pull/26026">#26026</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-location</code></strong>
<ul>
<li>[Web] <code>getPermissionsAsync</code> no longer prompts the user for permission instead we use the new browser API <code>navigator.permissions.query</code> to check the permission status. (<a href="https://redirect.github.com/expo/expo/pull/26837">#26836</a> by <a href="https://github.com/hems"><code>@​hems</code></a>) (<a href="https://redirect.github.com/expo/expo/pull/26837">#26837</a> by <a href="https://github.com/hems"><code>@​hems</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-local-authentication</code></strong>
<ul>
<li><code>SecurityLevel.BIOMETRIC</code> has been deprecated in favour of <code>SecurityLevel.BIOMETRIC_STRONG</code> and <code>SecurityLevel.BIOMETRIC_WEAK</code>. Using <code>SecurityLevel.BIOMETRIC</code> might lead to unexpected behaviour. (<a href="https://redirect.github.com/expo/expo/pull/26768">#26768</a> by <a href="https://github.com/behenate"><code>@​behenate</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-modules-core</code></strong>
<ul>
<li>Removed <code>ReactNativeHostHandler.onRegisterJSIModules</code> interface. (<a href="https://redirect.github.com/expo/expo/pull/26357">#26357</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
<li>Dropped supports for React Native 0.73 and lower. (<a href="https://redirect.github.com/expo/expo/pull/27601">#27601</a>, <a href="https://redirect.github.com/expo/expo/pull/27689">#27689</a>, <a href="https://redirect.github.com/expo/expo/pull/27629">#27629</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-sms</code></strong>
<ul>
<li>[web] <code>sendSMSAsync</code> now throws error code <code>ERR_UNAVAILABLE</code> instead of <code>E_SMS_UNAVAILABLE</code>. (<a href="https://redirect.github.com/expo/expo/pull/27437">#27437</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-sqlite</code></strong>
<ul>
<li>Refactor <code>expo-sqlite/next</code> API to be more React idiomatic. (<a href="https://redirect.github.com/expo/expo/pull/25657">#25657</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
<li>Moved the previous default export as <code>expo-sqlite/legacy</code> and promoted <code>expo-sqlite/next</code> as the default. <code>expo-sqlite/next</code> import is still as-is for backward compatibility. (<a href="https://redirect.github.com/expo/expo/pull/28278">#28278</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
</ul>
</li>
</ul>
<h3>🎉 New features</h3>
<ul>
<li><strong><code>expo-barcode-scanner</code></strong>
<ul>
<li><code>BarCodeScannerResult</code> now returns an additional <code>raw</code> field corresponding to the barcode value as it was encoded in the barcode without parsing. Will always be undefined on iOS. (<a href="https://redirect.github.com/expo/expo/pull/25391">#25391</a> by <a href="https://github.com/ajacquierbret"><code>@​ajacquierbret</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-blur</code></strong>
<ul>
<li>Added support for Apple tvOS. (<a href="https://redirect.github.com/expo/expo/pull/26965">#26965</a> by <a href="https://github.com/douglowder"><code>@​douglowder</code></a>)</li>
<li>Mark React client components with &quot;use client&quot; directives. (<a href="https://redirect.github.com/expo/expo/pull/27300">#27300</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-asset</code></strong>
<ul>
<li>Added config plugin to allow assets to be linked at build time. (<a href="https://redirect.github.com/expo/expo/pull/27052">#27052</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
<li>Add Apple TV support to the new iOS native module. (<a href="https://redirect.github.com/expo/expo/pull/27823">#27823</a> by <a href="https://github.com/douglowder"><code>@​douglowder</code></a>)</li>
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
<li>See full diff in <a href="https://github.com/expo/expo/commits/HEAD/packages/expo">compare view</a></li>
</ul>
</details>
<br />

Updates `ws` from 6.2.2 to 6.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>6.2.3</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 6.x release line (eeb76d31).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d87f3b6d3a00513af9bbb74f45ba9183af4e5f43"><code>d87f3b6</code></a> [dist] 6.2.3</li>
<li><a href="https://github.com/websockets/ws/commit/eeb76d313e2a00dd5247ca3597bba7877d064a63"><code>eeb76d3</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/6.2.2...6.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `braces` from 3.0.2 to 3.0.3
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/micromatch/braces/commit/74b2db2938fad48a2ea54a9c8bf27a37a62c350d"><code>74b2db2</code></a> 3.0.3</li>
<li><a href="https://github.com/micromatch/braces/commit/88f1429a0f47e1dd3813de35211fc97ffda27f9e"><code>88f1429</code></a> update eslint. lint, fix unit tests.</li>
<li><a href="https://github.com/micromatch/braces/commit/415d660c3002d1ab7e63dbf490c9851da80596ff"><code>415d660</code></a> Snyk js braces 6838727 (<a href="https://redirect.github.com/micromatch/braces/issues/40">#40</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/190510f79db1adf21d92798b0bb6fccc1f72c9d6"><code>190510f</code></a> fix tests, skip 1 test in test/braces.expand</li>
<li><a href="https://github.com/micromatch/braces/commit/716eb9f12d820b145a831ad678618731927e8856"><code>716eb9f</code></a> readme bump</li>
<li><a href="https://github.com/micromatch/braces/commit/a5851e57f45c3431a94d83fc565754bc10f5bbc3"><code>a5851e5</code></a> Merge pull request <a href="https://redirect.github.com/micromatch/braces/issues/37">#37</a> from coderaiser/fix/vulnerability</li>
<li><a href="https://github.com/micromatch/braces/commit/2092bd1fb108d2c59bd62e243b70ad98db961538"><code>2092bd1</code></a> feature: braces: add maxSymbols (<a href="https://github.com/micromatch/braces/issues/">https://github.com/micromatch/braces/issues/</a>...</li>
<li><a href="https://github.com/micromatch/braces/commit/9f5b4cf47329351bcb64287223ffb6ecc9a5e6d3"><code>9f5b4cf</code></a> fix: vulnerability (<a href="https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727">https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/98414f9f1fabe021736e26836d8306d5de747e0d"><code>98414f9</code></a> remove funding file</li>
<li><a href="https://github.com/micromatch/braces/commit/665ab5d561c017a38ba7aafd92cc6655b91d8c14"><code>665ab5d</code></a> update keepEscaping doc (<a href="https://redirect.github.com/micromatch/braces/issues/27">#27</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/micromatch/braces/compare/3.0.2...3.0.3">compare view</a></li>
</ul>
</details>
<br />

Updates `express` from 4.18.2 to 4.19.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.19.2</h2>
<h2>What's Changed</h2>
<ul>
<li><a href="https://github.com/expressjs/express/commit/0b746953c4bd8e377123527db11f9cd866e39f94">Improved fix for open redirect allow list bypass</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/expressjs/express/compare/4.19.1...4.19.2">https://github.com/expressjs/express/compare/4.19.1...4.19.2</a></p>
<h2>4.19.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix ci after location patch by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5552">expressjs/express#5552</a></li>
<li>fixed un-edited version in history.md for 4.19.0 by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5556">expressjs/express#5556</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/expressjs/express/compare/4.19.0...4.19.1">https://github.com/expressjs/express/compare/4.19.0...4.19.1</a></p>
<h2>4.19.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix typo in release date by <a href="https://github.com/UlisesGascon"><code>@​UlisesGascon</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5527">expressjs/express#5527</a></li>
<li>docs: nominating <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> to be project captian by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5511">expressjs/express#5511</a></li>
<li>docs: loosen TC activity rules by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5510">expressjs/express#5510</a></li>
<li>Add note on how to update docs for new release by <a href="https://github.com/crandmck"><code>@​crandmck</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5541">expressjs/express#5541</a></li>
<li><a href="https://redirect.github.com/expressjs/express/pull/5551/commits/660ccf5fa33dd0baab069e5c8ddd9ffe7d8bbff1">Prevent open redirect allow list bypass due to encodeurl</a></li>
<li>Release 4.19.0 by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5551">expressjs/express#5551</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/crandmck"><code>@​crandmck</code></a> made their first contribution in <a href="https://redirect.github.com/expressjs/express/pull/5541">expressjs/express#5541</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/expressjs/express/compare/4.18.3...4.19.0">https://github.com/expressjs/express/compare/4.18.3...4.19.0</a></p>
<h2>4.18.3</h2>
<h2>Main Changes</h2>
<ul>
<li>Fix routing requests without method</li>
<li>deps: body-parser@1.20.2
<ul>
<li>Fix strict json error message on Node.js 19+</li>
<li>deps: content-type@~1.0.5</li>
<li>deps: raw-body@2.5.2</li>
</ul>
</li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Use https: protocol instead of deprecated git: protocol by <a href="https://github.com/vcsjones"><code>@​vcsjones</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5032">expressjs/express#5032</a></li>
<li>build: Node.js@16.18 and Node.js@18.12 by <a href="https://github.com/abenhamdine"><code>@​abenhamdine</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5034">expressjs/express#5034</a></li>
<li>ci: update actions/checkout to v3 by <a href="https://github.com/armujahid"><code>@​armujahid</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5027">expressjs/express#5027</a></li>
<li>test: remove unused function arguments in params by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5124">expressjs/express#5124</a></li>
<li>Remove unused originalIndex from acceptParams by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5119">expressjs/express#5119</a></li>
<li>Fixed typos by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5117">expressjs/express#5117</a></li>
<li>examples: remove unused params by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5113">expressjs/express#5113</a></li>
<li>fix: parameter str is not described in JSDoc by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5130">expressjs/express#5130</a></li>
<li>fix: typos in History.md by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5131">expressjs/express#5131</a></li>
<li>build : add Node.js@19.7 by <a href="https://github.com/abenhamdine"><code>@​abenhamdine</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5028">expressjs/express#5028</a></li>
<li>test: remove unused function arguments in params by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5137">expressjs/express#5137</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.19.2 / 2024-03-25</h1>
<ul>
<li>Improved fix for open redirect allow list bypass</li>
</ul>
<h1>4.19.1 / 2024-03-20</h1>
<ul>
<li>Allow passing non-strings to res.location with new encoding handling checks</li>
</ul>
<h1>4.19.0 / 2024-03-20</h1>
<ul>
<li>Prevent open redirect allow list bypass due to encodeurl</li>
<li>deps: cookie@0.6.0</li>
</ul>
<h1>4.18.3 / 2024-02-29</h1>
<ul>
<li>Fix routing requests without method</li>
<li>deps: body-parser@1.20.2
<ul>
<li>Fix strict json error message on Node.js 19+</li>
<li>deps: content-type@~1.0.5</li>
<li>deps: raw-body@2.5.2</li>
</ul>
</li>
<li>deps: cookie@0.6.0
<ul>
<li>Add <code>partitioned</code> option</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/04bc62787be974874bc1467b23606c36bc9779ba"><code>04bc627</code></a> 4.19.2</li>
<li><a href="https://github.com/expressjs/express/commit/da4d763ff6ba9df6dbd8f1f0b1d05412dda934d5"><code>da4d763</code></a> Improved fix for open redirect allow list bypass</li>
<li><a href="https://github.com/expressjs/express/commit/4f0f6cc67d531431c096ea006c2191b92931bbc3"><code>4f0f6cc</code></a> 4.19.1</li>
<li><a href="https://github.com/expressjs/express/commit/a003cfab034fbadb1c78ae337ee8ab389adda217"><code>a003cfa</code></a> Allow passing non-strings to res.location with new encoding handling checks f...</li>
<li><a href="https://github.com/expressjs/express/commit/a1fa90fcea7d8e844e1c9938ad095d62669c3abd"><code>a1fa90f</code></a> fixed un-edited version in history.md for 4.19.0</li>
<li><a href="https://github.com/expressjs/express/commit/11f2b1db227fd42c2508c427032c1ec671b306be"><code>11f2b1d</code></a> build: fix build due to inconsistent supertest behavior in older versions</li>
<li><a href="https://github.com/expressjs/express/commit/084e36506a18774f85206a65d8da04dc1107fc1b"><code>084e365</code></a> 4.19.0</li>
<li><a href="https://github.com/expressjs/express/commit/0867302ddbde0e9463d0564fea5861feb708c2dd"><code>0867302</code></a> Prevent open redirect allow list bypass due to encodeurl</li>
<li><a href="https://github.com/expressjs/express/commit/567c9c665d0de4c344b8e160146050770233783c"><code>567c9c6</code></a> Add note on how to update docs for new release (<a href="https://redirect.github.com/expressjs/express/issues/5541">#5541</a>)</li>
<li><a href="https://github.com/expressjs/express/commit/69a4cf2819c4449ec6ea45649691fb43a528d5d1"><code>69a4cf2</code></a> deps: cookie@0.6.0</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.18.2...4.19.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~wesleytodd">wesleytodd</a>, a new releaser for express since your current version.</p>
</details>
<br />

Removes `ip`

Updates `react-native` from 0.72.6 to 0.74.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/releases">react-native's releases</a>.</em></p>
<blockquote>
<h2>0.74.2</h2>
<h3>Changed</h3>
<ul>
<li>Updated <code>typescript-eslint</code> monorepo to <code>v7</code>
(<a href="https://github.com/facebook/react-native/commit/91d725136e8fe0fd55fdfca5a4f5bd8ab527f94e">91d725136e</a> by <a href="https://github.com/huntie"><code>@​huntie</code></a>)</li>
<li>Upgrade CLI to <code>13.6.8</code> (<a href="https://github.com/facebook/react-native/commit/335f6ed83306bfa150c818d26dce4b279de4869f">335f6ed833</a> by <a href="https://github.com/szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Warn only in <code>init</code> command when CLI uses cached <code>npx</code> version (<a href="https://github.com/facebook/react-native/commit/b98c5b960ccc4fe9d2792c35994c414c709a3d7a">b98c5b960c</a> by <a href="https://github.com/szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
<li><code>selection</code> prop in <code>TextInput</code> was not being applied at component creation (<a href="https://github.com/facebook/react-native/commit/be09d12667044f237f08af410b2838062eb8e657">be09d12667</a> by <a href="https://github.com/alanleedev"><code>@​alanleedev</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Fixed dangling <code>mAttachedSurfaces</code> after <code>ReactHost.destroy()</code> (<a href="https://github.com/facebook/react-native/commit/c70d7910361f56bc361ad825fe13fb2178edfeba">c70d791036</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
<li>ReactSoftExceptions in ReactHostImpl only when Context is null (<a href="https://github.com/facebook/react-native/commit/ac3261ff608768ff43736b413c5a5ad67668af61">ac3261ff60</a> by <a href="https://github.com/arushikesarwani94"><code>@​arushikesarwani94</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Privacy Manifest aggregation failing due to no <code>NSPrivacyAccessedAPITypes</code> key (<a href="https://github.com/facebook/react-native/commit/fc4e0999206ec7c1f465bb2b1fea987e43485a82">fc4e099920</a> by <a href="https://github.com/renchap"><code>@​renchap</code></a>)</li>
<li>In privacy manifest post install script, handle the case where the file reference doesn't have a path (<a href="https://github.com/facebook/react-native/commit/4ad65ac59a2491db598abb7b32fb793e9693d5ac">4ad65ac59a</a> by <a href="https://github.com/robertying"><code>@​robertying</code></a>)</li>
<li>Fixed an issue where the <code>selectionColor</code> prop was not being applied on the <code>TextInput</code> component. (<a href="https://github.com/facebook/react-native/commit/2bde626a9fa2f782864937a5258ac494afe27f9f">2bde626a9f</a> by <a href="https://github.com/robinshin"><code>@​robinshin</code></a>)</li>
</ul>
<hr />
<!-- raw HTML omitted -->
<p>Hermes dSYMS:</p>
<ul>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.2/react-native-artifacts-0.74.2-hermes-framework-dSYM-debug.tar.gz">Debug</a></li>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.2/react-native-artifacts-0.74.2-hermes-framework-dSYM-release.tar.gz">Release</a></li>
</ul>
<hr />
<p>You can file issues or pick requests against this release <a href="https://github.com/reactwg/react-native-releases/issues/new/choose">here</a>.</p>
<hr />
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/">Upgrade Helper</a> ⚛️.</p>
<hr />
<p>View the whole changelog in the <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG.md">CHANGELOG.md file</a>.</p>
<h2>0.74.1</h2>
<h3>Added</h3>
<h4>iOS Specific</h4>
<ul>
<li>Implement privacy manifest aggregation  (<a href="https://github.com/facebook/react-native/commit/4be1fafec8edca5da5ebe515ad359d4178db7d23">4be1fafec8</a> by <a href="https://github.com/@aleqsio"><code>@​aleqsio</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG.md">react-native's changelog</a>.</em></p>
<blockquote>
<h2>v0.74.2</h2>
<h3>Changed</h3>
<ul>
<li>Updated <code>typescript-eslint</code> monorepo to <code>v7</code>
(<a href="https://github.com/facebook/react-native/commit/91d725136e8fe0fd55fdfca5a4f5bd8ab527f94e">91d725136e</a> by <a href="https://github.com/huntie"><code>@​huntie</code></a>)</li>
<li>Upgrade CLI to <code>13.6.8</code> (<a href="https://github.com/facebook/react-native/commit/335f6ed83306bfa150c818d26dce4b279de4869f">335f6ed833</a> by <a href="https://github.com/szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Warn only in <code>init</code> command when CLI uses cached <code>npx</code> version (<a href="https://github.com/facebook/react-native/commit/b98c5b960ccc4fe9d2792c35994c414c709a3d7a">b98c5b960c</a> by <a href="https://github.com/szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
<li><code>selection</code> prop in <code>TextInput</code> was not being applied at component creation (<a href="https://github.com/facebook/react-native/commit/be09d12667044f237f08af410b2838062eb8e657">be09d12667</a> by <a href="https://github.com/alanleedev"><code>@​alanleedev</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Fixed dangling <code>mAttachedSurfaces</code> after <code>ReactHost.destroy()</code> (<a href="https://github.com/facebook/react-native/commit/c70d7910361f56bc361ad825fe13fb2178edfeba">c70d791036</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
<li>ReactSoftExceptions in ReactHostImpl only when Context is null (<a href="https://github.com/facebook/react-native/commit/ac3261ff608768ff43736b413c5a5ad67668af61">ac3261ff60</a> by <a href="https://github.com/arushikesarwani94"><code>@​arushikesarwani94</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Privacy Manifest aggregation failing due to no <code>NSPrivacyAccessedAPITypes</code> key (<a href="https://github.com/facebook/react-native/commit/fc4e0999206ec7c1f465bb2b1fea987e43485a82">fc4e099920</a> by <a href="https://github.com/renchap"><code>@​renchap</code></a>)</li>
<li>In privacy manifest post install script, handle the case where the file reference doesn't have a path (<a href="https://github.com/facebook/react-native/commit/4ad65ac59a2491db598abb7b32fb793e9693d5ac">4ad65ac59a</a> by <a href="https://github.com/robertying"><code>@​robertying</code></a>)</li>
<li>Fixed an issue where the <code>selectionColor</code> prop was not being applied on the <code>TextInput</code> component. (<a href="https://github.com/facebook/react-native/commit/2bde626a9fa2f782864937a5258ac494afe27f9f">2bde626a9f</a> by <a href="https://github.com/robinshin"><code>@​robinshin</code></a>)</li>
</ul>
<h2>0.74.1</h2>
<h3>Added</h3>
<h4>iOS Specific</h4>
<ul>
<li>Implement privacy manifest aggregation  (<a href="https://github.com/facebook/react-native/commit/4be1fafec8edca5da5ebe515ad359d4178db7d23">4be1fafec8</a> by <a href="https://github.com/@aleqsio"><code>@​aleqsio</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Align debugger Chrome launch flags with Meta-internal version (<a href="https://github.com/facebook/react-native/commit/93956e267cd4f1a77adaa842a55ca6f2d0d1b9c5">93956e267c</a> by <a href="https://github.com/@motiz88"><code>@​motiz88</code></a>)</li>
<li>Update &quot;Open Debugger&quot; to print extended Flipper guidance (<a href="https://github.com/facebook/react-native/commit/261a58761c2e7e10cc5cf0a63ed9785e1cdf097c">261a58761c</a> by <a href="https://github.com/@huntie"><code>@​huntie</code></a>)</li>
<li>Enable event loop by default when bridgeless is enabled (<a href="https://github.com/facebook/react-native/commit/b440672468b6d1d99cd322a4348dd90150703f24">b440672468</a> by <a href="https://github.com/@rubennorte"><code>@​rubennorte</code></a>)</li>
<li>Upgrade <code>@react-native-community/cli</code> to 13.6.6 (<a href="https://github.com/facebook/react-native/commit/58b1f9b2d4f617290a3a535153ff1e93a4672038">58b1f9b2d4</a> by <a href="https://github.com/@szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Support more stubbed methods in <code>BridgelessCatalystInstance</code> (<a href="https://github.com/facebook/react-native/commit/cc1c69799e284b368e3eaaac0ccd8e238384857f">cc1c69799e</a> by <a href="https://github.com/@javache"><code>@​javache</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Reset animation state in TouchableOpacity and TouchableBounce (<a href="https://github.com/facebook/react-native/commit/165cabb21f2419bde63acb4b52be2f4fb7a2ec2e">165cabb21f</a> by <a href=""><code>@​sammy-SChttps://github.com/@sammy-</code></a>)</li>
<li>Add missing struct member initialization in Props.h (<a href="https://github.com/facebook/react-native/commit/13739510fb1c2400fbae1df1635fb93dae55abaa">13739510fb</a> by <a href="https://github.com/@alanleedev"><code>@​alanleedev</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react-native/commit/17c0b1766f7e3c1c3a59f7701704f0ea6a6f6bc3"><code>17c0b17</code></a> Release 0.74.2</li>
<li><a href="https://github.com/facebook/react-native/commit/053f1d9822831187149bb57effc677dad99d723c"><code>053f1d9</code></a> Fix dangling surfaces in ReactHostImpl (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44393">#44393</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/0f44ca644bcf7c124226b42ad484d1e6643c4270"><code>0f44ca6</code></a> chore: Increase iOS script portability (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44417">#44417</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/2e21543017006ee6418c6953d976593d07407755"><code>2e21543</code></a> [LOCAL] Fix prettier</li>
<li><a href="https://github.com/facebook/react-native/commit/58f232c6c20475309a7cd789863e88a6888bd8f2"><code>58f232c</code></a> [LOCAL] Bump hermes version</li>
<li><a href="https://github.com/facebook/react-native/commit/1e3d2161e85906e781b2272a9ffefb3dfcf09191"><code>1e3d216</code></a> Merge branch '0.74-stable' of <a href="https://github.com/facebook/react-native">https://github.com/facebook/react-native</a> into 0...</li>
<li><a href="https://github.com/facebook/react-native/commit/335f6ed83306bfa150c818d26dce4b279de4869f"><code>335f6ed</code></a> feat: upgrade CLI to <code>13.6.8</code> (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44757">#44757</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/752c173da529b48ead482be5088af6758f08ee65"><code>752c173</code></a> Fix Privacy Manifest generator when it does not contain a `NSPrivacyAccessedA...</li>
<li><a href="https://github.com/facebook/react-native/commit/1860441d848b8f620e0b959e43122628b1cd04c9"><code>1860441</code></a> fix: warn only in <code>init</code> command when CLI uses cached <code>npx</code> version (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44644">#44644</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/a88a3c5bbfbb2d7ea1e9af6f8bea11542bf88cf1"><code>a88a3c5</code></a> iOS: Fixes textinput onscroll event payload (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/43445">#43445</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/react-native/commits/v0.74.2/packages/react-native">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:31:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /kafka_events in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:31:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    Bump ws from 7.5.9 to 7.5.10 in /oid4vci/demo/frontend in the npm_and_yarn group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group in /oid4vci/demo/frontend with 1 update: [ws](https://github.com/websockets/ws).

Updates `ws` from 7.5.9 to 7.5.10
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>7.5.10</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 7.x release line (22c28763).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d962d70649e393841ee1ed726a8f7ffbe90d0c06"><code>d962d70</code></a> [dist] 7.5.10</li>
<li><a href="https://github.com/websockets/ws/commit/22c28763234aa75a7e1b76f5c01c181260d7917f"><code>22c2876</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/7.5.9...7.5.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ws&package-manager=npm_and_yarn&previous-version=7.5.9&new-version=7.5.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 22:31:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/648" class=".btn">#648</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /rpc in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /rpc with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/647" class=".btn">#647</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /redis_events in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:30:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/646" class=".btn">#646</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /connection_update/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /connection_update/integration with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:30:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/645" class=".btn">#645</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /basicmessage_storage in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /basicmessage_storage with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/644" class=".btn">#644</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /redis_events/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events/integration with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/643" class=".btn">#643</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /connection_update in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /connection_update with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/642" class=".btn">#642</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /oid4vci in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /oid4vci with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:29:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in /plugin_globals in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /plugin_globals with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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
        Created At 2024-06-17 22:29:38 +0000 UTC
    </div>
</div>

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

