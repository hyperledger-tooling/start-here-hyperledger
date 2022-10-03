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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/836" class=".btn">#836</a>
            </td>
            <td>
                <b>
                    Bump ejs, @vue/cli-plugin-babel, @vue/cli-service, @vue/cli-plugin-eslint, @vue/cli-plugin-router and @vue/cli-plugin-typescript in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [ejs](https://github.com/mde/ejs). It's no longer used after updating ancestor dependencies [ejs](https://github.com/mde/ejs), [@vue/cli-plugin-babel](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-babel), [@vue/cli-service](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-service), [@vue/cli-plugin-eslint](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-eslint), [@vue/cli-plugin-router](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-router) and [@vue/cli-plugin-typescript](https://github.com/vuejs/vue-cli/tree/HEAD/packages/@vue/cli-plugin-typescript). These dependencies need to be updated together.

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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-03 08:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/833" class=".btn">#833</a>
            </td>
            <td>
                <b>
                    Bump async from 2.6.3 to 2.6.4 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) from 2.6.3 to 2.6.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/v2.6.4/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v2.6.4</h1>
<ul>
<li>Fix potential prototype pollution exploit (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1828">#1828</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/c6bdaca4f9175c14fc655d3783c6af6a883e6514"><code>c6bdaca</code></a> Version 2.6.4</li>
<li><a href="https://github.com/caolan/async/commit/8870da9d5022bab310413041b4079e10db3980b7"><code>8870da9</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/4df6754ef4e96a742956df8782fee27242a2ea12"><code>4df6754</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/8f7f90342a6571ba1c197d747ebed30c368096d2"><code>8f7f903</code></a> Fix prototype pollution vulnerability (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1828">#1828</a>)</li>
<li>See full diff in <a href="https://github.com/caolan/async/compare/v2.6.3...v2.6.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async&package-manager=npm_and_yarn&previous-version=2.6.3&new-version=2.6.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/833"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-03 07:55:26 +0000 UTC
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

