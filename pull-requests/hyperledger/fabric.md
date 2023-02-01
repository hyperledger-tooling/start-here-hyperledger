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
                PR <a href="https://github.com/hyperledger/fabric/pull/3977" class=".btn">#3977</a>
            </td>
            <td>
                <b>
                    Move purge private data tests to separate runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 10:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3975" class=".btn">#3975</a>
            </td>
            <td>
                <b>
                    Add BFT support to gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extend the gateway Submit() logic to concurrently send transaction to all available orderers if the channel is configured to use BFT ordering service.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 16:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3974" class=".btn">#3974</a>
            </td>
            <td>
                <b>
                    Improve logging for orderer endpoint override (backport #3969)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3969 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-28 16:15:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3973" class=".btn">#3973</a>
            </td>
            <td>
                <b>
                    Improve logging for orderer endpoint override (backport #3969)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3969 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-28 16:14:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3972" class=".btn">#3972</a>
            </td>
            <td>
                <b>
                    Remove whitespace character from ORDERER_GENERAL_LISTENPORT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: kartik chauhan <chauhan.kartik25@gmail.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->
env variable `ORDERER_GENERAL_ LISTENPORT` in section `Experimenting with the orderer service` of the page https://github.com/hyperledger/fabric/tree/main/orderer contains a whitespace character. Fixed the issue by removing the whitespace character.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->
https://github.com/hyperledger/fabric/issues/3971

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-28 03:57:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3970" class=".btn">#3970</a>
            </td>
            <td>
                <b>
                    Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test whether a new peer is able to reconcile from a purged peer

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 17:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3969" class=".btn">#3969</a>
            </td>
            <td>
                <b>
                    Improve logging for orderer endpoint override
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When writing log messages for orderer connections, the log address was being extracted from the wrong object.  This is fixed here. Also a debug log message is now written before connecting if the address is overridden.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 17:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3968" class=".btn">#3968</a>
            </td>
            <td>
                <b>
                    Retire inactive maintainers.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Jay Guo's last activities:

| Date | Time | Type | Action
|---|---|---|---
| 2022-07-03 | 15:36:02Z | IssueCommentEvent | created
| 2022-03-14 | 06:34:18Z | PullRequestEvent | opened
| 2022-03-14 | 02:58:20Z | IssueCommentEvent | created
| 2022-03-06 | 11:19:57Z | IssueCommentEvent | created
| 2022-03-04 | 07:43:17Z | IssuesEvent | reopened
| 2022-03-04 | 07:43:16Z | IssueCommentEvent | created

Senthilnathan Natarajan's last activity:

| Date | Time | Type | Action
|---|---|---|---
| 2022-03-25 | 04:01:13Z | PullRequestReviewEvent | created


Signed-off-by: Ry Jones <ry@linux.com>

#### Type of change

- Documentation update

#### Description

Retire inactive maintainers

#### Additional details

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 16:54:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3967" class=".btn">#3967</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.4.3 to 1.5.16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.4.3 to 1.5.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/releases">github.com/containerd/containerd's releases</a>.</em></p>
<blockquote>
<h2>containerd 1.5.16</h2>
<p>Welcome to the v1.5.16 release of containerd!</p>
<p>The sixteenth patch release for containerd 1.5 contains a fix for CVE-2022-23471.</p>
<h3>Notable Updates</h3>
<ul>
<li><strong>Fix goroutine leak during Exec in CRI plugin</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-2qjp-425j-52j9">GHSA-2qjp-425j-52j9</a>)</li>
</ul>
<p>See the changelog for complete list of changes</p>
<p>Please try out the release binaries and report any issues at
<a href="https://github.com/containerd/containerd/issues">https://github.com/containerd/containerd/issues</a>.</p>
<h3>Contributors</h3>
<ul>
<li>Derek McGowan</li>
<li>Danny Canter</li>
<li>Phil Estes</li>
<li>Sebastiaan van Stijn</li>
</ul>
<h3>Changes</h3>
<!-- raw HTML omitted -->
<ul>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-2qjp-425j-52j9">GHSA-2qjp-425j-52j9</a>
<ul>
<li>Prepare release notes for v1.5.16</li>
<li>CRI stream server: Fix goroutine leak in Exec</li>
</ul>
</li>
<li>[release/1.5] update to go1.18.9 (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/7767">#7767</a>)
<ul>
<li>[release/1.5] update to go1.18.9</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
<h3>Dependency Changes</h3>
<p>This release has no dependency changes</p>
<p>Previous release can be found at <a href="https://github.com/containerd/containerd/releases/tag/v1.5.15">v1.5.15</a></p>
<h2>containerd 1.5.15</h2>
<p>Welcome to the v1.5.15 release of containerd!</p>
<p>The fifteenth patch release for containerd 1.5 includes various fixes including a
fix for a long time issue with CNI resource leakage.</p>
<h3>Notable Updates</h3>
<ul>
<li><strong>Fix CNI leaks by changing pod network setup order in CRI plugin</strong> (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/7464">#7464</a>)</li>
<li><strong>Fix request retry on push</strong> (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/7479">#7479</a>)</li>
<li><strong>Fix lease labels unexpectedly overwriting expiration</strong> (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/7746">#7746</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/2e3140a0e09d288a9086474752b4478aa0964e7c"><code>2e3140a</code></a> Merge pull request from GHSA-2qjp-425j-52j9</li>
<li><a href="https://github.com/containerd/containerd/commit/189c7c339bd67877a9a588b92550018d578de21b"><code>189c7c3</code></a> Prepare release notes for v1.5.16</li>
<li><a href="https://github.com/containerd/containerd/commit/6cd11527fcc2b4e4efab90cd677dd87d6fe2e4e8"><code>6cd1152</code></a> CRI stream server: Fix goroutine leak in Exec</li>
<li><a href="https://github.com/containerd/containerd/commit/2f59a97ae97074721f4a4749821e46603a90f720"><code>2f59a97</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/7767">#7767</a> from thaJeztah/1.5_update_go_1.18.9</li>
<li><a href="https://github.com/containerd/containerd/commit/46e2ef099401a051780688ad0b6a72b35b9b3681"><code>46e2ef0</code></a> [release/1.5] update to go1.18.9</li>
<li><a href="https://github.com/containerd/containerd/commit/99a380dbf7a22ad7937ff96516b94261b5281926"><code>99a380d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/7759">#7759</a> from dmcgowan/prepare-1.5.15</li>
<li><a href="https://github.com/containerd/containerd/commit/9ab22bf3e3d85e802e8dbe8c8934c8e0368b44f0"><code>9ab22bf</code></a> Prepare release notes for v1.5.15</li>
<li><a href="https://github.com/containerd/containerd/commit/a0a9a0e22b0eaa76025c6a466d723b691e506175"><code>a0a9a0e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/7746">#7746</a> from austinvazquez/cherry-pick-c4dee237f57a7f7895aaa...</li>
<li><a href="https://github.com/containerd/containerd/commit/1de818aa1ae0ec60de5fd23544f5e7cef2c6087f"><code>1de818a</code></a> Fix order of operations when setting lease labels</li>
<li><a href="https://github.com/containerd/containerd/commit/7b7a9fb605a811ac2ae3ebd115921306aaa73a96"><code>7b7a9fb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/7722">#7722</a> from thaJeztah/1.5_protobuf_extensions_fix</li>
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.4.3...v1.5.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.4.3&new-version=1.5.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 15:48:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3966" class=".btn">#3966</a>
            </td>
            <td>
                <b>
                    Fix maintainers file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add Yoav Tock to list of maintainers.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 15:47:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3965" class=".btn">#3965</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc from 1.0.0-rc8 to 1.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.0.0-rc8 to 1.1.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/releases">github.com/opencontainers/runc's releases</a>.</em></p>
<blockquote>
<h2>runc 1.1 -- &quot;A plan depends as much upon execution as it does upon concept.&quot;</h2>
<p>This release only contains very minor changes from v1.1.0-rc.1 and is
the first release of the 1.1.y release series of runc. We do not plan to make
any new releases of the 1.0.y release series of runc, so users are strongly
encouraged to update to 1.1.0.</p>
<p>Changed:</p>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
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
<p>Thanks to the following people who made this release possible:</p>
<ul>
<li>Akihiro Suda <a href="mailto:akihiro.suda.cz@hco.ntt.co.jp">akihiro.suda.cz@hco.ntt.co.jp</a></li>
<li>Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></li>
<li>Kir Kolyshkin <a href="mailto:kolyshkin@gmail.com">kolyshkin@gmail.com</a></li>
</ul>
<p>Signed-off-by: Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></p>
<h2>runc 1.1-rc1 -- &quot;He who controls the spice controls the universe.&quot;</h2>
<p>This release is the first release candidate for the next minor release
following runc 1.0. It contains all of the bugfixes included in runc 1.0
patch releases (up to and including 1.0.3).</p>
<p>A fair few new features have been added, and several features have been
deprecated (with plans for removal in runc 1.2). At the moment we only
plan to do a single release candidate for runc 1.1, and once 1.1.0 is
released we will not continue updating the 1.0.z runc branch.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/blob/main/CHANGELOG.md">github.com/opencontainers/runc's changelog</a>.</em></p>
<blockquote>
<h2>[1.1.2] - 2022-05-11</h2>
<blockquote>
<p>I should think I'm going to be a perpetual student.</p>
</blockquote>
<h3>Security</h3>
<ul>
<li>A bug was found in runc where runc exec --cap executed processes with
non-empty inheritable Linux process capabilities, creating an atypical Linux
environment. For more information, see <a href="https://github.com/opencontainers/runc/security/advisories/GHSA-f3fp-gc8g-vw66">GHSA-f3fp-gc8g-vw66</a> and
CVE-2022-29162.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>runc spec</code> no longer sets any inheritable capabilities in the created
example OCI spec (<code>config.json</code>) file.</li>
</ul>
<h2>[1.1.1] - 2022-03-28</h2>
<blockquote>
<p>Violence is the last refuge of the incompetent.</p>
</blockquote>
<h3>Added</h3>
<ul>
<li>CI is now also run on centos-stream-9. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li><code>runc run/start</code> can now run a container with read-only <code>/dev</code> in OCI spec,
rather than error out. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3355">#3355</a>)</li>
<li><code>runc exec</code> now ensures that <code>--cgroup</code> argument is a sub-cgroup. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3403">#3403</a>)</li>
<li>libcontainer systemd v2 manager no longer errors out if one of the files
listed in <code>/sys/kernel/cgroup/delegate</code> do not exist in container's cgroup.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3387">#3387</a>, <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3404">#3404</a>)</li>
<li>Loose OCI spec validation to avoid bogus &quot;Intel RDT is not supported&quot; error.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3406">#3406</a>)</li>
<li>libcontainer/cgroups no longer panics in cgroup v1 managers if <code>stat</code>
of <code>/sys/fs/cgroup/unified</code> returns an error other than ENOENT. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3435">#3435</a>)</li>
</ul>
<h2>[1.1.0] - 2022-01-14</h2>
<blockquote>
<p>A plan depends as much upon execution as it does upon concept.</p>
</blockquote>
<h3>Changed</h3>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
</ul>
<h2>[1.1.0-rc.1] - 2021-12-14</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/runc/commit/a916309fff0f838eb94e928713dbc3c0d0ac7aa4"><code>a916309</code></a> VERSION: release 1.1.2</li>
<li><a href="https://github.com/opencontainers/runc/commit/364ec0f1b4fa188ad96049c590ecb42fa70ea165"><code>364ec0f</code></a> runc: do not set inheritable capabilities</li>
<li><a href="https://github.com/opencontainers/runc/commit/58546650ce11cdc2e2690bcb1de4a468e691de6d"><code>5854665</code></a> merge branch 'pr-3439' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/8959e372549a81ac6a7cc25281f6b8a423d847ca"><code>8959e37</code></a> VERSION: back to development</li>
<li><a href="https://github.com/opencontainers/runc/commit/52de29d7e0f8c0899bd7efb8810dd07f0073fa87"><code>52de29d</code></a> VERSION: release 1.1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/2636e1cb3643c87f98b7b8a950c88087656e7645"><code>2636e1c</code></a> CHANGELOG.md: add 1.1.1 release notes</li>
<li><a href="https://github.com/opencontainers/runc/commit/ae28db14244c87ab1e26db09a8ad6e5b2882ccc7"><code>ae28db1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a> from kolyshkin/1.1-add-centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/036cc348994b7fa573380401644a6faac9e102e7"><code>036cc34</code></a> CI/cirrus: add centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/c65363285b3eee6e2e3a7b356f8967ae17263d41"><code>c653632</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3438">#3438</a> from kolyshkin/1.1-fix-badges</li>
<li><a href="https://github.com/opencontainers/runc/commit/db953158e14658c62ad6cda9ac087bdb1b1e3e8c"><code>db95315</code></a> README.md: add cirrus-ci badge</li>
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.0.0-rc8...v1.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.0.0-rc8&new-version=1.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 15:47:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3964" class=".btn">#3964</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/image-spec from 1.0.1 to 1.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/image-spec](https://github.com/opencontainers/image-spec) from 1.0.1 to 1.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/image-spec/releases">github.com/opencontainers/image-spec's releases</a>.</em></p>
<blockquote>
<h2>v1.0.2</h2>
<p>This release was voted on by the maintainers and PASSED (+5 -0 <a href="https://github-redirect.dependabot.com/opencontainers/image-spec/issues/2">#2</a>), to mitigate the CVE-2021-41190 advisory.</p>
<p>This release is rebased directly on the prior tagged release (not including the commits that have occurred on main). Corresponding commits have been added to main, such that main is ready for a future next release.</p>
<p><img src="https://user-images.githubusercontent.com/67049/142260429-9da17e3d-c6dd-4721-89bb-0ef72ef69c22.gif" alt="R" /></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/image-spec/commit/67d2d5658fe0476ab9bf414cec164077ebff3920"><code>67d2d56</code></a> version: release 1.0.2</li>
<li><a href="https://github.com/opencontainers/image-spec/commit/dcdcb7f2cf08641d03189e5b09be32de5dcfe459"><code>dcdcb7f</code></a> specs-go: adding <code>mediaType</code> to the index and manifest structures</li>
<li><a href="https://github.com/opencontainers/image-spec/commit/5f3148525b82017cb470ff5f54b37aae4003eb07"><code>5f31485</code></a> *.md: bring mediaType out of reserved status</li>
<li>See full diff in <a href="https://github.com/opencontainers/image-spec/compare/v1.0.1...v1.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/image-spec&package-manager=go_modules&previous-version=1.0.1&new-version=1.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 15:47:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3962" class=".btn">#3962</a>
            </td>
            <td>
                <b>
                    Fix the build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The commit https://github.com/hyperledger/fabric/commit/116551e788071298854f3d61df198b32d0b3156d added a scenario test that uses the FullEtcdRaft() network.  This had been removed in an earlier commit. The test has been changed to use BasicEtcRaft()

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 15:26:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3960" class=".btn">#3960</a>
            </td>
            <td>
                <b>
                    Release commit for v2.5.0-beta
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.5.0-beta.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 16:35:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3959" class=".btn">#3959</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.10 (main)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.10.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 16:01:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3958" class=".btn">#3958</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.10 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.10.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 15:56:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3957" class=".btn">#3957</a>
            </td>
            <td>
                <b>
                    Nominate Yoav Tock to be a maintainer of Fabric core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Yoav has been a significant contributor to Fabric core's ordering service. 

He designed and implemented the system channel removal feature which is one of the two main features in Fabric v2.3.

He also took part in the implementation of the SmartBFT consensus library (https://github.com/SmartBFT-Go/consensus/) which is now being introduced as the first BFT consensus of Fabric. 

Currently, he plays an important role in the re-architecture of the ordering service for Fabric v3.0 which includes:

- Removing the support for Kafka 
- Removing the system channel from the ordering service
- Inverting the control between the Fabric consensus and the dependencies. 

Additionally, he participates in code reviews of pull requests with high risk potential such as: https://github.com/hyperledger/fabric/pull/3863 and https://github.com/hyperledger/fabric/pull/3651

Lastly, he is among the top contributors of code in the last several months.

I therefore nominate Yoav as a maintainer of Fabric core. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 14:31:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3956" class=".btn">#3956</a>
            </td>
            <td>
                <b>
                    Update my email address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit updates my email address to my new IBM email

Signed-off-by: Yacov Manevich <yacov.manevich@ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 14:28:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3955" class=".btn">#3955</a>
            </td>
            <td>
                <b>
                    Release commit for v2.4.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.4.8.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 14:18:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3954" class=".btn">#3954</a>
            </td>
            <td>
                <b>
                    Document broadcast timeout (backport #3952)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3952 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-26 13:31:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3953" class=".btn">#3953</a>
            </td>
            <td>
                <b>
                    License name in swagger should be Apache-2.0 (backport #3951)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3951 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-26 13:30:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3952" class=".btn">#3952</a>
            </td>
            <td>
                <b>
                    Document broadcast timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add details of the broadcastTimeout config option to the Gateway docs page

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 10:49:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3951" class=".btn">#3951</a>
            </td>
            <td>
                <b>
                    License name in swagger should be Apache-2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #3949 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 10:49:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3950" class=".btn">#3950</a>
            </td>
            <td>
                <b>
                    Update release action to trigger from tag (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update release action to trigger from tag instead of manual workflow_dispatch.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 05:54:51 +0000 UTC
    </div>
</div>

