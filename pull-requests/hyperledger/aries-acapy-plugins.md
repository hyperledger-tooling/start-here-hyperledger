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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:31:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump follow-redirects from 1.15.4 to 1.15.6 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.15.4 to 1.15.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/35a517c5861d79dc8bff7db8626013d20b711b06"><code>35a517c</code></a> Release version 1.15.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/c4f847f85176991f95ab9c88af63b1294de8649b"><code>c4f847f</code></a> Drop Proxy-Authorization across hosts.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8526b4a1b2ab3a2e4044299377df623a661caa76"><code>8526b4a</code></a> Use GitHub for disclosure.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/b1677ce00110ee50dc5da576751d39b281fc4944"><code>b1677ce</code></a> Release version 1.15.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d8914f7982403ea096b39bd594a00ee9d3b7e224"><code>d8914f7</code></a> Preserve fragment in responseUrl.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.15.4...v1.15.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.15.4&new-version=1.15.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-16 22:45:00 +0000 UTC
    </div>
</div>

