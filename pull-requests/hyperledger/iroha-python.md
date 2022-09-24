---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Bump protobuf from 3.20.1 to 3.20.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobuf](https://github.com/protocolbuffers/protobuf) from 3.20.1 to 3.20.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf's releases</a>.</em></p>
<blockquote>
<h2>Protocol Buffers v3.20.2</h2>
<h1>C++</h1>
<ul>
<li>Reduce memory consumption of MessageSet parsing</li>
<li>This release addresses a <a href="https://github.com/protocolbuffers/protobuf/security/advisories/GHSA-8gq9-2x98-w8hf">Security Advisory for C++ and Python users</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/a20c65f2cd549445fda907f7b83894c8eb7427d6"><code>a20c65f</code></a> Updating changelog</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/c49fe79af9c295960477b7568f1765b202093143"><code>c49fe79</code></a> Updating version.json and repo version numbers to: 20.2</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/806d7e4ce6f1fd0545cae226b94cb0249ea495c7"><code>806d7e4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10544">#10544</a> from deannagarcia/3.20.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/ae718b39020ae6e6f8f5568e357d6893fd0fd29c"><code>ae718b3</code></a> Add missing includes</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/b4c395aaedfacb32e2414d361fa85968c0991b34"><code>b4c395a</code></a> Apply patch</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/6439c5c01349e74d4deb57c844a7ad4b7b13a302"><code>6439c5c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10531">#10531</a> from protocolbuffers/deannagarcia-patch-7</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/22c79e6e4ca8be2bc2f700b2cdddca84d84659ce"><code>22c79e6</code></a> Update version.json</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/c1a2d2ec29314975e725021ffe4334926dbaa56c"><code>c1a2d2e</code></a> Fix python release on macos (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10512">#10512</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/a826282e15efe3ae3a2aebb040fb1691b2233a1e"><code>a826282</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10505">#10505</a> from deannagarcia/3.20.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/7639a710e10beb47bfc62f363680f7b04e8b3d26"><code>7639a71</code></a> Add version file</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.20.1...v3.20.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobuf&package-manager=pip&previous-version=3.20.1&new-version=3.20.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 22:18:09 +0000 UTC
    </div>
</div>

