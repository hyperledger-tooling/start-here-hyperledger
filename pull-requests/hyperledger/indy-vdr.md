---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Update Cargo.toml time package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I think this should fix the mac build errors, though I'm still not sure why it's only happening on mac
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 17:12:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    chore(deps): bump rust from 1.41-slim to 1.79-slim in /docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps rust from 1.41-slim to 1.79-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rust&package-manager=docker&previous-version=1.41-slim&new-version=1.79-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 11:55:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/302" class=".btn">#302</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump react-native from 0.67.2 to 0.74.2 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-native](https://github.com/facebook/react-native/tree/HEAD/packages/react-native) from 0.67.2 to 0.74.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/releases">react-native's releases</a>.</em></p>
<blockquote>
<h2>0.74.2</h2>
<h3>Changed</h3>
<ul>
<li>Updated <code>typescript-eslint</code> monorepo to <code>v7</code>
(<a href="https://github.com/facebook/react-native/commit/91d725136e8fe0fd55fdfca5a4f5bd8ab527f94e">91d725136e</a> by <a href="https://github.com/huntie"><code>@​huntie</code></a>)</li>
<li>Upgrade CLI to <code>13.6.8</code> (<a href="https://github.com/facebook/react-native/commit/335f6ed83306bfa150c818d26dce4b279de4869f">335f6ed833</a> by <a href="https://github.com/szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Warn only in <code>init</code> command when CLI uses cached <code>npx</code> version (<a href="https://github.com/facebook/react-native/commit/b98c5b960ccc4fe9d2792c35994c414c709a3d7a">b98c5b960c</a> by <a href="https://github.com/szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
<li><code>selection</code> prop in <code>TextInput</code> was not being applied at component creation (<a href="https://github.com/facebook/react-native/commit/be09d12667044f237f08af410b2838062eb8e657">be09d12667</a> by <a href="https://github.com/alanleedev"><code>@​alanleedev</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Fixed dangling <code>mAttachedSurfaces</code> after <code>ReactHost.destroy()</code> (<a href="https://github.com/facebook/react-native/commit/c70d7910361f56bc361ad825fe13fb2178edfeba">c70d791036</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
<li>ReactSoftExceptions in ReactHostImpl only when Context is null (<a href="https://github.com/facebook/react-native/commit/ac3261ff608768ff43736b413c5a5ad67668af61">ac3261ff60</a> by <a href="https://github.com/arushikesarwani94"><code>@​arushikesarwani94</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Privacy Manifest aggregation failing due to no <code>NSPrivacyAccessedAPITypes</code> key (<a href="https://github.com/facebook/react-native/commit/fc4e0999206ec7c1f465bb2b1fea987e43485a82">fc4e099920</a> by <a href="https://github.com/renchap"><code>@​renchap</code></a>)</li>
<li>In privacy manifest post install script, handle the case where the file reference doesn't have a path (<a href="https://github.com/facebook/react-native/commit/4ad65ac59a2491db598abb7b32fb793e9693d5ac">4ad65ac59a</a> by <a href="https://github.com/robertying"><code>@​robertying</code></a>)</li>
<li>Fixed an issue where the <code>selectionColor</code> prop was not being applied on the <code>TextInput</code> component. (<a href="https://github.com/facebook/react-native/commit/2bde626a9fa2f782864937a5258ac494afe27f9f">2bde626a9f</a> by <a href="https://github.com/robinshin"><code>@​robinshin</code></a>)</li>
</ul>
<hr />
<!-- raw HTML omitted -->
<p>Hermes dSYMS:</p>
<ul>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.2/react-native-artifacts-0.74.2-hermes-framework-dSYM-debug.tar.gz">Debug</a></li>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.2/react-native-artifacts-0.74.2-hermes-framework-dSYM-release.tar.gz">Release</a></li>
</ul>
<hr />
<p>You can file issues or pick requests against this release <a href="https://github.com/reactwg/react-native-releases/issues/new/choose">here</a>.</p>
<hr />
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/">Upgrade Helper</a> ⚛️.</p>
<hr />
<p>View the whole changelog in the <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG.md">CHANGELOG.md file</a>.</p>
<h2>0.74.1</h2>
<h3>Added</h3>
<h4>iOS Specific</h4>
<ul>
<li>Implement privacy manifest aggregation  (<a href="https://github.com/facebook/react-native/commit/4be1fafec8edca5da5ebe515ad359d4178db7d23">4be1fafec8</a> by <a href="https://github.com/@aleqsio"><code>@​aleqsio</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG-pre-070.md">react-native's changelog</a>.</em></p>
<blockquote>
<h1>Changelog (pre 0.70)</h1>
<p>This file contains all changelogs for releases in the 0.60-0.69 range. Please check out the other <code>CHANGELOG-*.md</code> files for newer and older versions.</p>
<h2>v0.69.12</h2>
<h3>Changed</h3>
<ul>
<li>[0.69] Bump CLI to ^8.0.7, Metro to 0.70.4 (<a href="https://github.com/facebook/react-native/commit/56807fadfacf3c5cc62a8d1948b3d72ca51a5e6b">56807fadfa</a> by <a href="https://github.com/robhogan"><code>@​robhogan</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>[0.69] Use <code>Content-Location</code> header in bundle response as JS source URL (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/37501">#37501</a>) (<a href="https://github.com/facebook/react-native/commit/367fc7ad5254c5dd2c8ef38248766173525cc77c">367fc7ad52</a> by <a href="https://github.com/robhogan"><code>@​robhogan</code></a>)</li>
</ul>
<h3>Fixed</h3>
<h4>Android specific</h4>
<ul>
<li>Prevent crash in runAnimationStep on OnePlus and Oppo devices (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/37487">#37487</a>) (<a href="https://github.com/facebook/react-native/commit/4db7a10e257c664aced8cd8a1737d7ed9ced14fe">4db7a10e25</a> by <a href="https://github.com/hsource"><code>@​hsource</code></a>)</li>
</ul>
<h2>v0.69.11</h2>
<h3>Fixed</h3>
<h4>iOS specific</h4>
<ul>
<li>Make 0.69 compatible with Xcode 15 (thanks to <a href="https://github.com/AlexanderEggers"><code>@​AlexanderEggers</code></a> for the commit in main) (<a href="https://github.com/facebook/react-native/commit/37e8df1cdce4a66763c720b1b0768d049def9518">37e8df1cdc</a>)</li>
</ul>
<h2>v0.69.10</h2>
<h3>Fixed</h3>
<h4>Android specific</h4>
<ul>
<li>Minimize EditText Spans 8/N: CustomStyleSpan (<a href="https://github.com/facebook/react-native/commit/b384bb613bf533aebf3271ba335c61946fcd3303">b384bb613b</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize EditText Spans 6/N: letterSpacing (<a href="https://github.com/facebook/react-native/commit/5791cf1f7b43aed1d98cad7bcc272d97ab659111">5791cf1f7b</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 5/N: Strikethrough and Underline (<a href="https://github.com/facebook/react-native/commit/0869ea29db6a4ca20b9043d592a2233ae1a0e7a2">0869ea29db</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 4/N: ReactForegroundColorSpan (<a href="https://github.com/facebook/react-native/commit/8c9c8ba5adb59f7f891a5307a0bce7200dd3ac7d">8c9c8ba5ad</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 3/N: ReactBackgroundColorSpan (<a href="https://github.com/facebook/react-native/commit/cc0ba57ea42d876155b2fd7d9ee78604ff8aa57a">cc0ba57ea4</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 1/N: Fix precedence (<a href="https://github.com/facebook/react-native/commit/1743dd7ab40998c4d3491e3b2c56c531daf5dc47">1743dd7ab4</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Fix measurement of uncontrolled TextInput after edit (<a href="https://github.com/facebook/react-native/commit/8a0fe30591e21b90a3481c1ef3eeadd4b592f3ed">8a0fe30591</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
</ul>
<h2>v0.69.9</h2>
<h3>Changed</h3>
<h4>iOS specific</h4>
<ul>
<li>Relax Ruby requirements (<a href="https://github.com/facebook/react-native/commit/4e015c69d646b320d58888f70af566c1d753eaed">4e015c69d6</a> by <a href="https://github.com/cipolleschi"><code>@​cipolleschi</code></a>)</li>
</ul>
<h3>Fixed</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react-native/commit/17c0b1766f7e3c1c3a59f7701704f0ea6a6f6bc3"><code>17c0b17</code></a> Release 0.74.2</li>
<li><a href="https://github.com/facebook/react-native/commit/053f1d9822831187149bb57effc677dad99d723c"><code>053f1d9</code></a> Fix dangling surfaces in ReactHostImpl (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44393">#44393</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/0f44ca644bcf7c124226b42ad484d1e6643c4270"><code>0f44ca6</code></a> chore: Increase iOS script portability (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44417">#44417</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/2e21543017006ee6418c6953d976593d07407755"><code>2e21543</code></a> [LOCAL] Fix prettier</li>
<li><a href="https://github.com/facebook/react-native/commit/58f232c6c20475309a7cd789863e88a6888bd8f2"><code>58f232c</code></a> [LOCAL] Bump hermes version</li>
<li><a href="https://github.com/facebook/react-native/commit/1e3d2161e85906e781b2272a9ffefb3dfcf09191"><code>1e3d216</code></a> Merge branch '0.74-stable' of <a href="https://github.com/facebook/react-native">https://github.com/facebook/react-native</a> into 0...</li>
<li><a href="https://github.com/facebook/react-native/commit/335f6ed83306bfa150c818d26dce4b279de4869f"><code>335f6ed</code></a> feat: upgrade CLI to <code>13.6.8</code> (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44757">#44757</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/752c173da529b48ead482be5088af6758f08ee65"><code>752c173</code></a> Fix Privacy Manifest generator when it does not contain a `NSPrivacyAccessedA...</li>
<li><a href="https://github.com/facebook/react-native/commit/1860441d848b8f620e0b959e43122628b1cd04c9"><code>1860441</code></a> fix: warn only in <code>init</code> command when CLI uses cached <code>npx</code> version (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44644">#44644</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/a88a3c5bbfbb2d7ea1e9af6f8bea11542bf88cf1"><code>a88a3c5</code></a> iOS: Fixes textinput onscroll event payload (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/43445">#43445</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/react-native/commits/v0.74.2/packages/react-native">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~react-native-bot">react-native-bot</a>, a new releaser for react-native since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-native&package-manager=npm_and_yarn&previous-version=0.67.2&new-version=0.74.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 11:25:27 +0000 UTC
    </div>
</div>

