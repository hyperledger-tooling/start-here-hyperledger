---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1882" class=".btn">#1882</a>
            </td>
            <td>
                <b>
                    chore: fix licenses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These files are auto-generated with ISC as
the default licese. Switched to Apache 2

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 16:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1880" class=".btn">#1880</a>
            </td>
            <td>
                <b>
                    docs(faq): Add instructions to install in Apple M1 processor (ARM-based)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Description of the installation process for Apple M1 processors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 12:57:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1879" class=".btn">#1879</a>
            </td>
            <td>
                <b>
                    feat(cactus-api-client): common verifier-factory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span>
            </td>
            <td>
                - Adjust SocketIOApiClient and common Verifier behavior to previous one in cmd-socketio, fix related tests.
- Extract Verifier interfaces to common location to ensure interface compatibility between old and new verifier / verifier factory (both should implement same interface).
- Create new package cactus-verifier-client for common verifier related stuff, to prevent circular dependencies.
- Add verifier-factory to create verifiers by supplying it's ID only, based on initial configuration. Configuration is set in ctor, but can be read from a file as in cmd-socketio scenarious. VerifierFactory config should be compatible with existing ledgerPluginInfo.

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 17:50:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1875" class=".btn">#1875</a>
            </td>
            <td>
                <b>
                    build(deps): bump url-parse from 1.5.3 to 1.5.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [url-parse](https://github.com/unshiftio/url-parse) from 1.5.3 to 1.5.10.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/unshiftio/url-parse/commit/8cd4c6c6435c1ea32243ec20c9cfe535251ec524"><code>8cd4c6c</code></a> 1.5.10</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ce7a01f2e10738b17812f57c7b6b5de4ea4c0298"><code>ce7a01f</code></a> [fix] Improve handling of empty port</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/00714900ea1e8ba0a1f87b9f8399001e47f060ec"><code>0071490</code></a> [doc] Update JSDoc comment</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/a7044e3e8bb2308ac0f74264d01951aeaca0d66f"><code>a7044e3</code></a> [minor] Use more descriptive variable name</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/d547792414a414b2f341a805141beafee728addf"><code>d547792</code></a> [security] Add credits for CVE-2022-0691</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ad23357ad5fd9a6b011d049466e9ecff723e52b8"><code>ad23357</code></a> 1.5.9</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/0e3fb542d60ddbf6933f22eb9b1e06e25eaa5b63"><code>0e3fb54</code></a> [fix] Strip all control characters from the beginning of the URL</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/61864a8eccff714a45d23db85a814e3c6ee0baba"><code>61864a8</code></a> [security] Add credits for CVE-2022-0686</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/bb0104d6439cf7c2662afbd9411e0772a9639664"><code>bb0104d</code></a> 1.5.8</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/d5c64791ef496ca5459ae7f2176a31ea53b127e5"><code>d5c6479</code></a> [fix] Handle the case where the port is specified but empty</li>
<li>Additional commits viewable in <a href="https://github.com/unshiftio/url-parse/compare/1.5.3...1.5.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url-parse&package-manager=npm_and_yarn&previous-version=1.5.3&new-version=1.5.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 16:35:23 +0000 UTC
    </div>
</div>

