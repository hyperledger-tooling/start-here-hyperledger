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
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/308" class=".btn">#308</a>
            </td>
            <td>
                <b>
                    chore(deps): update hyper requirement from 0.14 to 1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [hyper](https://github.com/hyperium/hyper) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/releases">hyper's releases</a>.</em></p>
<blockquote>
<h2>v0.14.29</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>http1:</strong> start header read timeout immediately (<a href="https://redirect.github.com/hyperium/hyper/issues/3305">#3305</a>) (<a href="https://github.com/hyperium/hyper/commit/b5c2592fde5e20d29c69428c85aef3d682ee36bc">b5c2592f</a>)</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>http2:</strong> add config for <code>max_local_error_reset_streams</code> in server (<a href="https://redirect.github.com/hyperium/hyper/issues/3528">#3528</a>) (<a href="https://github.com/hyperium/hyper/commit/dedcb674f35eaec765a42b550caabe6f694d86d1">dedcb674</a>)</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/jeromegn"><code>@​jeromegn</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/hyper/pull/3305">hyperium/hyper#3305</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperium/hyper/compare/v0.14.28...v0.14.29">https://github.com/hyperium/hyper/compare/v0.14.28...v0.14.29</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/blob/v0.14.29/CHANGELOG.md">hyper's changelog</a>.</em></p>
<blockquote>
<h3>v0.14.29 (2024-06-03)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>http1:</strong> start header read timeout immediately (<a href="https://redirect.github.com/hyperium/hyper/issues/3305">#3305</a>) (<a href="https://github.com/hyperium/hyper/commit/b5c2592fde5e20d29c69428c85aef3d682ee36bc">b5c2592f</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>http2:</strong> add config for <code>max_local_error_reset_streams</code> in server (<a href="https://redirect.github.com/hyperium/hyper/issues/3528">#3528</a>) (<a href="https://github.com/hyperium/hyper/commit/dedcb674f35eaec765a42b550caabe6f694d86d1">dedcb674</a>)</li>
</ul>
<h3>v0.14.28 (2023-12-18)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong>
<ul>
<li>panic when pool idle timeout set to zero (<a href="https://redirect.github.com/hyperium/hyper/issues/3365">#3365</a>) (<a href="https://github.com/hyperium/hyper/commit/34d38008499de37d9b5b65440b3123ccd05c7510">34d38008</a>)</li>
<li>divide by zero error when DNS returns no addrs (<a href="https://redirect.github.com/hyperium/hyper/issues/3355">#3355</a>) (<a href="https://github.com/hyperium/hyper/commit/41eaf2042b8169d3dd067d49cfdbdaaf36678903">41eaf204</a>)</li>
<li>Do not strip <code>path</code> and <code>scheme</code> components from URIs for HTTP/2 Extended CONNEC (<a href="https://github.com/hyperium/hyper/commit/45aa62494127066c63c987a57cc5eae2c5361886">45aa6249</a>)</li>
<li>early respond from server shouldn't propagate reset error (<a href="https://redirect.github.com/hyperium/hyper/issues/3274">#3274</a>) (<a href="https://github.com/hyperium/hyper/commit/aac6760e032050dd47f5dbd32f852bf1ede9312b">aac6760e</a>, closes <a href="https://redirect.github.com/hyperium/hyper/issues/2872">#2872</a>)</li>
</ul>
</li>
<li><strong>http1:</strong>
<ul>
<li>add internal limit for chunked extensions (<a href="https://redirect.github.com/hyperium/hyper/issues/3495">#3495</a>) (<a href="https://github.com/hyperium/hyper/commit/344a87822951a46d252843ccc0b48e62988fc85b">344a8782</a>)</li>
<li>reject chunked headers missing a digit (<a href="https://redirect.github.com/hyperium/hyper/issues/3494">#3494</a>) (<a href="https://github.com/hyperium/hyper/commit/5eca028f4142e3e73f6d6188a4076f4db292b252">5eca028f</a>)</li>
</ul>
</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>body:</strong> deprecate to_bytes() and aggregate() (<a href="https://redirect.github.com/hyperium/hyper/issues/3466">#3466</a>) (<a href="https://github.com/hyperium/hyper/commit/7f382ad64326e1470912feb310d348fd79099c44">7f382ad6</a>)</li>
<li><strong>client:</strong> add <code>conn::http1::Connection::without_shutdown()</code> method (<a href="https://redirect.github.com/hyperium/hyper/issues/3431">#3431</a>) (<a href="https://github.com/hyperium/hyper/commit/ad504977b520a9582e5516a08b2f1028ef1b5e45">ad504977</a>)</li>
<li><strong>server:</strong> add <code>Builder::local_addr()</code> (<a href="https://redirect.github.com/hyperium/hyper/issues/3278">#3278</a>) (<a href="https://github.com/hyperium/hyper/commit/d342c2c714498d33891fa285a3c9ae991dc34769">d342c2c7</a>)</li>
</ul>
<h3>v0.14.27 (2023-06-26)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>http1:</strong>
<ul>
<li>send error on Incoming body when connection errors (<a href="https://redirect.github.com/hyperium/hyper/issues/3256">#3256</a>) (<a href="https://github.com/hyperium/hyper/commit/b107655ff8557d001bb8e558752f5f2247381e98">b107655f</a>, closes <a href="https://redirect.github.com/hyperium/hyper/issues/3253">#3253</a>)</li>
<li>properly end chunked bodies when it was known to be empty (<a href="https://redirect.github.com/hyperium/hyper/issues/3254">#3254</a>) (<a href="https://github.com/hyperium/hyper/commit/32422c47ec35e7405873277c87de14c18dbb98bd">32422c47</a>, closes <a href="https://redirect.github.com/hyperium/hyper/issues/3252">#3252</a>)</li>
</ul>
</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>client:</strong> include connection info in <code>Client::send_request</code> errors (<a href="https://redirect.github.com/hyperium/hyper/issues/2749">#2749</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper/commit/4e61351c1c07f59f8d7b79dcb37c1384acb9f3cb"><code>4e61351</code></a> v0.14.29</li>
<li><a href="https://github.com/hyperium/hyper/commit/b5c2592fde5e20d29c69428c85aef3d682ee36bc"><code>b5c2592</code></a> fix(http1): start header read timeout immediately (<a href="https://redirect.github.com/hyperium/hyper/issues/3305">#3305</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/093665e3c318b1360df5a7338facc2b47ac5b54a"><code>093665e</code></a> refactor(lib): allow warnings in 0.14.x (<a href="https://redirect.github.com/hyperium/hyper/issues/3677">#3677</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/dedcb674f35eaec765a42b550caabe6f694d86d1"><code>dedcb67</code></a> feat(http2): add config for <code>max_local_error_reset_streams</code> in server (<a href="https://redirect.github.com/hyperium/hyper/issues/3528">#3528</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/98a7ab039461cd859e835ae4d15413489fe5cf6b"><code>98a7ab0</code></a> v0.14.28</li>
<li><a href="https://github.com/hyperium/hyper/commit/344a87822951a46d252843ccc0b48e62988fc85b"><code>344a878</code></a> fix(http1): add internal limit for chunked extensions (<a href="https://redirect.github.com/hyperium/hyper/issues/3495">#3495</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/5eca028f4142e3e73f6d6188a4076f4db292b252"><code>5eca028</code></a> fix(http1): reject chunked headers missing a digit (<a href="https://redirect.github.com/hyperium/hyper/issues/3494">#3494</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/7f382ad64326e1470912feb310d348fd79099c44"><code>7f382ad</code></a> feat(body): deprecate to_bytes() and aggregate() (<a href="https://redirect.github.com/hyperium/hyper/issues/3466">#3466</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/ad504977b520a9582e5516a08b2f1028ef1b5e45"><code>ad50497</code></a> feat(client): add <code>conn::http1::Connection::without_shutdown()</code> method (<a href="https://redirect.github.com/hyperium/hyper/issues/3431">#3431</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/48997034ed388ae7e0cb083ab1d343df312919a2"><code>4899703</code></a> chore(ci): cache rust dependency</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/hyper/compare/v0.14.0...v0.14.29">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:54:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump react-native from 0.67.2 to 0.74.3 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-native](https://github.com/facebook/react-native/tree/HEAD/packages/react-native) from 0.67.2 to 0.74.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/releases">react-native's releases</a>.</em></p>
<blockquote>
<h2>0.74.3</h2>
<h3>Added</h3>
<ul>
<li>Add the ReactMarkerConstants.CONTENT_APPEARED support on Android in bridgeless mode. (<a href="https://github.com/facebook/react-native/commit/3c4d7618f00751b08f73ffcec9ef1f69d44136da">3c4d7618f0</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Feat: update CLI to 13.6.9 (<a href="https://github.com/facebook/react-native/commit/d1e2a3506152abde9b870b1a63f16d00ec277ea6">d1e2a35061</a> by <a href="https://github.com/szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Support <code>customizeRootView</code> from <code>RCTRootViewFactory</code> (<a href="https://github.com/facebook/react-native/commit/3c4d7618f00751b08f73ffcec9ef1f69d44136da">3c4d761</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Codegen computes output path relative to project root instead of current working directory. (<a href="https://github.com/facebook/react-native/commit/d3e0430deac573fd44792e6005d5de20e9ad2797">d3e0430dea</a> by <a href="https://github.com/dmytrorykun"><code>@​dmytrorykun</code></a>)</li>
</ul>
<h3>Android specific</h3>
<ul>
<li>Android native rejections should be instanceof Error (<a href="https://github.com/facebook/react-native/commit/f4b0fcb92263667754348f82030f85cc941846ba">f4b0fcb9</a> by <a href="https://github.com/huzhanbo1996">huzhanbo1996</a>)</li>
<li>Tentative fix for NPE <code>JavaTimerManager$IdleCallbackRunnable.cancel</code> (<a href="https://github.com/facebook/react-native/commit/988bf162a0f36d9919cebbebc1fca27b58be4ae5">988bf162a0</a> by <a href="https://github.com/cortinico"><code>@​cortinico</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Fixed Multiline TextInput with a fixed height scrolls to the bottom when changing AttributedText (<a href="https://github.com/facebook/react-native/commit/e210c7c5741202a6e1b372731b50fdb59a7232bb">e210c7c5</a> by <a href="https://github.com/fabOnReact"><code>@​fabOnReact</code></a>)</li>
<li>Fixed border being drawn over children when no color was set (<a href="https://github.com/facebook/react-native/commit/a2b52af3bcc273cf85f01510c24d4e8da1b45656">a2b52af3</a> by <a href="https://github.com/j-piasecki"><code>@​j-piasecki</code></a>)</li>
</ul>
<hr />
<!-- raw HTML omitted -->
<p>Hermes dSYMS:</p>
<ul>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.3/react-native-artifacts-0.74.3-hermes-framework-dSYM-debug.tar.gz">Debug</a></li>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.3/react-native-artifacts-0.74.3-hermes-framework-dSYM-release.tar.gz">Release</a></li>
</ul>
<hr />
<p>You can file issues or pick requests against this release <a href="https://github.com/reactwg/react-native-releases/issues/new/choose">here</a>.</p>
<hr />
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/">Upgrade Helper</a> ⚛️.</p>
<hr />
<p>View the whole changelog in the <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG.md">CHANGELOG.md file</a>.</p>
<h2>0.74.2</h2>
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
<li><a href="https://github.com/facebook/react-native/commit/8e5a9360bb8dbf27f05261f11085c1972265ce15"><code>8e5a936</code></a> Release 0.74.3</li>
<li><a href="https://github.com/facebook/react-native/commit/3d53992051f698665b93a0d2747aaa75b51f3af5"><code>3d53992</code></a> fix: typo when cherry picking from kotlin to java</li>
<li><a href="https://github.com/facebook/react-native/commit/3c4d7618f00751b08f73ffcec9ef1f69d44136da"><code>3c4d761</code></a> Back out &quot;Revert D58459930: [react-native][PR] Add ReactMarkerConstants.CONTE...</li>
<li><a href="https://github.com/facebook/react-native/commit/bdf6583c7e5538648e624afd0883aaf392b7eef8"><code>bdf6583</code></a> Fix output path for generated artifacts (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/45165">#45165</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/3a1ff948399c7ff568c9f86a4616f2fed7b53616"><code>3a1ff94</code></a> [Hermes] Bump Hermes (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/45220">#45220</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/d1e2a3506152abde9b870b1a63f16d00ec277ea6"><code>d1e2a35</code></a> feat: update CLI to 13.6.9 (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44793">#44793</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/7dd6549e099d018027473760c3486c0623f2b65f"><code>7dd6549</code></a> Continue running microtasks when parent task throws</li>
<li><a href="https://github.com/facebook/react-native/commit/487c8489f1fb88b07acbcd61c223f7c3c0c32f9a"><code>487c848</code></a> Refactor: RuntimeScheduler: Delete ErrorUtils.h (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/43953">#43953</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/37b33c34baf4be78f24d3bc3d0a0910da9180827"><code>37b33c3</code></a> Small refactor in RuntimeScheduler_Modern to favor references over shared_ptr...</li>
<li><a href="https://github.com/facebook/react-native/commit/988bf162a0f36d9919cebbebc1fca27b58be4ae5"><code>988bf16</code></a> Tentative fix for NPE <code>JavaTimerManager$IdleCallbackRunnable.cancel</code> (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44852">#44852</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/react-native/commits/v0.74.3/packages/react-native">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~react-native-bot">react-native-bot</a>, a new releaser for react-native since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-native&package-manager=npm_and_yarn&previous-version=0.67.2&new-version=0.74.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 11:48:03 +0000 UTC
    </div>
</div>

