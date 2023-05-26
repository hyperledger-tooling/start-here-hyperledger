---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2437" class=".btn">#2437</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in corda-4-8-all-in-one Fixes #2064 
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
        Created At 2023-05-24 06:55:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2436" class=".btn">#2436</a>
            </td>
            <td>
                <b>
                    style: 2021-09-20 linter warnings batch 8 / 26 #1357
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                submitting fixes for issue #1357  minus the linter warning ID 79 and 80 as they have been already solved in batch 9 #1478.
created this new PR as the old one was getting a bit cluttered, sorry for the inconvineance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 22:28:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2434" class=".btn">#2434</a>
            </td>
            <td>
                <b>
                    feat:  add ci action to check for unsorter package.json files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                     - Remove not working check-package-json-sort.ts script.
     - Add ci action to check for unsorted package.json files.

Closes: #2356
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 12:49:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2433" class=".btn">#2433</a>
            </td>
            <td>
                <b>
                    build(deps): bump requests from 2.26.0 to 2.31.0 in /packages-python/cactus_validator_socketio_indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.26.0 to 2.31.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.31.0</h2>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>v2.30.0</h2>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
<h2>v2.29.0</h2>
<h2>2.29.0 (2023-04-26)</h2>
<p><strong>Improvements</strong></p>
<ul>
<li>Requests now defers chunked requests to the urllib3 implementation to improve
standardization. (<a href="https://redirect.github.com/psf/requests/issues/6226">#6226</a>)</li>
<li>Requests relaxes header component requirements to support bytes/str subclasses. (<a href="https://redirect.github.com/psf/requests/issues/6356">#6356</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
<h2>2.29.0 (2023-04-26)</h2>
<p><strong>Improvements</strong></p>
<ul>
<li>Requests now defers chunked requests to the urllib3 implementation to improve
standardization. (<a href="https://redirect.github.com/psf/requests/issues/6226">#6226</a>)</li>
<li>Requests relaxes header component requirements to support bytes/str subclasses. (<a href="https://redirect.github.com/psf/requests/issues/6356">#6356</a>)</li>
</ul>
<h2>2.28.2 (2023-01-12)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4"><code>147c851</code></a> v2.31.0</li>
<li><a href="https://github.com/psf/requests/commit/74ea7cf7a6a27a4eeb2ae24e162bcc942a6706d5"><code>74ea7cf</code></a> Merge pull request from GHSA-j8r2-6x86-q33q</li>
<li><a href="https://github.com/psf/requests/commit/302225334678490ec66b3614a9dddb8a02c5f4fe"><code>3022253</code></a> test on pypy 3.8 and pypy 3.9 on windows and macos (<a href="https://redirect.github.com/psf/requests/issues/6424">#6424</a>)</li>
<li><a href="https://github.com/psf/requests/commit/b639e66c816514e40604d46f0088fbceec1a5149"><code>b639e66</code></a> test on py3.12 (<a href="https://redirect.github.com/psf/requests/issues/6448">#6448</a>)</li>
<li><a href="https://github.com/psf/requests/commit/d3d504436ef0c2ac7ec8af13738b04dcc8c694be"><code>d3d5044</code></a> Fixed a small typo (<a href="https://redirect.github.com/psf/requests/issues/6452">#6452</a>)</li>
<li><a href="https://github.com/psf/requests/commit/2ad18e0e10e7d7ecd5384c378f25ec8821a10a29"><code>2ad18e0</code></a> v2.30.0</li>
<li><a href="https://github.com/psf/requests/commit/f2629e9e3c7ce3c3c8c025bcd8db551101cbc773"><code>f2629e9</code></a> Remove strict parameter (<a href="https://redirect.github.com/psf/requests/issues/6434">#6434</a>)</li>
<li><a href="https://github.com/psf/requests/commit/87d63de8739263bbe17034fba2285c79780da7e8"><code>87d63de</code></a> v2.29.0</li>
<li><a href="https://github.com/psf/requests/commit/51716c4ef390136b0d4b800ec7665dd5503e64fc"><code>51716c4</code></a> enable the warnings plugin (<a href="https://redirect.github.com/psf/requests/issues/6416">#6416</a>)</li>
<li><a href="https://github.com/psf/requests/commit/a7da1ab3498b10ec3a3582244c94b2845f8a8e71"><code>a7da1ab</code></a> try on ubuntu 22.04 (<a href="https://redirect.github.com/psf/requests/issues/6418">#6418</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.26.0...v2.31.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.26.0&new-version=2.31.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 02:43:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2432" class=".btn">#2432</a>
            </td>
            <td>
                <b>
                    build(deps): bump requests from 2.26.0 to 2.31.0 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.26.0 to 2.31.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.31.0</h2>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>v2.30.0</h2>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
<h2>v2.29.0</h2>
<h2>2.29.0 (2023-04-26)</h2>
<p><strong>Improvements</strong></p>
<ul>
<li>Requests now defers chunked requests to the urllib3 implementation to improve
standardization. (<a href="https://redirect.github.com/psf/requests/issues/6226">#6226</a>)</li>
<li>Requests relaxes header component requirements to support bytes/str subclasses. (<a href="https://redirect.github.com/psf/requests/issues/6356">#6356</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
<h2>2.29.0 (2023-04-26)</h2>
<p><strong>Improvements</strong></p>
<ul>
<li>Requests now defers chunked requests to the urllib3 implementation to improve
standardization. (<a href="https://redirect.github.com/psf/requests/issues/6226">#6226</a>)</li>
<li>Requests relaxes header component requirements to support bytes/str subclasses. (<a href="https://redirect.github.com/psf/requests/issues/6356">#6356</a>)</li>
</ul>
<h2>2.28.2 (2023-01-12)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4"><code>147c851</code></a> v2.31.0</li>
<li><a href="https://github.com/psf/requests/commit/74ea7cf7a6a27a4eeb2ae24e162bcc942a6706d5"><code>74ea7cf</code></a> Merge pull request from GHSA-j8r2-6x86-q33q</li>
<li><a href="https://github.com/psf/requests/commit/302225334678490ec66b3614a9dddb8a02c5f4fe"><code>3022253</code></a> test on pypy 3.8 and pypy 3.9 on windows and macos (<a href="https://redirect.github.com/psf/requests/issues/6424">#6424</a>)</li>
<li><a href="https://github.com/psf/requests/commit/b639e66c816514e40604d46f0088fbceec1a5149"><code>b639e66</code></a> test on py3.12 (<a href="https://redirect.github.com/psf/requests/issues/6448">#6448</a>)</li>
<li><a href="https://github.com/psf/requests/commit/d3d504436ef0c2ac7ec8af13738b04dcc8c694be"><code>d3d5044</code></a> Fixed a small typo (<a href="https://redirect.github.com/psf/requests/issues/6452">#6452</a>)</li>
<li><a href="https://github.com/psf/requests/commit/2ad18e0e10e7d7ecd5384c378f25ec8821a10a29"><code>2ad18e0</code></a> v2.30.0</li>
<li><a href="https://github.com/psf/requests/commit/f2629e9e3c7ce3c3c8c025bcd8db551101cbc773"><code>f2629e9</code></a> Remove strict parameter (<a href="https://redirect.github.com/psf/requests/issues/6434">#6434</a>)</li>
<li><a href="https://github.com/psf/requests/commit/87d63de8739263bbe17034fba2285c79780da7e8"><code>87d63de</code></a> v2.29.0</li>
<li><a href="https://github.com/psf/requests/commit/51716c4ef390136b0d4b800ec7665dd5503e64fc"><code>51716c4</code></a> enable the warnings plugin (<a href="https://redirect.github.com/psf/requests/issues/6416">#6416</a>)</li>
<li><a href="https://github.com/psf/requests/commit/a7da1ab3498b10ec3a3582244c94b2845f8a8e71"><code>a7da1ab</code></a> try on ubuntu 22.04 (<a href="https://redirect.github.com/psf/requests/issues/6418">#6418</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.26.0...v2.31.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.26.0&new-version=2.31.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 02:40:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2430" class=".btn">#2430</a>
            </td>
            <td>
                <b>
                    docs(weaver/samples): pin solc to v0.8.8 and turn off IR for Besu asset exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Without having it pinned to v0.8.8, some breaking changes that solc
has snuck in [1] [2] around v0.8.15 (for IR) are breaking the contract
deployment in a way that opcodes end up in the migration contract's
constructor that Besu does not recognize ("opcode INVALID" in the besu
logs if you set the log level to "ALL") in the Besu logs and then sends
back an "internal error" message via the JSON-RPC response, which is a
bug IMO it should state that the user input was invalid (user input
being the contract)
2. Disabled IR in the truffle (solc) config which is a step backwards
because it's a new feature of the solidity compiler that has certain
benefits to it compared to the legacy compilation mode, but enabling it
breaks the build so it just had to be done. In the future if someone
has time to do a deep dive on why exactly it's failing, then it should
be re-enabled because having the legacy compilation mode being our default
is technical debt that should be paid off rather sooner than later because
we never know how it will come back to cause different issues later on.

When IR is enabled, the following error occurs (even on the pinned v0.8.8 solc):
> Compiling ./contracts/transferInterface.sol
> YulException: Variable var_amount_3290 is 9 slot(s) too deep inside the stack.

[1] https://docs.soliditylang.org/en/v0.8.15/ir-breaking-changes.html#semantic-only-changes
[2] https://github.com/ethereum/solidity/issues/13311#issuecomment-1199274310

Fixes #2423

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 01:58:40 +0000 UTC
    </div>
</div>

