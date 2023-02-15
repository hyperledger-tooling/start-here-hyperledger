---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3525" class=".btn">#3525</a>
            </td>
            <td>
                <b>
                    chore(deps): bump github.com/gogo/protobuf from 1.3.1 to 1.3.2 in /test/bdd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/gogo/protobuf](https://github.com/gogo/protobuf) from 1.3.1 to 1.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gogo/protobuf/releases">github.com/gogo/protobuf's releases</a>.</em></p>
<blockquote>
<h2>Release v.1.3.2</h2>
<h2>Tested versions:</h2>
<p>go 1.15.6
protoc 3.14.0</p>
<h2>Bug fixes:</h2>
<p>skippy peanut butter</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gogo/protobuf/commit/b03c65ea87cdc3521ede29f62fe3ce239267c1bc"><code>b03c65e</code></a> skippy peanut butter</li>
<li><a href="https://github.com/gogo/protobuf/commit/550e88954e617545f49920b752c154d72abf1d8d"><code>550e889</code></a> update to go version 1.15.6 and protoc 3.14.0 (<a href="https://github-redirect.dependabot.com/gogo/protobuf/issues/717">#717</a>)</li>
<li><a href="https://github.com/gogo/protobuf/commit/deb6fe8ca7c6d06584bfbd40ca407bf69d9fd2aa"><code>deb6fe8</code></a> Update Readme.md</li>
<li>See full diff in <a href="https://github.com/gogo/protobuf/compare/v1.3.1...v1.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/gogo/protobuf&package-manager=go_modules&previous-version=1.3.1&new-version=1.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 22:44:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3524" class=".btn">#3524</a>
            </td>
            <td>
                <b>
                    chore(deps): bump github.com/opencontainers/runc from 0.1.1 to 1.1.2 in /test/bdd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 0.1.1 to 1.1.2.
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
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v0.1.1...v1.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=0.1.1&new-version=1.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 23:46:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3523" class=".btn">#3523</a>
            </td>
            <td>
                <b>
                    chore(deps): bump minimist from 1.2.5 to 1.2.8 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/minimistjs/minimist) from 1.2.5 to 1.2.8.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/minimistjs/minimist/blob/main/CHANGELOG.md">minimist's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.7...v1.2.8">v1.2.8</a> - 2023-02-09</h2>
<h3>Merged</h3>
<ul>
<li>[Fix] Fix long option followed by single dash <a href="https://github-redirect.dependabot.com/minimistjs/minimist/pull/17"><code>[#17](https://github.com/minimistjs/minimist/issues/17)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://github-redirect.dependabot.com/minimistjs/minimist/pull/12"><code>[#12](https://github.com/minimistjs/minimist/issues/12)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://github-redirect.dependabot.com/minimistjs/minimist/pull/10"><code>[#10](https://github.com/minimistjs/minimist/issues/10)</code></a></li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[Fix] Fix long option followed by single dash (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/17">#17</a>) <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Tests] Remove duplicate test (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/12">#12</a>) <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] Fix long option followed by single dash <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Fix] opt.string works with multiple aliases (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/10">#10</a>) <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
<li>[Fix] Fix handling of short option with non-trivial equals <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/5"><code>[#5](https://github.com/minimistjs/minimist/issues/5)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>Merge tag 'v0.2.3' <a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/5368ca4147e974138a54cc0dc4cea8f756546b70"><code>5368ca4</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/e5f5067259ceeaf0b098d14bec910f87e58708c7"><code>e5f5067</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/62fde7d935f83417fb046741531a9e2346a36976"><code>62fde7d</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/36ac5d0d95e4947d074e5737d94814034ca335d1"><code>36ac5d0</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/minimistjs/minimist/commit/73923d223553fca08b1ba77e3fbc2a492862ae4c"><code>73923d2</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/minimistjs/minimist/commit/d80727df77bfa9e631044d7f16368d8f09242c91"><code>d80727d</code></a></li>
<li>[eslint] add eslint; rules to enable later are warnings <a href="https://github.com/minimistjs/minimist/commit/48bc06a1b41f00e9cdf183db34f7a51ba70e98d4"><code>48bc06a</code></a></li>
<li>[eslint] fix indentation <a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a></li>
<li>[readme] rename and add badges <a href="https://github.com/minimistjs/minimist/commit/5df0fe49211bd09a3636f8686a7cb3012c3e98f0"><code>5df0fe4</code></a></li>
<li>[Dev Deps] switch from <code>covert</code> to <code>nyc</code> <a href="https://github.com/minimistjs/minimist/commit/a48b128fdb8d427dfb20a15273f83e38d97bef07"><code>a48b128</code></a></li>
<li>[Dev Deps] update <code>covert</code>, <code>tape</code>; remove unnecessary <code>tap</code> <a href="https://github.com/minimistjs/minimist/commit/f0fb958e9a1fe980cdffc436a211b0bda58f621b"><code>f0fb958</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/minimistjs/minimist/commit/3639e0c819359a366387e425ab6eabf4c78d3caa"><code>3639e0c</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/minimistjs/minimist/commit/be2e038c342d8333b32f0fde67a0026b79c8150e"><code>be2e038</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/minimistjs/minimist/commit/282b570e7489d01b03f2d6d3dabf79cd3e5f84cf"><code>282b570</code></a></li>
<li>isConstructorOrProto adapted from PR <a href="https://github.com/minimistjs/minimist/commit/ef9153fc52b6cea0744b2239921c5dcae4697f11"><code>ef9153f</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/3124ed3e46306301ebb3c834874ce0241555c2c4"><code>3124ed3</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/minimistjs/minimist/commit/4b927de696d561c636b4f43bf49d4597cb36d6d6"><code>4b927de</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/minimistjs/minimist/commit/b32d9bd0ab340f4e9f8c3a97ff2a4424f25fab8c"><code>b32d9bd</code></a></li>
<li>[meta] update repo URLs <a href="https://github.com/minimistjs/minimist/commit/f9fdfc032c54884d9a9996a390c63cd0719bbe1a"><code>f9fdfc0</code></a></li>
<li>[actions] Avoid 0.6 tests due to build failures <a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/minimistjs/minimist/commit/950eaa74f112e04d23e9c606c67472c46739b473"><code>950eaa7</code></a></li>
<li>[Dev Deps] add missing <code>npmignore</code> dev dep <a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a></li>
<li>Merge tag 'v0.2.2' <a href="https://github.com/minimistjs/minimist/commit/980d7ac61a0b4bd552711251ac107d506b23e41f"><code>980d7ac</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.6...v1.2.7">v1.2.7</a> - 2022-10-10</h2>
<h3>Commits</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/minimistjs/minimist/commit/6901ee286bc4c16da6830b48b46ce1574703cea1"><code>6901ee2</code></a> v1.2.8</li>
<li><a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a> Merge tag 'v0.2.3'</li>
<li><a href="https://github.com/minimistjs/minimist/commit/c0b26618322e94adea26c68e613ef0be482c6c63"><code>c0b2661</code></a> v0.2.3</li>
<li><a href="https://github.com/minimistjs/minimist/commit/63b8fee87b8e7a003216d5d77ba5d6decf3cfb0d"><code>63b8fee</code></a> [Fix] Fix long option followed by single dash (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/17">#17</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/72239e6f0ea77d8be0ad4f682b7ae7d142144395"><code>72239e6</code></a> [Tests] Remove duplicate test (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/12">#12</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a> [eslint] fix indentation</li>
<li><a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a> [Dev Deps] add missing <code>npmignore</code> dev dep</li>
<li><a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a> [Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/9ec4d279ced72ea2f60237218e71cc03aa0dfdd6"><code>9ec4d27</code></a> [Fix] Fix long option followed by single dash</li>
<li><a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a> [actions] Avoid 0.6 tests due to build failures</li>
<li>Additional commits viewable in <a href="https://github.com/minimistjs/minimist/compare/v1.2.5...v1.2.8">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for minimist since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 09:00:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3522" class=".btn">#3522</a>
            </td>
            <td>
                <b>
                    chore: Additional validation when creating disclosed claims (verifier)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Additional validation when processing disclosures to assemble disclosed claims:

- If there is more than one place where the digest is included, the Verifier MUST reject the Presentation.
- If the claim name already exists at the same level, the Verifier MUST reject the Presentation.
- If the claim value contains an object with an _sd key (at the top level or nested deeper), the Verifier MUST reject the Presentation.

Closes #3519



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 18:20:28 +0000 UTC
    </div>
</div>

