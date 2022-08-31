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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/821" class=".btn">#821</a>
            </td>
            <td>
                <b>
                    fix missing condition on revoc check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/821"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 14:43:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/819" class=".btn">#819</a>
            </td>
            <td>
                <b>
                    use websockets for events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - switched from webhook to websocket for event handling
- removed webhook handlers and settings
- added netty native libraries
- added default values to some rest calls
- merge revocation status when loading matching credentials only if revocable and not revoked

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/819"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 15:34:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    Bump smartsquaregmbh/delete-old-packages from 0.4.0 to 0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [smartsquaregmbh/delete-old-packages](https://github.com/smartsquaregmbh/delete-old-packages) from 0.4.0 to 0.5.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/smartsquaregmbh/delete-old-packages/releases">smartsquaregmbh/delete-old-packages's releases</a>.</em></p>
<blockquote>
<h2>v0.5.0</h2>
<h4>:warning: This release includes breaking changes!</h4>
<ul>
<li><em>Breaking</em>: Removed <code>version</code> option.
<ul>
<li>To keep this package simple, this option has been removed. Very similar results can be achieved with <code>semver-pattern</code>.</li>
</ul>
</li>
<li><em>Potentially breaking</em>: Rewrite in TypeScript.</li>
<li>Support for ghcr.io packages. See the new section in the <a href="https://github.com/SmartsquareGmbH/delete-old-packages#ghcrio-packages">README</a>.</li>
<li>Improved error handling and logging.</li>
<li>New <code>type</code> option.</li>
</ul>
<blockquote>
<p>Since this release includes major changes and has not been tested as much as previous versions, it is marked as a pre-release. Please try it with the <code>dry-run</code> option and report bugs or missing features!</p>
</blockquote>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/53e0b59f56449a9fdbcec8dcc6d1b038b8a29992"><code>53e0b59</code></a> Bump version to 0.5.0</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/27998e516f375efe57cce37d8b9c4ce10495a790"><code>27998e5</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/237c4313ac8418bccec9cfb095312f56908d2ceb"><code>237c431</code></a> Update README</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/678055d997ba78aeb17fdfac019b7e14ad533fe2"><code>678055d</code></a> Update dependencies</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/2dd5dd734ccd2d1f4d038921270aaaaaf3cfdfe8"><code>2dd5dd7</code></a> Refactor a bit</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/a9319e534a8a97c5fe0053c63ba24209882998f0"><code>a9319e5</code></a> Validate user and organization input combination</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/1d029e77275be61a9e2d517e3e2f5248410a4169"><code>1d029e7</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/b04aafe88d0f3f9d3f2eece3ab4f9043d143d305"><code>b04aafe</code></a> Add cause to query package errors</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/de048edb051d2fd9daa6d47098ebe025d5b731e8"><code>de048ed</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/becea094ebba3952d40d01ffffb194ce205def1f"><code>becea09</code></a> Improve error handling</li>
<li>Additional commits viewable in <a href="https://github.com/smartsquaregmbh/delete-old-packages/compare/v0.4.0...v0.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smartsquaregmbh/delete-old-packages&package-manager=github_actions&previous-version=0.4.0&new-version=0.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/818"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 13:46:53 +0000 UTC
    </div>
</div>

