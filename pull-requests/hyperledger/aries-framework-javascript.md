---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Fix: did sov service type resolving
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes behavior with the service resolution & types behavior with did:sov resolution. This additionally renames the `IndyDidResolver` to `SovDidResolver` to reduce confusion and prevent collision with the did:indy method in the future. Happy for any feedback/thoughts here.


@TimoGlastra if you could take a look at this one to ensure I didn't miss something here that'd be appreciated! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 00:20:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    feat: extension module creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Export some convenience types and classes to facilitate extension/plug-in development and add a fully-working dummy extension module in samples directory.

I'm not sure if it's the right place to put all this stuff, but I believe it could help developers to add custom protocols and wallet storage to their controllers, so it's worth for it to be somewhere :-).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:38:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    refactor: remove verkeys and did docs from connection record
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
        Created At 2022-03-29 19:52:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    fix: allow to set tags in MediationRecord constructor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow to optionally set tags for MediationRecord in class constructor (as it is in other records such as ConnectionRecord, ProofRecord, etc.). This is not currently used in regular flows but could be useful when mocking framework records.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 16:07:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    feat: bbs createKey, sign and verify
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **MARKED AS DRAFT** because the `react-native-bbs-signatures` is not yet released and merging this will break the React Native environment if bbs-signatures are being used.

Almost every change in this PR will be reverted when support for `aries-askar` is added, as we can then do all the functionality inside the wallet instead of the AFJ level. 

- Adds bls12381g1 and bls12381g2 to `indyWallet.createKey`
- Adds bls12381g2 to `indyWallet.sign`
- Adds bls12381g2 to `indyWallet.verify`
- Store and retrieve the keyPair in the wallet via the public key
- Added tests for the indy wallet
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 09:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    build(deps): bump plist from 3.0.4 to 3.0.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [plist](https://github.com/TooTallNate/node-plist) from 3.0.4 to 3.0.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/TooTallNate/plist.js/blob/master/History.md">plist's changelog</a>.</em></p>
<blockquote>
<h1>3.0.5 / 2022-03-23</h1>
<ul>
<li><a href="https://github.com/TooTallNate/plist.js/commit/96e2303d059e6be0c9e0c4773226d14b4758de52">[<code>96e2303d05</code>]</a> Prototype Pollution using .parse() <a href="https://github-redirect.dependabot.com/TooTallNate/node-plist/issues/114">#114</a> (mario-canva)</li>
<li>update browserify from 16 to 17</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/TooTallNate/node-plist/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plist&package-manager=npm_and_yarn&previous-version=3.0.4&new-version=3.0.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-26 12:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    build(deps): bump minimist from 1.2.5 to 1.2.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:37:03 +0000 UTC
    </div>
</div>

