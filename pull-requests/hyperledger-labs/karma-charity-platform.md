---
layout: default
title: karma-charity-platform
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/karma-charity-platform
---

# karma-charity-platform <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/karma-charity-platform){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Fixing building the chaincode image from Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexander Zemtsov <a.zemtsov@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 13:18:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Bump node-forge from 1.2.1 to 1.3.1 in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [node-forge](https://github.com/digitalbazaar/forge) from 1.2.1 to 1.3.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/digitalbazaar/forge/blob/main/CHANGELOG.md">node-forge's changelog</a>.</em></p>
<blockquote>
<h2>1.3.1 - 2022-03-29</h2>
<h3>Fixes</h3>
<ul>
<li>RFC 3447 and RFC 8017 allow for optional <code>DigestAlgorithm</code> <code>NULL</code> parameters
for <code>sha*</code> algorithms and require <code>NULL</code> paramters for <code>md2</code> and <code>md5</code>
algorithms.</li>
</ul>
<h2>1.3.0 - 2022-03-17</h2>
<h3>Security</h3>
<ul>
<li>Three RSA PKCS#1 v1.5 signature verification issues were reported by Moosa
Yahyazadeh (<a href="mailto:moosa-yahyazadeh@uiowa.edu">moosa-yahyazadeh@uiowa.edu</a>).</li>
<li><strong>HIGH</strong>: Leniency in checking <code>digestAlgorithm</code> structure can lead to
signature forgery.
<ul>
<li>The code is lenient in checking the digest algorithm structure. This can
allow a crafted structure that steals padding bytes and uses unchecked
portion of the PKCS#1 encoded message to forge a signature when a low
public exponent is being used. For more information, please see
<a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24771">CVE-2022-24771</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-cfm4-qjh2-4765">GHSA-cfm4-qjh2-4765</a></li>
</ul>
</li>
<li><strong>HIGH</strong>: Failing to check tailing garbage bytes can lead to signature
forgery.
<ul>
<li>The code does not check for tailing garbage bytes after decoding a
<code>DigestInfo</code> ASN.1 structure. This can allow padding bytes to be removed
and garbage data added to forge a signature when a low public exponent is
being used.  For more information, please see <a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA
signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24772">CVE-2022-24772</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-x4jg-mjrx-434g">GHSA-x4jg-mjrx-434g</a></li>
</ul>
</li>
<li><strong>MEDIUM</strong>: Leniency in checking type octet.
<ul>
<li><code>DigestInfo</code> is not properly checked for proper ASN.1 structure. This can
lead to successful verification with signatures that contain invalid
structures but a valid digest.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24773">CVE-2022-24773</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-2r2c-g63r-vccr">GHSA-2r2c-g63r-vccr</a></li>
</ul>
</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[asn1] Add fallback to pretty print invalid UTF8 data.</li>
<li>[asn1] <code>fromDer</code> is now more strict and will default to ensuring all input
bytes are parsed or throw an error. A new option <code>parseAllBytes</code> can disable
this behavior.
<ul>
<li><strong>NOTE</strong>: The previous behavior is being changed since it can lead to
security issues with crafted inputs. It is possible that code doing custom
DER parsing may need to adapt to this new behavior and optional flag.</li>
</ul>
</li>
<li>[rsa] Add and use a validator to check for proper structure of parsed ASN.1</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/digitalbazaar/forge/commit/a0a4a4264bedb3296974b9675349c9c190144aeb"><code>a0a4a42</code></a> Release 1.3.1.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/a33830f61c351e8e3a34309767e8dd0de148376b"><code>a33830f</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/740954d747ac56b76a6e1ae12a057c9548843436"><code>740954d</code></a> Allow optional DigestAlgorithm parameters.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/56f4316b4cc6592e678f8c416209c45984b6547b"><code>56f4316</code></a> Allow DigestInfo.DigestAlgorith.parameters to be optional</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/cbf0bd590d47fe3120a57e7c36f2f4e64381ad81"><code>cbf0bd5</code></a> Start 1.3.1-0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/6c5b90133d46af63d139b98bf65371732c8c7dad"><code>6c5b901</code></a> Release 1.3.0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/0f3972ad5883a9869703c6f54a0627bc454bca47"><code>0f3972a</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/dc77b39dd347e7f8b60a0f25a311fe5f06130579"><code>dc77b39</code></a> Fix error checking.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/bb822c02df0b61211836472e29b9790cc541cdb2"><code>bb822c0</code></a> Add advisory links.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/d4395fec831622837ecfec9e428d4620e208f9a8"><code>d4395fe</code></a> Update changelog.</li>
<li>Additional commits viewable in <a href="https://github.com/digitalbazaar/forge/compare/v1.2.1...v1.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-forge&package-manager=npm_and_yarn&previous-version=1.2.1&new-version=1.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Bump async from 2.6.3 to 2.6.4 in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) from 2.6.3 to 2.6.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/v2.6.4/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v2.6.4</h1>
<ul>
<li>Fix potential prototype pollution exploit (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1828">#1828</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/c6bdaca4f9175c14fc655d3783c6af6a883e6514"><code>c6bdaca</code></a> Version 2.6.4</li>
<li><a href="https://github.com/caolan/async/commit/8870da9d5022bab310413041b4079e10db3980b7"><code>8870da9</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/4df6754ef4e96a742956df8782fee27242a2ea12"><code>4df6754</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/8f7f90342a6571ba1c197d747ebed30c368096d2"><code>8f7f903</code></a> Fix prototype pollution vulnerability (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1828">#1828</a>)</li>
<li>See full diff in <a href="https://github.com/caolan/async/compare/v2.6.3...v2.6.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async&package-manager=npm_and_yarn&previous-version=2.6.3&new-version=2.6.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Bump moment from 2.29.1 to 2.29.2 in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [moment](https://github.com/moment/moment) from 2.29.1 to 2.29.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment/blob/develop/CHANGELOG.md">moment's changelog</a>.</em></p>
<blockquote>
<h3>2.29.2 <a href="https://gist.github.com/ichernev/1904b564f6679d9aac1ae08ce13bc45c">See full changelog</a></h3>
<ul>
<li>Release Apr 3 2022</li>
</ul>
<p>Address <a href="https://github.com/moment/moment/security/advisories/GHSA-8hfj-j24r-96c4">https://github.com/moment/moment/security/advisories/GHSA-8hfj-j24r-96c4</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moment/moment/commit/75e2ac573e8cd62086a6bc6dc1b8d271e2804391"><code>75e2ac5</code></a> Build 2.29.2</li>
<li><a href="https://github.com/moment/moment/commit/5a2987758edc7d413d1248737d9d0d1b65a70450"><code>5a29877</code></a> Bump version to 2.29.2</li>
<li><a href="https://github.com/moment/moment/commit/4fd847b7a8c7065d88ba0a64b727660190dd45d7"><code>4fd847b</code></a> Update changelog for 2.29.2</li>
<li><a href="https://github.com/moment/moment/commit/4211bfc8f15746be4019bba557e29a7ba83d54c5"><code>4211bfc</code></a> [bugfix] Avoid loading path-looking locales from fs</li>
<li><a href="https://github.com/moment/moment/commit/f2a813afcfd0dd6e63812ea74c46ecc627f6a6a6"><code>f2a813a</code></a> [misc] Fix indentation (according to prettier)</li>
<li><a href="https://github.com/moment/moment/commit/7a10de889de64c2519f894a84a98030bec5022d9"><code>7a10de8</code></a> [test] Avoid hours around DST</li>
<li><a href="https://github.com/moment/moment/commit/e96809208c9d1b1bbe22d605e76985770024de42"><code>e968092</code></a> [locale] ar-ly: fix locale name (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5828">#5828</a>)</li>
<li><a href="https://github.com/moment/moment/commit/53d7ee6ad8c60c891571c7085db91831bbc095b4"><code>53d7ee6</code></a> [misc] fix builds (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5836">#5836</a>)</li>
<li><a href="https://github.com/moment/moment/commit/52019f1dda47c3e598aaeaa4ac89d5a574641604"><code>52019f1</code></a> [misc] Specify length of toArray return type (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5766">#5766</a>)</li>
<li><a href="https://github.com/moment/moment/commit/0dcaaa689d02dde824029b09ab6aa64ff351ee2e"><code>0dcaaa6</code></a> [locale] tr: update translation of Monday and Saturday (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5756">#5756</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/moment/moment/compare/2.29.1...2.29.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=moment&package-manager=npm_and_yarn&previous-version=2.29.1&new-version=2.29.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /explorer/backend/src/packages/application/api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /platform/backend/src/packages/application/api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /chaincode/src/packages/application/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:48:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Transfer code from the original repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexander Zemtsov <a.zemtsov@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 11:53:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/1" class=".btn">#1</a>
            </td>
            <td>
                <b>
                    Initial commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tracy Kuhrt <tracy.a.kuhrt@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 20:18:45 +0000 UTC
    </div>
</div>

