---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3082" class=".btn">#3082</a>
            </td>
            <td>
                <b>
                    chore(deps): bump github.com/tidwall/gjson from 1.6.7 to 1.12.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/tidwall/gjson](https://github.com/tidwall/gjson) from 1.6.7 to 1.12.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tidwall/gjson/commit/db0033701cccc8e2e43b77d03e4f509a48b6b2f2"><code>db00337</code></a> Set array index as key for ForEach</li>
<li><a href="https://github.com/tidwall/gjson/commit/bd7621203094fc92fdbc342eb37610d27468269f"><code>bd76212</code></a> Add syntax badge</li>
<li><a href="https://github.com/tidwall/gjson/commit/9eae1fa87b82d1ecee31a4be512ce589409c1120"><code>9eae1fa</code></a> Added JSON Literals</li>
<li><a href="https://github.com/tidwall/gjson/commit/d3a134957c5d50327f8aaa4b101e164da140de9c"><code>d3a1349</code></a> Fix modifier bug in multipath selector</li>
<li><a href="https://github.com/tidwall/gjson/commit/6b6af2ad5e5c06e6cc3968ca7a2c0f9c20da8924"><code>6b6af2a</code></a> Added new static value character</li>
<li><a href="https://github.com/tidwall/gjson/commit/2c9fd2476ab6648576dc53a77d8f629e1a697689"><code>2c9fd24</code></a> Added Path and Paths for getting the original path of a Result</li>
<li><a href="https://github.com/tidwall/gjson/commit/7cadbb575617824cfa39a8a7e1cf0b059a7c6f67"><code>7cadbb5</code></a> Ensure Parse handles NaN/Inf and returns correct Index</li>
<li><a href="https://github.com/tidwall/gjson/commit/0b52f9a3618fb33e3cde84f9db7b73e324dff643"><code>0b52f9a</code></a> Fix empty string operator not matching</li>
<li><a href="https://github.com/tidwall/gjson/commit/8ac7a764ca2d496c4c78bf9465433b2334e968ad"><code>8ac7a76</code></a> Update README.md</li>
<li><a href="https://github.com/tidwall/gjson/commit/5784e4879e8c7411bb2d6fc841166e1de837ed9a"><code>5784e48</code></a> cleanup test</li>
<li>Additional commits viewable in <a href="https://github.com/tidwall/gjson/compare/v1.6.7...v1.12.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/tidwall/gjson&package-manager=go_modules&previous-version=1.6.7&new-version=1.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 09:42:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3080" class=".btn">#3080</a>
            </td>
            <td>
                <b>
                    fix: don't set recipientKeys and routingKeys if empty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 16:37:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3079" class=".btn">#3079</a>
            </td>
            <td>
                <b>
                    refactor: change webkms to fit refactored kms service, add bdd tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Change format of remote kms api calls to correspond to changes in kms service api

**Description:**
Make changes to webkms and remote crytro to work with new version of kms service.
Add bdd tests for webkms and remote crypto.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 14:52:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3077" class=".btn">#3077</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 2.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 2.5.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Adding Node.js version file support</h2>
<p>In scope of this release we add the <code>node-version-file</code> input and update <code>actions/cache</code> dependency to the latest version.</p>
<h2>Adding Node.js version file support</h2>
<p>The new input (<code>node-version-file</code>) provides functionality to specify the path to the file containing Node.js's version with such behaviour:</p>
<ul>
<li>If the file does not exist the action will throw an error.</li>
<li>If you specify both <code>node-version</code> and <code>node-version-file</code> inputs, the action will use value from the <code>node-version</code> input and throw the following warning: <code>Both node-version and node-version-file inputs are specified, only node-version will be used</code>.</li>
<li>For now the action does not support all of the variety of values for Node.js version files. The action can handle values according to the <a href="https://github.com/actions/setup-node#supported-version-syntax">documentation</a> and values with <code>v</code> prefix (<code>v14</code>)</li>
</ul>
<pre lang="yaml"><code>steps:
  - uses: actions/checkout@v2
  - name: Setup node from node version file
    uses: actions/setup-node@v2
    with:
      node-version-file: '.nvmrc'
  - run: npm install
  - run: npm test
</code></pre>
<h2>Update actions/cache dependency to 1.0.8 version.</h2>
<p>We updated actions/cache dependency to the latest version (1.0.8). For more information please refer to the <a href="https://github.com/actions/toolkit/blob/main/packages/cache/RELEASES.md">toolkit/cache</a>.</p>
<h2>Add &quot;cache-hit&quot; output</h2>
<p>This release introduces a new output: <code>cache-hit</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a>).</p>
<p>The <code>cache-hit</code> output contains boolean value indicating that an exact match was found for the key. It shows that the action uses already existing cache or not. The output is available only if cache is enabled.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/04c56d2f954f1e4c69436aa54cfef261a018f458"><code>04c56d2</code></a> update cache to 1.0.8 (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/367">#367</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/d08cf222111d5c1d21b3cd4b958937f818d10d9a"><code>d08cf22</code></a> Adding Node.js version file support (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/338">#338</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/360ab8b75b056fc18d368ee27a78d34e29c0b2d9"><code>360ab8b</code></a> Fix typo in the <code>bug_report</code> template (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/353">#353</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/fd4bd829f2dd6b6c1420bd94a93449c54612ffc2"><code>fd4bd82</code></a> Add issue and pull request templates (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/344">#344</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/a4b8ed2f4e9dd97eeae325f6967ce23d5478bd53"><code>a4b8ed2</code></a> Update dependencies (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/346">#346</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/270253e841af726300e85d718a5f606959b2903c"><code>270253e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a> from WtfJoke/addCacheHitOutPut</li>
<li><a href="https://github.com/actions/setup-node/commit/d1178716dbbe024f9d459612c22072517a781faa"><code>d117871</code></a> Add 'cache-hit' as output</li>
<li><a href="https://github.com/actions/setup-node/commit/041bafb67276a76a9cc88cd8a4e99165e9eb287d"><code>041bafb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/322">#322</a> from brcrista/brcrista/check-dist</li>
<li><a href="https://github.com/actions/setup-node/commit/996306e892eb8e97c8cfe8226ee043ae86a8f377"><code>996306e</code></a> rm <strong>tests</strong>/verify-no-unstaged-changes.sh</li>
<li><a href="https://github.com/actions/setup-node/commit/85d412253086d787de7add5f46dcf5964224c032"><code>85d4122</code></a> Fix triggers in licensed.yml</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v2.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=2.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 08:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3076" class=".btn">#3076</a>
            </td>
            <td>
                <b>
                    feat: Credential Fulfillment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added a library that allows you to parse Credential Fulfillment objects and resolve VCs from them based on an Issue Credential Message's attachment. This Credential Fulfillment implementation is based on the specification at https://identity.foundation/credential-manifest/#credential-fulfillment.

- Refactored the CredentialManifest.ResolveOutputDescriptors method to take in a *verifiable.Credential object instead of a []byte, in order to make the expected type more explicit.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 03:19:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3075" class=".btn">#3075</a>
            </td>
            <td>
                <b>
                    feat: command controllers for wallet issuance flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added JS, REST command controllers for wallet issuance interfaces.
- Part of  #3073

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 21:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3074" class=".btn">#3074</a>
            </td>
            <td>
                <b>
                    feat: WACI issuance flow interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                based on [WACI Issuance in Universal
Wallet](https://github.com/w3c-ccg/universal-wallet-interop-spec/issues/101)

- added propose credential interface
- added request credential interface
- added tests
- Closes #3073

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 16:24:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3072" class=".btn">#3072</a>
            </td>
            <td>
                <b>
                    feat: connectionRecord in OOBV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change includes ConnectionRecord creation in OOBV2 and requires invitation attachment messages to include `from`
header representing the sender's DID.


Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 15:24:48 +0000 UTC
    </div>
</div>

