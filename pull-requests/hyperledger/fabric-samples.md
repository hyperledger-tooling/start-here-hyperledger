---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/822" class=".btn">#822</a>
            </td>
            <td>
                <b>
                    add js chaincode for the private data concept
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: abdou.chakhkhar <abdelmoula.chakhkhar@uit.ac.ma>

In this PR, I implemented the js chaincode for the private data concept, which s gonna allow the js developers to get familiarized so quickly with private data APIs in the nodejs SDK.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 14:59:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/821" class=".btn">#821</a>
            </td>
            <td>
                <b>
                    Bump moment-timezone from 0.5.33 to 0.5.37 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [moment-timezone](https://github.com/moment/moment-timezone) from 0.5.33 to 0.5.37.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment-timezone/releases">moment-timezone's releases</a>.</em></p>
<blockquote>
<h2>Release 0.5.34</h2>
<ul>
<li>Updated data to IANA TZDB <code>2021e</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment-timezone/blob/develop/changelog.md">moment-timezone's changelog</a>.</em></p>
<blockquote>
<h3><code>0.5.37</code> <em>2022.08-25</em></h3>
<ul>
<li>Re-publish npm package, because of extra folder present in 0.5.36, check
<a href="https://github-redirect.dependabot.com/moment/moment-timezone/issues/999">moment/moment-timezone#999</a></li>
</ul>
<h3><code>0.5.36</code> <em>2022.08-25</em></h3>
<ul>
<li>IANA TZDB 2022c</li>
<li>improvements/fixes to data pipeline</li>
</ul>
<h3><code>0.5.35</code> <em>2022-08-23</em></h3>
<ul>
<li>Fix command injection in data pipeline <a href="https://github.com/moment/moment-timezone/security/advisories/GHSA-56x4-j7p9-fcf9">https://github.com/moment/moment-timezone/security/advisories/GHSA-56x4-j7p9-fcf9</a></li>
<li>Fix cleartext transmission of sensitive information <a href="https://github.com/moment/moment-timezone/security/advisories/GHSA-v78c-4p63-2j6c">https://github.com/moment/moment-timezone/security/advisories/GHSA-v78c-4p63-2j6c</a></li>
</ul>
<p>Thanks to the OpenSSF Alpha-Omega project for reporting these!</p>
<h3><code>0.5.34</code> <em>2020-11-10</em></h3>
<ul>
<li>Updated data to IANA TZDB <code>2021e</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moment/moment-timezone/commit/ffe6f340a6bdae6be1cbc1cbef4a4f2b87e2c63c"><code>ffe6f34</code></a> Add changelog for 0.5.37</li>
<li><a href="https://github.com/moment/moment-timezone/commit/450ca6304ba62baf27817ed7840828eee4e3b0c5"><code>450ca63</code></a> Bump version to 0.5.37</li>
<li><a href="https://github.com/moment/moment-timezone/commit/95f1a9b5cd3a15b8c75bd36029152ff1b43a5136"><code>95f1a9b</code></a> Build moment-timezone 0.5.36</li>
<li><a href="https://github.com/moment/moment-timezone/commit/abba28c7b0e1faf7df8592806007fcb2753b3078"><code>abba28c</code></a> Add changelog for 0.5.36</li>
<li><a href="https://github.com/moment/moment-timezone/commit/ac6de03cf34610068185961613d719bc050c7d2b"><code>ac6de03</code></a> Bump version to 0.5.36</li>
<li><a href="https://github.com/moment/moment-timezone/commit/7a5cadf9cbece0a9c7b9da0ee244c21375eb33a6"><code>7a5cadf</code></a> tests: Fix country tests for 2022c</li>
<li><a href="https://github.com/moment/moment-timezone/commit/6754c75f5be4fbb16e90e336c9decbad6b506388"><code>6754c75</code></a> data: generate 2022c data+tests</li>
<li><a href="https://github.com/moment/moment-timezone/commit/f74a364b1aac2c96cedd0a8cf5c7188268b9bcde"><code>f74a364</code></a> bugfix: Wipe tests/zones before generation</li>
<li><a href="https://github.com/moment/moment-timezone/commit/e850f9fa6d3b440c51ae0cda7d9d573627839167"><code>e850f9f</code></a> grunt: do not bundle zone and contry tests</li>
<li><a href="https://github.com/moment/moment-timezone/commit/f13e22b069f9115eddad5294a4c0f5335c61590a"><code>f13e22b</code></a> data: automatically create data/*/VERSION.json for latest</li>
<li>Additional commits viewable in <a href="https://github.com/moment/moment-timezone/compare/0.5.33...0.5.37">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=moment-timezone&package-manager=npm_and_yarn&previous-version=0.5.33&new-version=0.5.37)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 04:50:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/820" class=".btn">#820</a>
            </td>
            <td>
                <b>
                    Update nano test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix minor bugs, and add network.sh script to simplify standing up the network

Note: the updated peerNadmin.sh scripts no longer create or join a channel and now only configure the environment for the relevant peer

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 13:57:03 +0000 UTC
    </div>
</div>

