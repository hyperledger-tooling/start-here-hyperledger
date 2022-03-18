---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump simple-git from 2.45.1 to 3.3.0 in /opssc-agent/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [simple-git](https://github.com/steveukx/git-js/tree/HEAD/simple-git) from 2.45.1 to 3.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/steveukx/git-js/releases">simple-git's releases</a>.</em></p>
<blockquote>
<h2>simple-git@3.3.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>d119ec4: Resolves potential command injection vulnerability by preventing use of <code>--upload-pack</code> in <code>git.fetch</code></li>
</ul>
<h2>simple-git@3.2.6</h2>
<h3>Patch Changes</h3>
<ul>
<li>80651d5: Resolve issue in prePublish script</li>
</ul>
<h2>simple-git@3.2.4</h2>
<h3>Patch Changes</h3>
<ul>
<li>d35987b: Release with changesets</li>
</ul>
<h2>simple-git simple-git-v3.1.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>specify repository with <code>directory</code> identifier to be discoverable within monorepo (<a href="https://www.github.com/steveukx/git-js/commit/655e23ce70e94e9213a0da2001ad883966c37b2e">655e23c</a>)</li>
</ul>
<h2>simple-git simple-git-v3.1.0</h2>
<h3>Features</h3>
<ul>
<li>optionally include ignored files in <code>StatusResult</code> (<a href="https://www.github.com/steveukx/git-js/commit/70e676759012d26ab644644e10f7957fba51ae2f">70e6767</a>), closes <a href="https://github-redirect.dependabot.com/steveukx/git-js/issues/718">#718</a></li>
</ul>
<h2>simple-git simple-git-v3.0.4</h2>
<h3>Bug Fixes</h3>
<ul>
<li>support parsing empty responses (<a href="https://www.github.com/steveukx/git-js/commit/91eb7fb01fe466468537621cb94b9f932026506e">91eb7fb</a>), closes <a href="https://github-redirect.dependabot.com/steveukx/git-js/issues/713">#713</a></li>
</ul>
<h2>simple-git simple-git-v3.0.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>allow branches without labels (<a href="https://www.github.com/steveukx/git-js/commit/07a138808fb0b78068da83030698a957e567541c">07a1388</a>)</li>
<li>implement v3 deprecations (<a href="https://www.github.com/steveukx/git-js/commit/ed6d18e88a6a4f9fd18d4733a94b491e0e9e3ba1">ed6d18e</a>)</li>
<li>publish v3 as <code>latest</code> (<a href="https://www.github.com/steveukx/git-js/commit/5db4434d00acba560fe2569c04f9813cde026468">5db4434</a>)</li>
</ul>
<h2>simple-git simple-git-v3.0.2</h2>
<h3>Bug Fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/steveukx/git-js/blob/main/simple-git/CHANGELOG.md">simple-git's changelog</a>.</em></p>
<blockquote>
<h2>3.3.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>d119ec4: Resolves potential command injection vulnerability by preventing use of <code>--upload-pack</code> in <code>git.fetch</code></li>
</ul>
<h2>3.2.6</h2>
<h3>Patch Changes</h3>
<ul>
<li>80651d5: Resolve issue in prePublish script</li>
</ul>
<h2>3.2.5</h2>
<h3>Patch Changes</h3>
<ul>
<li>ac4f38f: Show readme in published package.</li>
</ul>
<h2>3.2.4</h2>
<h3>Patch Changes</h3>
<ul>
<li>d35987b: Release with changesets</li>
</ul>
<h2>3.2.3</h2>
<h3>Patch Changes</h3>
<ul>
<li>1e4c591: Release with changesets</li>
</ul>
<h2>3.2.2</h2>
<h3>Patch Changes</h3>
<ul>
<li>497d416: Releasing with changeset</li>
</ul>
<h2>3.2.1</h2>
<h3>Patch Changes</h3>
<ul>
<li>0c3085d: Releasing library through changesets</li>
</ul>
<h2>3.2.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>b47aa19: Switch to <code>changesets</code> as version and changelog manager</li>
</ul>
<h3><a href="https://www.github.com/steveukx/git-js/compare/simple-git-v3.1.0...simple-git-v3.1.1">3.1.1</a> (2022-01-26)</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/steveukx/git-js/commit/91133663c9f264c31148744c1a5bd56ec46d952e"><code>9113366</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/d119ec44222796cf14f6dde60bf8c40931b5a125"><code>d119ec4</code></a> Prevent use of <code>--upload-pack</code> as a command in <code>git.fetch</code> to avoid potential...</li>
<li><a href="https://github.com/steveukx/git-js/commit/fcc7618f901501040e454f6629755b97f5b63c90"><code>fcc7618</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/80651d56bd9017b5da34a4f0fa31bbd4ce9ddae7"><code>80651d5</code></a> Remove pre-publish step of copying <code>readme.md</code>, no longer required</li>
<li><a href="https://github.com/steveukx/git-js/commit/6838e244a10cc76ab5b8204ddabf95757861bec4"><code>6838e24</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/e9f046173059b4fce08e066a14381c1256e5ea79"><code>e9f0461</code></a> Move workspace readme into the <code>simple-git</code> package, symlink to it from the w...</li>
<li><a href="https://github.com/steveukx/git-js/commit/7a29566b1950d16dd1978e3fd6f7abdfeb3e94ad"><code>7a29566</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/c4f937d93dd3c6b76fd8b94b454ed030cc47ce71"><code>c4f937d</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/c4861657fb8298d5c2e7989c62b3d99c9e656894"><code>c486165</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/497d416498c4715ec8d06632ac02bda2f24697fc"><code>497d416</code></a> Running the changesets release</li>
<li>Additional commits viewable in <a href="https://github.com/steveukx/git-js/commits/simple-git@3.3.0/simple-git">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-git&package-manager=npm_and_yarn&previous-version=2.45.1&new-version=3.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 22:06:48 +0000 UTC
    </div>
</div>

