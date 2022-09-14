---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Bump trim-newlines from 1.0.0 to 3.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [trim-newlines](https://github.com/sindresorhus/trim-newlines) from 1.0.0 to 3.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/trim-newlines/releases">trim-newlines's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<p>Breaking:</p>
<ul>
<li>Require Node.js 8 (<a href="https://github-redirect.dependabot.com/sindresorhus/trim-newlines/issues/1">#1</a>)  75db891</li>
</ul>
<p>Enhancements:</p>
<ul>
<li>Add TypeScript definition (<a href="https://github-redirect.dependabot.com/sindresorhus/trim-newlines/issues/1">#1</a>)  75db891</li>
</ul>
<p><a href="https://github.com/sindresorhus/trim-newlines/compare/v2.0.0...v3.0.0">https://github.com/sindresorhus/trim-newlines/compare/v2.0.0...v3.0.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/sindresorhus/trim-newlines/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=trim-newlines&package-manager=npm_and_yarn&previous-version=1.0.0&new-version=3.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 15:48:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    Join channel better error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Modem [nikhil.modem@ibm.com](mailto:nikhil.modem@ibm.com)

#### Type of change

- Bug fix
- Improvement (improvement to code, performance, etc)

#### Description
- When entering a non-existent channel name when adding a peer to a channel, the error message was not caught and formatted well.
- Now checks the grpc status and formats the error message properly 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 07:52:53 +0000 UTC
    </div>
</div>

