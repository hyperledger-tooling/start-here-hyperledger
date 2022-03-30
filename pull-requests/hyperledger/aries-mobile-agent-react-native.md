---
layout: default
title: aries-mobile-agent-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-react-native
---

# aries-mobile-agent-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 15:23:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    Update pull request template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Updated the pull request template:

- I removed the box for running the linter. Its an automated task and I just noted that the PR won't be reviewed until all automated tests / tasks run successfully.
- I added a check box to indicate that sufficient tests have been added so that code coverage is not reduced.

# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 20:43:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade react-native-screens from 3.7.2 to 3.13.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <h3>Snyk has created this PR to upgrade react-native-screens from 3.7.2 to 3.13.1.</h3>

![merge advice](https://app.snyk.io/badges/merge-advice/?package_manager=npm&package_name=react-native-screens&from_version=3.7.2&to_version=3.13.1&pr_id=abbfa8d2-e668-47eb-a8de-ea0f26e0f2a6&visibility=true&has_feature_flag=false)
:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **10 versions** ahead of your current version.
- The recommended version was released **24 days ago**, on 2022-03-03.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>react-native-screens</b></summary>
    <ul>
      <li>
        <b>3.13.1</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.13.1">2022-03-03</a></br><p>Patch release adding <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1157061456" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1351" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1351/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1351">#1351</a> that suppresses <code>Function components cannot be given refs. Attempts to access this ref will fail</code> warning on Fabric architecture.</p>
      </li>
      <li>
        <b>3.13.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.13.0">2022-02-28</a></br><p>Minor release fixing bugs, improving typings, and adding some functionalities <g-emoji class="g-emoji" alias="tada" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f389.png">🎉</g-emoji></p>
<h2><g-emoji class="g-emoji" alias="bug" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f41b.png">🐛</g-emoji> Bug fixes</h2>
<ul>
<li>resetViewToScreen on prepareToRecycle (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1147026267" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1339" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1339/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1339">#1339</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a></li>
<li>fix fast ios modal push (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1140077610" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1326" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1326/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1326">#1326</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/WoLewicki/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/WoLewicki">@ WoLewicki</a></li>
<li>remove react-native-gradle-plugin from dependencies (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1154049114" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1346" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1346/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1346">#1346</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a> and <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/tido64/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/tido64">@ tido64</a></li>
<li>apply initial navigation bar color (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1149883495" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1344" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1344/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1344">#1344</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/burakgormek/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/burakgormek">@ burakgormek</a></li>
</ul>
<h2><g-emoji class="g-emoji" alias="+1" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f44d.png">👍</g-emoji> Improvements</h2>
<ul>
<li>add stack nesting on Fabric (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1149153222" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1343" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1343/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1343">#1343</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a></li>
</ul>
<h2><g-emoji class="g-emoji" alias="1234" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f522.png">🔢</g-emoji> Miscellaneous</h2>
<ul>
<li>bump TestsExample/ to react-native 0.68rc1 (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1137227288" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1316" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1316/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1316">#1316</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a></li>
<li>update react-native-safe-area-context to fabric compatible version (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1143718503" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1333" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1333/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1333">#1333</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/janicduplessis/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/janicduplessis">@ janicduplessis</a></li>
<li>remove patch-package from FabricExample (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1145819405" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1335" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1335/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1335">#1335</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a></li>
<li>add cache-dependency-path on Android (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1145953381" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1336" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1336/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1336">#1336</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a></li>
</ul>
<p><g-emoji class="g-emoji" alias="raised_hands" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f64c.png">🙌</g-emoji> Thank you for your contributions!</p>
      </li>
      <li>
        <b>3.12.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.12.0">2022-02-17</a></br><p>This minor release includes initial support for Fabric architecture <g-emoji class="g-emoji" alias="tada" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f389.png">🎉</g-emoji></p>
<p>To learn about what we've achieved so far check out our <a href="https://blog.swmansion.com/introducing-fabric-to-react-native-screens-fd17bf18858e" rel="nofollow">Introducing Fabric to React Native Screens</a> blog post.</p>
<h2>Changes:</h2>
<ul>
<li>Add Fabric example app (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1096299961" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1261" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1261/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1261">#1261</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/Ubax/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/Ubax">@ Ubax</a></li>
<li>Publish Fabric and classic architecture release (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1128204409" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1308" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1308/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1308">#1308</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/Ubax/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/Ubax">@ Ubax</a></li>
<li>Add test build Fabric workflows (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1138836809" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1321" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1321/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1321">#1321</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a> and <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/Ubax/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/Ubax">@ Ubax</a></li>
<li>Fix headerTitle &amp; title props (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1138820764" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1320" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1320/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1320">#1320</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a></li>
<li>Remove enableFabric requirement (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1138532679" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1319" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1319/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1319">#1319</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/Ubax/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/Ubax">@ Ubax</a></li>
<li>Remove additional config steps required when running Fabric version on Android (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1138846185" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1322" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1322/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1322">#1322</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kmagiera/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kmagiera">@ kmagiera</a></li>
<li>Fix Android props on Paper (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1140020477" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1325" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1325/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1325">#1325</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/Ubax/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/Ubax">@ Ubax</a></li>
<li>Reword sentences in Fabric section (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1141156002" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1327" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1327/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1327">#1327</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kacperkapusciak/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kacperkapusciak">@ kacperkapusciak</a></li>
<li>Cleanup build process for pre-codegen versions of react-native (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1141226819" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1328" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1328/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1328">#1328</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kmagiera/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kmagiera">@ kmagiera</a></li>
</ul>
      </li>
      <li>
        <b>3.11.1</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.11.1">2022-02-11</a></br><p>Patch release adding <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1132178544" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1313" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1313/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1313">#1313</a> that fixes incorrect swipe direction default.</p>
      </li>
      <li>
        <b>3.11.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.11.0">2022-02-09</a></br><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.11.0"> Read more </a>
      </li>
      <li>
        <b>3.10.2</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.10.2">2022-01-17</a></br><p>Patch release adding <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1087800765" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1245" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1245/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1245">#1245</a> that removes the use of <code>jcenter()</code> in the library</p>
      </li>
      <li>
        <b>3.10.1</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.10.1">2021-12-07</a></br><p>Patch release adding <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1073375131" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-screens/issues/1233" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-screens/pull/1233/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-screens/pull/1233">#1233</a> for usage in Expo SDK.</p>
      </li>
      <li>
        <b>3.10.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.10.0">2021-12-02</a></br><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.10.0"> Read more </a>
      </li>
      <li>
        <b>3.9.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.9.0">2021-10-29</a></br><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.9.0"> Read more </a>
      </li>
      <li>
        <b>3.8.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.8.0">2021-09-28</a></br><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases/tag/3.8.0"> Read more </a>
      </li>
      <li>
        <b>3.7.2</b> - 2021-09-14
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/releases">react-native-screens GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>react-native-screens</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/8e6def11f78396ac927f63c0967f9615f05e6291">8e6def1</a> Release 3.13.1</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/12702dbab31fbc0987e67c49ec42d3a7a1301fc4">12702db</a> fix: wrap Screen component with React.forwardRef on Fabric (#1351)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/1c038717d97310dbe90455a6f2975c2ee95bd4c0">1c03871</a> Release 3.13.0</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/da080e3e092f01db361996b407b1fe7e88346999">da080e3</a> fix: apply initial navigation bar color (#1344)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/71e9eee3557802677a05285fb7f0849ebb573138">71e9eee</a> fix: add stack nesting on Fabric (#1343)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/01b1af65dd4ec0b0e8cfb6bd9ada4147c93bbbe4">01b1af6</a> fix: remove react-native-gradle-plugin from dependencies (#1346)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/dc3d4330a04083c754505632b071241c162f572e">dc3d433</a> fix: fast ios modal push (#1326)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/fdbefc6cc076a2186bd33fcdd6f4174ca1570ac2">fdbefc6</a> fix: resetViewToScreen on prepareToRecycle (#1339)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/f33e553228ae2f89bb13b24d23249cd657d5c644">f33e553</a> chore(deps): bump ajv from 6.12.2 to 6.12.6 (#1314)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/835de81223711655d4231d1ecaae8a1c03dc1109">835de81</a> chore(deps): bump node-fetch from 2.6.6 to 2.6.7 in /FabricExample (#1318)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/7c6e14b45834cf009c7069d46a528cf792d2a15e">7c6e14b</a> fix: add cache-dependency-path on Android (#1336)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/47e078c14db97dc8da2743d92d32feeffcb86954">47e078c</a> fix: remove patch-package from FabricExample (#1335)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/ccb6da6c2bac250cebe5afb9ba2462d7455d34f0">ccb6da6</a> feat: update react-native-safe-area-context to fabric compatible version (#1333)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/3cc53f7fe1e8d708be4ee81093885e89c7da5644">3cc53f7</a> chore: bump TestsExample/ to react-native 0.68rc1 (#1316)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/48bc5039519c54eac1535385de4dc84cfedae3bd">48bc503</a> Release 3.12.0</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/b963e87058ce0adaa2deba86532024f64fa2bd65">b963e87</a> Cleanup build process for pre-codegen versions of react-native. (#1328)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/4b2e8651467834fb4a35e78b3fe54a09afcbf990">4b2e865</a> docs: reword sentences in Fabric section (#1327)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/08464d2b9ac175a2c5f005547d3afc4c9863a1e4">08464d2</a> fix: Fixes android props on paper</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/c05fb38ab9c2e20ebe1f1f3cec914d49c2dcd7c7">c05fb38</a> Remove additional config steps required when running Fabric version on Android (#1322)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/2151c13b0e297776463d5c1622d791dc02520c9c">2151c13</a> feat: Removes enableFabric requirement (#1319)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/36c7db5105ca7babaadb6f23ab7e3ab6a8cd4a14">36c7db5</a> fix: headerTitle &amp; title props (#1320)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/59e5ef20f7a2f4d1354ed5f077bfff0abd3dc8d2">59e5ef2</a> feat: add test build Fabric workflows (#1321)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/b22efc187d41ee4a95ad82321b68459ac10c8e8e">b22efc1</a> feat: Publish fabric and classic architecture release (#1308)</li>
      <li><a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/commit/99117a899e697b18e974a1df1bb7a426741a367a">99117a8</a> feat: Adds fabric example app (#1261)</li>
    </ul>

   <a href="https://snyk.io/redirect/github/software-mansion/react-native-screens/compare/18919e0db162c76969a36e8cca2ad2ba84615772...8e6def11f78396ac927f63c0967f9615f05e6291">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiJhYmJmYThkMi1lNjY4LTQ3ZWItYThkZS1lYTBmMjZlMGYyYTYiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6ImFiYmZhOGQyLWU2NjgtNDdlYi1hOGRlLWVhMGYyNmUwZjJhNiJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?pkg&#x3D;react-native-screens&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"abbfa8d2-e668-47eb-a8de-ea0f26e0f2a6","prPublicId":"abbfa8d2-e668-47eb-a8de-ea0f26e0f2a6","dependencies":[{"name":"react-native-screens","from":"3.7.2","to":"3.13.1"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"970c0602-00b4-4afb-af02-b424dbfd28c3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":10,"publishedDate":"2022-03-03T10:04:59.082Z"},"templateVariants":["merge-advice-badge-shown"],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 08:30:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade react-i18next from 11.13.0 to 11.15.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <h3>Snyk has created this PR to upgrade react-i18next from 11.13.0 to 11.15.5.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **10 versions** ahead of your current version.
- The recommended version was released **a month ago**, on 2022-02-22.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>react-i18next</b></summary>
    <ul>
      <li>
        <b>11.15.5</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.15.5">2022-02-22</a></br><p>11.15.5</p>
      </li>
      <li>
        <b>11.15.4</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.15.4">2022-02-08</a></br><p>11.15.4</p>
      </li>
      <li>
        <b>11.15.3</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.15.3">2022-01-02</a></br><p>11.15.3</p>
      </li>
      <li>
        <b>11.15.2</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.15.2">2021-12-28</a></br><p>11.15.2</p>
      </li>
      <li>
        <b>11.15.1</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.15.1">2021-12-13</a></br><p>11.15.1</p>
      </li>
      <li>
        <b>11.15.0</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.15.0">2021-12-10</a></br><p>11.15.0</p>
      </li>
      <li>
        <b>11.14.3</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.14.3">2021-11-22</a></br><p>11.14.3</p>
      </li>
      <li>
        <b>11.14.2</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.14.2">2021-11-12</a></br><p>11.14.2</p>
      </li>
      <li>
        <b>11.14.1</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.14.1">2021-11-10</a></br><p>11.14.1</p>
      </li>
      <li>
        <b>11.14.0</b> - <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases/tag/v11.14.0">2021-11-09</a></br><p>11.14.0</p>
      </li>
      <li>
        <b>11.13.0</b> - 2021-10-28
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/i18next/react-i18next/releases">react-i18next GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>react-i18next</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/4839b63e349acfeb17e03a30500c031e494e2908">4839b63</a> update year</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/9bcce514da825fc55cf09641ff2fb28bd461e2cd">9bcce51</a> 11.15.5</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/ff0cd094e6d2561b80323703b982143b4f532330">ff0cd09</a> release</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/3f066684f4dc3c88316fe3f3bf62f09932f4cbfa">3f06668</a> Fix never return with plurals (#1453)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/97d5d07afddd7acda2870338ac305dcbe858fc5b">97d5d07</a> Bump url-parse from 1.5.4 to 1.5.7 in /example/react (#1452)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/d9cf62d09c57bd21a05110e5b9399bebbd2415d9">d9cf62d</a> update some deps in example</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/7012eed224fbfbb23eda179f3275ec4440313523">7012eed</a> 11.15.4</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/0b2b652701d752e4f71ffbf9d668f0aa88cbb804">0b2b652</a> release</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/1b7fbca64905723f25b47c25fc09a4af31e68c77">1b7fbca</a> add values field to Plural component in macros (#1446)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/e91ed946979d8a27cf0dd255c5ac7e516e02c073">e91ed94</a> 11.15.3</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/e129ba93383a447acb32e1875b7fe2d71e5998e6">e129ba9</a> release</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/566a984923c1f18786908ef38b3bad23246febbf">566a984</a> fix types (#1436)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/83cc2b63622b9b872815767d6307208ffbfb22a0">83cc2b6</a> 11.15.2</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/7d931b04e49bfd4a3ac6e58c4d46c058d925e1a1">7d931b0</a> release</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/3701357b389ece7936be07874373ec04d9b9c169">3701357</a> Fixes #1418 (#1419)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/95fad545d98cca2c700fa1c38d372e46240ea833">95fad54</a> add link to gitbook repo</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/71d3542d9132cd679ae9af4f2fb8e8e0ad24127f">71d3542</a> extend escaped test #1430</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/6fda2143c7dda1d702bb62ad0dd6d8aa75e6c606">6fda214</a> 11.15.1</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/552e20f6844a82a3dfb8b2b48eda41c5494b8bd3">552e20f</a> release</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/0905c3a041031254501cbc600c3d60f6f21217d9">0905c3a</a> Add missing types (#1429)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/8b0108d3e32443e24b6d22aa11f05ffb2630b27e">8b0108d</a> 11.15.0</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/2ec81c507aefd431608246a3543d8d7c52dce3dc">2ec81c5</a> update changelog</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/fdfd5925928c940de9f357189d8c5aaba02e75fe">fdfd592</a> Merge pull request #1426 from cuyl/master</li>
      <li><a href="https://snyk.io/redirect/github/i18next/react-i18next/commit/985f73079742c4172b0ae4b3e0c04f3715b16501">985f730</a> feat: add props to enable unespace</li>
    </ul>

   <a href="https://snyk.io/redirect/github/i18next/react-i18next/compare/269021e4256685269c8d0149744c68685d026cdd...4839b63e349acfeb17e03a30500c031e494e2908">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiIzNmYyYWZiYy04NmM0LTRiMTItYmQ5Zi05ZTFhNDZhNWRmNTMiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjM2ZjJhZmJjLTg2YzQtNGIxMi1iZDlmLTllMWE0NmE1ZGY1MyJ9fQ==" width="0" height="0"/><img src="https://app.snyk.io/badges/merge-advice/?package_manager=npm&package_name=react-i18next&from_version=11.13.0&to_version=11.15.5&pr_id=36f2afbc-86c4-4b12-bd9f-9e1a46a5df53&visibility=false&has_feature_flag=false" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?pkg&#x3D;react-i18next&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"36f2afbc-86c4-4b12-bd9f-9e1a46a5df53","prPublicId":"36f2afbc-86c4-4b12-bd9f-9e1a46a5df53","dependencies":[{"name":"react-i18next","from":"11.13.0","to":"11.15.5"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"970c0602-00b4-4afb-af02-b424dbfd28c3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":10,"publishedDate":"2022-02-22T07:39:14.189Z"},"templateVariants":["merge-advice-badge-shown"],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 08:30:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade react-native-reanimated from 2.2.4 to 2.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <h3>Snyk has created this PR to upgrade react-native-reanimated from 2.2.4 to 2.4.1.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **13 versions** ahead of your current version.
- The recommended version was released **2 months ago**, on 2022-02-07.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>react-native-reanimated</b></summary>
    <ul>
      <li>
        <b>2.4.1</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.4.1">2022-02-07</a></br><h2>What's Changed</h2>
<ul>
<li>Fix path for Web (CI build) in <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1125965521" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2962" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2962/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2962">#2962</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a class="commit-link" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/compare/2.4.0...2.4.1"><tt>2.4.0...2.4.1</tt></a></p>
      </li>
      <li>
        <b>2.4.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.4.0">2022-02-05</a></br><a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.4.0"> Read more </a>
      </li>
      <li>
        <b>2.3.3</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.3.3">2022-03-01</a></br><h2>What's Changed</h2>
<ul>
<li>Fix path for Web (CI build)</li>
</ul>
<p><strong>Full Changelog</strong>: <a class="commit-link" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/compare/2.3.2...2.3.3"><tt>2.3.2...2.3.3</tt></a></p>
      </li>
      <li>
        <b>2.3.2</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.3.2">2022-02-07</a></br><h2>What's Changed</h2>
<ul>
<li>Fix chrome debugger for iOS</li>
</ul>
      </li>
      <li>
        <b>2.3.1</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.3.1">2021-12-14</a></br><h1><g-emoji class="g-emoji" alias="bulb" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4a1.png">💡</g-emoji> Main changes</h1>
<p>Two fixes for Expo</p>
<ul>
<li>Fix duplicated BuildConfig error in release build <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1074746885" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2713" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2713/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2713">#2713</a></li>
<li>Import react classes from formal react module <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1075535269" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2720" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2720/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2720">#2720</a></li>
</ul>
<h2><g-emoji class="g-emoji" alias="raised_hands" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f64c.png">🙌</g-emoji>  Thank you for your contributions!</h2>
      </li>
      <li>
        <b>2.3.0</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.3.0">2021-12-07</a></br><h1><g-emoji class="g-emoji" alias="bulb" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4a1.png">💡</g-emoji> Main changes</h1>
<ul>
<li>Layout Reanimation (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="903863866" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2058" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2058/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2058">#2058</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/Szymon20000/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/Szymon20000">@ Szymon20000</a> and <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>Introducing Keyframe-like animation definition schema (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="941796951" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2195" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2195/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2195">#2195</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/jmysliv/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/jmysliv">@ jmysliv</a></li>
</ul>

<h1><g-emoji class="g-emoji" alias="bug" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f41b.png">🐛</g-emoji>  Bug fixes</h1>
<ul>
<li>Fix problems with polyfills (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="933633114" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2161" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2161/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2161">#2161</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>Fixed transparent colors in interpolateColors (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="985334370" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2354" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2354/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2354">#2354</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/jmysliv/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/jmysliv">@ jmysliv</a></li>
<li>Fixed removing native views without ViewManager (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1016126610" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2486" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2486/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2486">#2486</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>Fix/fix duplicate c++ symbols jsi (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1023934886" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2530" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2530/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2530">#2530</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>fix: ios native stack and RN modals (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1037237693" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2581" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2581/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2581">#2581</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/WoLewicki/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/WoLewicki">@ WoLewicki</a></li>
<li>Detach old animated styles and props (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1043438805" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2600" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2600/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2600">#2600</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/tomekzaw/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/tomekzaw">@ tomekzaw</a></li>
<li>Fix measure in iOS Modal (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1062289532" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2654" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2654/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2654">#2654</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
</ul>
<h1><g-emoji class="g-emoji" alias="+1" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f44d.png">👍</g-emoji>  Improvements</h1>
<ul>
<li>Shared style (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="749023786" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/1470" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/1470/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/1470">#1470</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>Performance optimization (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="844897594" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/1879" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/1879/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/1879">#1879</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>Add cpplint to check C++ code (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="871022462" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/1979" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/1979/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/1979">#1979</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/mrousavy/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/mrousavy">@ mrousavy</a></li>
<li>Handling JSError on iOS (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="929857965" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2153" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2153/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2153">#2153</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>Basic chrome debugger support (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="942165821" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2197" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2197/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2197">#2197</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/piaskowyk/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/piaskowyk">@ piaskowyk</a></li>
<li>Attach pointer to worklet runtime in main runtime (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="960270594" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2253" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2253/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2253">#2253</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/wkozyra95/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/wkozyra95">@ wkozyra95</a></li>
<li>Support for nested objects in animations (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="961741892" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2257" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2257/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2257">#2257</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/jmysliv/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/jmysliv">@ jmysliv</a></li>
<li>Auto-workletize React Native Gesture Handler callback functions (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="999076680" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2433" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2433/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2433">#2433</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/tomekzaw/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/tomekzaw">@ tomekzaw</a></li>
<li>Add support for animating transform matrices (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1020909486" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2511" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2511/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2511">#2511</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/kmagiera/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/kmagiera">@ kmagiera</a></li>
<li>Add global method that allows manipulation of states in Gesture Handler (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1022351652" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2519" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2519/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2519">#2519</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/j-piasecki/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/j-piasecki">@ j-piasecki</a></li>
<li>Reanimated 120 fps (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1055898407" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2636" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2636/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2636">#2636</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/tomekzaw/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/tomekzaw">@ tomekzaw</a></li>
<li>Add <code>performance.now()</code> to Worklets (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1069235873" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2679" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2679/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2679">#2679</a>) by <a class="user-mention" data-hovercard-type="user" data-hovercard-url="/users/mrousavy/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/mrousavy">@ mrousavy</a></li>
</ul>

<p><strong>Full Changelog</strong>: <a class="commit-link" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/compare/2.2.4...2.3.0"><tt>2.2.4...2.3.0</tt></a></p>
<p><g-emoji class="g-emoji" alias="warning" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/26a0.png">⚠️</g-emoji> Please note that we no longer support React Native 0.62. Please upgrade to 0.63+.</p>
<h2><g-emoji class="g-emoji" alias="raised_hands" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f64c.png">🙌</g-emoji>  Thank you for your contributions!</h2>
      </li>
      <li>
        <b>2.3.0-beta.4</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.3.0-beta.4">2021-11-26</a></br><a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.3.0-beta.4"> Read more </a>
      </li>
      <li>
        <b>2.3.0-beta.3</b> - 2021-10-18
      </li>
      <li>
        <b>2.3.0-beta.2</b> - 2021-09-30
      </li>
      <li>
        <b>2.3.0-beta.1</b> - 2021-09-24
      </li>
      <li>
        <b>2.3.0-alpha.3</b> - 2021-09-03
      </li>
      <li>
        <b>2.3.0-alpha.2</b> - 2021-07-29
      </li>
      <li>
        <b>2.3.0-alpha.1</b> - 2021-06-07
      </li>
      <li>
        <b>2.2.4</b> - <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases/tag/2.2.4">2021-10-29</a></br><h1><g-emoji class="g-emoji" alias="key" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f511.png">🔑</g-emoji>  Key changes</h1>
<ul>
<li>Added support for <code>react-native@0.67</code> - <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1036780026" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2579" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2579/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2579">#2579</a></li>
<li>Fix problem with flavor names in Gradle - <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1032891063" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2564" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2564/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2564">#2564</a></li>
<li>Fix setNativeProps for web - <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="968181346" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2280" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2280/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2280">#2280</a></li>
<li>Add fallback for not yet supported RN versions - <a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1031177391" data-permission-text="Title is private" data-url="https://github.com/software-mansion/react-native-reanimated/issues/2553" data-hovercard-type="pull_request" data-hovercard-url="/software-mansion/react-native-reanimated/pull/2553/hovercard" href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/pull/2553">#2553</a></li>
</ul>
<p>All changes: <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/compare/@ piaskowyk/2.2.3...@ piaskowyk/2.2.4?expand=1">compare 2.2.3 - 2.2.4</a></p>
<h2><g-emoji class="g-emoji" alias="raised_hands" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f64c.png">🙌</g-emoji>  Thank you for your contributions!</h2>
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/software-mansion/react-native-reanimated/releases">react-native-reanimated GitHub release notes</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiI3OTc3NTAyZC1jMzUyLTQ0NTItOTMwMy1jNmFiMzQwYjk5OTQiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6Ijc5Nzc1MDJkLWMzNTItNDQ1Mi05MzAzLWM2YWIzNDBiOTk5NCJ9fQ==" width="0" height="0"/><img src="https://app.snyk.io/badges/merge-advice/?package_manager=npm&package_name=react-native-reanimated&from_version=2.2.4&to_version=2.4.1&pr_id=7977502d-c352-4452-9303-c6ab340b9994&visibility=false&has_feature_flag=false" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?pkg&#x3D;react-native-reanimated&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"7977502d-c352-4452-9303-c6ab340b9994","prPublicId":"7977502d-c352-4452-9303-c6ab340b9994","dependencies":[{"name":"react-native-reanimated","from":"2.2.4","to":"2.4.1"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"970c0602-00b4-4afb-af02-b424dbfd28c3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":13,"publishedDate":"2022-02-07T19:11:28.960Z"},"templateVariants":["merge-advice-badge-shown"],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 08:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade react-native from 0.66.1 to 0.67.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <h3>Snyk has created this PR to upgrade react-native from 0.66.1 to 0.67.3.</h3>

![merge advice](https://app.snyk.io/badges/merge-advice/?package_manager=npm&package_name=react-native&from_version=0.66.1&to_version=0.67.3&pr_id=8856d4a1-bcad-4c9e-b355-a23139607807&visibility=true&has_feature_flag=false)
:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **14 versions** ahead of your current version.
- The recommended version was released **a month ago**, on 2022-02-22.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>react-native</b></summary>
    <ul>
      <li>
        <b>0.67.3</b> - <a href="https://snyk.io/redirect/github/facebook/react-native/releases/tag/v0.67.3">2022-02-22</a></br><h3>Fixed</h3>
<h4>Android specific</h4>
<ul>
<li>Text with adjustsFontSizeToFit changes the text layout infinitely (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/c1db41f060908e6ab001aaace7c20c610056f59a">c1db41f060</a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Fix a broken input for the Korean alphabet in TextInput (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/1a83dc36ce0af33ac7a3c311354fce4bfa5ba1a3">1a83dc36ce</a> by <a href="https://snyk.io/redirect/github/bernard-kms">@ bernard-kms</a>)</li>
</ul>
<hr>
<p>You can participate in the conversation on the status of this release at this <a href="https://snyk.io/redirect/github/reactwg/react-native-releases/discussions/15" data-hovercard-type="discussion" data-hovercard-url="/reactwg/react-native-releases/discussions/15/hovercard">discussion</a></p>
<hr>
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/" rel="nofollow">upgrade helper</a> <g-emoji class="g-emoji" alias="atom_symbol" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/269b.png">⚛️</g-emoji></p>
<hr>
<p>You can find the whole changelog history in the <a href="https://snyk.io/redirect/github/facebook/react-native/blob/main/CHANGELOG.md">changelog.md file</a>.</p>
      </li>
      <li>
        <b>0.67.2</b> - <a href="https://snyk.io/redirect/github/facebook/react-native/releases/tag/v0.67.2">2022-01-31</a></br><h3>Fixed</h3>
<ul>
<li>Fix error "mockModal is not a function" (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/507b05f4c02b46109f483a2b79c924a775fd7bd3">507b05f4c0</a> by <a href="https://snyk.io/redirect/github/AntoineDoubovetzky">@ AntoineDoubovetzky</a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Fix potential crash if ReactRootView does not have insets attached. (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/6239e2f5ce82f7c2e683eb4699b9ce3ff1b58ac5">6239e2f5ce</a> by <a href="https://snyk.io/redirect/github/enahum">@ enahum</a>)</li>
<li>Upgrading OkHttp from 4.9.1 to 4.9.2 to fix CVE-2021-0341. (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/e896d21ced3c0c917c2fc0044d2b93b44df9a081">e896d21</a> by <a href="https://snyk.io/redirect/github/owjsub">@ owjsub</a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Fix <code>Time.h</code> patch not being applied when running <code>pod install --project-directory=ios</code> (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/60cef850bd3fd12c32ee1196bd19a559592d1465">60cef850bd</a> by <a href="https://snyk.io/redirect/github/tido64">@ tido64</a>)</li>
<li>Find-node.sh now respects .nvmrc (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/35bcf934b186e581d100d43e563044300759557f">35bcf934b1</a> by <a href="https://snyk.io/redirect/github/igrayson">@ igrayson</a>)</li>
</ul>
<hr>
<p>You can participate in the conversation on the status of this release at this <a href="https://snyk.io/redirect/github/reactwg/react-native-releases/discussions/14" data-hovercard-type="discussion" data-hovercard-url="/reactwg/react-native-releases/discussions/14/hovercard">discussion</a></p>
<hr>
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/" rel="nofollow">upgrade helper</a> <g-emoji class="g-emoji" alias="atom_symbol" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/269b.png">⚛️</g-emoji></p>
<hr>
<p>You can find the whole changelog history in the <a href="https://snyk.io/redirect/github/facebook/react-native/blob/main/CHANGELOG.md">changelog.md file</a>.</p>
      </li>
      <li>
        <b>0.67.1</b> - <a href="https://snyk.io/redirect/github/facebook/react-native/releases/tag/v0.67.1">2022-01-20</a></br><p>A patch release including fixes to unblock Detox and Android JSC builds</p>
<ul>
<li>Remove alert's window when call to <code>hide</code>. (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/a46a99e12039c2b92651af1996489d660e237f1b">a46a99e120</a> by <a href="https://snyk.io/redirect/github/asafkorem">@ asafkorem</a>)</li>
<li>Do not remove libjscexecutor.so from release builds (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/574a773f8f55fe7808fbb672066be8174c64d76d">574a773f8f</a> by <a href="https://snyk.io/redirect/github/cortinico">@ cortinico</a>)</li>
</ul>
<hr>
<p>You can participate in the conversation on the status of this release at this <a href="https://snyk.io/redirect/github/reactwg/react-native-releases/discussions/12" data-hovercard-type="discussion" data-hovercard-url="/reactwg/react-native-releases/discussions/12/hovercard">discussion</a></p>
<hr>
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/" rel="nofollow">upgrade helper</a> <g-emoji class="g-emoji" alias="atom_symbol" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/269b.png">⚛️</g-emoji></p>
<hr>
<p>You can find the whole changelog history in the <a href="https://snyk.io/redirect/github/facebook/react-native/blob/main/CHANGELOG.md">changelog.md file</a>.</p>
      </li>
      <li>
        <b>0.67.0</b> - 2022-01-18
      </li>
      <li>
        <b>0.67.0-rc.6</b> - 2021-12-14
      </li>
      <li>
        <b>0.67.0-rc.5</b> - 2021-12-06
      </li>
      <li>
        <b>0.67.0-rc.4</b> - 2021-11-30
      </li>
      <li>
        <b>0.67.0-rc.3</b> - 2021-11-05
      </li>
      <li>
        <b>0.67.0-rc.2</b> - 2021-10-25
      </li>
      <li>
        <b>0.67.0-rc.1</b> - 2021-10-22
      </li>
      <li>
        <b>0.67.0-rc.0</b> - 2021-10-16
      </li>
      <li>
        <b>0.66.4</b> - 2021-12-09
      </li>
      <li>
        <b>0.66.3</b> - 2021-11-10
      </li>
      <li>
        <b>0.66.2</b> - 2021-11-04
      </li>
      <li>
        <b>0.66.1</b> - 2021-10-15
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/facebook/react-native/releases">react-native GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>react-native</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/b94a36ad8b9b313fa9173fdf8b77b80d3f1a89c3">b94a36a</a> [0.67.3] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/27fc80f3b97a7a352b8f8570e5dd8ee7951b3e53">27fc80f</a> Fixed - Text with adjustsFontSizeToFit changes the text layout infinitely (#33135)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/1aca3d1cfe6956d749f72c33212f1f16dbb0e1fd">1aca3d1</a> Fix a broken input for the Korean alphabet in TextInput (#32523)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/da420c99acea69e7c6a08795385b8a16df0b2853">da420c9</a> [0.67.2] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/3a67c27ee107148d762c4735eefb60a067b28f51">3a67c27</a> Android: Fix crash when WindowInsets is null on ReactRootView (#32989)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/e896d21ced3c0c917c2fc0044d2b93b44df9a081">e896d21</a> Android: upgrading OkHttp from 4.9.1 to 4.9.2 to fix CVE-2021-0341 (#32968)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/ac810c0a0c41257481bae2a109c65e00bd9e2bca">ac810c0</a> fix(jest/setup): fix circular dependencies in mockModal (#32964)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/d9424878a851b1a2286af6cba2ac8c198e845ed5">d942487</a> Use CircleCI API to trigger releases (#32937)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/983f0be3341c5fff8c0f979ec53ea1ad55fe1a1b">983f0be</a> fix(ios): fix &#x60;Time.h&#x60; patch not being applied (#32961)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/5590fd7092dcb8a53d7860e3449500e46005d042">5590fd7</a> fix: find-node.sh now respects .nvmrc (#32712)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/25f3d310d975a974cb3eec3e033a4b38c810dd79">25f3d31</a> [0.67.1] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/96ad60e3a1e9f92113e2357cd8ac7b187cfbc9cb">96ad60e</a> Do not remove libjscexecutor.so from release builds (#32932)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/218b4c19bb25d6ae44b3c2f211bf790b56239074">218b4c1</a> fix(iOS): remove alert&#x27;s window when call to &#x60;hide&#x60;. (#32833)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/857dbd9b208308d66b8827a1df46b0b452c13f07">857dbd9</a> [0.67.0] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/900af2b3b6d4904e0e92502dd218995aec36d6bc">900af2b</a> TODO dummy commit</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/842aac5a3c9c10e229b2da8da02e2a18f5807916">842aac5</a> Update bump-oss-version.js to guide releaser through release actions (#32769)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/a59141fb2813861fc923a71593b96c8fb70bdb9b">a59141f</a> Update comments in publish-npm and leverage isTaggedLatest</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/e7296d6b343b70b016c77d59a8e05829b11a6cbe">e7296d6</a> Remove usages of bump-oss-version from generated scripts</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/6fc004e95f30e13945bbbe223e44de19ddec4c36">6fc004e</a> Use tag to set publish version (#32757)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/c3aa86bea2c776d761b80ee2f8828fd2e50d7ea9">c3aa86b</a> [0.67.0-rc.6] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/22e4c8e1e743a92fba5898a911c6b245782e2ed0">22e4c8e</a> Fix error when pod has no IPHONEOS_DEPLOYMENT_TARGET (#32746)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/73afb97e89f8c1567428ad40346aac253b9f7550">73afb97</a> [0.67.0-rc.5] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/f269c2d71926b3f0deb80bc45f29b767e8e159ad">f269c2d</a> Fix workflow for automating version bumps</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/1c73abbbb68f67361dc8969603273cef805a7f95">1c73abb</a> isTaggedVersion checks if the commit has a version tag on it</li>
    </ul>

   <a href="https://snyk.io/redirect/github/facebook/react-native/compare/d48ed4a4bb8cf1db78b72d370b64cd120bdb9099...b94a36ad8b9b313fa9173fdf8b77b80d3f1a89c3">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiI4ODU2ZDRhMS1iY2FkLTRjOWUtYjM1NS1hMjMxMzk2MDc4MDciLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6Ijg4NTZkNGExLWJjYWQtNGM5ZS1iMzU1LWEyMzEzOTYwNzgwNyJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?pkg&#x3D;react-native&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"8856d4a1-bcad-4c9e-b355-a23139607807","prPublicId":"8856d4a1-bcad-4c9e-b355-a23139607807","dependencies":[{"name":"react-native","from":"0.66.1","to":"0.67.3"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"970c0602-00b4-4afb-af02-b424dbfd28c3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":14,"publishedDate":"2022-02-22T14:46:41.872Z"},"templateVariants":["merge-advice-badge-shown"],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 08:29:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade i18next from 21.4.0 to 21.6.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <h3>Snyk has created this PR to upgrade i18next from 21.4.0 to 21.6.13.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **23 versions** ahead of your current version.
- The recommended version was released **24 days ago**, on 2022-03-03.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>i18next</b></summary>
    <ul>
      <li>
        <b>21.6.13</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.13">2022-03-03</a></br><ul>
<li>make sure resolvedLanguage is set if lazy loading resources</li>
</ul>
      </li>
      <li>
        <b>21.6.12</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.12">2022-02-23</a></br><ul>
<li>fix ordinal-suffixes for saveMissingWithPlurals <a href="https://snyk.io/redirect/github/i18next/i18next/pull/1734" data-hovercard-type="pull_request" data-hovercard-url="/i18next/i18next/pull/1734/hovercard">1734</a></li>
</ul>
      </li>
      <li>
        <b>21.6.11</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.11">2022-02-07</a></br><ul>
<li>make sure key and additionally optional defaultValue are passed to parseMissingKeyHandler function <a href="https://snyk.io/redirect/github/i18next/react-i18next/issues/1445" data-hovercard-type="issue" data-hovercard-url="/i18next/react-i18next/issues/1445/hovercard">1445</a></li>
</ul>
      </li>
      <li>
        <b>21.6.10</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.10">2022-01-26</a></br><ul>
<li>fix: types for hasLoadedNamespace <a href="https://snyk.io/redirect/github/i18next/i18next/pull/1724" data-hovercard-type="pull_request" data-hovercard-url="/i18next/i18next/pull/1724/hovercard">1724</a></li>
</ul>
      </li>
      <li>
        <b>21.6.9</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.9">2022-01-25</a></br><ul>
<li>fix: respect skipOnVariables option passed in t function also for $t() usage</li>
</ul>
      </li>
      <li>
        <b>21.6.8</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.8">2022-01-25</a></br><ul>
<li>fix: respect skipOnVariables option passed in t function</li>
</ul>
      </li>
      <li>
        <b>21.6.7</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.7">2022-01-21</a></br><ul>
<li>fix: consistently lowercase new formatter names internally</li>
</ul>
      </li>
      <li>
        <b>21.6.6</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.6">2022-01-11</a></br><ul>
<li>fix: deepFind fallback when accessing missing flat dotted key <a href="https://snyk.io/redirect/github/i18next/i18next/issues/1719" data-hovercard-type="issue" data-hovercard-url="/i18next/i18next/issues/1719/hovercard">1719</a></li>
</ul>
      </li>
      <li>
        <b>21.6.5</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.5">2022-01-04</a></br><ul>
<li>fix: passed format parameter value truncation in options argument for custom formatter <a href="https://snyk.io/redirect/github/i18next/i18next/issues/1715" data-hovercard-type="issue" data-hovercard-url="/i18next/i18next/issues/1715/hovercard">1715</a></li>
</ul>
      </li>
      <li>
        <b>21.6.4</b> - <a href="https://snyk.io/redirect/github/i18next/i18next/releases/tag/v21.6.4">2021-12-28</a></br><ul>
<li>fix: skipOnVariables (and all other interpolation options should respect defaults) <a href="https://snyk.io/redirect/github/i18next/i18next/issues/1711" data-hovercard-type="issue" data-hovercard-url="/i18next/i18next/issues/1711/hovercard">1711</a></li>
</ul>
      </li>
      <li>
        <b>21.6.3</b> - 2021-12-18
      </li>
      <li>
        <b>21.6.2</b> - 2021-12-16
      </li>
      <li>
        <b>21.6.1</b> - 2021-12-16
      </li>
      <li>
        <b>21.6.0</b> - 2021-12-08
      </li>
      <li>
        <b>21.5.6</b> - 2021-12-07
      </li>
      <li>
        <b>21.5.5</b> - 2021-12-07
      </li>
      <li>
        <b>21.5.4</b> - 2021-11-29
      </li>
      <li>
        <b>21.5.3</b> - 2021-11-23
      </li>
      <li>
        <b>21.5.2</b> - 2021-11-16
      </li>
      <li>
        <b>21.5.1</b> - 2021-11-16
      </li>
      <li>
        <b>21.5.0</b> - 2021-11-15
      </li>
      <li>
        <b>21.4.2</b> - 2021-11-09
      </li>
      <li>
        <b>21.4.1</b> - 2021-11-08
      </li>
      <li>
        <b>21.4.0</b> - 2021-11-02
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/i18next/i18next/releases">i18next GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>i18next</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/430a93161b7adaf8580324ea2b2858bd7a2e71a5">430a931</a> 21.6.13</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/de6f7243dc201f0500204890b1955dc5b8b22398">de6f724</a> make sure resolvedLanguage is set if lazy loading resources</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/f2f72f13df1fe643816069620e7b8edcab4773d2">f2f72f1</a> 21.6.12</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/91d98200c6aebfed177a152ac7274d8c4cf0acda">91d9820</a> release</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/00a7ebfbc4ab0eb94fc6d75126c429b87fe7146c">00a7ebf</a> Fixed ordinal-suffixes for saveMissingWithPlurals (#1734)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/3989b0752f0c10b787ea5fddf00f026c3abd34d1">3989b07</a> fix link</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/cb23709e8d798a4b0806e226f08fc4e836ce5a02">cb23709</a> 21.6.11</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/cc639337a7031db91d525982c4989932eb9ad26d">cc63933</a> make sure key and additionally optional defaultValue are passed to parseMissingKeyHandler function, fixes #1445</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/c891f923a1396a0485f36c51b3d93652015dcec7">c891f92</a> use different currencies in test</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/bfa0c0f0c4a69cf16af7112ded3679b52737ac36">bfa0c0f</a> 21.6.10</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/4287229fd03a682bb0cb399d91b9f1234a3c2190">4287229</a> prepare version</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/4a7dcd42e5083e7f035583e9ab96ac04978525a5">4a7dcd4</a> fix typing and documentation of &#x60;hasLoadedNamespace&#x60; (#1724)</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/ce01d6dfbf33e09c1163661557b6d347878f35dc">ce01d6d</a> 21.6.9</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/cdd0c6fcec694ee962bcabb2f04d4c45c66c6755">cdd0c6f</a> fix: respect skipOnVariables option passed in t function also for $t() usage, #1721</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/7d7dcf84c48b9c9673f0976674b9265696293b8a">7d7dcf8</a> 21.6.8</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/cae51271992cc3f7859e4601d970418221778fc8">cae5127</a> fix: respect skipOnVariables option passed in t function #1721</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/79c0fa2ea597af5cb571f28c5a29b3ea171ddb66">79c0fa2</a> some funding information</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/3cc45cfab2ae75fb992e71428199ab3c2b6d268c">3cc45cf</a> 21.6.7</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/75463d2df329f10042d6652e0d696cd0e2c18d87">75463d2</a> missing trim</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/08159c1cbada63df065f414c37b547e9e34335ca">08159c1</a> fix: consistently lowercase new formatter names internally, #1722</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/aad62416735de81cf982b589bd770f0d140c08bc">aad6241</a> 21.6.6</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/12f9a6a3e6d191d618c71a94889aabe2df202f25">12f9a6a</a> fix #1719</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/69f2ac52ebcfab8d0b113c9609f67e7a63c85463">69f2ac5</a> update year in license</li>
      <li><a href="https://snyk.io/redirect/github/i18next/i18next/commit/9331e28c76cb46007d4a63a95d36dfeaabcfc862">9331e28</a> 21.6.5</li>
    </ul>

   <a href="https://snyk.io/redirect/github/i18next/i18next/compare/1c72609a940182869ada8ab95e250446ef8f1582...430a93161b7adaf8580324ea2b2858bd7a2e71a5">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiIwOWFhMjMyYy1lNTQ4LTQwOGYtYWNmYy1kM2UyNDU4ODAzYjQiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjA5YWEyMzJjLWU1NDgtNDA4Zi1hY2ZjLWQzZTI0NTg4MDNiNCJ9fQ==" width="0" height="0"/><img src="https://app.snyk.io/badges/merge-advice/?package_manager=npm&package_name=i18next&from_version=21.4.0&to_version=21.6.13&pr_id=09aa232c-e548-408f-acfc-d3e2458803b4&visibility=false&has_feature_flag=false" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3/settings/integration?pkg&#x3D;i18next&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"09aa232c-e548-408f-acfc-d3e2458803b4","prPublicId":"09aa232c-e548-408f-acfc-d3e2458803b4","dependencies":[{"name":"i18next","from":"21.4.0","to":"21.6.13"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/clecio.varjao/project/970c0602-00b4-4afb-af02-b424dbfd28c3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"970c0602-00b4-4afb-af02-b424dbfd28c3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":23,"publishedDate":"2022-03-03T09:39:37.478Z"},"templateVariants":["merge-advice-badge-shown"],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 08:29:48 +0000 UTC
    </div>
</div>

