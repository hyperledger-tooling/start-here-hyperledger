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
                PR <a href="https://github.com/hyperledger/cello/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    Bump jinja2 from 2.11.2 to 2.11.3 in /src/agent/docker-rest-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jinja2](https://github.com/pallets/jinja) from 2.11.2 to 2.11.3.
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
</blockquote>
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
<li>See full diff in <a href="https://github.com/pallets/jinja/compare/2.11.2...2.11.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jinja2&package-manager=pip&previous-version=2.11.2&new-version=2.11.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 03:02:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.25.11 to 1.26.5 in /src/agent/docker-rest-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.25.11 to 1.26.5.
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
<h1>1.26.5 (2021-05-26)</h1>
<ul>
<li>Fixed deprecation warnings emitted in Python 3.10.</li>
<li>Updated vendored <code>six</code> library to 1.16.0.</li>
<li>Improved performance of URL parser when splitting
the authority component.</li>
</ul>
<h1>1.26.4 (2021-03-15)</h1>
<ul>
<li>Changed behavior of the default <code>SSLContext</code> when connecting to HTTPS proxy
during HTTPS requests. The default <code>SSLContext</code> now sets <code>check_hostname=True</code>.</li>
</ul>
<h1>1.26.3 (2021-01-26)</h1>
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
<h1>1.26.2 (2020-11-12)</h1>
<ul>
<li>Fixed an issue where <code>wrap_socket</code> and <code>CERT_REQUIRED</code> wouldn't
be imported properly on Python 2.7.8 and earlier (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2052">#2052</a>)</li>
</ul>
<h1>1.26.1 (2020-11-11)</h1>
<ul>
<li>Fixed an issue where two <code>User-Agent</code> headers would be sent if a
<code>User-Agent</code> header key is passed as <code>bytes</code> (Pull <a href="https://github-redirect.dependabot.com/urllib3/urllib3/issues/2047">#2047</a>)</li>
</ul>
<h1>1.26.0 (2020-11-10)</h1>
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
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/1.25.11...1.26.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.25.11&new-version=1.26.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 03:02:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    Bump django from 3.1.13 to 3.1.14 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [django](https://github.com/django/django) from 3.1.13 to 3.1.14.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/django/django/commit/840bebf1eef1c2a373158262cdfec611dc535658"><code>840bebf</code></a> [3.1.x] Bumped version for 3.1.14 release.</li>
<li><a href="https://github.com/django/django/commit/22bd17488159601bf0741b70ae7932bffea8eced"><code>22bd174</code></a> [3.1.x] Fixed <a href="https://github-redirect.dependabot.com/django/django/issues/30530">#30530</a>, CVE-2021-44420 -- Fixed potential bypass of an upstream...</li>
<li><a href="https://github.com/django/django/commit/cfb780dafe29e2243d9b48d0783b729b315341bb"><code>cfb780d</code></a> [3.1.x] Added stub release notes 3.1.14 and 2.2.25.</li>
<li><a href="https://github.com/django/django/commit/61c2d58d017874283921537f8ff1fe31b7652a63"><code>61c2d58</code></a> [3.1.x] Added 'formatter' to spelling wordlist.</li>
<li><a href="https://github.com/django/django/commit/9dd1f9572fa5024deb1615266a0cd9995b27bd41"><code>9dd1f95</code></a> [3.1.x] Fixed <a href="https://github-redirect.dependabot.com/django/django/issues/33082">#33082</a> -- Fixed CommandTests.test_subparser_invalid_option on P...</li>
<li><a href="https://github.com/django/django/commit/febc980e89591ffdc6df86cbeac13d7dfd89876e"><code>febc980</code></a> [3.1.x] Refs <a href="https://github-redirect.dependabot.com/django/django/issues/31676">#31676</a> -- Updated technical board description in organization docs.</li>
<li><a href="https://github.com/django/django/commit/34a0bb5d50506b0992c6f6208e15c8b5f1a5a0b1"><code>34a0bb5</code></a> [3.1.x] Refs <a href="https://github-redirect.dependabot.com/django/django/issues/31676">#31676</a> -- Added Mergers and Releasers to organization docs.</li>
<li><a href="https://github.com/django/django/commit/d94b1e44b2614ed30a9ed8f5bd557013ed578d19"><code>d94b1e4</code></a> [3.1.x] Refs <a href="https://github-redirect.dependabot.com/django/django/issues/31676">#31676</a> -- Removed Core team from organization docs.</li>
<li><a href="https://github.com/django/django/commit/cd391be832ca4ea4a58824ab2d498b752b111b1b"><code>cd391be</code></a> [3.1.x] Fixed typo in docs/releases/3.1.13.txt.</li>
<li><a href="https://github.com/django/django/commit/cb149dd1946c4ec5f15a8edd4df062d1c0a5e93a"><code>cb149dd</code></a> [3.1.x] Refs <a href="https://github-redirect.dependabot.com/django/django/issues/31676">#31676</a> -- Removed Django Core-Mentorship mailing list references...</li>
<li>Additional commits viewable in <a href="https://github.com/django/django/compare/3.1.13...3.1.14">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=django&package-manager=pip&previous-version=3.1.13&new-version=3.1.14)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 03:02:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    Bump django-filter from 2.0.0 to 2.4.0 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [django-filter](https://github.com/carltongibson/django-filter) from 2.0.0 to 2.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/carltongibson/django-filter/releases">django-filter's releases</a>.</em></p>
<blockquote>
<h2>Version 2.4.0</h2>
<ul>
<li>
<p>SECURITY: Added a <code>MaxValueValidator</code> to the form field for
<code>NumberFilter</code>. This prevents a potential DoS attack if numbers with very
large exponents were subsequently converted to integers.</p>
<p>The default limit value for the validator is <code>1e50</code>.</p>
<p>The new <code>NumberFilter.get_max_validator()</code> allows customising the used
validator, and may return <code>None</code> to disable the validation entirely.</p>
</li>
<li>
<p>Added testing against Django 3.1 and Python 3.9.</p>
<p>In addition tests against Django main development branch are now required to
pass.</p>
</li>
</ul>
<h2>Version 2.3.0</h2>
<p><a href="https://github.com/carltongibson/django-filter/blob/master/CHANGES.rst#version-230-2020-6-5">https://github.com/carltongibson/django-filter/blob/master/CHANGES.rst#version-230-2020-6-5</a></p>
<h2>Version 2.2</h2>
<p>Highlights:</p>
<ul>
<li>Added <code>DjangoFilterBackend.get_schema_operation_parameters()</code> for DRF 3.10+
OpenAPI schema generation. (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1086">#1086</a>)</li>
<li>Added <code>lookup_expr</code> to <code>MultipleChoiceFilter</code> (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1054">#1054</a>)</li>
<li>Dropped support for EOL Python 3.4</li>
</ul>
<h2>Version 2.1.0</h2>
<ul>
<li>
<p>Fixed a regression in <code>FilterView</code> introduced in 2.0. An empty <code>QuerySet</code> was
incorrectly used whenever the <code>FilterSet</code> was unbound (i.e. when there were
no <code>GET</code> parameters).  The correct, pre-2.0 behaviour is now restored.</p>
<p>A workaround was to set <code>strict=False</code> on the <code>FilterSet</code>. This is no
longer necessary, so you may restore <code>strict</code> behaviour as desired.</p>
</li>
<li>
<p>Added <code>IsoDateTimeFromToRangeFilter</code>. Allows From-To filtering using
ISO-8601 formatted dates.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/carltongibson/django-filter/blob/main/CHANGES.rst">django-filter's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.4.0 (2020-9-27)</h2>
<ul>
<li>
<p>SECURITY: Added a <code>MaxValueValidator</code> to the form field for
<code>NumberFilter</code>. This prevents a potential DoS attack if numbers with very
large exponents were subsequently converted to integers.</p>
<p>The default limit value for the validator is <code>1e50</code>.</p>
<p>The new <code>NumberFilter.get_max_validator()</code> allows customising the used
validator, and may return <code>None</code> to disable the validation entirely.</p>
</li>
<li>
<p>Added testing against Django 3.1 and Python 3.9.</p>
<p>In addition tests against Django main development branch are now required to
pass.</p>
</li>
</ul>
<h2>Version 2.3.0 (2020-6-5)</h2>
<ul>
<li>Fixed import of FieldDoesNotExist. (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1127">#1127</a>)</li>
<li>Added testing against Django 3.0. (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1125">#1125</a>)</li>
<li>Declared support for, and added testing against, Python 3.8. (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1138">#1138</a>)</li>
<li>Fix filterset multiple inheritance bug (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1131">#1131</a>)</li>
<li>Allowed customising default lookup expression. (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1129">#1129</a>)</li>
<li>Drop Django 2.1 and below (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1180">#1180</a>)</li>
<li>Fixed IsoDateTimeRangeFieldTests for Django 3.1</li>
<li>Require tests to pass against Django <code>master</code>.</li>
</ul>
<h2>Version 2.2 (2019-7-16)</h2>
<ul>
<li>Added <code>DjangoFilterBackend.get_schema_operation_parameters()</code> for DRF 3.10+
OpenAPI schema generation. (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1086">#1086</a>)</li>
<li>Added <code>lookup_expr</code> to <code>MultipleChoiceFilter</code> (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1054">#1054</a>)</li>
<li>Dropped support for EOL Python 3.4</li>
</ul>
<h2>Version 2.1 (2019-1-20)</h2>
<ul>
<li>
<p>Fixed a regression in <code>FilterView</code> introduced in 2.0. An empty <code>QuerySet</code> was
incorrectly used whenever the FilterSet was unbound (i.e. when there were
no GET parameters).  The correct, pre-2.0 behaviour is now restored.</p>
<p>A workaround was to set <code>strict=False</code> on the <code>FilterSet</code>. This is no
longer necessary, so you may restore <code>strict</code> behaviour as desired.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/carltongibson/django-filter/commit/78210722d920f803a8142e48969bc37f0f8324ed"><code>7821072</code></a> Postpone move to CalVer.</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/fd5824e286a8af88c2225ed647983fc163af2be0"><code>fd5824e</code></a> Restore version declaration in setup.py.</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/c9daa68e2f20a87773ad0960486a64e63feb5cf6"><code>c9daa68</code></a> Version 20.9.0.</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/c045bbeb4597df2f9bb7e0c716066a13bef5a48c"><code>c045bbe</code></a> Droped using bumpversion.</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/b1f56ed5a0f623f59488c95633265a33c4760505"><code>b1f56ed</code></a> Use single version reference from main module.</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/451d372715da9cf23d417d54a85dee16b5f59af1"><code>451d372</code></a> Update docs copyright year.</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/82c9a420d2ab9addcb20d6702e74afa5c04cd91f"><code>82c9a42</code></a> Added MaxValueValidator to NumberFilter.</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/2ebce743d5facbe4fe628b79fa916a3f5ef09c21"><code>2ebce74</code></a> Confirmed compatibility with Python 3.9. (<a href="https://github-redirect.dependabot.com/carltongibson/django-filter/issues/1270">#1270</a>)</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/85c9572b092492d3a39be35d269dbc3e7453ed69"><code>85c9572</code></a> Run tests with GitHub Actions</li>
<li><a href="https://github.com/carltongibson/django-filter/commit/d9f389f1a408a8d4ae21f2e5a73f7a3125078905"><code>d9f389f</code></a> Update Jinja test dependency.</li>
<li>Additional commits viewable in <a href="https://github.com/carltongibson/django-filter/compare/2.0.0...2.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=django-filter&package-manager=pip&previous-version=2.0.0&new-version=2.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 03:02:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    [#issue-412]Delete the dockefile of 0.9.0 version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                delete the dockefile of 0.9.0 version

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>

Close #412
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 09:18:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    [#issue-410]Add chaincode management page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add chaincode management page

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>

Close #410
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 09:09:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/409" class=".btn">#409</a>
            </td>
            <td>
                <b>
                    [#issue-408] implement chaincode list & query_committed function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                implement chaincode list & query_committed function

Close #408

Signed-off-by: tianxuanhong1 <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-19 06:17:34 +0000 UTC
    </div>
</div>

