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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    switch default ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger-labs/business-partner-agent/issues/377

deprecate bosch test ledger and use bcovrin test ledger as the new default

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/838"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 14:23:48 +0000 UTC
    </div>
</div>

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

