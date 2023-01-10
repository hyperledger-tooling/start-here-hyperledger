---
layout: default
title: karma-charity-platform
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/karma-charity-platform
---

# karma-charity-platform <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/karma-charity-platform){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    Bump jsonwebtoken, @nestjs/jwt and passport-jwt in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) to 9.0.0 and updates ancestor dependencies [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken), [@nestjs/jwt](https://github.com/nestjs/jwt) and [passport-jwt](https://github.com/mikenicholson/passport-jwt). These dependencies need to be updated together.

Updates `jsonwebtoken` from 8.5.1 to 9.0.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/auth0/node-jsonwebtoken/blob/master/CHANGELOG.md">jsonwebtoken's changelog</a>.</em></p>
<blockquote>
<h2>9.0.0 - 2022-12-21</h2>
<p><strong>Breaking changes: See <a href="https://github.com/auth0/node-jsonwebtoken/wiki/Migration-Notes:-v8-to-v9">Migration from v8 to v9</a></strong></p>
<h3>Breaking changes</h3>
<ul>
<li>Removed support for Node versions 11 and below.</li>
<li>The verify() function no longer accepts unsigned tokens by default. ([834503079514b72264fd13023a3b8d648afd6a16]<a href="https://github.com/auth0/node-jsonwebtoken/commit/834503079514b72264fd13023a3b8d648afd6a16">https://github.com/auth0/node-jsonwebtoken/commit/834503079514b72264fd13023a3b8d648afd6a16</a>)</li>
<li>RSA key size must be 2048 bits or greater. ([ecdf6cc6073ea13a7e71df5fad043550f08d0fa6]<a href="https://github.com/auth0/node-jsonwebtoken/commit/ecdf6cc6073ea13a7e71df5fad043550f08d0fa6">https://github.com/auth0/node-jsonwebtoken/commit/ecdf6cc6073ea13a7e71df5fad043550f08d0fa6</a>)</li>
<li>Key types must be valid for the signing / verification algorithm</li>
</ul>
<h3>Security fixes</h3>
<ul>
<li>security: fixes <code>Arbitrary File Write via verify function</code> - CVE-2022-23529</li>
<li>security: fixes <code>Insecure default algorithm in jwt.verify() could lead to signature validation bypass</code> - CVE-2022-23540</li>
<li>security: fixes <code>Insecure implementation of key retrieval function could lead to Forgeable Public/Private Tokens from RSA to HMAC</code> - CVE-2022-23541</li>
<li>security: fixes <code>Unrestricted key type could lead to legacy keys usage</code> - CVE-2022-23539</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/e1fa9dcc12054a8681db4e6373da1b30cf7016e3"><code>e1fa9dc</code></a> Merge pull request from GHSA-8cf7-32gw-wr33</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/5eaedbf2b01676d952336e73b4d2efba847d2d1b"><code>5eaedbf</code></a> chore(ci): remove github test actions job (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/861">#861</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/cd4163eb1407aab0b3148f91b0b9c26276b96c6b"><code>cd4163e</code></a> chore(ci): configure Github Actions jobs for Tests &amp; Security Scanning (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/856">#856</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/ecdf6cc6073ea13a7e71df5fad043550f08d0fa6"><code>ecdf6cc</code></a> fix!: Prevent accidental use of insecure key sizes &amp; misconfiguration of secr...</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/834503079514b72264fd13023a3b8d648afd6a16"><code>8345030</code></a> fix(sign&amp;verify)!: Remove default <code>none</code> support from <code>sign</code> and <code>verify</code> met...</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/7e6a86b1c25e5fd05733c52c118848341aba1c4e"><code>7e6a86b</code></a> Upload OpsLevel YAML (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/849">#849</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/74d5719bd03993fcf71e3b176621f133eb6138c0"><code>74d5719</code></a> docs: update references vercel/ms references (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/770">#770</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/d71e383862fc735991fd2e759181480f066bf138"><code>d71e383</code></a> docs: document &quot;invalid token&quot; error</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/37650031fd0bac1a5b0d682bbfcf8c1705917aa9"><code>3765003</code></a> docs: fix spelling in README.md: Peak -&gt; Peek (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/754">#754</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/a46097e962621ab2ba718d1da6025cdeba3597c8"><code>a46097e</code></a> docs: make decode impossible to discover before verify</li>
<li>Additional commits viewable in <a href="https://github.com/auth0/node-jsonwebtoken/compare/v8.5.1...v9.0.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~julien.wollscheid">julien.wollscheid</a>, a new releaser for jsonwebtoken since your current version.</p>
</details>
<br />

Updates `@nestjs/jwt` from 8.0.1 to 10.0.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/jwt/releases"><code>@​nestjs/jwt</code>'s releases</a>.</em></p>
<blockquote>
<h2>Release 10.0.1</h2>
<ul>
<li>chore(husky): change npx --no to --no-install (7218087)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1144">#1144</a> from nestjs/renovate/typescript-eslint-monorepo (0274acc)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1150">#1150</a> from nestjs/renovate/prettier-2.x (c6bbf14)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.47.1 (414aea3)</li>
<li>chore(deps): update dependency prettier to v2.8.1 (44fd45a)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1149">#1149</a> from nestjs/renovate/commitlint-monorepo (d8ed56a)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1057">#1057</a> from nestjs/renovate/jsonwebtoken-8.x (74a21f9)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1159">#1159</a> from nestjs/renovate/release-it-15.x (f367329)</li>
<li>chore(deps): update dependency release-it to v15.5.1 (b3f4fc7)</li>
<li>chore(deps): update commitlint monorepo to v17.3.0 (15ad133)</li>
<li>fix(deps): update dependency <code>@​types/jsonwebtoken</code> to v8.5.9 (d14521f)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1158">#1158</a> from nestjs/renovate/node-18.x (cc04cce)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.11.18 (3ebfaf0)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1146">#1146</a> from nestjs/renovate/typescript-4.x (a14a3be)</li>
<li>chore(deps): update dependency typescript to v4.9.4 (df59940)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1157">#1157</a> from nestjs/dependabot/npm_and_yarn/minimatch-3.1.2 (e5661b9)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1151">#1151</a> from nestjs/renovate/lint-staged-13.x (8d74976)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1148">#1148</a> from nestjs/renovate/eslint-8.x (76b0ee3)</li>
<li>chore(deps): bump minimatch from 3.0.4 to 3.1.2 (f3dd100)</li>
<li>chore(deps): update dependency lint-staged to v13.1.0 (7b3319a)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1145">#1145</a> from nestjs/renovate/jest-monorepo (a97c753)</li>
<li>Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1155">#1155</a> from nestjs/renovate/npm-jsonwebtoken-vulnerability (73a7440)</li>
<li>chore(deps): update dependency eslint to v8.30.0 (8a6a459)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.2.4 (20c2366)</li>
<li>chore(deps): update dependency jsonwebtoken to 9.0.0 [security] (98a4464)</li>
<li>chore: use npm v8 (27d843c)</li>
<li>chore(deps): update dependency jest to v29.3.1 (ef435fb)</li>
<li>chore(deps): update dependency husky to v8.0.2 (9582491)</li>
<li>chore(deps): update dependency jest to v29.3.0 (52fef84)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.42.1 (e2d47cc)</li>
<li>chore(deps): update nest monorepo to v9.2.0 (fcb7300)</li>
<li>chore(deps): update dependency eslint to v8.27.0 (8d99cb8)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.2.2 (8094086)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.11.9 (f36d84b)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.2.1 (c15602f)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.42.0 (ca2de19)</li>
<li>chore(deps): update commitlint monorepo to v17.2.0 (a5ed87c)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.11.8 (78834c9)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.11.7 (3a6ce6f)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.11.6 (8235062)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18 (697649c)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.41.0 (a168713)</li>
<li>chore(deps): update dependency jest to v29.2.2 (44181e6)</li>
<li>chore(deps): update nest monorepo to v9.1.6 (79a5f32)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v16.18.0 (167b84f)</li>
<li>chore(deps): update dependency eslint to v8.26.0 (76af6b2)</li>
<li>chore(deps): update nest monorepo to v9.1.5 (ab124c9)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v16.11.68 (5cc2ce3)</li>
<li>chore(deps): update dependency jest to v29.2.1 (41bdc6a)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/jwt/commit/53b90d0cf84243ac32e463e9633b9a882a6d2e18"><code>53b90d0</code></a> chore(): release v10.0.1</li>
<li><a href="https://github.com/nestjs/jwt/commit/7218087455f9e0e43ba10333e3a245823f988bab"><code>7218087</code></a> chore(husky): change npx --no to --no-install</li>
<li><a href="https://github.com/nestjs/jwt/commit/0274acc621d5613753695c211d4fa083b32a60d2"><code>0274acc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1144">#1144</a> from nestjs/renovate/typescript-eslint-monorepo</li>
<li><a href="https://github.com/nestjs/jwt/commit/c6bbf14f715bd931bd2aa67b8ae62790ea2b8ec9"><code>c6bbf14</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1150">#1150</a> from nestjs/renovate/prettier-2.x</li>
<li><a href="https://github.com/nestjs/jwt/commit/414aea31886e4902452742b2ceff807cf79e08dc"><code>414aea3</code></a> chore(deps): update typescript-eslint monorepo to v5.47.1</li>
<li><a href="https://github.com/nestjs/jwt/commit/44fd45aee78f89a1a9c7a6da8decc39a35091a2d"><code>44fd45a</code></a> chore(deps): update dependency prettier to v2.8.1</li>
<li><a href="https://github.com/nestjs/jwt/commit/d8ed56ab98aff9b0e14e563aeca4b56b557fe2a3"><code>d8ed56a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1149">#1149</a> from nestjs/renovate/commitlint-monorepo</li>
<li><a href="https://github.com/nestjs/jwt/commit/74a21f94c36a52abc30926aefc3749341f648f00"><code>74a21f9</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1057">#1057</a> from nestjs/renovate/jsonwebtoken-8.x</li>
<li><a href="https://github.com/nestjs/jwt/commit/f367329524a306ae9cf792225b43ba159943935c"><code>f367329</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nestjs/jwt/issues/1159">#1159</a> from nestjs/renovate/release-it-15.x</li>
<li><a href="https://github.com/nestjs/jwt/commit/b3f4fc7a046950b7f9bd146019d1bc3cce9b4eb1"><code>b3f4fc7</code></a> chore(deps): update dependency release-it to v15.5.1</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/jwt/compare/8.0.1...10.0.1">compare view</a></li>
</ul>
</details>
<br />

Updates `passport-jwt` from 4.0.0 to 4.0.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/fed94fa005c5b2dcb7e6d5d5372e3b20cae898f1"><code>fed94fa</code></a> 4.0.1 release</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/cfb5566413849ab0836c7785cc5d1d108976d576"><code>cfb5566</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mikenicholson/passport-jwt/issues/248">#248</a> from mikenicholson/update-minmatch</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/8e4ad5b8d2ba4056f53205a8137b74a24e2b0709"><code>8e4ad5b</code></a> Address minmatch vulnerability</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/e9cf2ce08a312130ac4ee40d37a8cc7b2249c953"><code>e9cf2ce</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mikenicholson/passport-jwt/issues/247">#247</a> from mikenicholson/jsonwebtoken-9</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/bfbc6cc6132cf487ce76bf5560965b589d68a56b"><code>bfbc6cc</code></a> Update jsonwebtoken to 9.0.0</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/a49b43e3364cd1bdc60131e4e17dfb07db5e6283"><code>a49b43e</code></a> Update minimist due to prototype pollution vulnerability in previous version</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/a5137c67dedc4c08d718782d2d0d9f40f2ded956"><code>a5137c6</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mikenicholson/passport-jwt/issues/192">#192</a> from markhoney/patch-1</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/ea824cd3a63885a1795a2c119306cc770dbfb78e"><code>ea824cd</code></a> Update jsonwebtoken and run npm audit fix</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/8e57eec8033c805006e16e33b42658046e1f4ff4"><code>8e57eec</code></a> Remove older node versions shiping npm without support for &quot;ci&quot;</li>
<li><a href="https://github.com/mikenicholson/passport-jwt/commit/3ab9305209fe8bb4d62405400608407f29b127c0"><code>3ab9305</code></a> Add CI workflow in GitHub Actions</li>
<li>Additional commits viewable in <a href="https://github.com/mikenicholson/passport-jwt/compare/v4.0.0...v4.0.1">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 08:56:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    Bump json5 from 2.2.1 to 2.2.3 in /platform/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 2.2.1 to 2.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=2.2.1&new-version=2.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 08:56:50 +0000 UTC
    </div>
</div>

