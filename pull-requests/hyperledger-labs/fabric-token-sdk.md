---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/541" class=".btn">#541</a>
            </td>
            <td>
                <b>
                    enhance the token store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR passes to the token store functions also the content of the token stored on the ledger
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 10:14:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/540" class=".btn">#540</a>
            </td>
            <td>
                <b>
                    RWS-based vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR refactors the code to better split the RWS-based token vault. This will make more clear that a different implementation can be plugged.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 09:38:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/539" class=".btn">#539</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc from 1.1.5 to 1.1.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.1.5 to 1.1.12.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/releases">github.com/opencontainers/runc's releases</a>.</em></p>
<blockquote>
<h2>runc 1.1.12 -- &quot;Now you're thinking with Portals™!&quot;</h2>
<p>This is the twelfth patch release in the 1.1.z release branch of runc.
It fixes a high-severity container breakout vulnerability involving
leaked file descriptors, and users are strongly encouraged to update as
soon as possible.</p>
<ul>
<li>
<p>Fix <a href="https://github.com/opencontainers/runc/security/advisories/GHSA-xr7r-f8xq-vfvv">CVE-2024-21626</a>, a container breakout attack that took advantage of
a file descriptor that was leaked internally within runc (but never
leaked to the container process).</p>
<p>In addition to fixing the leak, several strict hardening measures were
added to ensure that future internal leaks could not be used to break
out in this manner again.</p>
<p>Based on our research, while no other container runtime had a similar
leak, none had any of the hardening steps we've introduced (and some
runtimes would not check for any file descriptors that a calling
process may have leaked to them, allowing for container breakouts due
to basic user error).</p>
</li>
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
<p>Thanks to all of the contributors who made this release possible:</p>
<ul>
<li>Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></li>
<li>hang.jiang <a href="mailto:hang.jiang@daocloud.io">hang.jiang@daocloud.io</a></li>
<li>lfbzhm <a href="mailto:lifubang@acmcoder.com">lifubang@acmcoder.com</a></li>
</ul>
<p>Signed-off-by: Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/blob/v1.1.12/CHANGELOG.md">github.com/opencontainers/runc's changelog</a>.</em></p>
<blockquote>
<h2>[1.1.12] - 2024-01-31</h2>
<blockquote>
<p>Now you're thinking with Portals™!</p>
</blockquote>
<h3>Security</h3>
<ul>
<li>Fix <a href="https://github.com/opencontainers/runc/security/advisories/GHSA-xr7r-f8xq-vfvv">CVE-2024-21626</a>, a container breakout attack that took
advantage of a file descriptor that was leaked internally within runc (but
never leaked to the container process). In addition to fixing the leak,
several strict hardening measures were added to ensure that future internal
leaks could not be used to break out in this manner again. Based on our
research, while no other container runtime had a similar leak, none had any
of the hardening steps we've introduced (and some runtimes would not check
for any file descriptors that a calling process may have leaked to them,
allowing for container breakouts due to basic user error).</li>
</ul>
<h2>[1.1.11] - 2024-01-01</h2>
<blockquote>
<p>Happy New Year!</p>
</blockquote>
<h3>Fixed</h3>
<ul>
<li>Fix several issues with userns path handling. (<a href="https://redirect.github.com/opencontainers/runc/issues/4122">#4122</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/4124">#4124</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/4134">#4134</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/4144">#4144</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Support memory.peak and memory.swap.peak in cgroups v2.
Add <code>swapOnlyUsage</code> in <code>MemoryStats</code>. This field reports swap-only usage.
For cgroupv1, <code>Usage</code> and <code>Failcnt</code> are set by subtracting memory usage
from memory+swap usage. For cgroupv2, <code>Usage</code>, <code>Limit</code>, and <code>MaxUsage</code>
are set. (<a href="https://redirect.github.com/opencontainers/runc/issues/4000">#4000</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/4010">#4010</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/4131">#4131</a>)</li>
<li>build(deps): bump github.com/cyphar/filepath-securejoin. (<a href="https://redirect.github.com/opencontainers/runc/issues/4140">#4140</a>)</li>
</ul>
<h2>[1.1.10] - 2023-10-31</h2>
<blockquote>
<p>Śruba, przykręcona we śnie, nie zmieni sytuacji, jaka panuje na jawie.</p>
</blockquote>
<h3>Added</h3>
<ul>
<li>Support for <code>hugetlb.&lt;pagesize&gt;.rsvd</code> limiting and accounting. Fixes the
issue of postres failing when hugepage limits are set. (<a href="https://redirect.github.com/opencontainers/runc/issues/3859">#3859</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/4077">#4077</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fixed permissions of a newly created directories to not depend on the value
of umask in tmpcopyup feature implementation. (<a href="https://redirect.github.com/opencontainers/runc/issues/3991">#3991</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/4060">#4060</a>)</li>
<li>libcontainer: cgroup v1 GetStats now ignores missing <code>kmem.limit_in_bytes</code>
(fixes the compatibility with Linux kernel 6.1+). (<a href="https://redirect.github.com/opencontainers/runc/issues/4028">#4028</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/runc/commit/51d5e94601ceffbbd85688df1c928ecccbfa4685"><code>51d5e94</code></a> VERSION: release 1.1.12</li>
<li><a href="https://github.com/opencontainers/runc/commit/2a4ed3e75b9e80d93d1836a9c4c1ebfa2b78870e"><code>2a4ed3e</code></a> merge 1.1-ghsa-xr7r-f8xq-vfvv into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/e9665f4d606b64bf9c4652ab2510da368bfbd951"><code>e9665f4</code></a> init: don't special-case logrus fds</li>
<li><a href="https://github.com/opencontainers/runc/commit/683ad2ff3b01fb142ece7a8b3829de17150cf688"><code>683ad2f</code></a> libcontainer: mark all non-stdio fds O_CLOEXEC before spawning init</li>
<li><a href="https://github.com/opencontainers/runc/commit/b6633f48a8c970433737b9be5bfe4f25d58a5aa7"><code>b6633f4</code></a> cgroup: plug leaks of /sys/fs/cgroup handle</li>
<li><a href="https://github.com/opencontainers/runc/commit/284ba3057e428f8d6c7afcc3b0ac752e525957df"><code>284ba30</code></a> init: close internal fds before execve</li>
<li><a href="https://github.com/opencontainers/runc/commit/fbe3eed1e568a376f371d2ced1b4ac16b7d7adde"><code>fbe3eed</code></a> setns init: do explicit lookup of execve argument early</li>
<li><a href="https://github.com/opencontainers/runc/commit/0994249a5ec4e363bfcf9af58a87a722e9a3a31b"><code>0994249</code></a> init: verify after chdir that cwd is inside the container</li>
<li><a href="https://github.com/opencontainers/runc/commit/506552a88bd3455e80a9b3829568e94ec0160309"><code>506552a</code></a> Fix File to Close</li>
<li><a href="https://github.com/opencontainers/runc/commit/099ff69336840fecf3fc0ab13aab4c3aded640c3"><code>099ff69</code></a> merge <a href="https://redirect.github.com/opencontainers/runc/issues/4177">#4177</a> into opencontainers/runc:release-1.1</li>
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.1.5...v1.1.12">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.1.5&new-version=1.1.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 22:56:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/538" class=".btn">#538</a>
            </td>
            <td>
                <b>
                    new public params management
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR introduces the following changes:
- Token Driver: public parameters must be available at time of instantiation
- AuditorDB does not require a tms anymore
- if the vault contains the public params, the corresponding tms is instantiated immediately
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 10:20:25 +0000 UTC
    </div>
</div>

