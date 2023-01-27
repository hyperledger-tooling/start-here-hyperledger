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
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump simple-git from 3.15.0 to 3.16.0 in /opssc-agent/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [simple-git](https://github.com/steveukx/git-js/tree/HEAD/simple-git) from 3.15.0 to 3.16.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/steveukx/git-js/releases">simple-git's releases</a>.</em></p>
<blockquote>
<h2>simple-git@3.16.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>97fde2c: Support the use of <code>-B</code> in place of the default <code>-b</code> in checkout methods</li>
<li>0a623e5: Adds vulnerability detection to prevent use of <code>--upload-pack</code> and <code>--receive-pack</code> without explicitly opting in.</li>
</ul>
<h3>Patch Changes</h3>
<ul>
<li>ec97a39: Include restricting the use of git push --exec with other allowUnsafePack exclusions, thanks to <a href="https://github.com/stsewd"><code>@​stsewd</code></a> for the suggestion.</li>
</ul>
<h2>simple-git@3.15.1</h2>
<h3>Patch Changes</h3>
<ul>
<li>de570ac: Resolves an issue whereby non-strings can be passed into the config switch detector.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/steveukx/git-js/blob/main/simple-git/CHANGELOG.md">simple-git's changelog</a>.</em></p>
<blockquote>
<h2>3.16.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>97fde2c: Support the use of <code>-B</code> in place of the default <code>-b</code> in checkout methods</li>
<li>0a623e5: Adds vulnerability detection to prevent use of <code>--upload-pack</code> and <code>--receive-pack</code> without explicitly opting in.</li>
</ul>
<h3>Patch Changes</h3>
<ul>
<li>ec97a39: Include restricting the use of git push --exec with other allowUnsafePack exclusions, thanks to <a href="https://github.com/stsewd"><code>@​stsewd</code></a> for the suggestion.</li>
</ul>
<h2>3.15.1</h2>
<h3>Patch Changes</h3>
<ul>
<li>de570ac: Resolves an issue whereby non-strings can be passed into the config switch detector.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/steveukx/git-js/commit/1a129523abadb877ad3e0bad362cc06593f04135"><code>1a12952</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/ec97a39ab60b89e870c5170121cd9c1603cc1951"><code>ec97a39</code></a> Block unsafe pack (push --exec) (<a href="https://github.com/steveukx/git-js/tree/HEAD/simple-git/issues/882">#882</a>)</li>
<li><a href="https://github.com/steveukx/git-js/commit/0a623e53fd4b7617ca9c4d1d51bc53d105f52b2b"><code>0a623e5</code></a> Feat/unsafe pack (<a href="https://github.com/steveukx/git-js/tree/HEAD/simple-git/issues/881">#881</a>)</li>
<li><a href="https://github.com/steveukx/git-js/commit/97fde2c44f08abfdfa591c03d883b215f2d547d3"><code>97fde2c</code></a> Add support for using the <code>-B</code> modifier instead of the default <code>-b</code> when usin...</li>
<li><a href="https://github.com/steveukx/git-js/commit/edfd4595194d83663a0299a63c32cb150a78b6da"><code>edfd459</code></a> Update readme.md</li>
<li><a href="https://github.com/steveukx/git-js/commit/c9fc61f4abfb4f738ab9f4b5bd146555b7b9735c"><code>c9fc61f</code></a> Version Packages</li>
<li><a href="https://github.com/steveukx/git-js/commit/de570acd052660bad0165347de5d2f86a494ae1b"><code>de570ac</code></a> Fix/non strings (<a href="https://github.com/steveukx/git-js/tree/HEAD/simple-git/issues/867">#867</a>)</li>
<li>See full diff in <a href="https://github.com/steveukx/git-js/commits/simple-git@3.16.0/simple-git">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-git&package-manager=npm_and_yarn&previous-version=3.15.0&new-version=3.16.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-27 04:17:28 +0000 UTC
    </div>
</div>

