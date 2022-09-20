---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2033" class=".btn">#2033</a>
            </td>
            <td>
                <b>
                    [chore] merge develop to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                merge develop to main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 16:08:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2032" class=".btn">#2032</a>
            </td>
            <td>
                <b>
                    [chore] Fix DCI lint errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix DCI lint errors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 15:53:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2031" class=".btn">#2031</a>
            </td>
            <td>
                <b>
                    Bump jsdom and react-scripts in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsdom](https://github.com/jsdom/jsdom) and [react-scripts](https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts). These dependencies needed to be updated together.
Updates `jsdom` from 11.12.0 to 16.7.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jsdom/jsdom/releases">jsdom's releases</a>.</em></p>
<blockquote>
<h2>Version 16.7.0</h2>
<ul>
<li>Added <code>AbortSignal.abort()</code>. (ninevra)</li>
<li>Added dummy <code>x</code> and <code>y</code> properties to the return value of <code>getBoundingClientRect()</code>. (eiko)</li>
<li>Implemented wrapping for <code>textareaEl.value</code> if the <code>wrap=&quot;&quot;</code> attribute is specified. (ninevra)</li>
<li>Changed newline normalization in <code>&lt;textarea&gt;</code>s according to <a href="https://blog.whatwg.org/newline-normalizations-in-form-submission">recent HTML Standard updates</a>. (ninevra)</li>
<li>Fixed some bad cascade computation in <code>getComputedStyle()</code>. (romain-trotard)</li>
</ul>
<h2>Version 16.6.0</h2>
<ul>
<li>Added <code>parentNode.replaceChildren()</code>. (<a href="https://github.com/ninevra"><code>@​ninevra</code></a>)</li>
<li>Fixed jsdom's handling of when code running inside the jsdom throws <code>null</code> or <code>undefined</code> as an exception. (<a href="https://github.com/mbest"><code>@​mbest</code></a>)</li>
<li>Removed the dependency on the deprecated <a href="https://www.npmjs.com/package/request"><code>request</code></a> package, in the process fixing several issues with the <code>XMLHttpRequest</code> implementation around header processing. Thanks go to <a href="https://github.com/tobyhinloopen"><code>@​tobyhinloopen</code></a>, <a href="https://github.com/andrewaylett"><code>@​andrewaylett</code></a>, and especially <a href="https://github.com/vegardbb"><code>@​vegardbb</code></a>, for completing this months-long effort!</li>
</ul>
<h2>Version 16.5.3</h2>
<ul>
<li>Fixed infinite recursion when using <code>MutationObserver</code>s to observe elements inside a <code>MutationObserver</code> callback.</li>
</ul>
<h2>Version 16.5.2</h2>
<ul>
<li>Fixed <code>Access-Control-Allow-Headers: *</code> to work with <code>XMLHttpRequest</code>. (silviot)</li>
<li>Fixed <code>xhr.response</code> to strip any leading BOM when <code>xhr.responseType</code> is <code>&quot;json&quot;</code>.</li>
<li>Fixed <code>new Text()</code> and <code>new Comment()</code> constructors to properly set the resulting node's <code>ownerDocument</code>.</li>
<li>Fixed <code>customElements.whenDefined()</code> to resolve its returned promise with the custom element constructor, per recent spec updates. (ExE-Boss)</li>
<li>Fixed parsing to ensure that <code>&lt;svg&gt;\&lt;template&gt;&lt;/template&gt;&lt;/svg&gt;</code> does not throw an exception, but instead correctly produces a SVG-namespace <code>\&lt;template&gt;</code> element.</li>
<li>Fixed <code>domParser.parseFromString()</code> to treat <code>&lt;noscript&gt;</code> elements appropriately.</li>
<li>Fixed form control validity checking when the control was outside the <code>&lt;form&gt;</code> element and instead associated using the <code>form=&quot;&quot;</code> attribute.</li>
<li>Fixed <code>legendEl.form</code> to return the correct result based on its parent <code>&lt;fieldset&gt;</code>.</li>
<li>Fixed <code>optionEl.text</code> to exclude <code>&lt;script&gt;</code> descendants.</li>
<li>Fixed radio buttons and checkboxes to not fire <code>input</code> and <code>change</code> events when disconnected.</li>
<li>Fixed <code>inputEl.indeterminate</code> to reset to its previous value when canceling a <code>click</code> event on a checkbox or radio button.</li>
<li>Fixed the behavior of event handler attributes (e.g. <code>onclick=&quot;...code...&quot;</code>) when there were global variables named <code>element</code> or <code>formOwner</code>. (ExE-Boss)</li>
<li>On Node.js v14.6.0+ where <code>WeakRef</code>s are available, fixed <code>NodeIterator</code> to no longer stop working when more than ten <code>NodeIterator</code> instances are created, and to use less memory due to inactive <code>NodeIterator</code>s sticking around. (ExE-Boss)</li>
</ul>
<h2>Version 16.5.1</h2>
<ul>
<li>Fixed a regression that broke <code>customElements.get()</code> in v16.5.0. (fdesforges)</li>
<li>Fixed <code>window.event</code> to have a setter which overwrites the <code>window.event</code> property with the given value, per the specification. This fixes an issue where after upgrading to jsdom v16.5.0 you would no longer be able to set a global variable named <code>event</code> in the jsdom context.</li>
</ul>
<h2>Version 16.5.0</h2>
<ul>
<li>Added <code>window.queueMicrotask()</code>.</li>
<li>Added <code>window.event</code>.</li>
<li>Added <code>inputEvent.inputType</code>. (diegohaz)</li>
<li>Removed <code>ondragexit</code> from <code>Window</code> and friends, per a spec update.</li>
<li>Fixed the URL of <code>about:blank</code> iframes. Previously it was getting set to the parent's URL. (SimonMueller)</li>
<li>Fixed the loading of subresources from the filesystem when they had non-ASCII filenames.</li>
<li>Fixed the <code>hidden=&quot;&quot;</code> attribute to cause <code>display: none</code> per the user-agent stylesheet. (ph-fritsche)</li>
<li>Fixed the <code>new File()</code> constructor to no longer convert <code>/</code> to <code>:</code>, per <a href="https://github-redirect.dependabot.com/w3c/FileAPI/issues/41">a pending spec update</a>.</li>
<li>Fixed mutation observer callbacks to be called with the <code>MutationObserver</code> instance as their <code>this</code> value.</li>
<li>Fixed <code>&lt;input type=checkbox&gt;</code> and <code>&lt;input type=radio&gt;</code> to be mutable even when disabled, per <a href="https://github-redirect.dependabot.com/whatwg/html/pull/5805">a spec update</a>.</li>
<li>Fixed <code>XMLHttpRequest</code> to not fire a redundant final <code>progress</code> event if a <code>progress</code> event was previously fired with the same <code>loaded</code> value. This would usually occur with small files.</li>
<li>Fixed <code>XMLHttpRequest</code> to expose the <code>Content-Length</code> header on cross-origin responses.</li>
<li>Fixed <code>xhr.response</code> to return <code>null</code> for failures that occur during the middle of the download.</li>
<li>Fixed edge cases around passing callback functions or event handlers. (ExE-Boss)</li>
<li>Fixed edge cases around the properties of proxy-like objects such as <code>localStorage</code> or <code>dataset</code>. (ExE-Boss)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jsdom/jsdom/blob/master/Changelog.md">jsdom's changelog</a>.</em></p>
<blockquote>
<h2>16.7.0</h2>
<ul>
<li>Added <code>AbortSignal.abort()</code>. (ninevra)</li>
<li>Added dummy <code>x</code> and <code>y</code> properties to the return value of <code>getBoundingClientRect()</code>. (eiko)</li>
<li>Implemented wrapping for <code>textareaEl.value</code> if the <code>wrap=&quot;&quot;</code> attribute is specified. (ninevra)</li>
<li>Changed newline normalization in <code>&lt;textarea&gt;</code>s according to <a href="https://blog.whatwg.org/newline-normalizations-in-form-submission">recent HTML Standard updates</a>. (ninevra)</li>
<li>Fixed some bad cascade computation in <code>getComputedStyle()</code>. (romain-trotard)</li>
</ul>
<h2>16.6.0</h2>
<ul>
<li>Added <code>parentNode.replaceChildren()</code>. (ninevra)</li>
<li>Fixed jsdom's handling of when code running inside the jsdom throws <code>null</code> or <code>undefined</code> as an exception. (mbest)</li>
<li>Removed the dependency on the deprecated <a href="https://www.npmjs.com/package/request"><code>request</code></a> package, in the process fixing several issues with the <code>XMLHttpRequest</code> implementation around header processing. Special thanks to vegardbb for completing this months-long effort!</li>
</ul>
<h2>16.5.3</h2>
<ul>
<li>Fixed infinite recursion when using <code>MutationObserver</code>s to observe elements inside a <code>MutationObserver</code> callback.</li>
</ul>
<h2>16.5.2</h2>
<ul>
<li>Fixed <code>Access-Control-Allow-Headers: *</code> to work with <code>XMLHttpRequest</code>. (silviot)</li>
<li>Fixed <code>xhr.response</code> to strip any leading BOM when <code>xhr.responseType</code> is <code>&quot;json&quot;</code>.</li>
<li>Fixed <code>new Text()</code> and <code>new Comment()</code> constructors to properly set the resulting node's <code>ownerDocument</code>.</li>
<li>Fixed <code>customElements.whenDefined()</code> to resolve its returned promise with the custom element constructor, per recent spec updates. (ExE-Boss)</li>
<li>Fixed parsing to ensure that <code>&lt;svg&gt;\&lt;template&gt;&lt;/template&gt;&lt;/svg&gt;</code> does not throw an exception, but instead correctly produces a SVG-namespace <code>\&lt;template&gt;</code> element.</li>
<li>Fixed <code>domParser.parseFromString()</code> to treat <code>&lt;noscript&gt;</code> elements appropriately.</li>
<li>Fixed form control validity checking when the control was outside the <code>&lt;form&gt;</code> element and instead associated using the <code>form=&quot;&quot;</code> attribute.</li>
<li>Fixed <code>legendEl.form</code> to return the correct result based on its parent <code>&lt;fieldset&gt;</code>.</li>
<li>Fixed <code>optionEl.text</code> to exclude <code>&lt;script&gt;</code> descendants.</li>
<li>Fixed radio buttons and checkboxes to not fire <code>input</code> and <code>change</code> events when disconnected.</li>
<li>Fixed <code>inputEl.indeterminate</code> to reset to its previous value when canceling a <code>click</code> event on a checkbox or radio button.</li>
<li>Fixed the behavior of event handler attributes (e.g. <code>onclick=&quot;...code...&quot;</code>) when there were global variables named <code>element</code> or <code>formOwner</code>. (ExE-Boss)</li>
<li>On Node.js v14.6.0+ where <code>WeakRef</code>s are available, fixed <code>NodeIterator</code> to no longer stop working when more than ten <code>NodeIterator</code> instances are created, and to use less memory due to inactive <code>NodeIterator</code>s sticking around. (ExE-Boss)</li>
</ul>
<h2>16.5.1</h2>
<ul>
<li>Fixed a regression that broke <code>customElements.get()</code> in v16.5.0. (fdesforges)</li>
<li>Fixed <code>window.event</code> to have a setter which overwrites the <code>window.event</code> property with the given value, per the specification. This fixes an issue where after upgrading to jsdom v16.5.0 you would no longer be able to set a global variable named <code>event</code> in the jsdom context.</li>
</ul>
<h2>16.5.0</h2>
<ul>
<li>Added <code>window.queueMicrotask()</code>.</li>
<li>Added <code>window.event</code>.</li>
<li>Added <code>inputEvent.inputType</code>. (diegohaz)</li>
<li>Removed <code>ondragexit</code> from <code>Window</code> and friends, per a spec update.</li>
<li>Fixed the URL of <code>about:blank</code> iframes. Previously it was getting set to the parent's URL. (SimonMueller)</li>
<li>Fixed the loading of subresources from the filesystem when they had non-ASCII filenames.</li>
<li>Fixed the <code>hidden=&quot;&quot;</code> attribute to cause <code>display: none</code> per the user-agent stylesheet. (ph-fritsche)</li>
<li>Fixed the <code>new File()</code> constructor to no longer convert <code>/</code> to <code>:</code>, per <a href="https://github-redirect.dependabot.com/w3c/FileAPI/issues/41">a pending spec update</a>.</li>
<li>Fixed mutation observer callbacks to be called with the <code>MutationObserver</code> instance as their <code>this</code> value.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jsdom/jsdom/commit/1aa3cbc2eea649b91995583725610c6b98e91251"><code>1aa3cbc</code></a> Version 16.7.0</li>
<li><a href="https://github.com/jsdom/jsdom/commit/df1f5516b05915c85d2fb9a2342a94c13292d9d9"><code>df1f551</code></a> Don't run WebSocketStream tests</li>
<li><a href="https://github.com/jsdom/jsdom/commit/eb105b234207eee72cafb146281ca90d46b40db3"><code>eb105b2</code></a> Fix browser tests by enabling SharedArrayBuffer</li>
<li><a href="https://github.com/jsdom/jsdom/commit/0dedfc0532572bbcc622681d002ce68f30464df0"><code>0dedfc0</code></a> Fix some bad cascade computation in getComputedStyle()</li>
<li><a href="https://github.com/jsdom/jsdom/commit/8021a568cede2a5b1af12ea1e988184cf51daade"><code>8021a56</code></a> Fix &quot;configuation&quot; typo (<a href="https://github-redirect.dependabot.com/jsdom/jsdom/issues/3213">#3213</a>)</li>
<li><a href="https://github.com/jsdom/jsdom/commit/a7febe31bb8d3279076a95e5835ce935064d4261"><code>a7febe3</code></a> Fix typo in level2/html.js (<a href="https://github-redirect.dependabot.com/jsdom/jsdom/issues/3222">#3222</a>)</li>
<li><a href="https://github.com/jsdom/jsdom/commit/c9896c0c79be303842a4a8a311c548563dd9476f"><code>c9896c0</code></a> Return x, y properties from Element.getBoundingClientRect (<a href="https://github-redirect.dependabot.com/jsdom/jsdom/issues/3187">#3187</a>)</li>
<li><a href="https://github.com/jsdom/jsdom/commit/346ea9810ab68616254b6a18a62beb518d0eb2ce"><code>346ea98</code></a> Update web-platform tests (<a href="https://github-redirect.dependabot.com/jsdom/jsdom/issues/3203">#3203</a>)</li>
<li><a href="https://github.com/jsdom/jsdom/commit/364c77d10d260ad6fdcb9411a125920700504c6b"><code>364c77d</code></a> Bump to ws 7.4.6</li>
<li><a href="https://github.com/jsdom/jsdom/commit/93ba6a01c11c759b81900db4a07d8f219a949bf8"><code>93ba6a0</code></a> We are now on Matrix (<a href="https://github-redirect.dependabot.com/jsdom/jsdom/issues/3207">#3207</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/jsdom/jsdom/compare/11.12.0...16.7.0">compare view</a></li>
</ul>
</details>
<br />

Updates `react-scripts` from 2.1.8 to 5.0.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG-2.x.md">react-scripts's changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 and Newer Versions</h2>
<p><strong>Please refer to <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG.md">CHANGELOG.md</a> for the newer versions.</strong></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/create-react-app/commit/19fa58d527ae74f2b6baa0867463eea1d290f9a5"><code>19fa58d</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/9802941ff049a28da2682801bc182a29761b71f4"><code>9802941</code></a> fix: webpack noise printed only if error or warning (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12245">#12245</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/2eef1d0a1db2e84cdcd6e7ca941c85a48cc7cc65"><code>2eef1d0</code></a> Update templates to use React 18 <code>createRoot</code> (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12220">#12220</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/221e511730ca51c036c6954a9d2ee7659ff860f9"><code>221e511</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/5614c87bfbaae0ce52ac15aedd2cd0f91ffd420d"><code>5614c87</code></a> Add support for Tailwind (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11717">#11717</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/20edab4894b301f6b90dad0f90a2f82c52a7ac66"><code>20edab4</code></a> fix(webpackDevServer): disable overlay for warnings (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11413">#11413</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/3afbbc0ab922fb982bb275ccb3fe5beecdf5f889"><code>3afbbc0</code></a> Update all dependencies (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11624">#11624</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/f5467d5e77d51a3f23dd5fa70697dbab79832489"><code>f5467d5</code></a> feat(eslint-config-react-app): support ESLint 8.x (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11375">#11375</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/c7627ce96c4674f327081f101dd0e2771be4d045"><code>c7627ce</code></a> Update webpack and dev server (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11646">#11646</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/544befeb536a89b0ff95792df70bb037b17f55b9"><code>544befe</code></a> Update package.json (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11597">#11597</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/create-react-app/commits/react-scripts@5.0.1/packages/react-scripts">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 11:49:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2030" class=".btn">#2030</a>
            </td>
            <td>
                <b>
                    Bump shell-quote and react-scripts in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/substack/node-shell-quote) and [react-scripts](https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts). These dependencies needed to be updated together.
Updates `shell-quote` from 1.6.1 to 1.7.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/substack/node-shell-quote/releases">shell-quote's releases</a>.</em></p>
<blockquote>
<h2>v1.7.2</h2>
<ul>
<li>Fix a regression introduced in 1.6.3. This reverts the Windows path quoting fix. (<a href="https://github.com/substack/node-shell-quote/commit/144e1c20cd57549a414c827fb3032e60b7b8721c">144e1c2</a>)</li>
</ul>
<h2>v1.7.1</h2>
<ul>
<li>Fix <code>$</code> being removed when not part of an environment variable name. (<a href="https://github.com/Admin"><code>@​Adman</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/32">#32</a>)</li>
</ul>
<h2>v1.7.0</h2>
<ul>
<li>Add support for parsing <code>&gt;&gt;</code> and <code>&gt;&amp;</code> redirection operators. (<a href="https://github.com/forivall"><code>@​forivall</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/16">#16</a>)</li>
<li>Add support for parsing <code>&lt;(</code> process substitution operator. (<a href="https://github.com/cuonglm"><code>@​cuonglm</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/15">#15</a>)</li>
</ul>
<h2>v1.6.3</h2>
<ul>
<li>Fix Windows path quoting problems. (<a href="https://github.com/dy"><code>@​dy</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/34">#34</a>)</li>
</ul>
<h2>v1.6.2</h2>
<ul>
<li>Remove dependencies in favour of native methods. (<a href="https://github.com/zertosh"><code>@​zertosh</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/21">#21</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/substack/node-shell-quote/blob/master/CHANGELOG.md">shell-quote's changelog</a>.</em></p>
<blockquote>
<h2>1.7.3</h2>
<ul>
<li>Fix a security issue where the regex for windows drive letters allowed some shell meta-characters
to escape the quoting rules. (CVE-2021-42740)</li>
</ul>
<h2>1.7.2</h2>
<ul>
<li>Fix a regression introduced in 1.6.3. This reverts the Windows path quoting fix. (<a href="https://github.com/substack/node-shell-quote/commit/144e1c20cd57549a414c827fb3032e60b7b8721c">144e1c2</a>)</li>
</ul>
<h2>1.7.1</h2>
<ul>
<li>Fix <code>$</code> being removed when not part of an environment variable name. (<a href="https://github.com/Admin"><code>@​Adman</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/32">#32</a>)</li>
</ul>
<h2>1.7.0</h2>
<ul>
<li>Add support for parsing <code>&gt;&gt;</code> and <code>&gt;&amp;</code> redirection operators. (<a href="https://github.com/forivall"><code>@​forivall</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/16">#16</a>)</li>
<li>Add support for parsing <code>&lt;(</code> process substitution operator. (<a href="https://github.com/cuonglm"><code>@​cuonglm</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/15">#15</a>)</li>
</ul>
<h2>1.6.3</h2>
<ul>
<li>Fix Windows path quoting problems. (<a href="https://github.com/dy"><code>@​dy</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/34">#34</a>)</li>
</ul>
<h2>1.6.2</h2>
<ul>
<li>Remove dependencies in favour of native methods. (<a href="https://github.com/zertosh"><code>@​zertosh</code></a> in <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/pull/21">#21</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/node-shell-quote/commit/6a8a899c62a58a30fb128a7079f02826ed4faee0"><code>6a8a899</code></a> 1.7.3</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/5799416ed454aa4ec9afafc895b4e31760ea1abe"><code>5799416</code></a> fix for security issue with windows drive letter regex</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/c7de931fa4ed0975ea9756983c88334fe4b8cde5"><code>c7de931</code></a> Add security.md</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/414853f1fd98553368ce7507cd26ebae88d71b46"><code>414853f</code></a> Update readme.markdown (<a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/43">#43</a>)</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/0fc4a978131ab68cace9c9a57cee245b6b70e595"><code>0fc4a97</code></a> use Github Actions (<a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/42">#42</a>)</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/89a1993809eb7620ec985c3b6869c9079287c35a"><code>89a1993</code></a> 1.7.2</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/df7e4c7449c3fe1e8960dd345e1a9fd02cad7e44"><code>df7e4c7</code></a> add test for <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/37">#37</a></li>
<li><a href="https://github.com/substack/node-shell-quote/commit/144e1c20cd57549a414c827fb3032e60b7b8721c"><code>144e1c2</code></a> revert windows path unescaping, fixes <a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/37">#37</a></li>
<li><a href="https://github.com/substack/node-shell-quote/commit/c24f3aa665a1d9b61b43d63c743624deb165a0c7"><code>c24f3aa</code></a> ci: nvs does not have iojs</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/c2950fba942da2d2e17a8fb5a4eaf8f8c72d1ab3"><code>c2950fb</code></a> 1.7.1</li>
<li>Additional commits viewable in <a href="https://github.com/substack/node-shell-quote/compare/1.6.1...1.7.3">compare view</a></li>
</ul>
</details>
<br />

Updates `react-scripts` from 2.1.8 to 5.0.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG-2.x.md">react-scripts's changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 and Newer Versions</h2>
<p><strong>Please refer to <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG.md">CHANGELOG.md</a> for the newer versions.</strong></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/create-react-app/commit/19fa58d527ae74f2b6baa0867463eea1d290f9a5"><code>19fa58d</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/9802941ff049a28da2682801bc182a29761b71f4"><code>9802941</code></a> fix: webpack noise printed only if error or warning (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12245">#12245</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/2eef1d0a1db2e84cdcd6e7ca941c85a48cc7cc65"><code>2eef1d0</code></a> Update templates to use React 18 <code>createRoot</code> (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12220">#12220</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/221e511730ca51c036c6954a9d2ee7659ff860f9"><code>221e511</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/5614c87bfbaae0ce52ac15aedd2cd0f91ffd420d"><code>5614c87</code></a> Add support for Tailwind (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11717">#11717</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/20edab4894b301f6b90dad0f90a2f82c52a7ac66"><code>20edab4</code></a> fix(webpackDevServer): disable overlay for warnings (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11413">#11413</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/3afbbc0ab922fb982bb275ccb3fe5beecdf5f889"><code>3afbbc0</code></a> Update all dependencies (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11624">#11624</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/f5467d5e77d51a3f23dd5fa70697dbab79832489"><code>f5467d5</code></a> feat(eslint-config-react-app): support ESLint 8.x (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11375">#11375</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/c7627ce96c4674f327081f101dd0e2771be4d045"><code>c7627ce</code></a> Update webpack and dev server (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11646">#11646</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/544befeb536a89b0ff95792df70bb037b17f55b9"><code>544befe</code></a> Update package.json (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11597">#11597</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/create-react-app/commits/react-scripts@5.0.1/packages/react-scripts">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 11:48:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2029" class=".btn">#2029</a>
            </td>
            <td>
                <b>
                    Bump terser and react-scripts in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) and [react-scripts](https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts). These dependencies needed to be updated together.
Updates `terser` from 3.17.0 to 5.15.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v5.15.0</h2>
<ul>
<li>Basic support for ES2022 class static initializer blocks.</li>
<li>Add <code>AudioWorkletNode</code> constructor options to domprops list (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1230">#1230</a>)</li>
<li>Make identity function inliner not inline <code>id(...expandedArgs)</code></li>
</ul>
<h2>v5.14.2</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
<li>Source maps improvements (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1211">#1211</a>)</li>
<li>Performance improvements in long property access evaluation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1213">#1213</a>)</li>
</ul>
<h2>v5.14.1</h2>
<ul>
<li>keep_numbers option added to TypeScript defs (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1208">#1208</a>)</li>
<li>Fixed parsing of nested template strings (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1204">#1204</a>)</li>
</ul>
<h2>v5.14.0</h2>
<ul>
<li>Switched to <code>@​jridgewell/source-map</code> for sourcemap generation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1190">#1190</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1181">#1181</a>)</li>
<li>Fixed source maps with non-terminated segments (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1106">#1106</a>)</li>
<li>Enabled typescript types to be imported from the package (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1194">#1194</a>)</li>
<li>Extra DOM props have been added (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1191">#1191</a>)</li>
<li>Delete the AST while generating code, as a means to save RAM</li>
</ul>
<h2>v5.13.1</h2>
<ul>
<li>Removed self-assignments (<code>varname=varname</code>) (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1081">#1081</a>)</li>
<li>Separated inlining code (for inlining things into references, or removing IIFEs)</li>
<li>Allow multiple identifiers with the same name in <code>var</code> destructuring (eg <code>var { a, a } = x</code>) (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1176">#1176</a>)</li>
</ul>
<h2>v5.13.0</h2>
<ul>
<li>All calls to eval() were removed (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1171">#1171</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1184">#1184</a>)</li>
<li><code>source-map</code> was updated to 0.8.0-beta.0 (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1164">#1164</a>)</li>
<li>NavigatorUAData was added to domprops to avoid property mangling (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1166">#1166</a>)</li>
</ul>
<h2>v5.12.1</h2>
<ul>
<li>Fixed an issue with function definitions inside blocks (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1155">#1155</a>)</li>
<li>Fixed parens of <code>new</code> in some situations (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1159">#1159</a>)</li>
</ul>
<h2>v5.12.0</h2>
<ul>
<li><code>TERSER_DEBUG_DIR</code> environment variable</li>
<li><a href="https://github.com/copyright"><code>@​copyright</code></a> comments are now preserved with the comments=&quot;some&quot; option (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1153">#1153</a>)</li>
</ul>
<h2>v5.11.0</h2>
<ul>
<li>Unicode code point escapes (<code>\u{abcde}</code>) are not emitted inside RegExp literals anymore (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1147">#1147</a>)</li>
<li>acorn is now a regular dependency</li>
</ul>
<h2>v5.10.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/terser/terser/commit/13fe8ca67a3bee4bdec317aeab28728589c36505"><code>13fe8ca</code></a> 5.15.0</li>
<li><a href="https://github.com/terser/terser/commit/d397f55e49ab310d081b33b127887c711bbebbc8"><code>d397f55</code></a> update changelog</li>
<li><a href="https://github.com/terser/terser/commit/c677e285261a0f115409a42015bd3664c8416534"><code>c677e28</code></a> basic support for class static blocks. Closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1093">#1093</a></li>
<li><a href="https://github.com/terser/terser/commit/5ca7d868482a0bf4cac778ce970e7b817be09f38"><code>5ca7d86</code></a> fix (domprops): add AudioWorkletNode params to the domprops list (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1230">#1230</a>)</li>
<li><a href="https://github.com/terser/terser/commit/ea5dcc3e712cb3805160d69ba37d20f48891cca5"><code>ea5dcc3</code></a> avoid inlining <code>identityFn(...expandedArgs)</code>. closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1226">#1226</a></li>
<li><a href="https://github.com/terser/terser/commit/0136e8a05ef864666a6e95b0de8b679b0bc93338"><code>0136e8a</code></a> update changelog</li>
<li><a href="https://github.com/terser/terser/commit/c5cb19de2baafa1db60b1e8c387d9d995844f7ef"><code>c5cb19d</code></a> 5.14.2</li>
<li><a href="https://github.com/terser/terser/commit/a4da7349fdc92c05094f41d33d06d8cd4e90e76b"><code>a4da734</code></a> fix potential regexp DDOS</li>
<li><a href="https://github.com/terser/terser/commit/839b81b24d04f217e8c454990c8b1de7e5e68b6b"><code>839b81b</code></a> Add source mapping for closing <code>}</code> (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1211">#1211</a>)</li>
<li><a href="https://github.com/terser/terser/commit/645a092323fad50d2fc4c1c6b49ce1db0d9eeb4f"><code>645a092</code></a> Optimize property access evaluation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1213">#1213</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/terser/terser/compare/v3.17.0...v5.15.0">compare view</a></li>
</ul>
</details>
<br />

Updates `react-scripts` from 2.1.8 to 5.0.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG-2.x.md">react-scripts's changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 and Newer Versions</h2>
<p><strong>Please refer to <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG.md">CHANGELOG.md</a> for the newer versions.</strong></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/create-react-app/commit/19fa58d527ae74f2b6baa0867463eea1d290f9a5"><code>19fa58d</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/9802941ff049a28da2682801bc182a29761b71f4"><code>9802941</code></a> fix: webpack noise printed only if error or warning (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12245">#12245</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/2eef1d0a1db2e84cdcd6e7ca941c85a48cc7cc65"><code>2eef1d0</code></a> Update templates to use React 18 <code>createRoot</code> (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12220">#12220</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/221e511730ca51c036c6954a9d2ee7659ff860f9"><code>221e511</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/5614c87bfbaae0ce52ac15aedd2cd0f91ffd420d"><code>5614c87</code></a> Add support for Tailwind (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11717">#11717</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/20edab4894b301f6b90dad0f90a2f82c52a7ac66"><code>20edab4</code></a> fix(webpackDevServer): disable overlay for warnings (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11413">#11413</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/3afbbc0ab922fb982bb275ccb3fe5beecdf5f889"><code>3afbbc0</code></a> Update all dependencies (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11624">#11624</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/f5467d5e77d51a3f23dd5fa70697dbab79832489"><code>f5467d5</code></a> feat(eslint-config-react-app): support ESLint 8.x (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11375">#11375</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/c7627ce96c4674f327081f101dd0e2771be4d045"><code>c7627ce</code></a> Update webpack and dev server (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11646">#11646</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/544befeb536a89b0ff95792df70bb037b17f55b9"><code>544befe</code></a> Update package.json (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11597">#11597</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/create-react-app/commits/react-scripts@5.0.1/packages/react-scripts">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 11:48:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2028" class=".btn">#2028</a>
            </td>
            <td>
                <b>
                    Bump got and web3 in /examples/supplychain-app/quorum/smartContracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) and [web3](https://github.com/ethereum/web3.js). These dependencies needed to be updated together.
Updates `got` from 7.1.0 to 12.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v12.1.0</h2>
<h3>Improvements</h3>
<ul>
<li>Add <code>response.ok</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2043">#2043</a>)  22d58fb
<ul>
<li>This is only useful if you have <a href="https://github.com/sindresorhus/got/blob/main/documentation/2-options.md#throwhttperrors"><code>{throwHttpErrors: false}</code></a></li>
</ul>
</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>Do not redirect to UNIX sockets (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2047">#2047</a>)  861ccd9
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2022-33987">CVE-2022-33987</a></li>
<li><a href="https://github.com/sindresorhus/got/releases/tag/v11.8.5">Also back ported to v11</a></li>
</ul>
</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.4...v12.1.0">https://github.com/sindresorhus/got/compare/v12.0.4...v12.1.0</a></p>
<h2>v12.0.4</h2>
<ul>
<li>Remove stream lock - unreliable since Node 17.3.0 bb8eca924c338ca12d5b90d6a26aa28dbddb42ee</li>
</ul>
<h2>v12.0.3</h2>
<ul>
<li>Allow more types in the <code>json</code> option (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2015">#2015</a>)  eb045bf</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.2...v12.0.3">https://github.com/sindresorhus/got/compare/v12.0.2...v12.0.3</a></p>
<h2>v12.0.2</h2>
<ul>
<li>Fix <code>encoding</code> option with <code>{responseType: 'json'}</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1996">#1996</a>)  0703318</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.1...v12.0.2">https://github.com/sindresorhus/got/compare/v12.0.1...v12.0.2</a></p>
<h2>v12.0.1</h2>
<ul>
<li>Fix <code>nock</code> compatibility (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1959">#1959</a>)  bf39d2c</li>
<li>Fix missing export of <code>Request</code> TypeScript type (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1940">#1940</a>)  0f9f2b8</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.0...v12.0.1">https://github.com/sindresorhus/got/compare/v12.0.0...v12.0.1</a></p>
<h2>v12.0.0</h2>
<h3>Introducing Got v12.0.0 :tada:</h3>
<p>Long time no see! The latest Got version (v11.8.2) was released just in February ❄️
We have been working hard on squashing bugs and improving overall experience.</p>
<p>If you find Got useful, you might want to <a href="https://github.com/sindresorhus/got?sponsor=1">sponsor the Got maintainers</a>.</p>
<h3>This package is now pure ESM</h3>
<p><strong>Please <a href="https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c">read this</a>.</strong> Also see <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1789">sindresorhus/got#1789</a>.</p>
<ul>
<li><strong>Please don't open issues about <code>[ERR_REQUIRE_ESM]</code> and <code>Must use import to load ES Module</code> errors.</strong> This is a problem with your setup, not Got.</li>
<li>Please don't open issues about using Got with Jest. Jest does not fully support ESM.</li>
<li>Pretty much any problem with loading this package is a problem with your bundler, test framework, etc, not Got.</li>
<li>If you use TypeScript, you will want to stay on Got v11 until TypeScript 4.6 is out. <a href="https://github-redirect.dependabot.com/microsoft/TypeScript/issues/46452">Why.</a></li>
<li>If you use a bundler, make sure it supports ESM and that you have correctly configured it for ESM.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/ad92afa2eb8d51d46f98491c5ac58b9071fdd67e"><code>ad92afa</code></a> 12.1.0</li>
<li><a href="https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc"><code>861ccd9</code></a> Disable redirects to UNIX sockets (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2047">#2047</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/4cdcca382659050e1c73c7eb9542c8fb871d10aa"><code>4cdcca3</code></a> Check error instance for arguments test (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2044">#2044</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/22d58fb43aece59b3bc571c46f7eda7271f8e083"><code>22d58fb</code></a> Add <code>response.ok</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2043">#2043</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/c25af092bf792c2c7e29db848a569f2eb3e527f8"><code>c25af09</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/62455f5caf269218ab7510d9dda98328ea5a5e84"><code>62455f5</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/6f5c7ce1233c7a28fed12d64766fa19e8eb3b345"><code>6f5c7ce</code></a> Test Node.js 18</li>
<li><a href="https://github.com/sindresorhus/got/commit/c693422bcc40bb35d8f51fc6b4bf97cc71913896"><code>c693422</code></a> 12.0.4</li>
<li><a href="https://github.com/sindresorhus/got/commit/98ca6181a0390450b1e29c277d4670634695ce85"><code>98ca618</code></a> Fix accidental test deletion</li>
<li><a href="https://github.com/sindresorhus/got/commit/bb8eca924c338ca12d5b90d6a26aa28dbddb42ee"><code>bb8eca9</code></a> Remove stream lock - unreliable since Node 17.3.0</li>
<li>Additional commits viewable in <a href="https://github.com/sindresorhus/got/compare/v7.1.0...v12.1.0">compare view</a></li>
</ul>
</details>
<br />

Updates `web3` from 1.7.0 to 1.8.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/web3.js/releases">web3's releases</a>.</em></p>
<blockquote>
<h2>web3-eth@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-eth@4.0.0-alpha.0</code></p>
<h2>web3-core-requestmanager@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-core-requestmanager@4.0.0-alpha.0</code></p>
<h2>web3-providers-http@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-providers-http@4.0.0-alpha.0</code></p>
<h2>web3-providers-base@1.0.0-alpha.1</h2>
<h3>Changed</h3>
<ul>
<li>Update version to <code>1.0.0-alpha.1</code> for <code>web3-providers-base</code></li>
<li>Update version to <code>4.0.0-alpha.0</code> for <code>web3-utils</code> in <code>web3-providers-base</code></li>
</ul>
<h2>web3-utils@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-utils@4.0.0-alpha.0</code></p>
<h2>web3-packagetemplate@1.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-packagetemplate@1.0.0-alpha.0</code></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/1.x/CHANGELOG.md">web3's changelog</a>.</em></p>
<blockquote>
<h2>[1.7.0]</h2>
<h3>Added</h3>
<ul>
<li><code>maxPriorityFeePerGas</code> and <code>maxFeePerGas</code> added to <code>Transaction</code> and <code>TransactionConfig</code> interfaces (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4232">#4232</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4585">#4585</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix readthedoc's build for web3js documentation (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4425">#4425</a>)</li>
<li>Fix response sorting for batch requests (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4250">#4250</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Changed getFeeHistory first parameter type from <code>number</code> to <code>hex</code> according to the <a href="https://playground.open-rpc.org/?schemaUrl=https://raw.githubusercontent.com/ethereum/eth1.0-apis/assembled-spec/openrpc.json&amp;uiSchema%5BappBar%5D%5Bui:splitView%5D=false&amp;uiSchema%5BappBar%5D%5Bui:input%5D=false&amp;uiSchema%5BappBar%5D%5Bui:examplesDropdown%5D=false">spec</a> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4529">#4529</a>)</li>
</ul>
<h2>[1.7.1]</h2>
<h3>Added</h3>
<ul>
<li><code>transactionPollingInterval</code> added to web3, contract and method constructor options. defaults to 1 second. (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4584">#4584</a>)</li>
<li>Add example import for package level types (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4611">#4611</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix a typo in the documentation for <code>methods.myMethod.send</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4599">#4599</a>)</li>
<li>Use globalThis to locate global object if possible (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4613">#4613</a>)</li>
<li>Fix typos in web3-utils.rst (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4662">#4662</a>)</li>
<li>Added effectiveGasPrice to TransactionReceipt (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4692">#4692</a>)</li>
<li>Correction in documentation for <code>web3.eth.accounts.signTransaction</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4576">#4576</a>)</li>
<li>Updated README to include Webpack 5 create-react-app support instructions (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4173">#4173</a>)</li>
<li>Update the documentation for <code>methods.myMethod.estimateGas</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4702">#4702</a>)</li>
<li>Fix typos in REVIEW.md and TESTING.md (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4691">#4691</a>)</li>
<li>Fix encoding for &quot;0x&quot; string values (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4512">#4512</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Muted E2E gnosis dex tests in CI until fix for issue <a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4436">#4436</a> is applied (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4701">#4701</a>)</li>
</ul>
<h3>Removed</h3>
<ul>
<li>Removed deprecated Morden testnet code (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4339">#4339</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li>Ran <code>npm audit fix</code> to address vulnerabilities and update libraries (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4719">#4719</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4728">#4728</a>)</li>
</ul>
<h2>[1.7.2]</h2>
<h3>Changed</h3>
<ul>
<li>Remove deprecated <code>close</code> event listener (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4825">#4825</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4839">#4839</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li><code>npm audit fix</code> to update libraries (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4860">#4860</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/59b657b8c02af05575dc2d0ed321fa7d3aa8eaf6"><code>59b657b</code></a> Build for 1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/e69ea861628f5bf17ed55d16051342644488b46e"><code>e69ea86</code></a> v1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/09634f9ca4e5be7237fa968057bc60e657338f54"><code>09634f9</code></a> Manual build commit for 1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/81b06c91b674e85d0dbe762fac22b9355e7a030a"><code>81b06c9</code></a> v1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/a158594452cba79ae7c154b6f920715a938a6195"><code>a158594</code></a> npm i and CHANGELOG update for 1.8.0 release</li>
<li><a href="https://github.com/web3/web3.js/commit/f616e9f75b375ef5defdbb0ce44f11b9d14e1592"><code>f616e9f</code></a> docs: Fix example of tx usage (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5402">#5402</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/1052540c3667b3cd009d842eba7db910970f11f5"><code>1052540</code></a> Adding Twitter button (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5415">#5415</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/6311abe8cedd70a2863edee8adc381eb63515da4"><code>6311abe</code></a> Merge block tags support 5199 (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5410">#5410</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/bd99127301ca2d427780125ecbfaabb38a4b53a0"><code>bd99127</code></a> 4.x info messages in 1.x (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5412">#5412</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a6ebb2ac9bd7cb45d4a3385fd7a760e1778292e6"><code>a6ebb2a</code></a> Nikos/5071/investigate signtransaction testcases (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5377">#5377</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/web3.js/compare/v1.7.0...v1.8.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jdevcs">jdevcs</a>, a new releaser for web3 since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 11:43:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2027" class=".btn">#2027</a>
            </td>
            <td>
                <b>
                    Bump got and web3 in /examples/supplychain-app/quorum/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) and [web3](https://github.com/ethereum/web3.js). These dependencies needed to be updated together.
Updates `got` from 7.1.0 to 12.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v12.1.0</h2>
<h3>Improvements</h3>
<ul>
<li>Add <code>response.ok</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2043">#2043</a>)  22d58fb
<ul>
<li>This is only useful if you have <a href="https://github.com/sindresorhus/got/blob/main/documentation/2-options.md#throwhttperrors"><code>{throwHttpErrors: false}</code></a></li>
</ul>
</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>Do not redirect to UNIX sockets (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2047">#2047</a>)  861ccd9
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2022-33987">CVE-2022-33987</a></li>
<li><a href="https://github.com/sindresorhus/got/releases/tag/v11.8.5">Also back ported to v11</a></li>
</ul>
</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.4...v12.1.0">https://github.com/sindresorhus/got/compare/v12.0.4...v12.1.0</a></p>
<h2>v12.0.4</h2>
<ul>
<li>Remove stream lock - unreliable since Node 17.3.0 bb8eca924c338ca12d5b90d6a26aa28dbddb42ee</li>
</ul>
<h2>v12.0.3</h2>
<ul>
<li>Allow more types in the <code>json</code> option (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2015">#2015</a>)  eb045bf</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.2...v12.0.3">https://github.com/sindresorhus/got/compare/v12.0.2...v12.0.3</a></p>
<h2>v12.0.2</h2>
<ul>
<li>Fix <code>encoding</code> option with <code>{responseType: 'json'}</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1996">#1996</a>)  0703318</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.1...v12.0.2">https://github.com/sindresorhus/got/compare/v12.0.1...v12.0.2</a></p>
<h2>v12.0.1</h2>
<ul>
<li>Fix <code>nock</code> compatibility (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1959">#1959</a>)  bf39d2c</li>
<li>Fix missing export of <code>Request</code> TypeScript type (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1940">#1940</a>)  0f9f2b8</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.0...v12.0.1">https://github.com/sindresorhus/got/compare/v12.0.0...v12.0.1</a></p>
<h2>v12.0.0</h2>
<h3>Introducing Got v12.0.0 :tada:</h3>
<p>Long time no see! The latest Got version (v11.8.2) was released just in February ❄️
We have been working hard on squashing bugs and improving overall experience.</p>
<p>If you find Got useful, you might want to <a href="https://github.com/sindresorhus/got?sponsor=1">sponsor the Got maintainers</a>.</p>
<h3>This package is now pure ESM</h3>
<p><strong>Please <a href="https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c">read this</a>.</strong> Also see <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1789">sindresorhus/got#1789</a>.</p>
<ul>
<li><strong>Please don't open issues about <code>[ERR_REQUIRE_ESM]</code> and <code>Must use import to load ES Module</code> errors.</strong> This is a problem with your setup, not Got.</li>
<li>Please don't open issues about using Got with Jest. Jest does not fully support ESM.</li>
<li>Pretty much any problem with loading this package is a problem with your bundler, test framework, etc, not Got.</li>
<li>If you use TypeScript, you will want to stay on Got v11 until TypeScript 4.6 is out. <a href="https://github-redirect.dependabot.com/microsoft/TypeScript/issues/46452">Why.</a></li>
<li>If you use a bundler, make sure it supports ESM and that you have correctly configured it for ESM.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/ad92afa2eb8d51d46f98491c5ac58b9071fdd67e"><code>ad92afa</code></a> 12.1.0</li>
<li><a href="https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc"><code>861ccd9</code></a> Disable redirects to UNIX sockets (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2047">#2047</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/4cdcca382659050e1c73c7eb9542c8fb871d10aa"><code>4cdcca3</code></a> Check error instance for arguments test (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2044">#2044</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/22d58fb43aece59b3bc571c46f7eda7271f8e083"><code>22d58fb</code></a> Add <code>response.ok</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2043">#2043</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/c25af092bf792c2c7e29db848a569f2eb3e527f8"><code>c25af09</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/62455f5caf269218ab7510d9dda98328ea5a5e84"><code>62455f5</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/6f5c7ce1233c7a28fed12d64766fa19e8eb3b345"><code>6f5c7ce</code></a> Test Node.js 18</li>
<li><a href="https://github.com/sindresorhus/got/commit/c693422bcc40bb35d8f51fc6b4bf97cc71913896"><code>c693422</code></a> 12.0.4</li>
<li><a href="https://github.com/sindresorhus/got/commit/98ca6181a0390450b1e29c277d4670634695ce85"><code>98ca618</code></a> Fix accidental test deletion</li>
<li><a href="https://github.com/sindresorhus/got/commit/bb8eca924c338ca12d5b90d6a26aa28dbddb42ee"><code>bb8eca9</code></a> Remove stream lock - unreliable since Node 17.3.0</li>
<li>Additional commits viewable in <a href="https://github.com/sindresorhus/got/compare/v7.1.0...v12.1.0">compare view</a></li>
</ul>
</details>
<br />

Updates `web3` from 1.7.0 to 1.8.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/web3.js/releases">web3's releases</a>.</em></p>
<blockquote>
<h2>web3-eth@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-eth@4.0.0-alpha.0</code></p>
<h2>web3-core-requestmanager@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-core-requestmanager@4.0.0-alpha.0</code></p>
<h2>web3-providers-http@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-providers-http@4.0.0-alpha.0</code></p>
<h2>web3-providers-base@1.0.0-alpha.1</h2>
<h3>Changed</h3>
<ul>
<li>Update version to <code>1.0.0-alpha.1</code> for <code>web3-providers-base</code></li>
<li>Update version to <code>4.0.0-alpha.0</code> for <code>web3-utils</code> in <code>web3-providers-base</code></li>
</ul>
<h2>web3-utils@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-utils@4.0.0-alpha.0</code></p>
<h2>web3-packagetemplate@1.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-packagetemplate@1.0.0-alpha.0</code></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/1.x/CHANGELOG.md">web3's changelog</a>.</em></p>
<blockquote>
<h2>[1.7.0]</h2>
<h3>Added</h3>
<ul>
<li><code>maxPriorityFeePerGas</code> and <code>maxFeePerGas</code> added to <code>Transaction</code> and <code>TransactionConfig</code> interfaces (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4232">#4232</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4585">#4585</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix readthedoc's build for web3js documentation (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4425">#4425</a>)</li>
<li>Fix response sorting for batch requests (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4250">#4250</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Changed getFeeHistory first parameter type from <code>number</code> to <code>hex</code> according to the <a href="https://playground.open-rpc.org/?schemaUrl=https://raw.githubusercontent.com/ethereum/eth1.0-apis/assembled-spec/openrpc.json&amp;uiSchema%5BappBar%5D%5Bui:splitView%5D=false&amp;uiSchema%5BappBar%5D%5Bui:input%5D=false&amp;uiSchema%5BappBar%5D%5Bui:examplesDropdown%5D=false">spec</a> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4529">#4529</a>)</li>
</ul>
<h2>[1.7.1]</h2>
<h3>Added</h3>
<ul>
<li><code>transactionPollingInterval</code> added to web3, contract and method constructor options. defaults to 1 second. (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4584">#4584</a>)</li>
<li>Add example import for package level types (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4611">#4611</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix a typo in the documentation for <code>methods.myMethod.send</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4599">#4599</a>)</li>
<li>Use globalThis to locate global object if possible (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4613">#4613</a>)</li>
<li>Fix typos in web3-utils.rst (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4662">#4662</a>)</li>
<li>Added effectiveGasPrice to TransactionReceipt (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4692">#4692</a>)</li>
<li>Correction in documentation for <code>web3.eth.accounts.signTransaction</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4576">#4576</a>)</li>
<li>Updated README to include Webpack 5 create-react-app support instructions (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4173">#4173</a>)</li>
<li>Update the documentation for <code>methods.myMethod.estimateGas</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4702">#4702</a>)</li>
<li>Fix typos in REVIEW.md and TESTING.md (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4691">#4691</a>)</li>
<li>Fix encoding for &quot;0x&quot; string values (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4512">#4512</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Muted E2E gnosis dex tests in CI until fix for issue <a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4436">#4436</a> is applied (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4701">#4701</a>)</li>
</ul>
<h3>Removed</h3>
<ul>
<li>Removed deprecated Morden testnet code (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4339">#4339</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li>Ran <code>npm audit fix</code> to address vulnerabilities and update libraries (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4719">#4719</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4728">#4728</a>)</li>
</ul>
<h2>[1.7.2]</h2>
<h3>Changed</h3>
<ul>
<li>Remove deprecated <code>close</code> event listener (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4825">#4825</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4839">#4839</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li><code>npm audit fix</code> to update libraries (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4860">#4860</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/59b657b8c02af05575dc2d0ed321fa7d3aa8eaf6"><code>59b657b</code></a> Build for 1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/e69ea861628f5bf17ed55d16051342644488b46e"><code>e69ea86</code></a> v1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/09634f9ca4e5be7237fa968057bc60e657338f54"><code>09634f9</code></a> Manual build commit for 1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/81b06c91b674e85d0dbe762fac22b9355e7a030a"><code>81b06c9</code></a> v1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/a158594452cba79ae7c154b6f920715a938a6195"><code>a158594</code></a> npm i and CHANGELOG update for 1.8.0 release</li>
<li><a href="https://github.com/web3/web3.js/commit/f616e9f75b375ef5defdbb0ce44f11b9d14e1592"><code>f616e9f</code></a> docs: Fix example of tx usage (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5402">#5402</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/1052540c3667b3cd009d842eba7db910970f11f5"><code>1052540</code></a> Adding Twitter button (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5415">#5415</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/6311abe8cedd70a2863edee8adc381eb63515da4"><code>6311abe</code></a> Merge block tags support 5199 (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5410">#5410</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/bd99127301ca2d427780125ecbfaabb38a4b53a0"><code>bd99127</code></a> 4.x info messages in 1.x (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5412">#5412</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a6ebb2ac9bd7cb45d4a3385fd7a760e1778292e6"><code>a6ebb2a</code></a> Nikos/5071/investigate signtransaction testcases (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5377">#5377</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/web3.js/compare/v1.7.0...v1.8.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jdevcs">jdevcs</a>, a new releaser for web3 since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 11:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2026" class=".btn">#2026</a>
            </td>
            <td>
                <b>
                    Bump got and web3 in /examples/supplychain-app/besu/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) and [web3](https://github.com/ethereum/web3.js). These dependencies needed to be updated together.
Updates `got` from 7.1.0 to 12.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v12.1.0</h2>
<h3>Improvements</h3>
<ul>
<li>Add <code>response.ok</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2043">#2043</a>)  22d58fb
<ul>
<li>This is only useful if you have <a href="https://github.com/sindresorhus/got/blob/main/documentation/2-options.md#throwhttperrors"><code>{throwHttpErrors: false}</code></a></li>
</ul>
</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>Do not redirect to UNIX sockets (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2047">#2047</a>)  861ccd9
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2022-33987">CVE-2022-33987</a></li>
<li><a href="https://github.com/sindresorhus/got/releases/tag/v11.8.5">Also back ported to v11</a></li>
</ul>
</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.4...v12.1.0">https://github.com/sindresorhus/got/compare/v12.0.4...v12.1.0</a></p>
<h2>v12.0.4</h2>
<ul>
<li>Remove stream lock - unreliable since Node 17.3.0 bb8eca924c338ca12d5b90d6a26aa28dbddb42ee</li>
</ul>
<h2>v12.0.3</h2>
<ul>
<li>Allow more types in the <code>json</code> option (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2015">#2015</a>)  eb045bf</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.2...v12.0.3">https://github.com/sindresorhus/got/compare/v12.0.2...v12.0.3</a></p>
<h2>v12.0.2</h2>
<ul>
<li>Fix <code>encoding</code> option with <code>{responseType: 'json'}</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1996">#1996</a>)  0703318</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.1...v12.0.2">https://github.com/sindresorhus/got/compare/v12.0.1...v12.0.2</a></p>
<h2>v12.0.1</h2>
<ul>
<li>Fix <code>nock</code> compatibility (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1959">#1959</a>)  bf39d2c</li>
<li>Fix missing export of <code>Request</code> TypeScript type (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1940">#1940</a>)  0f9f2b8</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.0.0...v12.0.1">https://github.com/sindresorhus/got/compare/v12.0.0...v12.0.1</a></p>
<h2>v12.0.0</h2>
<h3>Introducing Got v12.0.0 :tada:</h3>
<p>Long time no see! The latest Got version (v11.8.2) was released just in February ❄️
We have been working hard on squashing bugs and improving overall experience.</p>
<p>If you find Got useful, you might want to <a href="https://github.com/sindresorhus/got?sponsor=1">sponsor the Got maintainers</a>.</p>
<h3>This package is now pure ESM</h3>
<p><strong>Please <a href="https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c">read this</a>.</strong> Also see <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1789">sindresorhus/got#1789</a>.</p>
<ul>
<li><strong>Please don't open issues about <code>[ERR_REQUIRE_ESM]</code> and <code>Must use import to load ES Module</code> errors.</strong> This is a problem with your setup, not Got.</li>
<li>Please don't open issues about using Got with Jest. Jest does not fully support ESM.</li>
<li>Pretty much any problem with loading this package is a problem with your bundler, test framework, etc, not Got.</li>
<li>If you use TypeScript, you will want to stay on Got v11 until TypeScript 4.6 is out. <a href="https://github-redirect.dependabot.com/microsoft/TypeScript/issues/46452">Why.</a></li>
<li>If you use a bundler, make sure it supports ESM and that you have correctly configured it for ESM.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/ad92afa2eb8d51d46f98491c5ac58b9071fdd67e"><code>ad92afa</code></a> 12.1.0</li>
<li><a href="https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc"><code>861ccd9</code></a> Disable redirects to UNIX sockets (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2047">#2047</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/4cdcca382659050e1c73c7eb9542c8fb871d10aa"><code>4cdcca3</code></a> Check error instance for arguments test (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2044">#2044</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/22d58fb43aece59b3bc571c46f7eda7271f8e083"><code>22d58fb</code></a> Add <code>response.ok</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2043">#2043</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/c25af092bf792c2c7e29db848a569f2eb3e527f8"><code>c25af09</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/62455f5caf269218ab7510d9dda98328ea5a5e84"><code>62455f5</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/6f5c7ce1233c7a28fed12d64766fa19e8eb3b345"><code>6f5c7ce</code></a> Test Node.js 18</li>
<li><a href="https://github.com/sindresorhus/got/commit/c693422bcc40bb35d8f51fc6b4bf97cc71913896"><code>c693422</code></a> 12.0.4</li>
<li><a href="https://github.com/sindresorhus/got/commit/98ca6181a0390450b1e29c277d4670634695ce85"><code>98ca618</code></a> Fix accidental test deletion</li>
<li><a href="https://github.com/sindresorhus/got/commit/bb8eca924c338ca12d5b90d6a26aa28dbddb42ee"><code>bb8eca9</code></a> Remove stream lock - unreliable since Node 17.3.0</li>
<li>Additional commits viewable in <a href="https://github.com/sindresorhus/got/compare/v7.1.0...v12.1.0">compare view</a></li>
</ul>
</details>
<br />

Updates `web3` from 1.7.0 to 1.8.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/web3.js/releases">web3's releases</a>.</em></p>
<blockquote>
<h2>web3-eth@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-eth@4.0.0-alpha.0</code></p>
<h2>web3-core-requestmanager@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-core-requestmanager@4.0.0-alpha.0</code></p>
<h2>web3-providers-http@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-providers-http@4.0.0-alpha.0</code></p>
<h2>web3-providers-base@1.0.0-alpha.1</h2>
<h3>Changed</h3>
<ul>
<li>Update version to <code>1.0.0-alpha.1</code> for <code>web3-providers-base</code></li>
<li>Update version to <code>4.0.0-alpha.0</code> for <code>web3-utils</code> in <code>web3-providers-base</code></li>
</ul>
<h2>web3-utils@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-utils@4.0.0-alpha.0</code></p>
<h2>web3-packagetemplate@1.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-packagetemplate@1.0.0-alpha.0</code></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/1.x/CHANGELOG.md">web3's changelog</a>.</em></p>
<blockquote>
<h2>[1.7.0]</h2>
<h3>Added</h3>
<ul>
<li><code>maxPriorityFeePerGas</code> and <code>maxFeePerGas</code> added to <code>Transaction</code> and <code>TransactionConfig</code> interfaces (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4232">#4232</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4585">#4585</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix readthedoc's build for web3js documentation (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4425">#4425</a>)</li>
<li>Fix response sorting for batch requests (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4250">#4250</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Changed getFeeHistory first parameter type from <code>number</code> to <code>hex</code> according to the <a href="https://playground.open-rpc.org/?schemaUrl=https://raw.githubusercontent.com/ethereum/eth1.0-apis/assembled-spec/openrpc.json&amp;uiSchema%5BappBar%5D%5Bui:splitView%5D=false&amp;uiSchema%5BappBar%5D%5Bui:input%5D=false&amp;uiSchema%5BappBar%5D%5Bui:examplesDropdown%5D=false">spec</a> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4529">#4529</a>)</li>
</ul>
<h2>[1.7.1]</h2>
<h3>Added</h3>
<ul>
<li><code>transactionPollingInterval</code> added to web3, contract and method constructor options. defaults to 1 second. (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4584">#4584</a>)</li>
<li>Add example import for package level types (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4611">#4611</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix a typo in the documentation for <code>methods.myMethod.send</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4599">#4599</a>)</li>
<li>Use globalThis to locate global object if possible (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4613">#4613</a>)</li>
<li>Fix typos in web3-utils.rst (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4662">#4662</a>)</li>
<li>Added effectiveGasPrice to TransactionReceipt (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4692">#4692</a>)</li>
<li>Correction in documentation for <code>web3.eth.accounts.signTransaction</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4576">#4576</a>)</li>
<li>Updated README to include Webpack 5 create-react-app support instructions (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4173">#4173</a>)</li>
<li>Update the documentation for <code>methods.myMethod.estimateGas</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4702">#4702</a>)</li>
<li>Fix typos in REVIEW.md and TESTING.md (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4691">#4691</a>)</li>
<li>Fix encoding for &quot;0x&quot; string values (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4512">#4512</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Muted E2E gnosis dex tests in CI until fix for issue <a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4436">#4436</a> is applied (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4701">#4701</a>)</li>
</ul>
<h3>Removed</h3>
<ul>
<li>Removed deprecated Morden testnet code (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4339">#4339</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li>Ran <code>npm audit fix</code> to address vulnerabilities and update libraries (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4719">#4719</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4728">#4728</a>)</li>
</ul>
<h2>[1.7.2]</h2>
<h3>Changed</h3>
<ul>
<li>Remove deprecated <code>close</code> event listener (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4825">#4825</a>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4839">#4839</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li><code>npm audit fix</code> to update libraries (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/4860">#4860</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/59b657b8c02af05575dc2d0ed321fa7d3aa8eaf6"><code>59b657b</code></a> Build for 1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/e69ea861628f5bf17ed55d16051342644488b46e"><code>e69ea86</code></a> v1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/09634f9ca4e5be7237fa968057bc60e657338f54"><code>09634f9</code></a> Manual build commit for 1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/81b06c91b674e85d0dbe762fac22b9355e7a030a"><code>81b06c9</code></a> v1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/a158594452cba79ae7c154b6f920715a938a6195"><code>a158594</code></a> npm i and CHANGELOG update for 1.8.0 release</li>
<li><a href="https://github.com/web3/web3.js/commit/f616e9f75b375ef5defdbb0ce44f11b9d14e1592"><code>f616e9f</code></a> docs: Fix example of tx usage (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5402">#5402</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/1052540c3667b3cd009d842eba7db910970f11f5"><code>1052540</code></a> Adding Twitter button (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5415">#5415</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/6311abe8cedd70a2863edee8adc381eb63515da4"><code>6311abe</code></a> Merge block tags support 5199 (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5410">#5410</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/bd99127301ca2d427780125ecbfaabb38a4b53a0"><code>bd99127</code></a> 4.x info messages in 1.x (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5412">#5412</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a6ebb2ac9bd7cb45d4a3385fd7a760e1778292e6"><code>a6ebb2a</code></a> Nikos/5071/investigate signtransaction testcases (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5377">#5377</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/web3.js/compare/v1.7.0...v1.8.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jdevcs">jdevcs</a>, a new releaser for web3 since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 11:41:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2025" class=".btn">#2025</a>
            </td>
            <td>
                <b>
                    [chore] merge main to develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge latest main to develop
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 11:35:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2024" class=".btn">#2024</a>
            </td>
            <td>
                <b>
                    [quorum] ibft consensus  fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manikanta-darsi <manikanta.darsi@accenture.com>

**Changelog**
- Fix ibft consensus  fix.

 

**Reviewed by**
@sownak @suvajit-sarkar @jagpreetsinghsasan 

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 08:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2023" class=".btn">#2023</a>
            </td>
            <td>
                <b>
                    [docs] added dci lint github workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>

**Changelog**
- Add dci lint github workflow
 

**Reviewed by**
@suvajit-sarkar 
@sownak 

 

**Linked issue**
#1949 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 07:08:43 +0000 UTC
    </div>
</div>

