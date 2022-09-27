---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/832" class=".btn">#832</a>
            </td>
            <td>
                <b>
                    Bump ejs, @vue/cli-plugin-babel, @vue/cli-plugin-e2e-cypress, @vue/cli-plugin-eslint, @vue/cli-plugin-router, @vue/cli-plugin-typescript, @vue/cli-plugin-unit-jest and @vue/cli-service in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [ejs](https://github.com/mde/ejs). It's no longer used after updating ancestor dependencies [ejs](https://github.com/mde/ejs), [@vue/cli-plugin-babel](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-babel), [@vue/cli-plugin-e2e-cypress](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-e2e-cypress), [@vue/cli-plugin-eslint](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-eslint), [@vue/cli-plugin-router](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-router), [@vue/cli-plugin-typescript](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-typescript), [@vue/cli-plugin-unit-jest](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-unit-jest) and [@vue/cli-service](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-service). These dependencies need to be updated together.

Removes `ejs`

Updates `@vue/cli-plugin-babel` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-babel</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-babel</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/75a6d690eee4c7b3e46528d6b1d7b0b7a6d2cf3d"><code>75a6d69</code></a> v5.0.0-rc.3</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-babel">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-e2e-cypress` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-e2e-cypress</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-e2e-cypress</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/27dba1ac6ddb9822b82734b726088e61463a5023"><code>27dba1a</code></a> fix: eliminate calling deprecated function in cli-plugin-e2e-cypress and cli-...</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44ef0e78d870ed582adc71464dd2336a68a"><code>697bb44</code></a> fix: should correctly resolve cypress bin path for Cypress 10</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/1452cd3fbf0f2e15cb33e5480744ddcbe6f48aa9"><code>1452cd3</code></a> feat: update cypress to 9.x</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-e2e-cypress">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-eslint` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-eslint</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-eslint</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/75a6d690eee4c7b3e46528d6b1d7b0b7a6d2cf3d"><code>75a6d69</code></a> v5.0.0-rc.3</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-eslint">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-router` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-router</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-router</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/75a6d690eee4c7b3e46528d6b1d7b0b7a6d2cf3d"><code>75a6d69</code></a> v5.0.0-rc.3</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-router">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-typescript` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-typescript</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-typescript</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/6b163f28fc3428284a06957f157f7825cd8fd74c"><code>6b163f2</code></a> chore: fix lint errors</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a648958b00758bd267743090a894c510ecaa8b40"><code>a648958</code></a> fix: compatibility with Vue 2.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/60356294218fca3f5919ad7e90e706b57e86cafb"><code>6035629</code></a> chore: remove redundant yorkie dependency in typescript plugin</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-typescript">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-unit-jest` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-unit-jest</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-unit-jest</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/9be19f0ef0ae4666f983c0c23809bb0c5847a714"><code>9be19f0</code></a> test: fix tsx import</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-unit-jest">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-service` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-service</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-service</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4dacd89b6edf63bef07fd80d3b6108f72b5"><code>0260e4d</code></a> fix: add devServer.server.type to useHttps judgement (<a href="https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-service/issues/7222">#7222</a>)</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/beffe8a50515c48b9ad5085e79d3c2b16ae76825"><code>beffe8a</code></a> fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
<li><a href="https://github.com/vuejs/vue-cli/commit/558dea2af693893ca75e372f286d92152bc8d960"><code>558dea2</code></a> fix: support <code>devServer.server</code> option, avoid deprecation warning</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/bddd64d5b7eba65e1b0f0ec36fd8af2e7d5e3ce6"><code>bddd64d</code></a> fix: optimize the judgment on whether HTTPS has been set in options (<a href="https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-service/issues/7202">#7202</a>)</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/fcf27e350e743a2fbc99d4c021dcd49e43cac929"><code>fcf27e3</code></a> fixup! fix: compatibility with Vue 2.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a648958b00758bd267743090a894c510ecaa8b40"><code>a648958</code></a> fix: compatibility with Vue 2.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-service">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR ...

_Description has been truncated_

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/832"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 07:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    Bump node-forge, @vue/cli-plugin-babel, @vue/cli-plugin-e2e-cypress, @vue/cli-plugin-eslint, @vue/cli-plugin-router, @vue/cli-plugin-typescript, @vue/cli-plugin-unit-jest and @vue/cli-service in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-forge](https://github.com/digitalbazaar/forge) to 1.3.1 and updates ancestor dependencies [node-forge](https://github.com/digitalbazaar/forge), [@vue/cli-plugin-babel](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-babel), [@vue/cli-plugin-e2e-cypress](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-e2e-cypress), [@vue/cli-plugin-eslint](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-eslint), [@vue/cli-plugin-router](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-router), [@vue/cli-plugin-typescript](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-typescript), [@vue/cli-plugin-unit-jest](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-unit-jest) and [@vue/cli-service](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-service). These dependencies need to be updated together.

Updates `node-forge` from 0.10.0 to 1.3.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/digitalbazaar/forge/blob/main/CHANGELOG.md">node-forge's changelog</a>.</em></p>
<blockquote>
<h2>1.3.1 - 2022-03-29</h2>
<h3>Fixes</h3>
<ul>
<li>RFC 3447 and RFC 8017 allow for optional <code>DigestAlgorithm</code> <code>NULL</code> parameters
for <code>sha*</code> algorithms and require <code>NULL</code> paramters for <code>md2</code> and <code>md5</code>
algorithms.</li>
</ul>
<h2>1.3.0 - 2022-03-17</h2>
<h3>Security</h3>
<ul>
<li>Three RSA PKCS#1 v1.5 signature verification issues were reported by Moosa
Yahyazadeh (<a href="mailto:moosa-yahyazadeh@uiowa.edu">moosa-yahyazadeh@uiowa.edu</a>).</li>
<li><strong>HIGH</strong>: Leniency in checking <code>digestAlgorithm</code> structure can lead to
signature forgery.
<ul>
<li>The code is lenient in checking the digest algorithm structure. This can
allow a crafted structure that steals padding bytes and uses unchecked
portion of the PKCS#1 encoded message to forge a signature when a low
public exponent is being used. For more information, please see
<a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24771">CVE-2022-24771</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-cfm4-qjh2-4765">GHSA-cfm4-qjh2-4765</a></li>
</ul>
</li>
<li><strong>HIGH</strong>: Failing to check tailing garbage bytes can lead to signature
forgery.
<ul>
<li>The code does not check for tailing garbage bytes after decoding a
<code>DigestInfo</code> ASN.1 structure. This can allow padding bytes to be removed
and garbage data added to forge a signature when a low public exponent is
being used.  For more information, please see <a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA
signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24772">CVE-2022-24772</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-x4jg-mjrx-434g">GHSA-x4jg-mjrx-434g</a></li>
</ul>
</li>
<li><strong>MEDIUM</strong>: Leniency in checking type octet.
<ul>
<li><code>DigestInfo</code> is not properly checked for proper ASN.1 structure. This can
lead to successful verification with signatures that contain invalid
structures but a valid digest.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24773">CVE-2022-24773</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-2r2c-g63r-vccr">GHSA-2r2c-g63r-vccr</a></li>
</ul>
</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[asn1] Add fallback to pretty print invalid UTF8 data.</li>
<li>[asn1] <code>fromDer</code> is now more strict and will default to ensuring all input
bytes are parsed or throw an error. A new option <code>parseAllBytes</code> can disable
this behavior.
<ul>
<li><strong>NOTE</strong>: The previous behavior is being changed since it can lead to
security issues with crafted inputs. It is possible that code doing custom
DER parsing may need to adapt to this new behavior and optional flag.</li>
</ul>
</li>
<li>[rsa] Add and use a validator to check for proper structure of parsed ASN.1</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/digitalbazaar/forge/commit/a0a4a4264bedb3296974b9675349c9c190144aeb"><code>a0a4a42</code></a> Release 1.3.1.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/a33830f61c351e8e3a34309767e8dd0de148376b"><code>a33830f</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/740954d747ac56b76a6e1ae12a057c9548843436"><code>740954d</code></a> Allow optional DigestAlgorithm parameters.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/56f4316b4cc6592e678f8c416209c45984b6547b"><code>56f4316</code></a> Allow DigestInfo.DigestAlgorith.parameters to be optional</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/cbf0bd590d47fe3120a57e7c36f2f4e64381ad81"><code>cbf0bd5</code></a> Start 1.3.1-0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/6c5b90133d46af63d139b98bf65371732c8c7dad"><code>6c5b901</code></a> Release 1.3.0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/0f3972ad5883a9869703c6f54a0627bc454bca47"><code>0f3972a</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/dc77b39dd347e7f8b60a0f25a311fe5f06130579"><code>dc77b39</code></a> Fix error checking.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/bb822c02df0b61211836472e29b9790cc541cdb2"><code>bb822c0</code></a> Add advisory links.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/d4395fec831622837ecfec9e428d4620e208f9a8"><code>d4395fe</code></a> Update changelog.</li>
<li>Additional commits viewable in <a href="https://github.com/digitalbazaar/forge/compare/0.10.0...v1.3.1">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-babel` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-babel</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-babel</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/75a6d690eee4c7b3e46528d6b1d7b0b7a6d2cf3d"><code>75a6d69</code></a> v5.0.0-rc.3</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-babel">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-e2e-cypress` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-e2e-cypress</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-e2e-cypress</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/27dba1ac6ddb9822b82734b726088e61463a5023"><code>27dba1a</code></a> fix: eliminate calling deprecated function in cli-plugin-e2e-cypress and cli-...</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44ef0e78d870ed582adc71464dd2336a68a"><code>697bb44</code></a> fix: should correctly resolve cypress bin path for Cypress 10</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/1452cd3fbf0f2e15cb33e5480744ddcbe6f48aa9"><code>1452cd3</code></a> feat: update cypress to 9.x</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-e2e-cypress">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-eslint` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-eslint</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-eslint</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/75a6d690eee4c7b3e46528d6b1d7b0b7a6d2cf3d"><code>75a6d69</code></a> v5.0.0-rc.3</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-eslint">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-router` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-router</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-router</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/75a6d690eee4c7b3e46528d6b1d7b0b7a6d2cf3d"><code>75a6d69</code></a> v5.0.0-rc.3</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-router">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-typescript` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-typescript</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-typescript</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/6b163f28fc3428284a06957f157f7825cd8fd74c"><code>6b163f2</code></a> chore: fix lint errors</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a648958b00758bd267743090a894c510ecaa8b40"><code>a648958</code></a> fix: compatibility with Vue 2.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/60356294218fca3f5919ad7e90e706b57e86cafb"><code>6035629</code></a> chore: remove redundant yorkie dependency in typescript plugin</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-typescript">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-unit-jest` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-unit-jest</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-unit-jest</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/9be19f0ef0ae4666f983c0c23809bb0c5847a714"><code>9be19f0</code></a> test: fix tsx import</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-unit-jest">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-service` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-service</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-service</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@v...

_Description has been truncated_

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/831"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 07:23:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    Bump jsdom and @vue/cli-plugin-unit-jest in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsdom](https://github.com/jsdom/jsdom) to 16.7.0 and updates ancestor dependency [@vue/cli-plugin-unit-jest](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-unit-jest). These dependencies need to be updated together.

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

Updates `@vue/cli-plugin-unit-jest` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-unit-jest</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-unit-jest</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/92d80a89122cea830a4e7e32946af64b4c3b62f7"><code>92d80a8</code></a> v5.0.1</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/c913cdcb67f4a8e7c1f8affd1a6ba9a93c0f3ebd"><code>c913cdc</code></a> v5.0.0</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/9be19f0ef0ae4666f983c0c23809bb0c5847a714"><code>9be19f0</code></a> test: fix tsx import</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-unit-jest">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/830"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 07:22:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    Bump async and @vue/cli-plugin-e2e-cypress in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) to 3.2.4 and updates ancestor dependency [@vue/cli-plugin-e2e-cypress](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-e2e-cypress). These dependencies need to be updated together.

Updates `async` from 2.6.3 to 3.2.4
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/master/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v3.2.4</h1>
<ul>
<li>Fix a bug in <code>priorityQueue</code> where it didn't wait for the result. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1725">#1725</a>)</li>
<li>Fix a bug where <code>unshiftAsync</code> was included in <code>priorityQueue</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1790">#1790</a>)</li>
</ul>
<h1>v3.2.3</h1>
<ul>
<li>Fix bugs in comment parsing in <code>autoInject</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1767">#1767</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1780">#1780</a>)</li>
</ul>
<h1>v3.2.2</h1>
<ul>
<li>Fix potential prototype pollution exploit</li>
</ul>
<h1>v3.2.1</h1>
<ul>
<li>Use <code>queueMicrotask</code> if available to the environment (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1761">#1761</a>)</li>
<li>Minor perf improvement in <code>priorityQueue</code> (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1727">#1727</a>)</li>
<li>More examples in documentation (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1726">#1726</a>)</li>
<li>Various doc fixes (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1708">#1708</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1712">#1712</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1717">#1717</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1740">#1740</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1739">#1739</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1749">#1749</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1756">#1756</a>)</li>
<li>Improved test coverage (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1754">#1754</a>)</li>
</ul>
<h1>v3.2.0</h1>
<ul>
<li>Fix a bug in Safari related to overwriting <code>func.name</code></li>
<li>Remove built-in browserify configuration (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1653">#1653</a>)</li>
<li>Varios doc fixes (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1688">#1688</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1703">#1703</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1704">#1704</a>)</li>
</ul>
<h1>v3.1.1</h1>
<ul>
<li>Allow redefining <code>name</code> property on wrapped functions.</li>
</ul>
<h1>v3.1.0</h1>
<ul>
<li>Added <code>q.pushAsync</code> and <code>q.unshiftAsync</code>, analagous to <code>q.push</code> and <code>q.unshift</code>, except they always do not accept a callback, and reject if processing the task errors. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1659">#1659</a>)</li>
<li>Promises returned from <code>q.push</code> and <code>q.unshift</code> when a callback is not passed now resolve even if an error ocurred. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1659">#1659</a>)</li>
<li>Fixed a parsing bug in <code>autoInject</code> with complicated function bodies (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1663">#1663</a>)</li>
<li>Added ES6+ configuration for Browserify bundlers (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1653">#1653</a>)</li>
<li>Various doc fixes (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1664">#1664</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1658">#1658</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1665">#1665</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1652">#1652</a>)</li>
</ul>
<h1>v3.0.1</h1>
<h2>Bug fixes</h2>
<ul>
<li>Fixed a regression where arrays passed to <code>queue</code> and <code>cargo</code> would be completely flattened. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1645">#1645</a>)</li>
<li>Clarified Async's browser support (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1643">#1643</a>)</li>
</ul>
<h1>v3.0.0</h1>
<p>The <code>async</code>/<code>await</code> release!</p>
<p>There are a lot of new features and subtle breaking changes in this major version, but the biggest feature is that most Async methods return a Promise if you omit the callback, meaning you can <code>await</code> them from within an <code>async</code> function.</p>
<pre lang="js"><code>const results = await async.mapLimit(urls, 5, async url =&gt; {
    const resp = await fetch(url)
    return resp.body
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/f3ab51af76ca87ebe3ec67b3dd6dec4959e04816"><code>f3ab51a</code></a> Version 3.2.4</li>
<li><a href="https://github.com/caolan/async/commit/7ea2cec7398b33a15daf5c3bd9bda6ae78caf297"><code>7ea2cec</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/bef7befc734e4b712ab6ffc82463cc40c1037056"><code>bef7bef</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/03eeab36ae5a0454bbf67b881f087692e0b7c7e4"><code>03eeab3</code></a> Bump yargs from 17.4.1 to 17.5.1 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1843">#1843</a>)</li>
<li><a href="https://github.com/caolan/async/commit/387efcf80f5b2c454effd2a64c75ff3c634ec3bd"><code>387efcf</code></a> Bump eslint from 8.14.0 to 8.17.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1849">#1849</a>)</li>
<li><a href="https://github.com/caolan/async/commit/131225a8c82fda93010b8b82da46e9a23b6b1816"><code>131225a</code></a> Bump karma from 6.3.19 to 6.3.20 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1844">#1844</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4cfa89cb240d9748d5bfee0656fbed08cf80cc10"><code>4cfa89c</code></a> Bump eslint from 8.14.0 to 8.16.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1845">#1845</a>)</li>
<li><a href="https://github.com/caolan/async/commit/90e940cbb5a051db7c2a28169769f97eef99fdd6"><code>90e940c</code></a> Bump rollup from 2.71.1 to 2.75.5 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1846">#1846</a>)</li>
<li><a href="https://github.com/caolan/async/commit/dd72cf5f614bcf2b08ae2678f6e8ffbd28136804"><code>dd72cf5</code></a> Bump <code>@​babel/eslint-parser</code> from 7.17.0 to 7.18.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1847">#1847</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4ae026e8da11f817f274f264dd3a9ec7ef3307c5"><code>4ae026e</code></a> Bump babel-minify from 0.5.1 to 0.5.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1848">#1848</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/caolan/async/compare/v2.6.3...v3.2.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
</details>
<br />

Updates `@vue/cli-plugin-e2e-cypress` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-e2e-cypress</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-e2e-cypress</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/27dba1ac6ddb9822b82734b726088e61463a5023"><code>27dba1a</code></a> fix: eliminate calling deprecated function in cli-plugin-e2e-cypress and cli-...</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44ef0e78d870ed582adc71464dd2336a68a"><code>697bb44</code></a> fix: should correctly resolve cypress bin path for Cypress 10</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/1452cd3fbf0f2e15cb33e5480744ddcbe6f48aa9"><code>1452cd3</code></a> feat: update cypress to 9.x</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-e2e-cypress">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/829"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 07:22:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    Bump minimist and @vue/cli-plugin-e2e-cypress in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) to 1.2.6 and updates ancestor dependency [@vue/cli-plugin-e2e-cypress](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-e2e-cypress). These dependencies need to be updated together.

Updates `minimist` from 1.2.5 to 1.2.6
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/substack/minimist/commits">compare view</a></li>
</ul>
</details>
<br />

Updates `@vue/cli-plugin-e2e-cypress` from 4.5.15 to 5.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/releases"><code>@​vue/cli-plugin-e2e-cypress</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.8</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/0260e4d">0260e4d</a> fix: add devServer.server.type to useHttps judgement (<a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7222">vuejs/vue-cli#7222</a>)</li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/07052c4">07052c4</a> fix: Vue CLI UI graphql subscription server error, fixes <a href="https://github-redirect.dependabot.com/vuejs/vue-cli/issues/7221">vuejs/vue-cli#7221</a></li>
</ul>
</li>
</ul>
<h2>v5.0.7</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.6</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>v5.0.5</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> fix(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-plugin-e2e-cypress</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44">[697bb44]</a> fix: should correctly resolve cypress bin path for Cypress 10 (Note that the project is still created with Cypress 9 by default, but you can upgrade to Cypress 10 on your own now)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>v5.0.4</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Andrei (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>v5.0.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-cli/blob/dev/CHANGELOG.md"><code>@​vue/cli-plugin-e2e-cypress</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.7 (2022-07-05)</h2>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7202">#7202</a>, [<a href="https://github.com/vuejs/vue-cli/commit/558dea2">558dea2</a>] fix: support <code>devServer.server</code> option, avoid deprecation warnings (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>, <a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
<li>[<a href="https://github.com/vuejs/vue-cli/commit/beffe8a">beffe8a</a>] fix: allow disabling progress plugin via <code>devServer.client.progress</code></li>
</ul>
</li>
<li><code>@vue/cli-ui</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7210">#7210</a> chore: upgrade to apollo-server-express 3.x</li>
</ul>
</li>
</ul>
<h4>Committers: 2</h4>
<ul>
<li>BackRunner (<a href="https://github.com/backrunner"><code>@​backrunner</code></a>)</li>
<li>Haoqun Jiang (<a href="https://github.com/sodatea"><code>@​sodatea</code></a>)</li>
</ul>
<h2>5.0.6 (2022-06-16)</h2>
<p>Fix compatibility with the upcoming Vue 2.7 (currently in alpha) and Vue Loader 15.10 (currently in beta).</p>
<p>In Vue 2.7, <code>vue-template-compiler</code> is no longer a required peer dependency. Rather, there's a new export under the main package as <code>vue/compiler-sfc</code>.</p>
<h2>5.0.5 (2022-06-16)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7167">#7167</a> feat(upgrade): prevent changing the structure of package.json file during upgrade (<a href="https://github.com/blzsaa"><code>@​blzsaa</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7023">#7023</a> fix: windows vue.config.mjs support (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Martijn Jacobs (<a href="https://github.com/maerteijn"><code>@​maerteijn</code></a>)</li>
<li>ZHAO Jinxiang (<a href="https://github.com/xiaoxiangmoe"><code>@​xiaoxiangmoe</code></a>)</li>
<li><a href="https://github.com/blzsaa"><code>@​blzsaa</code></a></li>
</ul>
<h2>5.0.4 (2022-03-22)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>@vue/cli-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/vuejs/vue-cli/pull/7005">#7005</a> Better handling of <code>publicPath: 'auto'</code> (<a href="https://github.com/AndreiSoroka"><code>@​AndreiSoroka</code></a>)</li>
</ul>
</li>
<li><code>@vue/cli-shared-utils</code>, <code>@vue/cli-ui</code>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/75826d6">75826d6</a> fix: replace <code>node-ipc</code> with <code>@achrinza/node-ipc</code> to further secure the dependency chain</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-cli/commit/b154dbd7aca4b4538e6c483b1d4b817499d7b8eb"><code>b154dbd</code></a> v5.0.8</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/4a0655f7ac09b64d2b47506e7f21e7923d43262b"><code>4a0655f</code></a> v5.0.7</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ef08a08c41b028a2484f262414a8c91d151febc7"><code>ef08a08</code></a> v5.0.6</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/98c66c93ae45d3347f62c56838caab86561ad4f7"><code>98c66c9</code></a> v5.0.5</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/27dba1ac6ddb9822b82734b726088e61463a5023"><code>27dba1a</code></a> fix: eliminate calling deprecated function in cli-plugin-e2e-cypress and cli-...</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/697bb44ef0e78d870ed582adc71464dd2336a68a"><code>697bb44</code></a> fix: should correctly resolve cypress bin path for Cypress 10</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/1452cd3fbf0f2e15cb33e5480744ddcbe6f48aa9"><code>1452cd3</code></a> feat: update cypress to 9.x</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/ca97fc2920a3fc9b0288d5fabef1a97356b8da23"><code>ca97fc2</code></a> v5.0.4</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/dd53f26bc0c51fec7c5fb2c18f4769de984ad79c"><code>dd53f26</code></a> v5.0.3</li>
<li><a href="https://github.com/vuejs/vue-cli/commit/a859b1fdf26bca3fcd44b535965926da333d11f8"><code>a859b1f</code></a> v5.0.2</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-cli/commits/v5.0.8/packages/@vue/cli-plugin-e2e-cypress">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/828"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 07:22:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    Bump vuetify from 2.6.6 to 2.6.10 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [vuetify](https://github.com/vuetifyjs/vuetify/tree/HEAD/packages/vuetify) from 2.6.6 to 2.6.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuetifyjs/vuetify/releases">vuetify's releases</a>.</em></p>
<blockquote>
<h2>v2.6.10</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>VCalendar:</strong> prevent XSS from eventName function (<a href="https://github.com/vuetifyjs/vuetify/commit/ade1434927f55a0eccf3d54f900f24c5fa85a176">ade1434</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15757">#15757</a></li>
<li><strong>VDialog:</strong> don't try to focus <code>tabindex=&quot;-1&quot;</code> or hidden inputs (<a href="https://github.com/vuetifyjs/vuetify/commit/89e3850c5478c7bf0ae6081a95f6d2b39e690e8f">89e3850</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15745">#15745</a></li>
<li><strong>VMenu:</strong> disable activatorFixed when attach is enabled (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15709">#15709</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/464529a0358704c27463b660eead65925adf0f6d">464529a</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14922">#14922</a></li>
<li><strong>VTextField:</strong> only show clear icon on hover or when focused (<a href="https://github.com/vuetifyjs/vuetify/commit/7a51ad0140dd17f9d718f6ceb84226d305c2c379">7a51ad0</a>)</li>
<li><strong>VTextField:</strong> prevent tabbing to clear button (<a href="https://github.com/vuetifyjs/vuetify/commit/f8ee680b1d78182852822fd12b63dd00a5803f40">f8ee680</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/11202">#11202</a></li>
<li><strong>web-types:</strong> add support for VDataTable pattern slots (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15694">#15694</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/ac45c98983717d5ee42c4e85de1deccbd698cc83">ac45c98</a>)</li>
</ul>
<h3>:microscope: Code Refactoring</h3>
<ul>
<li><strong>VSelect:</strong> render highlight with vnodes instead of innerHTML (<a href="https://github.com/vuetifyjs/vuetify/commit/4468e3c442284b512729e7b89768fd8762c2e9c1">4468e3c</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li><strong>VCalendar:</strong> <code>eventName</code> function can no longer render arbitrary HTML, convert to VNodes instead.
<code>eventSummary</code> can no longer be used with v-html, replace with <code>&lt;component :is=&quot;{ render: eventSummary }&quot; /&gt;</code></li>
</ul>
<h2>v2.6.9</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>VCalendar:</strong> add aria roles to monthly calendar (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14640">#14640</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/2cd34b4d29ee08b40d9b93e03ee38f50cb4a2a7f">2cd34b4</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14604">#14604</a></li>
<li><strong>VCalendar:</strong> forward all bound events to internal elements (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15592">#15592</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/299330cc64b9a3590822062dbba6f1028f6207d3">299330c</a>)</li>
<li><strong>VCarousel:</strong> add keys to delimiter buttons (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15459">#15459</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/8d3895bc0efd57bb2e5cc6bbf54c2b700e915be7">8d3895b</a>)</li>
<li><strong>VPagination:</strong> ignore invalid length values (<a href="https://github.com/vuetifyjs/vuetify/commit/f3f8d15e9c701c83ab12945ea105fe259aa87b7a">f3f8d15</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15499">#15499</a></li>
<li><strong>VRadio:</strong> change icon color when disabled (<a href="https://github.com/vuetifyjs/vuetify/commit/0cc43e293c0f64e12b210a543e2c71cf084f1ebc">0cc43e2</a>)</li>
<li><strong>VSwitch:</strong> only affect control opacity when disabled (<a href="https://github.com/vuetifyjs/vuetify/commit/1e0a4ad5cde6f4353a52ee5f5dc3731a602038f0">1e0a4ad</a>)</li>
</ul>
<h2>v2.6.8</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>VDataTable:</strong> display header text instead of value in group headers (<a href="https://github.com/vuetifyjs/vuetify/commit/100053fbd229edbab5f64287fe35ca203a24c4ce">100053f</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/11516">#11516</a></li>
<li><strong>VItemGroup:</strong> use valueComparator when updating value (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15395">#15395</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/8bedb7c05e7b4282ea71202cf9ffe562d31fe0f1">8bedb7c</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15394">#15394</a></li>
<li><strong>VSimpleCheckbox:</strong> directly specify ripple directive definition (<a href="https://github.com/vuetifyjs/vuetify/commit/00a9668d7a58bfd1ea3674e48cca2dc8336bbffc">00a9668</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/12224">#12224</a></li>
</ul>
<h2>v2.6.7</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>styles:</strong> resolve css validation errors (<a href="https://github.com/vuetifyjs/vuetify/commit/621f273bc1608038184255f57b10671dab2a031d">621f273</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15320">#15320</a></li>
<li><strong>VDialog:</strong> focus on internal content when shown (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14584">#14584</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/ffbaae129d36e40bb2926914f2960b09370befb2">ffbaae1</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14581">#14581</a></li>
<li><strong>VInput:</strong> allow text selection in disabled inputs (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14465">#14465</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/760490da75fc531fca9edcd4ef308f2698ba02aa">760490d</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14238">#14238</a></li>
<li><strong>VList:</strong> don't trigger keyboard events on disabled items (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15339">#15339</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/817df79726167fc547a86f1d7c0017080aa1a7e5">817df79</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15322">#15322</a></li>
<li><strong>VOtpInput:</strong> support paste and autofill on mobile (<a href="https://github.com/vuetifyjs/vuetify/commit/8c67ed8cf96334a86c6f087b7abfa845992098a2">8c67ed8</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14801">#14801</a></li>
<li><strong>VRadio:</strong> use correct disabled color for icons (<a href="https://github.com/vuetifyjs/vuetify/commit/31157988d61373af86c015e9e77ed7806b54b658">3115798</a>)</li>
<li><strong>VSelect:</strong> allow keyboard selection of items with value 0 (<a href="https://github.com/vuetifyjs/vuetify/commit/969aba42229275bd1d703d8c51890674105ac6c2">969aba4</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15166">#15166</a></li>
<li><strong>VTabs:</strong> use ResizeObserver if available (<a href="https://github.com/vuetifyjs/vuetify/commit/ff519c6121cc995069caba9b232c216633d6f801">ff519c6</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/4733">#4733</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/10455">#10455</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/12783">#12783</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14195">#14195</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15316">#15316</a></li>
<li><strong>VTimeline:</strong> disable arrow shadow on clickable cards (<a href="https://github.com/vuetifyjs/vuetify/commit/27ba2c9b7663ce70a35556a3c4336fec44f87605">27ba2c9</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14193">#14193</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/fdfb6fc34d797d2798ae73b049f34e5098793caa"><code>fdfb6fc</code></a> chore(release): publish v2.6.10</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/cd193e41e4041ca0786f5dbcda454e94dd7bddb9"><code>cd193e4</code></a> fix(VSelectList): correct mask class</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/89e3850c5478c7bf0ae6081a95f6d2b39e690e8f"><code>89e3850</code></a> fix(VDialog): don't try to focus tabindex=&quot;-1&quot; or hidden inputs</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/4468e3c442284b512729e7b89768fd8762c2e9c1"><code>4468e3c</code></a> refactor(VSelect): render highlight with vnodes instead of innerHTML</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/ade1434927f55a0eccf3d54f900f24c5fa85a176"><code>ade1434</code></a> fix(VCalendar): prevent XSS from eventName function</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/464529a0358704c27463b660eead65925adf0f6d"><code>464529a</code></a> fix(VMenu): disabled activatorFixed when attach is enabled (<a href="https://github.com/vuetifyjs/vuetify/tree/HEAD/packages/vuetify/issues/15709">#15709</a>)</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/7a51ad0140dd17f9d718f6ceb84226d305c2c379"><code>7a51ad0</code></a> fix(VTextField): only show clear icon on hover or when focused</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/f8ee680b1d78182852822fd12b63dd00a5803f40"><code>f8ee680</code></a> fix(VTextField): prevent tabbing to clear button</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/170c7d14964d410deb70e6c4604fe6cef0608727"><code>170c7d1</code></a> chore(release): publish v2.6.9</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/2cd34b4d29ee08b40d9b93e03ee38f50cb4a2a7f"><code>2cd34b4</code></a> fix(VCalendar): add aria roles to monthly calendar (<a href="https://github.com/vuetifyjs/vuetify/tree/HEAD/packages/vuetify/issues/14640">#14640</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vuetifyjs/vuetify/commits/v2.6.10/packages/vuetify">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=vuetify&package-manager=npm_and_yarn&previous-version=2.6.6&new-version=2.6.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/827"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 22:29:13 +0000 UTC
    </div>
</div>

