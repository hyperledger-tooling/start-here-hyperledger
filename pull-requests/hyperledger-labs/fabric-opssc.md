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
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump ws from 7.5.4 to 7.5.10 in /opssc-agent/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ws](https://github.com/websockets/ws) from 7.5.4 to 7.5.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>7.5.10</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 7.x release line (22c28763).</li>
</ul>
<h2>7.5.9</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported bc8bd34e to the 7.x release line (0435e6e1).</li>
</ul>
<h2>7.5.8</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported 0fdcc0af to the 7.x release line (2758ed35).</li>
<li>Backported d68ba9e1 to the 7.x release line (dc1781bc).</li>
</ul>
<h2>7.5.7</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported 6946f5fe to the 7.x release line (1f72e2e1).</li>
</ul>
<h2>7.5.6</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported b8186dd1 to the 7.x release line (73dec34b).</li>
<li>Backported ed2b8039 to the 7.x release line (22a26afb).</li>
</ul>
<h2>7.5.5</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported ec9377ca to the 7.x release line (0e274acd).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d962d70649e393841ee1ed726a8f7ffbe90d0c06"><code>d962d70</code></a> [dist] 7.5.10</li>
<li><a href="https://github.com/websockets/ws/commit/22c28763234aa75a7e1b76f5c01c181260d7917f"><code>22c2876</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li><a href="https://github.com/websockets/ws/commit/8a78f8770618cc5a1ade485a7445cb6d6f46e2f2"><code>8a78f87</code></a> [dist] 7.5.9</li>
<li><a href="https://github.com/websockets/ws/commit/0435e6e12b8d38992cf0651cb8605dde2294bd25"><code>0435e6e</code></a> [security] Fix same host check for ws+unix: redirects</li>
<li><a href="https://github.com/websockets/ws/commit/4271f07cfc95cf7e1936388fb69e22a3731fa260"><code>4271f07</code></a> [dist] 7.5.8</li>
<li><a href="https://github.com/websockets/ws/commit/dc1781bc319cb347878d11cf730947d0bef69a51"><code>dc1781b</code></a> [security] Drop sensitive headers when following insecure redirects</li>
<li><a href="https://github.com/websockets/ws/commit/2758ed355073105a60b8b836b25265b8cdcb3b42"><code>2758ed3</code></a> [fix] Abort the handshake if the Upgrade header is invalid</li>
<li><a href="https://github.com/websockets/ws/commit/a370613fab74b82990582fa7728e130c5e87ee4c"><code>a370613</code></a> [dist] 7.5.7</li>
<li><a href="https://github.com/websockets/ws/commit/1f72e2e14f4fbb20265c228a43bb64ab915d8046"><code>1f72e2e</code></a> [security] Drop sensitive headers when following redirects (<a href="https://redirect.github.com/websockets/ws/issues/2013">#2013</a>)</li>
<li><a href="https://github.com/websockets/ws/commit/8ecd890800dfbe210298438ab9bb8dbe328f3e0b"><code>8ecd890</code></a> [dist] 7.5.6</li>
<li>Additional commits viewable in <a href="https://github.com/websockets/ws/compare/7.5.4...7.5.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ws&package-manager=npm_and_yarn&previous-version=7.5.4&new-version=7.5.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 02:28:24 +0000 UTC
    </div>
</div>

