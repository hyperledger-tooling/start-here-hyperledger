---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4144" class=".btn">#4144</a>
            </td>
            <td>
                <b>
                    add basic issue template/links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

re #4143

#### Description

Strangely, when I'm testing this on my work-fork, I go the bug-template and your vulnerability handling:

https://github.com/abebeos/fabric/issues/new/choose

No idea why, possibly once you merge to your repo this will behave as it should.

(nothing wrong to have the `Report vulnerability`, but it should not appear magically)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 16:54:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4142" class=".btn">#4142</a>
            </td>
            <td>
                <b>
                    use HasGet() instead of Has() and Get() on fastcache lib (backport #4141)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4141 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 15:27:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4141" class=".btn">#4141</a>
            </td>
            <td>
                <b>
                    use HasGet() instead of Has() and Get() on fastcache lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->


- Improvement (improvement to code, performance, etc)


#### Description

This pull request addresses the issue of inefficiency when retrieving a stored value from Fastcache by consolidating the two API calls, `Has()` and `Get()`, into a single call using the `HasGet()` API. By doing so, the performance overhead associated with making two API calls is eliminated.







            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 13:32:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4139" class=".btn">#4139</a>
            </td>
            <td>
                <b>
                    Update docs for v2.5.0 LTS status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs for v2.5.0 LTS status.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 18:52:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4138" class=".btn">#4138</a>
            </td>
            <td>
                <b>
                    Updates in main branch for v2.5.0 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates in main docs and scripts for v2.5.0 release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 18:45:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4137" class=".btn">#4137</a>
            </td>
            <td>
                <b>
                    streamline ubuntu/debian instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * remove '$' to allow for easier copy&paste
* reduce version information
* provide one main cli instructions block (for ubuntu)

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

- Documentation update

#### Description

re #4135 (first of several steps0

#### Additional details

Target audience are developers, no need for too much verbosity, the cli speaks usually for itself.

(this document needs a few more follow-up changes, but awaiting if this one gets merged in order to continue)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 12:45:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4133" class=".btn">#4133</a>
            </td>
            <td>
                <b>
                    Release commit for v2.5.0.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add release notes for v2.5.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 21:09:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4131" class=".btn">#4131</a>
            </td>
            <td>
                <b>
                    Upgrade doc for v2.5. (backport #4130)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4130 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 18:43:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4130" class=".btn">#4130</a>
            </td>
            <td>
                <b>
                    Upgrade doc for v2.5.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Edits to the upgrade doc for v2.5.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 17:05:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4129" class=".btn">#4129</a>
            </td>
            <td>
                <b>
                    remove version reference from doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

fixes #3203

(previous closed PR: #3204)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 20:54:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4128" class=".btn">#4128</a>
            </td>
            <td>
                <b>
                    bug fix 4127. Restore RSA support for x509 public key import on PKCS11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

<!--- Describe your changes in detail, including motivation. -->
While RSA has never been supported by Fabric for transaction signing and
verification, prior to version 2.x, MSPs could include CA certificates
that included RSA public keys. This was broken with the removal of the
unsupported RSA code.

It was fixed in SW but the error is still in PKCS11

This change modifies the key import function used by the MSP on PKCS11 to convert
an RSA public key to a bccsp.Key that can then be used as part of an MSP
identity.

This code does *not* add support for RSA on transaction paths.
#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues
https://github.com/hyperledger/fabric/issues/4127

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 14:51:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4125" class=".btn">#4125</a>
            </td>
            <td>
                <b>
                    Update govulncheck to use Go 1.20.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                govulncheck couldn't be found with just '1.20'.
Let's try the exact version '1.20.2'.

Also enable workflow_dispatch for on-demand runs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 17:22:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4124" class=".btn">#4124</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc from 1.1.4 to 1.1.5 (backport #4123)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4123 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 17:14:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4123" class=".btn">#4123</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc from 1.1.4 to 1.1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.1.4 to 1.1.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/releases">github.com/opencontainers/runc's releases</a>.</em></p>
<blockquote>
<h2>runc 1.1.5 -- &quot;囚われた屈辱は　反撃の嚆矢だ&quot;</h2>
<p>This is the fifth patch release in the 1.1.z series of runc, which fixes
three CVEs found in runc.</p>
<ul>
<li>
<p>CVE-2023-25809 is a vulnerability involving rootless containers where
(under specific configurations), the container would have write access
to the /sys/fs/cgroup/user.slice/... cgroup hierarchy. No other
hierarchies on the host were affected. This vulnerability was
discovered by Akihiro Suda.
<a href="https://github.com/opencontainers/runc/security/advisories/GHSA-m8cg-xc2p-r3fc">https://github.com/opencontainers/runc/security/advisories/GHSA-m8cg-xc2p-r3fc</a></p>
</li>
<li>
<p>CVE-2023-27561 was a regression which effectively re-introduced
CVE-2019-19921. This bug was present from v1.0.0-rc95 to v1.1.4. This
regression was discovered by <a href="https://github.com/Beuc"><code>@​Beuc</code></a>.
<a href="https://github.com/advisories/GHSA-vpvm-3wq2-2wvm">https://github.com/advisories/GHSA-vpvm-3wq2-2wvm</a></p>
</li>
<li>
<p>CVE-2023-28642 is a variant of CVE-2023-27561 and was fixed by the same
patch. This variant of the above vulnerability was reported by Lei
Wang.
<a href="https://github.com/opencontainers/runc/security/advisories/GHSA-g2j6-57v7-gm8c">https://github.com/opencontainers/runc/security/advisories/GHSA-g2j6-57v7-gm8c</a></p>
</li>
</ul>
<p>In addition, the following other fixes are included in this release:</p>
<ul>
<li>Fix the inability to use <code>/dev/null</code> when inside a container. (<a href="https://redirect.github.com/opencontainers/runc/issues/3620">#3620</a>)</li>
<li>Fix changing the ownership of host's <code>/dev/null</code> caused by fd redirection
(a regression in 1.1.1). (<a href="https://redirect.github.com/opencontainers/runc/issues/3674">#3674</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3731">#3731</a>)</li>
<li>Fix rare runc exec/enter unshare error on older kernels, including
CentOS &lt; 7.7. (<a href="https://redirect.github.com/opencontainers/runc/issues/3776">#3776</a>)</li>
<li>nsexec: Check for errors in <code>write_log()</code>. (<a href="https://redirect.github.com/opencontainers/runc/issues/3721">#3721</a>)</li>
</ul>
<h3>Static Linking Notices</h3>
<p>The <code>runc</code> binary distributed with this release are <em>statically linked</em> with
the following <a href="https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html">GNU LGPL-2.1</a> licensed libraries, with <code>runc</code> acting
as a &quot;work that uses the Library&quot;:</p>
<ul>
<li><a href="https://github.com/seccomp/libseccomp">libseccomp</a></li>
</ul>
<p>The versions of these libraries were not modified from their upstream versions,
but in order to comply with the LGPL-2.1 (§6(a)), we have attached the
complete source code for those libraries which (when combined with the attached
runc source code) may be used to exercise your rights under the LGPL-2.1.</p>
<p>However we strongly suggest that you make use of your distribution's packages
or download them from the authoritative upstream sources, especially since
these libraries are related to the security of your containers.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/blob/v1.1.5/CHANGELOG.md">github.com/opencontainers/runc's changelog</a>.</em></p>
<blockquote>
<h2>[1.1.5] - 2023-03-29</h2>
<blockquote>
<p>囚われた屈辱は
反撃の嚆矢だ</p>
</blockquote>
<h3>Fixed</h3>
<ul>
<li>Prohibit container's <code>/proc</code> and <code>/sys</code> to be symlinks (CVE-2019-19921,
CVE-2023-27561, CVE-2023-28642, <a href="https://redirect.github.com/opencontainers/runc/issues/3785">#3785</a>)</li>
<li>rootless: rework /sys/fs/cgroup mounts to avoid exposing the host's cgroup
hierarchy into the container. (CVE-2023-25809)</li>
<li>Fix the inability to use <code>/dev/null</code> when inside a container. (<a href="https://redirect.github.com/opencontainers/runc/issues/3620">#3620</a>)</li>
<li>Fix changing the ownership of host's <code>/dev/null</code> caused by fd redirection
(a regression in 1.1.1). (<a href="https://redirect.github.com/opencontainers/runc/issues/3674">#3674</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3731">#3731</a>)</li>
<li>Fix rare runc exec/enter unshare error on older kernels, inlcuding
CentOS &lt; 7.7. (<a href="https://redirect.github.com/opencontainers/runc/issues/3776">#3776</a>)</li>
<li>nsexec: Check for errors in <code>write_log()</code>. (<a href="https://redirect.github.com/opencontainers/runc/issues/3721">#3721</a>)</li>
<li>Various CI fixes and updates. (<a href="https://redirect.github.com/opencontainers/runc/issues/3618">#3618</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3630">#3630</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3640">#3640</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3729">#3729</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/runc/commit/f19387a6bec4944c770f7668ab51c4348d9c2f38"><code>f19387a</code></a> VERSION: release v1.1.5</li>
<li><a href="https://github.com/opencontainers/runc/commit/58a9abee210c5a72ab10904f96e0026f684f24e3"><code>58a9abe</code></a> Merge pull request from GHSA-m8cg-xc2p-r3fc</li>
<li><a href="https://github.com/opencontainers/runc/commit/27fb72c7ffdbd509b3c15b2bdb4df3d2192bfe7b"><code>27fb72c</code></a> merge branch 'pr-3776' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/8ec02ea1b14edac85a6e9a2b622ae44e15e11ccd"><code>8ec02ea</code></a> nsexec: retry unshare on EINVAL</li>
<li><a href="https://github.com/opencontainers/runc/commit/059d7730fc102052c90fea52c7b3c6f04fbbc487"><code>059d773</code></a> merge branch 'pr-3785' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/0abab45c9b97c113ff2cdc16f3a7388444c3fbec"><code>0abab45</code></a> Prohibit /proc and /sys to be symlinks</li>
<li><a href="https://github.com/opencontainers/runc/commit/0e6b818a2b0d24fdb6697614e5c5f115bbe8e3a5"><code>0e6b818</code></a> rootless: fix /sys/fs/cgroup mounts</li>
<li><a href="https://github.com/opencontainers/runc/commit/c6781d100a73d2dcef84e9376d85fff02235a2ed"><code>c6781d1</code></a> Merge pull request <a href="https://redirect.github.com/opencontainers/runc/issues/3721">#3721</a> from kinvolk/rata/nsfixes-backport</li>
<li><a href="https://github.com/opencontainers/runc/commit/f6e2cd3baf661e1f377088e13084ccb5aadf41e6"><code>f6e2cd3</code></a> nsexec: Check for errors in write_log()</li>
<li><a href="https://github.com/opencontainers/runc/commit/3775df9fcb7828594114866e1df346f44d22ad16"><code>3775df9</code></a> Merge pull request <a href="https://redirect.github.com/opencontainers/runc/issues/3731">#3731</a> from kolyshkin/1.1-fix-dev-null</li>
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.1.4...v1.1.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.1.4&new-version=1.1.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 14:50:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4122" class=".btn">#4122</a>
            </td>
            <td>
                <b>
                    Log peer config upon startup (#4118)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Log peer config upon startup.
Also log peer environment variables to help troubleshoot peer config.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 12:34:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4120" class=".btn">#4120</a>
            </td>
            <td>
                <b>
                    Log peer config upon startup (backport #4118)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4118 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 12:14:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4118" class=".btn">#4118</a>
            </td>
            <td>
                <b>
                    Log peer config upon startup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Log peer config upon startup.
Also log peer environment variables to help troubleshoot peer config.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 20:54:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4117" class=".btn">#4117</a>
            </td>
            <td>
                <b>
                    Orderer v3: clean orderer main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: Ie3b1ef94aa6f73a0ac98732cbb4f0bed20d4fe32

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

- Cleaning dead code in orderer/common/server/main.go
- Preventing the server to start with a system channel in the ledger
- Preventing the server to start with a system channel join-block
- Updating tests

#### Related issues

Issue: #3515 
Issue: #4020 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 16:22:54 +0000 UTC
    </div>
</div>

