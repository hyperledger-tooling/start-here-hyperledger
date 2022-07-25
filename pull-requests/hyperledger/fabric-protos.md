---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Revert "New service and messages for block attestation (#92)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 632b3efb5324c16d387b23f4d268515f9f3d53b9.

Block attestation service was added to main for v3.0, it should be removed in the new release-2.5 branch.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 15:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    Bump tzinfo from 1.2.9 to 1.2.10 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [tzinfo](https://github.com/tzinfo/tzinfo) from 1.2.9 to 1.2.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tzinfo/tzinfo/releases">tzinfo's releases</a>.</em></p>
<blockquote>
<h2>v1.2.10</h2>
<ul>
<li>Fixed a relative path traversal bug that could cause arbitrary files to be loaded with require when used with <code>RubyDataSource</code>. Please refer to
<a href="https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx">https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx</a> for details. CVE-2022-31163.</li>
<li>Ignore the SECURITY file from Arch Linux's tzdata package. <a href="https://github-redirect.dependabot.com/tzinfo/tzinfo/issues/134">#134</a>.</li>
</ul>
<p><a href="https://rubygems.org/gems/tzinfo/versions/1.2.10">TZInfo v1.2.10 on RubyGems.org</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tzinfo/tzinfo/blob/master/CHANGES.md">tzinfo's changelog</a>.</em></p>
<blockquote>
<h2>Version 1.2.10 - 19-Jul-2022</h2>
<ul>
<li>Fixed a relative path traversal bug that could cause arbitrary files to be
loaded with <code>require</code> when used with <code>RubyDataSource</code>. Please refer to
<a href="https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx">https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx</a> for
details. CVE-2022-31163.</li>
<li>Ignore the SECURITY file from Arch Linux's tzdata package. <a href="https://github-redirect.dependabot.com/tzinfo/tzinfo/issues/134">#134</a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tzinfo/tzinfo/commit/0814dcd6195f247cc90e62a46b86ff0b76e08ed6"><code>0814dcd</code></a> Fix the release date.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/fd05e2a61cc569cef81ebd1a90d0b57f69e401bd"><code>fd05e2a</code></a> Preparing v1.2.10.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/b98c32efd61289fe6f00a50ab8061e95962ea983"><code>b98c32e</code></a> Merge branch 'fix-directory-traversal-1.2' into 1.2</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/ac3ee6828afd67e6a8ee981cba791ee34d20e9fb"><code>ac3ee68</code></a> Remove unnecessary escaping of + within regex character classes.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/9d49bf9728a6d42e55f822c497ebf362e86a65a6"><code>9d49bf9</code></a> Fix relative path loading tests.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/394c381eb6a16eaeafb81196270c363234cf1956"><code>394c381</code></a> Remove <code>private_constant</code> for consistency and compatibility.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/5e9f99086f820573eb43ffe242e074b9a8295027"><code>5e9f990</code></a> Exclude Arch Linux's SECURITY file from the time zone index.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/17fc9e1fa918c24ca8c1915419d4cc15f56b6729"><code>17fc9e1</code></a> Workaround for 'Permission denied - NUL' errors with JRuby on Windows.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/6bd7a5191d9c1ca48a97420652460b8c4dec865d"><code>6bd7a51</code></a> Update copyright years.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/9905ca93abf7bf3e387bd592406e403cd18334c7"><code>9905ca9</code></a> Fix directory traversal in Timezone.get when using Ruby data source</li>
<li>Additional commits viewable in <a href="https://github.com/tzinfo/tzinfo/compare/v1.2.9...v1.2.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tzinfo&package-manager=bundler&previous-version=1.2.9&new-version=1.2.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 09:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Link to fabric-protos-go-apiv2 in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                APIv2 is the preferred published binding for end user use.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 08:43:46 +0000 UTC
    </div>
</div>

