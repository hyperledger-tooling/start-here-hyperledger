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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/504" class=".btn">#504</a>
            </td>
            <td>
                <b>
                    revocation notification working, needs french translation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: ryankoch13 <ryan.koch13@gmail.com>

# Summary of Changes

This PR removes the old management of revocation notification using the context providers and instead uses the new AFJ and react hook functionality to detect if a credential is revoked. Once a credential is revoked, a new notification will appear on the Home screen. If the credential details is viewed for the revoked credential it will add a metadata property to get rid of the notification. 

It should be noted that the "CredentialRevokedMessageTitle" was edited and a new string was added to the English localization file. Please let me know if anyone has suggestions on how to avoid these changes or update the other translation files to match. 

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-22 00:56:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/503" class=".btn">#503</a>
            </td>
            <td>
                <b>
                    fix: unable to toggle on
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fix issue where biometrics cannot be toggled on in Settings if it was never turned on in the first place.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 21:20:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    feat: Enable connection invites using shortened urls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This change enables connections using a url shortener request (see [https://github.com/hyperledger/aries-rfcs/tree/main/features/0434-outofband#url-shortening](https://github.com/hyperledger/aries-rfcs/tree/main/features/0434-outofband#url-shortening)).
To receive invites using a url shortener, I changed the call `agent?.oob.parseInvitation(uri)` to `agent?.oob.parseInvitationShortUrl(uri)`. They are basically the same, but the second one also has support to short urls. 

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [X] Updated documentation as needed for changed code and new or modified features;
- [X] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 20:17:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/501" class=".btn">#501</a>
            </td>
            <td>
                <b>
                    fix: add test ID to home nav
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add test ID to tab navigation.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 17:23:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/500" class=".btn">#500</a>
            </td>
            <td>
                <b>
                    chore(deps): bump react-native-reanimated from 2.2.4 to 2.11.0 in /core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [react-native-reanimated](https://github.com/software-mansion/react-native-reanimated) from 2.2.4 to 2.11.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/software-mansion/react-native-reanimated/releases">react-native-reanimated's releases</a>.</em></p>
<blockquote>
<h2>2.11.0</h2>
<h1>🚀 Main changes</h1>
<ul>
<li>Added new useScrollViewOffset hook <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3438">#3438</a></li>
<li>Added FrameTimings to the useFrameCallback hook</li>
<li>Fixes for building Reanimated in monorepo</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/software-mansion/react-native-reanimated/compare/2.10.0...2.11.0">https://github.com/software-mansion/react-native-reanimated/compare/2.10.0...2.11.0</a></p>
<p>Build: <a href="https://github.com/software-mansion/react-native-reanimated/actions/runs/3105231111">https://github.com/software-mansion/react-native-reanimated/actions/runs/3105231111</a></p>
<h2>🙌  Thank you for your contributions!</h2>
<h2>2.10.0</h2>
<h1>🚀 Main changes</h1>
<ul>
<li>Added <a href="https://docs.swmansion.com/react-native-reanimated/docs/next/api/hooks/useAnimatedKeyboard/"><code>useAnimatedKeyboard()</code></a> hook</li>
<li>Added <a href="https://docs.swmansion.com/react-native-reanimated/docs/next/api/hooks/useFrameCallback/"><code>useFrameCallback()</code></a> hook</li>
<li>Added support for React Native 0.70</li>
<li>Added support for react-native-v8 (building from source only)</li>
<li>Detect multiple versions of Reanimated.</li>
<li>And many different fixes.</li>
</ul>
<p>Build: <a href="https://github.com/software-mansion/react-native-reanimated/actions/runs/2889631689">https://github.com/software-mansion/react-native-reanimated/actions/runs/2889631689</a></p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/software-mansion/react-native-reanimated/compare/2.9.1...2.10.0">https://github.com/software-mansion/react-native-reanimated/compare/2.9.1...2.10.0</a></p>
<h2>2.9.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue with duplicated <code>libfolly_runtime.so</code> - <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3342">software-mansion/react-native-reanimated#3342</a></li>
</ul>
<p>Build: <a href="https://github.com/software-mansion/react-native-reanimated/actions/runs/2595830511">https://github.com/software-mansion/react-native-reanimated/actions/runs/2595830511</a></p>
<h2>🙌  Thank you for your contributions!</h2>
<h2>2.9.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Support for <code>react-native@0.69</code></li>
<li>Treeshaking - <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3278">software-mansion/react-native-reanimated#3278</a></li>
<li>Some fixes and improvements</li>
</ul>
<p>Package contains binaries for <code>react-native</code> in version from 0.65 to 0.69</p>
<p>Build: <a href="https://github.com/software-mansion/react-native-reanimated/actions/runs/2590392729">https://github.com/software-mansion/react-native-reanimated/actions/runs/2590392729</a></p>
<h2>🙌  Thank you for your contributions!</h2>
<h2>2.8.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Load <code>RNGestureHandlerModule</code> lazily on iOS by <a href="https://github.com/j-piasecki"><code>@​j-piasecki</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3166">software-mansion/react-native-reanimated#3166</a></li>
<li>fix: Fix <code>useAnimatedSensor</code> return type by <a href="https://github.com/mrousavy"><code>@​mrousavy</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3094">software-mansion/react-native-reanimated#3094</a></li>
<li>Add opts for relative source location by <a href="https://github.com/jiulongw"><code>@​jiulongw</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3141">software-mansion/react-native-reanimated#3141</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/7409602b93ecdaa9d8dcd90d7ae6a253a28fb2dc"><code>7409602</code></a> Add reanimated_utils.rb to package (<a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3667">#3667</a>)</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/1b0d64cf64ead1566f29433258b96a5451a510c8"><code>1b0d64c</code></a> Fix REANIMATED_PACKAGE_BUILD</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/b8fe6b44ae763ef07df74fc12d2f8b6958aa02b2"><code>b8fe6b4</code></a> Remove debug symbols for release package</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/4d9bd5450c7c04dba5ead6d00634493e1d4b5bfd"><code>4d9bd54</code></a> Resolve paths</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/49b664f8714553eeb4c3905da99ae01a8a550dac"><code>49b664f</code></a> Update name of property</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/ece45524a8c1b4c05ee18ac40ac494bd513d2d12"><code>ece4552</code></a> Recognize package buildnig mode</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/643d6905f76c44706be49fc68eb9e8db1525974d"><code>643d690</code></a> Update building script</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/e1fc0bf5256bf89ee4eb3f16308071d552d9147f"><code>e1fc0bf</code></a> Avoid checking same node_modules path</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/506ca087aeb51f0f1e90c6ed57c0a8d74ead0a12"><code>506ca08</code></a> Patch release build</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/6ba5b8187f825e0ce19fb4d4e884d945d3348da1"><code>6ba5b81</code></a> Remove hermes headers</li>
<li>Additional commits viewable in <a href="https://github.com/software-mansion/react-native-reanimated/compare/2.2.4...2.11.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-native-reanimated&package-manager=npm_and_yarn&previous-version=2.2.4&new-version=2.11.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-21 02:49:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/499" class=".btn">#499</a>
            </td>
            <td>
                <b>
                    chore(deps): bump react-native-reanimated from 2.2.4 to 2.10.0 in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [react-native-reanimated](https://github.com/software-mansion/react-native-reanimated) from 2.2.4 to 2.10.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/software-mansion/react-native-reanimated/releases">react-native-reanimated's releases</a>.</em></p>
<blockquote>
<h2>2.10.0</h2>
<h1>🚀 Main changes</h1>
<ul>
<li>Added <a href="https://docs.swmansion.com/react-native-reanimated/docs/next/api/hooks/useAnimatedKeyboard/"><code>useAnimatedKeyboard()</code></a> hook</li>
<li>Added <a href="https://docs.swmansion.com/react-native-reanimated/docs/next/api/hooks/useFrameCallback/"><code>useFrameCallback()</code></a> hook</li>
<li>Added support for React Native 0.70</li>
<li>Added support for react-native-v8 (building from source only)</li>
<li>Detect multiple versions of Reanimated.</li>
<li>And many different fixes.</li>
</ul>
<p>Build: <a href="https://github.com/software-mansion/react-native-reanimated/actions/runs/2889631689">https://github.com/software-mansion/react-native-reanimated/actions/runs/2889631689</a></p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/software-mansion/react-native-reanimated/compare/2.9.1...2.10.0">https://github.com/software-mansion/react-native-reanimated/compare/2.9.1...2.10.0</a></p>
<h2>2.9.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue with duplicated <code>libfolly_runtime.so</code> - <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3342">software-mansion/react-native-reanimated#3342</a></li>
</ul>
<p>Build: <a href="https://github.com/software-mansion/react-native-reanimated/actions/runs/2595830511">https://github.com/software-mansion/react-native-reanimated/actions/runs/2595830511</a></p>
<h2>🙌  Thank you for your contributions!</h2>
<h2>2.9.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Support for <code>react-native@0.69</code></li>
<li>Treeshaking - <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3278">software-mansion/react-native-reanimated#3278</a></li>
<li>Some fixes and improvements</li>
</ul>
<p>Package contains binaries for <code>react-native</code> in version from 0.65 to 0.69</p>
<p>Build: <a href="https://github.com/software-mansion/react-native-reanimated/actions/runs/2590392729">https://github.com/software-mansion/react-native-reanimated/actions/runs/2590392729</a></p>
<h2>🙌  Thank you for your contributions!</h2>
<h2>2.8.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Load <code>RNGestureHandlerModule</code> lazily on iOS by <a href="https://github.com/j-piasecki"><code>@​j-piasecki</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3166">software-mansion/react-native-reanimated#3166</a></li>
<li>fix: Fix <code>useAnimatedSensor</code> return type by <a href="https://github.com/mrousavy"><code>@​mrousavy</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3094">software-mansion/react-native-reanimated#3094</a></li>
<li>Add opts for relative source location by <a href="https://github.com/jiulongw"><code>@​jiulongw</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3141">software-mansion/react-native-reanimated#3141</a></li>
<li>Fix JSCRuntime destroyed with a dangling API object by <a href="https://github.com/lukmccall"><code>@​lukmccall</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3185">software-mansion/react-native-reanimated#3185</a></li>
</ul>
<h2>New Contributors</h2>
<p><a href="https://github.com/dylmye"><code>@​dylmye</code></a> <a href="https://github.com/jiulongw"><code>@​jiulongw</code></a> <a href="https://github.com/lukmccall"><code>@​lukmccall</code></a></p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/software-mansion/react-native-reanimated/compare/2.7.0...2.8.0">https://github.com/software-mansion/react-native-reanimated/compare/2.7.0...2.8.0</a></p>
<h2>🙌  Thank you for your contributions!</h2>
<h2>2.7.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove <code>opacity</code> from native props list by <a href="https://github.com/tomekzaw"><code>@​tomekzaw</code></a> in <a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/pull/3139">software-mansion/react-native-reanimated#3139</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/1b61196c1a5e2f05da533b6035c6663d0129bbc5"><code>1b61196</code></a> Release 2.10.0 (<a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3475">#3475</a>)</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/d3395e0a405c606703d34f5ec222e89d0f378474"><code>d3395e0</code></a> Revert &quot;Exclude META-INF&quot;</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/c25c71f7b3e23a4c061748671d6bef6be8a31b87"><code>c25c71f</code></a> Exclude META-INF</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/af31d7affb59d5f17fdf54990f82bb93398f285f"><code>af31d7a</code></a> Update Types</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/128f9c3e5c9fbef8f891ab0077feb098f6ac347a"><code>128f9c3</code></a> Patch 70</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/051e8e2feb7df74839dcde69f8ea1a91dc091051"><code>051e8e2</code></a> Set the newest RN version</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/3eca471538ea0280a52325f67a473b7d4b89af7d"><code>3eca471</code></a> 2.10.0</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/6668dd133feea1cea92a9d37ad6f07420374dd92"><code>6668dd1</code></a> Update plugin error message (<a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3437">#3437</a>)</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/d42b63cd67f71fe564be386fc4a8401d86111ff9"><code>d42b63c</code></a> Update NativeProxy.cpp (<a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3469">#3469</a>)</li>
<li><a href="https://github.com/software-mansion/react-native-reanimated/commit/98c628acea50a0ae6f54879742972691f4699ca3"><code>98c628a</code></a> Bumped gesture-handler and screens dependencies (<a href="https://github-redirect.dependabot.com/software-mansion/react-native-reanimated/issues/3468">#3468</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/software-mansion/react-native-reanimated/compare/2.2.4...2.10.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-native-reanimated&package-manager=npm_and_yarn&previous-version=2.2.4&new-version=2.10.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-21 02:49:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    refactor: namespaced exports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

The list of export items in `core/App/index.ts` is rapidly growing. I am proposing that we switch to export "namespaced" objects for better organization.

This PR does not remove any existing exports, so it doesn't break compatibility. Removal of the exports would be a breaking change that can be introduced later.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 22:58:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    feat: add indyLedgers to ConfigurationContext
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

In order to use another ledger than the ones configured in `core/configs/ledgers/indy`, a configuration is added on the ConfigurationContext.

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [X] Updated documentation as needed for changed code and new or modified features;
- [X] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 19:39:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    feat: added biometrics button unlock to PinEnter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>

# Summary of Changes

Added biometrics button on PinEnter screen to re-prompt the user if they decline biometrics
![bioButton1](https://user-images.githubusercontent.com/36937407/197018450-16c831b0-5ee8-4081-9b3c-be2ca6c7c0d7.png)

![bioButton2](https://user-images.githubusercontent.com/36937407/197018478-0e6002aa-9534-4318-a415-2f88fb5d1d14.png)

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 17:32:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/495" class=".btn">#495</a>
            </td>
            <td>
                <b>
                    feat: allow toggle biometrics from settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR allows the user to enable or disable biometrics via Settings.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 17:23:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    chore(deps): bump shell-quote and @react-native-community/cli-tools in /core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/ljharb/shell-quote) and [@react-native-community/cli-tools](https://github.com/react-native-community/cli/tree/HEAD/packages/tools). These dependencies needed to be updated together.
Updates `shell-quote` from 1.6.1 to 1.7.4
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/shell-quote/blob/main/CHANGELOG.md">shell-quote's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.7.3...v1.7.4">v1.7.4</a> - 2022-10-12</h2>
<h3>Merged</h3>
<ul>
<li>Add node_modules to .gitignore <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/48"><code>[#48](https://github.com/ljharb/shell-quote/issues/48)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a></li>
<li>[eslint] additional cleanup <a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a></li>
<li>[eslint] add eslint <a href="https://github.com/ljharb/shell-quote/commit/6ee1437df1b10a79bdf2aaa04f2bacc9f420dc15"><code>6ee1437</code></a></li>
<li>[readme] rename, add badges <a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a></li>
<li>[meta] update URLs <a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/ljharb/shell-quote/commit/f97411ef4d2f183200fc8a28beca9faf9b08a640"><code>f97411e</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/ljharb/shell-quote/commit/051f60857ad5035280208abdc348bf5ba42a6254"><code>051f608</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/ljharb/shell-quote/commit/dc1cc12b956ccd93d58aaaad263bee7d50576d27"><code>dc1cc12</code></a></li>
</ul>
<!-- raw HTML omitted -->
<h2>1.7.3</h2>
<ul>
<li>Fix a security issue where the regex for windows drive letters allowed some shell meta-characters
to escape the quoting rules. (CVE-2021-42740)</li>
</ul>
<h2>1.7.2</h2>
<ul>
<li>Fix a regression introduced in 1.6.3. This reverts the Windows path quoting fix. (<a href="https://github.com/ljharb/shell-quote/commit/144e1c20cd57549a414c827fb3032e60b7b8721c">144e1c2</a>)</li>
</ul>
<h2>1.7.1</h2>
<ul>
<li>Fix <code>$</code> being removed when not part of an environment variable name. (<a href="https://github.com/Admin"><code>@​Adman</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/32">#32</a>)</li>
</ul>
<h2>1.7.0</h2>
<ul>
<li>Add support for parsing <code>&gt;&gt;</code> and <code>&gt;&amp;</code> redirection operators. (<a href="https://github.com/forivall"><code>@​forivall</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/16">#16</a>)</li>
<li>Add support for parsing <code>&lt;(</code> process substitution operator. (<a href="https://github.com/cuonglm"><code>@​cuonglm</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/15">#15</a>)</li>
</ul>
<h2>1.6.3</h2>
<ul>
<li>Fix Windows path quoting problems. (<a href="https://github.com/dy"><code>@​dy</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/34">#34</a>)</li>
</ul>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.6.2">v1.6.2</a> - 2019-08-13</h2>
<h3>Merged</h3>
<ul>
<li>Use native JSON and Array methods <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/21"><code>[#21](https://github.com/ljharb/shell-quote/issues/21)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>fix whitespace <a href="https://github.com/ljharb/shell-quote/commit/72fb5a8ce29b4f67f28302af33c217b58f92e260"><code>72fb5a8</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/shell-quote/commit/5409e72ef6c905c4d1637883cd394f6f07abd934"><code>5409e72</code></a> v1.7.4</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a> [actions] add reusable workflows</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a> [meta] create FUNDING.yml; add <code>funding</code> in package.json</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a> [meta] add <code>auto-changelog</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a> [readme] rename, add badges</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a> [meta] update URLs</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a> [meta] add <code>safe-publish-latest</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a> [eslint] additional cleanup</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a> [eslint] fix indentation and whitespace</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.7.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for shell-quote since your current version.</p>
</details>
<br />

Updates `@react-native-community/cli-tools` from 6.1.0 to 6.2.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/react-native-community/cli/releases"><code>@​react-native-community/cli-tools</code>'s releases</a>.</em></p>
<blockquote>
<h2>v6.2.0</h2>
<h2>Features</h2>
<ul>
<li>support renamed <code>-PreactNativeArchitectures</code> (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1496">#1496</a>)</li>
</ul>
<h2>Fixes</h2>
<ul>
<li>better Handle EPERM on Windows (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1495">#1495</a>)</li>
<li>use <code>simclt</code> instead of deprecated <code>instruments</code> (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1484">#1484</a>)</li>
<li>platform-ios: add missing <code>ora</code> dependency (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1483">#1483</a>)</li>
</ul>
<h2>Chore &amp; Maintenance</h2>
<ul>
<li>bump lerna to 4 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1504">#1504</a>)</li>
<li>bump chalk to 4.x (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1505">#1505</a>)</li>
<li>GH Actions: lint &amp; unit tests (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1499">#1499</a>)</li>
<li>remove mkdirp (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1500">#1500</a>)</li>
<li>add 6.1.0 release to compatibility table (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1501">#1501</a>)</li>
<li>replace azure with github actions (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1494">#1494</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/react-native-community/cli/commit/7a10b39160d53caf43f36ae9e62d4bed942003ea"><code>7a10b39</code></a> Publish</li>
<li><a href="https://github.com/react-native-community/cli/commit/a327ac86983d8b1dc8020f4d10c27d0764695a25"><code>a327ac8</code></a> chore(deps): bump shell-quote to 1.7.3 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1642">#1642</a>)</li>
<li><a href="https://github.com/react-native-community/cli/commit/908eac093d84ef0a5786e3de0f480519ddcc3ecb"><code>908eac0</code></a> v6.2.0</li>
<li><a href="https://github.com/react-native-community/cli/commit/1ac43cce3df75bff069558ac13e8314a17d892e4"><code>1ac43cc</code></a> bump chalk to 4.x (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1505">#1505</a>)</li>
<li><a href="https://github.com/react-native-community/cli/commit/ad0883d8e9b20e30e85adacbfc0b525df5d72840"><code>ad0883d</code></a> chore(deps): remove mkdirp (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1500">#1500</a>)</li>
<li>See full diff in <a href="https://github.com/react-native-community/cli/commits/@react-native-community/cli-tools@6.2.1/packages/tools">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2022-10-19 21:08:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    chore(deps): bump shell-quote and @react-native-community/cli-tools in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/ljharb/shell-quote) and [@react-native-community/cli-tools](https://github.com/react-native-community/cli/tree/HEAD/packages/tools). These dependencies needed to be updated together.
Updates `shell-quote` from 1.6.1 to 1.7.4
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/shell-quote/blob/main/CHANGELOG.md">shell-quote's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.7.3...v1.7.4">v1.7.4</a> - 2022-10-12</h2>
<h3>Merged</h3>
<ul>
<li>Add node_modules to .gitignore <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/48"><code>[#48](https://github.com/ljharb/shell-quote/issues/48)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a></li>
<li>[eslint] additional cleanup <a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a></li>
<li>[eslint] add eslint <a href="https://github.com/ljharb/shell-quote/commit/6ee1437df1b10a79bdf2aaa04f2bacc9f420dc15"><code>6ee1437</code></a></li>
<li>[readme] rename, add badges <a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a></li>
<li>[meta] update URLs <a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/ljharb/shell-quote/commit/f97411ef4d2f183200fc8a28beca9faf9b08a640"><code>f97411e</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/ljharb/shell-quote/commit/051f60857ad5035280208abdc348bf5ba42a6254"><code>051f608</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/ljharb/shell-quote/commit/dc1cc12b956ccd93d58aaaad263bee7d50576d27"><code>dc1cc12</code></a></li>
</ul>
<!-- raw HTML omitted -->
<h2>1.7.3</h2>
<ul>
<li>Fix a security issue where the regex for windows drive letters allowed some shell meta-characters
to escape the quoting rules. (CVE-2021-42740)</li>
</ul>
<h2>1.7.2</h2>
<ul>
<li>Fix a regression introduced in 1.6.3. This reverts the Windows path quoting fix. (<a href="https://github.com/ljharb/shell-quote/commit/144e1c20cd57549a414c827fb3032e60b7b8721c">144e1c2</a>)</li>
</ul>
<h2>1.7.1</h2>
<ul>
<li>Fix <code>$</code> being removed when not part of an environment variable name. (<a href="https://github.com/Admin"><code>@​Adman</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/32">#32</a>)</li>
</ul>
<h2>1.7.0</h2>
<ul>
<li>Add support for parsing <code>&gt;&gt;</code> and <code>&gt;&amp;</code> redirection operators. (<a href="https://github.com/forivall"><code>@​forivall</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/16">#16</a>)</li>
<li>Add support for parsing <code>&lt;(</code> process substitution operator. (<a href="https://github.com/cuonglm"><code>@​cuonglm</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/15">#15</a>)</li>
</ul>
<h2>1.6.3</h2>
<ul>
<li>Fix Windows path quoting problems. (<a href="https://github.com/dy"><code>@​dy</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/34">#34</a>)</li>
</ul>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.6.2">v1.6.2</a> - 2019-08-13</h2>
<h3>Merged</h3>
<ul>
<li>Use native JSON and Array methods <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/21"><code>[#21](https://github.com/ljharb/shell-quote/issues/21)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>fix whitespace <a href="https://github.com/ljharb/shell-quote/commit/72fb5a8ce29b4f67f28302af33c217b58f92e260"><code>72fb5a8</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/shell-quote/commit/5409e72ef6c905c4d1637883cd394f6f07abd934"><code>5409e72</code></a> v1.7.4</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a> [actions] add reusable workflows</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a> [meta] create FUNDING.yml; add <code>funding</code> in package.json</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a> [meta] add <code>auto-changelog</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a> [readme] rename, add badges</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a> [meta] update URLs</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a> [meta] add <code>safe-publish-latest</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a> [eslint] additional cleanup</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a> [eslint] fix indentation and whitespace</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.7.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for shell-quote since your current version.</p>
</details>
<br />

Updates `@react-native-community/cli-tools` from 6.2.0 to 6.2.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/react-native-community/cli/commit/7a10b39160d53caf43f36ae9e62d4bed942003ea"><code>7a10b39</code></a> Publish</li>
<li><a href="https://github.com/react-native-community/cli/commit/a327ac86983d8b1dc8020f4d10c27d0764695a25"><code>a327ac8</code></a> chore(deps): bump shell-quote to 1.7.3 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1642">#1642</a>)</li>
<li>See full diff in <a href="https://github.com/react-native-community/cli/commits/@react-native-community/cli-tools@6.2.1/packages/tools">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2022-10-19 21:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    chore: update core AFJ to 0.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Akiff Manji <akiff.manji@gmail.com>

# Summary of Changes

Updates core AFJ module to 0.2.2 to align with app.

# Related Issues

#491 

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [ ] Updated documentation as needed for changed code and new or modified features;
- [ ] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 20:30:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    feat: card rendering using flexbox layout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This new simplified rendering strat relies on [Flexbox Layout](https://reactnative.dev/docs/flexbox) and automatically image scaling. As part of this automatic scaling the logo images MUST be provided in a predefined aspect ratio: 1:1  (width:height) for logos that shows issuer name, or `4:1` (width:height) for when the issuer name is hidden.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 01:11:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/489" class=".btn">#489</a>
            </td>
            <td>
                <b>
                    changed core/App folder to core/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>

# Summary of Changes

Changed outdated core/App folder to core/src folder. This makes the file structure easier to understand

# Related Issues

Resolves: #408 

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 22:19:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    chore(deps): bump @xmldom/xmldom from 0.7.5 to 0.7.6 in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@xmldom/xmldom](https://github.com/xmldom/xmldom) from 0.7.5 to 0.7.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/releases"><code>@​xmldom/xmldom</code>'s releases</a>.</em></p>
<blockquote>
<h2>0.7.6</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/441"><code>[#441](https://github.com/xmldom/xmldom/issues/441)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/jftanner"><code>@​jftanner</code></a>, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/blob/master/CHANGELOG.md"><code>@​xmldom/xmldom</code>'s changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">0.7.6</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/441"><code>[#441](https://github.com/xmldom/xmldom/issues/441)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/jftanner"><code>@​jftanner</code></a>, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.3...0.8.2">0.8.3</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.1...0.9.0-beta.2">0.9.0-beta.2</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.3...0.8.2">0.8.3</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.2...0.9.0-beta.1">0.9.0-beta.1</a></h2>
<h3>Fixed</h3>
<p><strong>Only use HTML rules if mimeType matches</strong> <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/338"><code>[#338](https://github.com/xmldom/xmldom/issues/338)</code></a>, fixes <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/203"><code>[#203](https://github.com/xmldom/xmldom/issues/203)</code></a></p>
<p>In the living specs for parsing XML and HTML, that this library is trying to implement,
there is a distinction between the different types of documents being parsed:
There are quite some rules that are different for parsing, constructing and serializing XML vs HTML documents.</p>
<p>So far xmldom was always &quot;detecting&quot; whether &quot;the HTML rules should be applied&quot; by looking at the current namespace. So from the first time an the HTML default namespace (<code>http://www.w3.org/1999/xhtml</code>) was found, every node was treated as being part of an HTML document. This misconception is the root cause for quite some reported bugs.</p>
<p>BREAKING CHANGE: HTML rules are no longer applied just because of the namespace, but require the <code>mimeType</code> argument passed to <code>DOMParser.parseFromString(source, mimeType)</code> to match <code>'text/html'</code>. Doing so implies all rules for handling casing for tag and attribute names when parsing, creation of nodes and searching nodes.</p>
<p>BREAKING CHANGE: Correct the return type of <code>DOMParser.parseFromString</code> to <code>Document | undefined</code>. In case of parsing errors it was always possible that &quot;the returned <code>Document</code>&quot; has not been created. In case you are using Typescript you now need to handle those cases.</p>
<p>BREAKING CHANGE: The instance property <code>DOMParser.options</code> is no longer available, instead use the individual <code>readonly</code> property per option (<code>assign</code>, <code>domHandler</code>, <code>errorHandler</code>, <code>normalizeLineEndings</code>, <code>locator</code>, <code>xmlns</code>). Those also provides the default value if the option was not passed. The 'locator' option is now just a boolean (default remains <code>true</code>).</p>
<p>BREAKING CHANGE: The following methods no longer allow a (non spec compliant) boolean argument to toggle &quot;HTML rules&quot;:</p>
<ul>
<li><code>XMLSerializer.serializeToString</code></li>
<li><code>Node.toString</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/xmldom/xmldom/commit/3ca016d7da634686dbcadd076dda07d28a8ffd45"><code>3ca016d</code></a> 0.7.6</li>
<li><a href="https://github.com/xmldom/xmldom/commit/b28e631b8bc42edca9df6eb68e5b84f78529b3cb"><code>b28e631</code></a> docs: Prepare CHANGELOG for 0.7.6</li>
<li><a href="https://github.com/xmldom/xmldom/commit/1f20aee8ef1a8f3964add1a188f723bbc54862a0"><code>1f20aee</code></a> fix: Backport PR-437 to 0.7.x branch</li>
<li>See full diff in <a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@xmldom/xmldom&package-manager=npm_and_yarn&previous-version=0.7.5&new-version=0.7.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-17 21:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    feat: oca image display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR let us use OCA format overlay to display images in the credential details.

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 13:07:49 +0000 UTC
    </div>
</div>

