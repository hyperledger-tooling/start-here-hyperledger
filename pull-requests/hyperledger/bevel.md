---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1968" class=".btn">#1968</a>
            </td>
            <td>
                <b>
                    Define what DLT is before the initialism is used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**

Just defined what the  Distributed Ledger Transaction means before the initialism is used. Makes reading the docs easier for nubes like me :)

 
**Reviewed by**
@jagpreetsinghsasan 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 23:26:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1967" class=".btn">#1967</a>
            </td>
            <td>
                <b>
                    Bump eventsource from 1.1.0 to 1.1.1 in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [eventsource](https://github.com/EventSource/eventsource) from 1.1.0 to 1.1.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/EventSource/eventsource/blob/master/HISTORY.md">eventsource's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">1.1.1</a></h1>
<ul>
<li>Do not include authorization and cookie headers on redirect to different origin (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/273">#273</a> Espen Hovlandsdal)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/EventSource/eventsource/commit/aa7a40843a978f42c0babdec125bf9e0a83bf515"><code>aa7a408</code></a> 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/56d489ef853a891deca121bbd463c732fee94dce"><code>56d489e</code></a> chore: rebuild polyfill</li>
<li><a href="https://github.com/EventSource/eventsource/commit/4a951e58b04118c9c4d3da3d27d454972a1b4b8d"><code>4a951e5</code></a> docs: update history for 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/f9f6416567bff62c1af2f4314be51d9870e94bc2"><code>f9f6416</code></a> fix: strip sensitive headers on redirect to different origin</li>
<li>See full diff in <a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=eventsource&package-manager=npm_and_yarn&previous-version=1.1.0&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 22:34:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1966" class=".btn">#1966</a>
            </td>
            <td>
                <b>
                    [fabric] Update sample configuration files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Update sample configuration files: network-fabric-add-new-channel.yaml, network-fabric-add-ordererorg.yaml, network-fabric-add-organization.yaml, network-fabric-remove-organization.yaml, network-fabricv-add-peer.yaml, network-fabricv2-raft-add-orderer.yaml and platforms/hyperledger-fabric/configuration/add-orderer-organization.yaml playbook

 

**Reviewed by**
@suvajit-sarkar
@jagpreetsinghsasan

 

**Linked issue**
#1950 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 06:24:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1965" class=".btn">#1965</a>
            </td>
            <td>
                <b>
                    [quorum] update quorum helm value templates for flux v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manikanta-darsi <manikanta.darsi@accenture.com>

**Changelog**
- Update  quorum helm value templates for flux v2.

 

**Reviewed by**
@sownak @suvajit-sarkar 

 

**Linked issue**
#1928 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 05:56:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1964" class=".btn">#1964</a>
            </td>
            <td>
                <b>
                    [chore] update molecule fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

- Fix added quorum and fabric missing variables in molecule test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 05:55:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1963" class=".btn">#1963</a>
            </td>
            <td>
                <b>
                    [fabric][quorum] molecule fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Fix missing variable in converge.yaml

 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 19:23:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1962" class=".btn">#1962</a>
            </td>
            <td>
                <b>
                    [chore] merge develop on feature/flux-v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 13:03:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1961" class=".btn">#1961</a>
            </td>
            <td>
                <b>
                    [indy] update image pull policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

- Update image pull policy to IfNotPresent


 

**Linked issue**
#1885 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 12:47:35 +0000 UTC
    </div>
</div>

