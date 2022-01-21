---
layout: default
title: aries-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-toolbox
---

# aries-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Various fixes and improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes:

- Improved formatting on various data summaries
- Presentations are now auto loaded on entering verification section
- Added status icons to credentials and presentations
  - Enabled removal of listings that were grouped by status. Now, each item is all in one list but status is indicated. This significantly simplified code in a few places.
- Make sure select inputs have English "no data" warnings instead of Chinese
- Add context menus (enables copy/paste through right clicks)
- Disable presentation proposal (which is not currently functional)
- Visual improvements for Agent List window
- Use enter key for triggering form actions where it makes sense
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 04:50:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    fix: invitations auto-accept defaults to true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Once form is cleared for next input

Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 20:08:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    fix: did creation form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 17:00:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump marked from 4.0.9 to 4.0.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [marked](https://github.com/markedjs/marked) from 4.0.9 to 4.0.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/markedjs/marked/releases">marked's releases</a>.</em></p>
<blockquote>
<h2>v4.0.10</h2>
<h2><a href="https://github.com/markedjs/marked/compare/v4.0.9...v4.0.10">4.0.10</a> (2022-01-13)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> fix redos vulnerabilities (<a href="https://github.com/markedjs/marked/commit/8f806573a3f6c6b7a39b8cdb66ab5ebb8d55a5f5">8f80657</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/markedjs/marked/commit/ae01170085e89ccd85c233547011eb88420a90cf"><code>ae01170</code></a> chore(release): 4.0.10 [skip ci]</li>
<li><a href="https://github.com/markedjs/marked/commit/fceda573673d7fb00a5e89476a0328d4ecdb7cb7"><code>fceda57</code></a> 🗜️ build [skip ci]</li>
<li><a href="https://github.com/markedjs/marked/commit/8f806573a3f6c6b7a39b8cdb66ab5ebb8d55a5f5"><code>8f80657</code></a> fix(security): fix redos vulnerabilities</li>
<li><a href="https://github.com/markedjs/marked/commit/c4a3ccd344b6929afa8a1d50ac54a721e57012c0"><code>c4a3ccd</code></a> Merge pull request from GHSA-rrrm-qjm4-v8hf</li>
<li><a href="https://github.com/markedjs/marked/commit/d7212a63841a581de54899c20943627f6aa5dbda"><code>d7212a6</code></a> chore(deps-dev): Bump jasmine from 4.0.0 to 4.0.1 (<a href="https://github-redirect.dependabot.com/markedjs/marked/issues/2352">#2352</a>)</li>
<li><a href="https://github.com/markedjs/marked/commit/5a84db5598030890052d27961cc4c8f5eb353df2"><code>5a84db5</code></a> chore(deps-dev): Bump rollup from 2.62.0 to 2.63.0 (<a href="https://github-redirect.dependabot.com/markedjs/marked/issues/2350">#2350</a>)</li>
<li><a href="https://github.com/markedjs/marked/commit/2bc67a5285800008b6dba4d716e6656e5d4ec55f"><code>2bc67a5</code></a> chore(deps-dev): Bump markdown-it from 12.3.0 to 12.3.2 (<a href="https://github-redirect.dependabot.com/markedjs/marked/issues/2351">#2351</a>)</li>
<li><a href="https://github.com/markedjs/marked/commit/98996b853c1b62ba6177c4453ee44f5de42619c9"><code>98996b8</code></a> chore(deps-dev): Bump <code>@​babel/preset-env</code> from 7.16.5 to 7.16.7 (<a href="https://github-redirect.dependabot.com/markedjs/marked/issues/2353">#2353</a>)</li>
<li><a href="https://github.com/markedjs/marked/commit/ebc2c953e7e8bafb6fa7e2792142dcbfbe959f15"><code>ebc2c95</code></a> chore(deps-dev): Bump highlight.js from 11.3.1 to 11.4.0 (<a href="https://github-redirect.dependabot.com/markedjs/marked/issues/2354">#2354</a>)</li>
<li>See full diff in <a href="https://github.com/markedjs/marked/compare/v4.0.9...v4.0.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=marked&package-manager=npm_and_yarn&previous-version=4.0.9&new-version=4.0.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 03:56:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    feat: added recent message history into compose tab
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: PeterStrob <peter@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 21:50:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    fix: predicate issue with self-attested attrs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Micah Peltier <micah6_8@yahoo.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 21:05:59 +0000 UTC
    </div>
</div>

