---
layout: default
title: aries-framework-go-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go-ext
---

# aries-framework-go-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump github.com/opencontainers/runc from 1.0.2 to 1.1.2 in /test/bdd/vdr/orb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.0.2 to 1.1.2.
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
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.0.2...v1.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.0.2&new-version=1.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 02:20:05 +0000 UTC
    </div>
</div>

