---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.64.0 to 1.64.1 in the go_modules group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps the go_modules group with 1 update: [google.golang.org/grpc](https://github.com/grpc/grpc-go).

Updates `google.golang.org/grpc` from 1.64.0 to 1.64.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.64.1</h2>
<h1>Dependencies</h1>
<ul>
<li>Update x/net/http2 to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-45288">CVE-2023-45288</a> (<a href="https://redirect.github.com/grpc/grpc-go/issues/7352">#7352</a>)</li>
<li>metadata: remove String method from MD to make printing consistent (<a href="https://redirect.github.com/grpc/grpc-go/issues/7374">#7374</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/4d833de0e0ea4345c2f8333f5e1d1155f93c5222"><code>4d833de</code></a> Change version to 1.64.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/7381">#7381</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e9193a42987f93cf634aedb7c6f32d607281f8c4"><code>e9193a4</code></a> *: update deps (<a href="https://redirect.github.com/grpc/grpc-go/issues/7375">#7375</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ab292411ddc0f3b7a7786754d1fe05264c3021eb"><code>ab29241</code></a> metadata: remove String method (<a href="https://redirect.github.com/grpc/grpc-go/issues/7374">#7374</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/355b9a557b63896fc569d8be1518905eabde0026"><code>355b9a5</code></a> Change version to 1.64.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/7219">#7219</a>)</li>
<li>See full diff in <a href="https://github.com/grpc/grpc-go/compare/v1.64.0...v1.64.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.64.0&new-version=1.64.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-ca/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 21:59:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/427" class=".btn">#427</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.15.0 to 3.19.1 in /docs in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /docs with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.15.0 to 3.19.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jaraco/zipp/blob/main/NEWS.rst">zipp's changelog</a>.</em></p>
<blockquote>
<h1>v3.19.1</h1>
<h2>Bugfixes</h2>
<ul>
<li>Improved handling of malformed zip files. (<a href="https://redirect.github.com/jaraco/zipp/issues/119">#119</a>)</li>
</ul>
<h1>v3.19.0</h1>
<h2>Features</h2>
<ul>
<li>Implement is_symlink. (<a href="https://redirect.github.com/jaraco/zipp/issues/117">#117</a>)</li>
</ul>
<h1>v3.18.2</h1>
<p>No significant changes.</p>
<h1>v3.18.1</h1>
<p>No significant changes.</p>
<h1>v3.18.0</h1>
<h2>Features</h2>
<ul>
<li>Bypass ZipFile.namelist in glob for better performance. (<a href="https://redirect.github.com/jaraco/zipp/issues/106">#106</a>)</li>
<li>Refactored glob functionality to support a more generalized solution with support for platform-specific path separators. (<a href="https://redirect.github.com/jaraco/zipp/issues/108">#108</a>)</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>Add special accounting for pypy when computing the stack level for text encoding warnings. (<a href="https://redirect.github.com/jaraco/zipp/issues/114">#114</a>)</li>
</ul>
<h1>v3.17.0</h1>
<p>Features</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jaraco/zipp/commit/6d1cb72aa55e0536f35d2af128994b5a61ca4c1a"><code>6d1cb72</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/fd604bd34f0343472521a36da1fbd22e793e14fd"><code>fd604bd</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/120">#120</a> from jaraco/bugfix/119-malformed-paths</li>
<li><a href="https://github.com/jaraco/zipp/commit/c18417ed2953e181728a7dac07bff88a2190abf7"><code>c18417e</code></a> Add news fragment.</li>
<li><a href="https://github.com/jaraco/zipp/commit/58115d2be968644ce71ce6bcc9b79826c82a1806"><code>58115d2</code></a> Employ SanitizedNames in CompleteDirs. Fixes broken test.</li>
<li><a href="https://github.com/jaraco/zipp/commit/564fcc10cdbfdaecdb33688e149827465931c9e0"><code>564fcc1</code></a> Add SanitizedNames mixin.</li>
<li><a href="https://github.com/jaraco/zipp/commit/79a309fe54dc6b7934fb72e9f31bcb58f2e9f547"><code>79a309f</code></a> Add some assertions about malformed paths.</li>
<li><a href="https://github.com/jaraco/zipp/commit/2d015c22348fab46ca765339f55f84fe9d6e8115"><code>2d015c2</code></a> Merge <a href="https://github.com/jaraco/skeleton">https://github.com/jaraco/skeleton</a></li>
<li><a href="https://github.com/jaraco/zipp/commit/a595a0fad054cd20b69d3e954c99174e3a548938"><code>a595a0f</code></a> Rename extras to align with core metadata spec.</li>
<li><a href="https://github.com/jaraco/zipp/commit/608f90a6e74919501577a1312dc5c7d8e1d391d7"><code>608f90a</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/3a22d724acf874111b43f87f7110225122ec3de5"><code>3a22d72</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/118">#118</a> from jaraco/feature/is-symlink</li>
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.15.0...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.15.0&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-ca/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 18:12:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/425" class=".btn">#425</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2023.11.17 to 2024.7.4 in /docs in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /docs with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2023.11.17 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2023.11.17...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2023.11.17&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-ca/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-05 23:32:07 +0000 UTC
    </div>
</div>

