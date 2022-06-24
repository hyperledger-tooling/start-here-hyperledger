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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    add ability to append ordering node to systemless
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
Added the ability to append ordering nodes to an existing cluster that are * not * using a system channel.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 18:41:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Bump got from 11.8.2 to 11.8.5 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) from 11.8.2 to 11.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v11.8.5</h2>
<ul>
<li>Backport security fix <a href="https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc">https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc</a>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2022-33987">CVE-2022-33987</a></li>
</ul>
</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5">https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5</a></p>
<h2>v11.8.3</h2>
<ul>
<li>Bump cacheable-request dependency (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1921">#1921</a>)  9463bb6</li>
<li>Fix <code>HTTPError</code> missing <code>.code</code> property (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1739">#1739</a>)  0e167b8</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v11.8.2...v11.8.3">https://github.com/sindresorhus/got/compare/v11.8.2...v11.8.3</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/5e17bb748c260b02e4cf716c2f4079a1c6a7481e"><code>5e17bb7</code></a> 11.8.5</li>
<li><a href="https://github.com/sindresorhus/got/commit/bce8ce7d528a675bd5a8d996e110b73674e290d2"><code>bce8ce7</code></a> Backport 861ccd9ac2237df762a9e2beed7edd88c60782dc</li>
<li><a href="https://github.com/sindresorhus/got/commit/8ced19215603f3eda25a9f5dce390f1b152fe9a3"><code>8ced192</code></a> Fix build</li>
<li><a href="https://github.com/sindresorhus/got/commit/670eb04b5b01622f489277d6fb1dd04a41d3cb51"><code>670eb04</code></a> 11.8.4</li>
<li><a href="https://github.com/sindresorhus/got/commit/20f29fe3726a4ddd104f557456dbd5275685e879"><code>20f29fe</code></a> Backport <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1543">#1543</a>: Initialize globalResponse in case of ignored HTTPError (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2017">#2017</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/0da732f4650c398f3b2fea672f8916e6c7004c8f"><code>0da732f</code></a> 11.8.3</li>
<li><a href="https://github.com/sindresorhus/got/commit/9463bb696d4ee909970e3fc609ee40b7644e3f6c"><code>9463bb6</code></a> Bump cacheable-request dependency (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1921">#1921</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/0e167b8b9505a7e9e4a4bbe39e9baeb1f5c4a1fd"><code>0e167b8</code></a> HTTPError code set to 'HTTPError' <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1711">#1711</a> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1739">#1739</a>)</li>
<li>See full diff in <a href="https://github.com/sindresorhus/got/compare/v11.8.2...v11.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=got&package-manager=npm_and_yarn&previous-version=11.8.2&new-version=11.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-23 08:31:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/233" class=".btn">#233</a>
            </td>
            <td>
                <b>
                    set default value for osnadmin_feats_enabled as true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
set default value for `osnadmin_feats_enabled` as `true`, was `false`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 13:37:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    channel participation apis - join orderer  via drill down
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature - adds new join osn to channel flows

#### Description
- Adds join orderer to channel via cluster drill down (this is a new modal)
   1. general join flow - from OS page -> can select join-channel button, then select existing OS to get config block, select channel name, select osn(s) to join
   2.  specific join flow - from OS page -> can select the channel, then select osn(s) to join

- changes create orderer flow - user must select if they want to use a system channel or not when creating a orderer 
   - (only applies if `osnadmin_feats_enabled` is enabled)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 20:52:56 +0000 UTC
    </div>
</div>

