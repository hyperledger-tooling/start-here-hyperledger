---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1271" class=".btn">#1271</a>
            </td>
            <td>
                <b>
                    Update minimum Java version.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Update the minimum Java version to Java 17+

## Issue fixed

Fixes #1270 

## Impacted parts

- [x] Documentation content
- [ ] Documentation page organization

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

- https://hyperledger-besu--1271.org.readthedocs.build/en/1271/public-networks/get-started/install/binary-distribution/
- https://hyperledger-besu--1271.org.readthedocs.build/en/1271/private-networks/get-started/install/binary-distribution/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 01:48:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    Bump markdown-include from 0.8.0 to 0.8.1 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [markdown-include](https://github.com/cmacmackin/markdown-include) from 0.8.0 to 0.8.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cmacmackin/markdown-include/releases">markdown-include's releases</a>.</em></p>
<blockquote>
<h2>v0.8.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix <code>inheritHeadingDepth</code> adding extra new lines by <a href="https://github.com/ldeluigi"><code>@​ldeluigi</code></a> in <a href="https://github-redirect.dependabot.com/cmacmackin/markdown-include/pull/43">cmacmackin/markdown-include#43</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cmacmackin/markdown-include/compare/v0.8.0...v0.8.1">https://github.com/cmacmackin/markdown-include/compare/v0.8.0...v0.8.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/8da79f095c8ef7e37018387fac5b63b870de077b"><code>8da79f0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/cmacmackin/markdown-include/issues/43">#43</a> from cmacmackin/fix-inherit-heading-depth</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/5135d01609e57b0052799fe5a67f2c2da6bfe060"><code>5135d01</code></a> Use more explicit <code>str.splitlines()</code></li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/7ae38cb8df9df7ed97e9169812675aa7a82a87d6"><code>7ae38cb</code></a> Fix <code>inheritHeadingDepth</code> adding extra newlines</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/4e08bb867ca64f633c901b76d9773f2aceff0001"><code>4e08bb8</code></a> Remove sha-bang</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/0ffd51029e55e9415454e16de968dc4026bc8f35"><code>0ffd510</code></a> Expand gitignore</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/aa4a3800d71da83bfbe27ec80b62aa63ea652040"><code>aa4a380</code></a> Simplify test resource directory path</li>
<li>See full diff in <a href="https://github.com/cmacmackin/markdown-include/compare/v0.8.0...v0.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=markdown-include&package-manager=pip&previous-version=0.8.0&new-version=0.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-02-14 00:00:56 +0000 UTC
    </div>
</div>

