---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    Fix returned credential exchange id 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">load-test</span>
            </td>
            <td>
                The response of issuing(send) a credential to a holder is the credential exchange id, but the returned id is not the UUID which is needed to refer to the appropriate credential exchange.

Usage:
- this is needed to automate revocation in the load test scenario (jmeter)

Signed-off-by: Driton Goxhufi <driton.goxhufi@bosch.io>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/847"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 12:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    Bump smartsquaregmbh/delete-old-packages from 0.5.0 to 0.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [smartsquaregmbh/delete-old-packages](https://github.com/smartsquaregmbh/delete-old-packages) from 0.5.0 to 0.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/smartsquaregmbh/delete-old-packages/releases">smartsquaregmbh/delete-old-packages's releases</a>.</em></p>
<blockquote>
<h2>v0.6.0</h2>
<ul>
<li>Support for npm.pkg.github.com packages. See the update README.</li>
<li>Dependency updates.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/cad3790a6a1fa9d0c7910d5a5db5c4f3a6ca2ff8"><code>cad3790</code></a> Update actions</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/3bd0acdf1ae784b91fbc752e41f18d7d450038d4"><code>3bd0acd</code></a> Use built in yarn caching in GH actions</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/2ebcd963e1a35e1e5d0a54aaaa2ced902ac6e08b"><code>2ebcd96</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/c1af69cfc67dc3795a5061e3c2682c805e1a2c7f"><code>c1af69c</code></a> Bump to 0.6.0 and update README</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/94bd58f8c62e2f3d40ea131569c6e10ee2e1e320"><code>94bd58f</code></a> Update dependencies and properly setup linting</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/dde18cd9ad8058380b87fc0abef8c8bb3907127e"><code>dde18cd</code></a> Refactor and add support for npm.pkg.github.com packages.</li>
<li>See full diff in <a href="https://github.com/smartsquaregmbh/delete-old-packages/compare/v0.5.0...v0.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smartsquaregmbh/delete-old-packages&package-manager=github_actions&previous-version=0.5.0&new-version=0.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/846"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 13:08:39 +0000 UTC
    </div>
</div>

