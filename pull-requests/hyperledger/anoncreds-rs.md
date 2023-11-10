---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    AnonCreds Credentials and Presentations using the W3C Verifiable Credentials Data Model Standard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * W3C credential and presentation definitions: tied to AnonCreds W3C form
* Method to convert legacy credential into W3C form
* Method to convert AnonCreds W3C credential into legacy form
* Methods to issue/process a credential in W3C form
* Methods to create/verify a presentation in W3C form
* Helper methods for W3C credential
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 08:54:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade react-native from 0.72.4 to 0.72.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to upgrade react-native from 0.72.4 to 0.72.6.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **2 versions** ahead of your current version.
- The recommended version was released **22 days ago**, on 2023-10-12.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>react-native</b></summary>
    <ul>
      <li>
        <b>0.72.6</b> - <a href="https://snyk.io/redirect/github/facebook/react-native/releases/tag/v0.72.6">2023-10-12</a></br><h3>Fixed</h3>
<ul>
<li>Fix a potential bug in <code>EventEmitter</code> when used with certain Babel configurations that incorrectly polyfill the spread operator for iterables (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/9b3bd637231e5e9e7d8b729c71842f3b7a2da373">9b3bd63723</a> by <a href="https://snyk.io/redirect/github/yungsters">@ yungsters</a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Set the max version of Active support to 7.0.8 (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/785f91b67a5d97e4e54d341279c878483a3d9a11">785f91b67a</a> by <a href="https://snyk.io/redirect/github/cipolleschi">@ cipolleschi</a>)</li>
</ul>
<hr>
<p>You can participate in the conversation on the status of this release in this <a href="https://snyk.io/redirect/github/reactwg/react-native-releases/discussions/91" data-hovercard-type="discussion" data-hovercard-url="/reactwg/react-native-releases/discussions/91/hovercard">discussion</a></p>
<hr>
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/" rel="nofollow">upgrade helper</a> ⚛️</p>
<hr>
<p>You can find the whole changelog history in the <a href="https://snyk.io/redirect/github/facebook/react-native/blob/main/CHANGELOG.md">changelog.md file</a>.</p>
      </li>
      <li>
        <b>0.72.5</b> - <a href="https://snyk.io/redirect/github/facebook/react-native/releases/tag/v0.72.5">2023-09-25</a></br>

<h3>Changed</h3>
<ul>
<li>Bump CLI to 11.3.7 (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/6f02d55debe818dcb1db753f2ca4cc0b804d0df5">6f02d55deb</a> by <a href="https://snyk.io/redirect/github/huntie">@ huntie</a>)</li>
<li>Bump @ react-native/codegen to 0.72.7 (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/4da991407da2791f22ded368ad04457b03be5ee3">4da991407d</a> by <a href="https://snyk.io/redirect/github/Titozzz">@ Titozzz</a>)</li>
</ul>
<h3>Fixed</h3>
<h4>Android specific</h4>
<ul>
<li>Fix building Android on Windows. (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/054ab62be0db5d14f02f5aeb4c696f037ea68794">054ab62be0</a> by <a href="https://snyk.io/redirect/github/alespergl">@ alespergl</a>)</li>
<li>A bug fix for Android builds with new arch on Windows host. (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/a323249e0a0f9c2fb75ee05d7da62a34f3c56be0">a323249e0a</a> by <a href="https://snyk.io/redirect/github/birdofpreyru">@ birdofpreyru</a>)</li>
<li>Fix null crash when using maintainVisibleContentPosition on Android (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/1a1a79871b2d040764537433b431bc3b416904e3">1a1a79871b</a> by <a href="https://snyk.io/redirect/github/janicduplessis">@ janicduplessis</a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>XCode 15 fixes (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/21763e85e39e17a19a1cf7a9026ef74517464749">21763e85e3</a>, <a href="https://snyk.io/redirect/github/facebook/react-native/commit/0dbd621c598e3ba7a203ec41bb70ce395ad1d62c">0dbd621c59</a> &amp; <a href="https://snyk.io/redirect/github/facebook/react-native/commit/8a5b2d673502037731ee6bc40fc64cdd22139011">8a5b2d6735</a>)</li>
<li>Fix timer background state when App is launched from background (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/a4ea737ae1773e7fd49969ae20b962bdd7481b37">a4ea737ae1</a> by <a href="https://snyk.io/redirect/github/zhongwuzw">@ zhongwuzw</a>)</li>
<li>Guard <code>JSGlobalContextSetInspectable</code> behind a compile time check for Xcode 14.3+ (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/3eeee11d7ac4075d0917233d3be4a9469f802d35">3eeee11d7a</a> by <a href="https://snyk.io/redirect/github/Saadnajmi">@ Saadnajmi</a>)</li>
<li>Re-enable direct debugging with JSC on iOS 16.4+ (<a href="https://snyk.io/redirect/github/facebook/react-native/commit/8b1bf058c4bcbf4e5ca45b0056217266a1ed870c">8b1bf058c4</a> by <a href="https://snyk.io/redirect/github/huntie">@ huntie</a>)</li>
</ul>
<hr>
<p>You can participate in the conversation on the status of this release in this <a href="https://snyk.io/redirect/github/reactwg/react-native-releases/discussions/89" data-hovercard-type="discussion" data-hovercard-url="/reactwg/react-native-releases/discussions/89/hovercard">discussion</a></p>
<hr>
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/" rel="nofollow">upgrade helper</a> ⚛️</p>
<hr>
<p>You can find the whole changelog history in the <a href="https://snyk.io/redirect/github/facebook/react-native/blob/main/CHANGELOG.md">changelog.md file</a>.</p>
      </li>
      <li>
        <b>0.72.4</b> - 2023-08-14
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
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/4fd3da2a877d5c4dc07ea26067f2eec98ac4fb19">4fd3da2</a> [0.72.6] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/6e3a130860bf5ae0fd37df0ddaaeb226cffe7312">6e3a130</a> [Local] Fix CI for 0.72, with Acitve Support and Xcode15 (#40855)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/9b3bd637231e5e9e7d8b729c71842f3b7a2da373">9b3bd63</a> RN: Switch EventEmitter to &#x60;Array.from(...)&#x60; (#39525)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/785f91b67a5d97e4e54d341279c878483a3d9a11">785f91b</a> Fix Gemfile, setting Active support to &lt; 7.1.0 (#39828)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/355025dae436ac9ec7635069042d2a9a4e24f680">355025d</a> Update Xcode 15 patches to be more robust (#39710)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/3c4cc59542762786ce4e70131a578ee7508f57e3">3c4cc59</a> Move hermes-engine.podspec and hermes-utils.rb from hermes-engine to hermes folders when building (#39575)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/1e38d4d4b15f55df721d4fb05596b957de3868e3">1e38d4d</a> [0.72.5] Bump version numbers</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/2a041cb967f734c5f8b5f77ab77980fc96a967f8">2a041cb</a> Add ld_classic flag to Hermes when building for Xcode 15 (#39516)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/8ccdb2cbe6f682163dc9e0f09987986ed003dbb3">8ccdb2c</a> Fix Xcode 15 RC issues (#39474)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/a5e110adcf21e67eeaff0d838ed18aef9a1f224d">a5e110a</a> Bump IPHONEOS_DEPLOYMENT_TARGET to 13.4 for 3rd party pods (#39478)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/f6fd6b8db009f4a919f7e698d27028bb7f07e278">f6fd6b8</a> 【iOS】Fix timer background state when App is launched from background (#39347)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/4da991407da2791f22ded368ad04457b03be5ee3">4da9914</a> bumped packages versions</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/6f02d55debe818dcb1db753f2ca4cc0b804d0df5">6f02d55</a> Bump CLI to 11.3.7 (#39280)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/a8ec20db215b40ca18c5aefdb05a19c4c75ec74f">a8ec20d</a> Allow RCTBundleURLProvider to request an inline source map (#37878) (#39033)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/f77e9af76189fd9ac74b013e29007058b7cf8662">f77e9af</a> Fix building Android on Windows (#39190)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/e9eca07f5222cb846c3069705cf48a9db9209863">e9eca07</a> Revert &quot;Fix build failure on iOS with pnpm and use_frameworks! (#38158)&quot; (#39177)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/66441e7e5d1cf52ee7d0317ab1654f7e491b40a2">66441e7</a> A fix in Codegen for Windows build host (#36542)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/05d36d986087b5ed0e582d759fd45294dcc307c8">05d36d9</a> Guard &#x60;JSGlobalContextSetInspectable&#x60; behind a compile time check for Xcode 14.3+ (#39037)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/26b49f9ff9a40900a9f48a0b2a25735cc2117b15">26b49f9</a> Adjust RawPropsPropNameLength&#x27;s type to account for increased number of props (#39008)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/7aeadbc249590688972b3968caf76f5fc80f7eda">7aeadbc</a> Fix null crash when using maintainVisibleContentPosition on Android (#38891)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/1794832a26b64ebec4e6c7878dba57d6dedd0574">1794832</a> Re-enable direct debugging with JSC on iOS 16.4+ (#37914)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/ef8ac7a3292e2ee335711927781c2fdf2f704dc3">ef8ac7a</a> chore(releases): improve bump oss script to allow less human errors (72 edition) (#38888)</li>
      <li><a href="https://snyk.io/redirect/github/facebook/react-native/commit/33fc55dc6e69f351f6152735f11e8aa46b6ad1dc">33fc55d</a> Add scripts and pipeline to poll for maven (#38980)</li>
    </ul>

   <a href="https://snyk.io/redirect/github/facebook/react-native/compare/ff27568f62c936c1e605594bc3ec178a188403f0...4fd3da2a877d5c4dc07ea26067f2eec98ac4fb19">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiJlZmJkNTExYi02Y2QxLTQ1NzQtOTMwYS04OTJkMjAzYjA3MTUiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6ImVmYmQ1MTFiLTZjZDEtNDU3NC05MzBhLTg5MmQyMDNiMDcxNSJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?pkg&#x3D;react-native&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"efbd511b-6cd1-4574-930a-892d203b0715","prPublicId":"efbd511b-6cd1-4574-930a-892d203b0715","dependencies":[{"name":"react-native","from":"0.72.4","to":"0.72.6"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"adcadd64-fca2-41e4-9476-aa9d33532df3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":2,"publishedDate":"2023-10-12T16:26:09.059Z"},"templateVariants":[],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 19:29:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade expo-status-bar from 1.6.0 to 1.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to upgrade expo-status-bar from 1.6.0 to 1.8.0.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **3 versions** ahead of your current version.
- The recommended version was released **2 months ago**, on 2023-09-15.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>expo-status-bar</b></summary>
    <ul>
      <li>
        <b>1.8.0</b> - 2023-09-15
      </li>
      <li>
        <b>1.7.1</b> - 2023-08-02
      </li>
      <li>
        <b>1.7.0</b> - 2023-07-28
      </li>
      <li>
        <b>1.6.0</b> - 2023-06-21
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/expo/expo/releases">expo-status-bar GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>expo-status-bar</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/ee2c866ba3c7fbc35ff2a3e896041cf15d3bd7c5">ee2c866</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/dbe276f86214969eac61dbda5a2b5596d5420aa0">dbe276f</a> [tools] Add publish-prod-home command (#24432)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/19a0af8df602248ddb9a6f5b761d4762adda085b">19a0af8</a> [go] Load embedded bundle and manifest in release builds (#24412)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/76d9873163267d55a07d3b4ca6e5b2fc9a298080">76d9873</a> Apple TV support 2: add TV template, fix config plugin, add CI (#24411)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/396e9f15b217cdeabc27ef3361442a9b18ea3b7c">396e9f1</a> [expo-updates][android] Make scopekey only required when getting database entity (#24466)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/ec9fe241beb15ca1bf923f9db9cab733b66549b6">ec9fe24</a> [ios][file-system] throw correct error (#24464)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/7b7829a694d0cf0e2000ae619857be0758e8c69c">7b7829a</a> [docs] Add note about Flipper RFC and point to debugging tools doc</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/46b58c59687d8381b86bf47f84ae9c3e3531e1e7">46b58c5</a> [docs] separate copy and link icons on headers/ collapsibles (#24448)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/b5b6a30f8b8679413253426fad7b2b21fbab1246">b5b6a30</a> [ios][clipboard] Increase test timeout (#24463)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/142d0b5531ef7b76208e388f74ddf43648510ad5">142d0b5</a> [notifications][Android] Remove badge manager (#24458)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/9c38e13cc4f98225a9ab2433f223fe738654dd8f">9c38e13</a> [core][Android] Add SharedRefs (#24446)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/82452ed93e12be5b45661ccd0f3f34f19fb3260f">82452ed</a> split create-expo tests out of Expo CLI tests (#24456)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/4c178d05e047784d3f1635abe51d07b5afb354e2">4c178d0</a> Move &#x60;process.env&#x60; polyfill strip to &#x60;expo/metro-config&#x60;. (#24455)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/92ddc08b26a11b987f4b39a094edc822d91c7108">92ddc08</a> Support mocking Node.js externals for client-side bundles. (#24453)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/a087816bdf1374b762fecdafd4da8caae5ea49c2">a087816</a> [dev-menu] [ENG-10036] update dev menu to make refresh more prominent (#24426)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/da565d55e432f8af13479f3d66e78610b9b9f2ad">da565d5</a> [docs] Fix FAQ about custom entry point in build migration guide (#24449)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/a000174d4c7d5d232b43211428ca6f9bb49c0199">a000174</a> [expo-device][docs] Fix broken link for app config doc (#24418)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/81dfc2fb50087c25fa70f1014003762be797715e">81dfc2f</a> [docs] Upgrade PNPM on Android workers to latest 8.7.5 (#24421)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/7c98c357c8fd70c070f7b96cdb44c9fe12cdd17e">7c98c35</a> feat(cli, router, metro, asset): add basePath support (#23911)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/6e021b288405021f8ece9507400b78a168b04b17">6e021b2</a> [core] Add native functions for UUIDv4 generation (#24199)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/59c279717b31cd7f5de168214b17183bf227d8b4">59c2797</a> [home] Fix apollo auth link spread ordering (#24435)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/52aab7ca6e6c9199d4e0714cb3d0aae2f5d4e3ce">52aab7c</a> Revert &quot;separate copy/ link icons on headers and collapsibles&quot;</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/0256b187bdeaa97c7592e6e0cf5ebeb58f283f66">0256b18</a> Revert &quot;remove round arrow from tippy to prevent opposite facing arrow when scrolled to page top&quot;</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/623daeb3e279007b48e035f807c654e2e550b198">623daeb</a> remove round arrow from tippy to prevent opposite facing arrow when scrolled to page top</li>
    </ul>

   <a href="https://snyk.io/redirect/github/expo/expo/compare/fa5ecca8251986b9f197cc14074eec0ab6dfb6db...ee2c866ba3c7fbc35ff2a3e896041cf15d3bd7c5">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiJmZDg2OTE5YS01YzMyLTRjMmYtOWVlZi01Y2Q4OTcyZDIyZjQiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6ImZkODY5MTlhLTVjMzItNGMyZi05ZWVmLTVjZDg5NzJkMjJmNCJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?pkg&#x3D;expo-status-bar&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"fd86919a-5c32-4c2f-9eef-5cd8972d22f4","prPublicId":"fd86919a-5c32-4c2f-9eef-5cd8972d22f4","dependencies":[{"name":"expo-status-bar","from":"1.6.0","to":"1.8.0"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"adcadd64-fca2-41e4-9476-aa9d33532df3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":3,"publishedDate":"2023-09-15T21:43:47.766Z"},"templateVariants":[],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 19:29:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade expo-splash-screen from 0.20.5 to 0.23.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to upgrade expo-splash-screen from 0.20.5 to 0.23.1.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **5 versions** ahead of your current version.
- The recommended version was released **2 months ago**, on 2023-09-18.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>expo-splash-screen</b></summary>
    <ul>
      <li>
        <b>0.23.1</b> - 2023-09-18
      </li>
      <li>
        <b>0.23.0</b> - 2023-09-15
      </li>
      <li>
        <b>0.22.0</b> - 2023-09-04
      </li>
      <li>
        <b>0.21.1</b> - 2023-08-02
      </li>
      <li>
        <b>0.21.0</b> - 2023-07-28
      </li>
      <li>
        <b>0.20.5</b> - 2023-07-29
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/expo/expo/releases">expo-splash-screen GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>expo-splash-screen</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/62f76105dfb436f7144440d6e6077d4ff3263842">62f7610</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/2d4e7de991c5fd68e928a6dcc1138244ca0e62f1">2d4e7de</a> router v3 public fixes (#24472)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/c9db3de737f6ca6702cee9903c7758bb96682b10">c9db3de</a> [expo-dev-menu] fix ts and linting (#24497)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/36864eca88552ba66197967b9d236a35771356a3">36864ec</a> [sqlite] fix load extension test (#24498)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/e77297bd05aa5faa37ee8fa9d799a0e64344ae81">e77297b</a> [notifications][Android] Convert almost all exported modules to Kotlin (#24462)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/c8170acce2d3cfd467be279e5beb5d1bcb116b05">c8170ac</a> [expo-contacts][docs] Fix broken link for app config doc (#24477)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/e6b55b93da2a9c8eff517214971fc7cda77b3ca5">e6b55b9</a> [docs] Add newsletter links to sidebar footer and Home page (#24482)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/eb9435b52a1c7a59eb3ececabae71d2b5ca4b16f">eb9435b</a> [notifications][Android] Remove vernsioned &#x60;ExpoBadge Manager&#x60;</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/a0708d8859c77ff334b9bc2f5e27e33d0910fce4">a0708d8</a> [notifications][Android] Fix BadgeManager not found in vendored code</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/09c2ed4acac3ef3b3a19f6179ce714668ed836bb">09c2ed4</a> [expo-intent-launcher] [Android] Fix the crash on fulfilled promises when ActivityNotFoundException is thrown (#24481)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/0685088eb2080915d5fad59bafe7a8593865a284">0685088</a> [docs] Update verbiage, fix formatting issues and vale warnings in API Routes guide (#24478)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/88cf444c9aad92f6378a45d8b32ca014d65dddae">88cf444</a> [iOS] Experimental new Video component (#24428)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/4b361cb0003654b0fbe2351ee17a032d776ca942">4b361cb</a> [android][sqlite] Add support for CRSQLite on Android (#24322)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/026e18859d13266c061bb348d5d6b1c649ca7871">026e188</a> [ios][updates] bump sqlite version (#24375)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/02196533a472a7f6e073a283fd9cf797dfa95514">0219653</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/e44650fda67f1705795dec6cf8fbb468825ea753">e44650f</a> [templates] Bump versions [skip ci]</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/aa59e54be8bf2248e0e58f38faee7e8b0efd1da2">aa59e54</a> Sync changelogs [skip ci]</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/e7d314738ddab2021957452a2d41818de874555f">e7d3147</a> [templates] Bump versions [skip ci]</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/2bd82552d004cba40601572c8f141f063150620c">2bd8255</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/ff40b4b373ce2944d1541f70969db65e3e5c1999">ff40b4b</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/0f5698e78938e67eb8c15a4e0928948c8c6a4ebf">0f5698e</a> Sync changelogs</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/489c2041c1cb62e36cc3e12e3f9de67a43b1d5b2">489c204</a> [ios] Remove legacy notifications module code (#24325)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/46f023faa11eac219c59b25dcd63be853aab7bd0">46f023f</a> [RFC] API Routes in Expo Router (#24429)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/dfc1bb8cb91ec4b34b00dc9c5bb1ebf42b7112be">dfc1bb8</a> publish project templates</li>
    </ul>

   <a href="https://snyk.io/redirect/github/expo/expo/compare/0d774d352ca6d11f83a3223199c8e5f6ba4c8e09...62f76105dfb436f7144440d6e6077d4ff3263842">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiI2YzhjNTQxZi05ZGU4LTQ3ZGQtYmZlNi0wY2YwNWU0NGYwOWMiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjZjOGM1NDFmLTlkZTgtNDdkZC1iZmU2LTBjZjA1ZTQ0ZjA5YyJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?pkg&#x3D;expo-splash-screen&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"6c8c541f-9de8-47dd-bfe6-0cf05e44f09c","prPublicId":"6c8c541f-9de8-47dd-bfe6-0cf05e44f09c","dependencies":[{"name":"expo-splash-screen","from":"0.20.5","to":"0.23.1"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"adcadd64-fca2-41e4-9476-aa9d33532df3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":5,"publishedDate":"2023-09-18T18:55:35.534Z"},"templateVariants":[],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 19:29:45 +0000 UTC
    </div>
</div>

