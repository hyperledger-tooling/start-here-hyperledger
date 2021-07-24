---
layout: default
title: indy-sdk-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk-react-native
---

# indy-sdk-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk-react-native/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    chore: update rn-indy-sdk references
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 22:21:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk-react-native/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Bump react-native from 0.59.10 to 0.62.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [react-native](https://github.com/facebook/react-native) from 0.59.10 to 0.62.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/releases">react-native's releases</a>.</em></p>
<blockquote>
<h2>v0.62.3</h2>
<p>This patch release is specifically targetted towards Xcode 12.5. The changes done are tailored to unblock developers still relying on v0.62 of RN.</p>
<p>Aside from bumping your version from 0.62.2 to 0.62.3, please make sure to add this line to your podfile (or modify it if you already had it):</p>
<pre><code>use_flipper!('Flipper' =&gt; '0.75.1', 'Flipper-Folly' =&gt; '2.5.3', 'Flipper-RSocket' =&gt; '1.3.1')
</code></pre>
<p>After which, do all the classic necessary cleans (node_modules, caches, pod folders, etc)(<a href="https://github.com/pmadruga/react-native-clean-project">react-native-clean-project</a> is your ally) then do <code>yarn install</code> and a <code>pod install --repo-update</code> (if pod install fails on an error about a Flipper package, just remove the relevant lines from the podfile.lock and run the pod install again).</p>
<p>The only other commit picked &amp; released along the Xcode 12.5 fixes is:</p>
<ul>
<li>Update validateBaseUrl to use latest regex (<a href="https://github.com/facebook/react-native/commit/ca09ae82715e33c9ac77b3fa55495cf84ba891c7">commit</a>) which fixes CVE-2020-1920, GHSL-2020-293.</li>
</ul>
<hr />
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/">upgrade helper</a> ⚛️</p>
<hr />
<p>You can find the whole <a href="https://github.com/react-native-community/react-native-releases/blob/master/CHANGELOG.md">changelog history</a> over at <code>react-native-releases</code>.</p>
<h2>v0.62.2</h2>
<p>This release fixes a few minor issues that were reported by the community. You can view the complete changelog <a href="https://github.com/react-native-community/releases/blob/master/CHANGELOG.md#v0622">here</a>.</p>
<p>You can participate in the conversation for the next patch release in the dedicated <a href="https://github-redirect.dependabot.com/react-native-community/releases/issues/188">issue</a>.</p>
<hr />
<p>To help you upgrade to this version, you can use the new <a href="https://react-native-community.github.io/upgrade-helper/">upgrade helper</a> ⚛️</p>
<hr />
<p>You can find the whole <a href="https://github.com/react-native-community/react-native-releases/blob/master/CHANGELOG.md">changelog history</a> over at <code>react-native-releases</code>.</p>
<h2>v0.62.1</h2>
<p>This release fixes a YellowBox regression in v0.62.0 where the Flipper network inspector causes YellowBox to crash the app due to using base64 images.</p>
<p>You can view the complete changelog <a href="https://github.com/react-native-community/releases/blob/master/CHANGELOG.md#v0621">here</a>.</p>
<p>You can participate in the conversation for the next patch release in the dedicated <a href="https://github-redirect.dependabot.com/react-native-community/releases/issues/184">issue</a>.</p>
<hr />
<p>To help you upgrade to this version, you can use the new <a href="https://react-native-community.github.io/upgrade-helper/">upgrade helper</a> ⚛️</p>
<hr />
<p>You can find the whole <a href="https://github.com/react-native-community/react-native-releases/blob/master/CHANGELOG.md">changelog history</a> over at <code>react-native-releases</code>.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react-native/commit/83425fa72f1f9a12f6b6deefd66fa8bd154a3651"><code>83425fa</code></a> [0.62.3] Bump version numbers</li>
<li><a href="https://github.com/facebook/react-native/commit/c6f4611dcbfbb64d5b54e242570e2a1acffcabef"><code>c6f4611</code></a> [local] change autolink to match requirements for FlipperFolly working with X...</li>
<li><a href="https://github.com/facebook/react-native/commit/c4ea556d64c7fc146d1412548788c48bbcc0f6bb"><code>c4ea556</code></a> [local] change podfile to rely on the autolink-ios rb file</li>
<li><a href="https://github.com/facebook/react-native/commit/ca09ae82715e33c9ac77b3fa55495cf84ba891c7"><code>ca09ae8</code></a> Update validateBaseUrl to use latest regex</li>
<li><a href="https://github.com/facebook/react-native/commit/166a5ddf88aca0d0235e48c624681eec095e9ef8"><code>166a5dd</code></a> Get ReactiveNative compiled with Clang 10 (<a href="https://github-redirect.dependabot.com/facebook/react-native/issues/28362">#28362</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/158b558e500576f434dec09417bb02cc0bc53f7a"><code>158b558</code></a> [local] update detox to work on Xcode 12</li>
<li><a href="https://github.com/facebook/react-native/commit/b9944e54ae35c2beed0e78ea454d871e0fe92ec6"><code>b9944e5</code></a> [0.62.2] Bump version numbers</li>
<li><a href="https://github.com/facebook/react-native/commit/f89c5098bec5ba1a3b4bee54b51d639beff559f6"><code>f89c509</code></a> Make Vibration.vibrate compatible with TurboModules (<a href="https://github-redirect.dependabot.com/facebook/react-native/issues/27951">#27951</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/8858d879eb689a9a7efda83c5f7e45f154a2f935"><code>8858d87</code></a> Exclude all FlipperKit transitive dependencies from iOS Release builds (<a href="https://github-redirect.dependabot.com/facebook/react-native/issues/28504">#28504</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/4fd9c9d544d741fb2df3ad849dfa4bdf4719ccf4"><code>4fd9c9d</code></a> Fix Appearance module when using Chrome Debugger</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/react-native/compare/v0.59.10...v0.62.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-native&package-manager=npm_and_yarn&previous-version=0.59.10&new-version=0.62.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 23:01:29 +0000 UTC
    </div>
</div>

