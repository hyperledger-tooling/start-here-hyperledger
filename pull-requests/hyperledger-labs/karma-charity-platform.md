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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    Bump json5 from 2.2.0 to 2.2.3 in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 2.2.0 to 2.2.3.
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
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
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
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=2.2.0&new-version=2.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-03 04:57:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths in /chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies need to be updated together.

Updates `json5` from 1.0.1 to 2.2.3
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
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v1.0.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.14.1 to 4.1.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[4.1.2] - 2023-01-02</h2>
<h3>Fixed</h3>
<ul>
<li>Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/232">#232</a>. Thanks to <a href="https://github.com/oparisblue"><code>@​oparisblue</code></a> for this PR!</li>
</ul>
<h2>[4.1.1] - 2022-11-30</h2>
<h3>Fixed</h3>
<ul>
<li>Skip stat call / throwing an exception when source files don't exist. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/225">#225</a>. Thanks to <a href="https://github.com/robstolarz"><code>@​robstolarz</code></a> for this PR!</li>
</ul>
<h2>[4.1.0] - 2022-08-06</h2>
<ul>
<li>Add support for nested main field selectors #. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/218">#218</a>. Thanks to <a href="https://github.com/aaronadamsCA"><code>@​aaronadamsCA</code></a> for this PR!</li>
</ul>
<h2>[4.0.0] - 2022-05-02</h2>
<h3>Changed</h3>
<ul>
<li>Ignore <code>--project</code>/<code>-P</code> CLI flag when explicit options are passed to <code>register</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/206">#206</a>.</li>
<li>Tolerate an undefined <code>baseUrl</code> compiler option. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/208">#208</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>cwd</code> option to <code>register</code> function that overrides where the <code>tsconfig.json</code> search begins. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/205">#205</a>.</li>
<li>Add support for <code>jsconfig.json</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/199">#199</a>. Thanks to <a href="https://github.com/F3n67u"><code>@​F3n67u</code></a> for this PR!</li>
<li>Let <code>paths</code> mappings be absolute paths. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/184">#184</a>.</li>
<li>Allow <code>baseUrl</code> in <code>tsconfig.json</code> to be an absolute path. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/174">#174</a>. Thanks to <a href="https://github.com/nwalters512"><code>@​nwalters512</code></a> for this PR!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/76dab7661d3cc158c751eba64b363b1d5e032e0f"><code>76dab76</code></a> v4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/4a5bfeed6a3bc4a0f34ae4a16ad376529e03a6a0"><code>4a5bfee</code></a> Update changelog for 4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9721a98718c9f6a35bb4029292204aaa90474bab"><code>9721a98</code></a> Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175 (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/232">#232</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/1b71683fa7d48a2e7b9cbae4825410594a1c7c81"><code>1b71683</code></a> v4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/73fdd5991d6542df4da0a6d22dbb18f5656b091d"><code>73fdd59</code></a> Update changelog for 4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/b732fcf0b894a65af5e997b284c40fc3e155837d"><code>b732fcf</code></a> Skip stat call / throwing when files don't exist (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/225">#225</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/206e49a4dd016e9f7086c8a938266f74f9301568"><code>206e49a</code></a> v4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/e71c964000808500a34d7ac4ced6c8b7e98b99b3"><code>e71c964</code></a> Update changelog for 4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9124aa60f18efb52562431d0ec8dd03b4b36ba6a"><code>9124aa6</code></a> Add support for nested main field selectors (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/218">#218</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f42003925f4d56458d41daed80013c8ad23c88ea"><code>f420039</code></a> Explicitly specify minimum Node.js version (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/212">#212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.14.1...v4.1.2">compare view</a></li>
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
        Created At 2023-01-03 04:56:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths in /explorer/backend/src/packages/application/api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies need to be updated together.

Updates `json5` from 1.0.1 to 2.2.3
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
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v1.0.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.12.0 to 4.1.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[4.1.2] - 2023-01-02</h2>
<h3>Fixed</h3>
<ul>
<li>Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/232">#232</a>. Thanks to <a href="https://github.com/oparisblue"><code>@​oparisblue</code></a> for this PR!</li>
</ul>
<h2>[4.1.1] - 2022-11-30</h2>
<h3>Fixed</h3>
<ul>
<li>Skip stat call / throwing an exception when source files don't exist. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/225">#225</a>. Thanks to <a href="https://github.com/robstolarz"><code>@​robstolarz</code></a> for this PR!</li>
</ul>
<h2>[4.1.0] - 2022-08-06</h2>
<ul>
<li>Add support for nested main field selectors #. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/218">#218</a>. Thanks to <a href="https://github.com/aaronadamsCA"><code>@​aaronadamsCA</code></a> for this PR!</li>
</ul>
<h2>[4.0.0] - 2022-05-02</h2>
<h3>Changed</h3>
<ul>
<li>Ignore <code>--project</code>/<code>-P</code> CLI flag when explicit options are passed to <code>register</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/206">#206</a>.</li>
<li>Tolerate an undefined <code>baseUrl</code> compiler option. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/208">#208</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>cwd</code> option to <code>register</code> function that overrides where the <code>tsconfig.json</code> search begins. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/205">#205</a>.</li>
<li>Add support for <code>jsconfig.json</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/199">#199</a>. Thanks to <a href="https://github.com/F3n67u"><code>@​F3n67u</code></a> for this PR!</li>
<li>Let <code>paths</code> mappings be absolute paths. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/184">#184</a>.</li>
<li>Allow <code>baseUrl</code> in <code>tsconfig.json</code> to be an absolute path. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/174">#174</a>. Thanks to <a href="https://github.com/nwalters512"><code>@​nwalters512</code></a> for this PR!</li>
</ul>
<h2>[3.14.1] - 2022-03-22</h2>
<h3>Fixed</h3>
<ul>
<li>Use minimist 1.2.6 for all depencencies becuase of pollution vulnerability. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/197">#197</a>. Thanks to <a href="https://github.com/gopijaganthan"><code>@​gopijaganthan</code></a> for this fix!</li>
</ul>
<h2>[3.14.0] - 2022-03-13</h2>
<h3>Added</h3>
<ul>
<li>Support for path mapping starting with <code>/</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/180">#180</a>, issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/113">#113</a>, and issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/128">#128</a>. Thanks to <a href="https://github.com/benevbright"><code>@​benevbright</code></a> for this fix!</li>
</ul>
<h2>[3.13.0] - 2022-03-03</h2>
<h3>Added</h3>
<ul>
<li>Include file extension in paths resolved from package.json &quot;main&quot; field. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/135">#135</a> and issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/133">#133</a>. Thanks to <a href="https://github.com/katywings"><code>@​katywings</code></a> for this fix!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/76dab7661d3cc158c751eba64b363b1d5e032e0f"><code>76dab76</code></a> v4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/4a5bfeed6a3bc4a0f34ae4a16ad376529e03a6a0"><code>4a5bfee</code></a> Update changelog for 4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9721a98718c9f6a35bb4029292204aaa90474bab"><code>9721a98</code></a> Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175 (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/232">#232</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/1b71683fa7d48a2e7b9cbae4825410594a1c7c81"><code>1b71683</code></a> v4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/73fdd5991d6542df4da0a6d22dbb18f5656b091d"><code>73fdd59</code></a> Update changelog for 4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/b732fcf0b894a65af5e997b284c40fc3e155837d"><code>b732fcf</code></a> Skip stat call / throwing when files don't exist (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/225">#225</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/206e49a4dd016e9f7086c8a938266f74f9301568"><code>206e49a</code></a> v4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/e71c964000808500a34d7ac4ced6c8b7e98b99b3"><code>e71c964</code></a> Update changelog for 4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9124aa60f18efb52562431d0ec8dd03b4b36ba6a"><code>9124aa6</code></a> Add support for nested main field selectors (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/218">#218</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f42003925f4d56458d41daed80013c8ad23c88ea"><code>f420039</code></a> Explicitly specify minimum Node.js version (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/212">#212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.12.0...v4.1.2">compare view</a></li>
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
        Created At 2023-01-03 04:56:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths in /chaincode/src/packages/application/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies need to be updated together.

Updates `json5` from 1.0.1 to 2.2.3
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
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v1.0.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.14.1 to 4.1.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[4.1.2] - 2023-01-02</h2>
<h3>Fixed</h3>
<ul>
<li>Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/232">#232</a>. Thanks to <a href="https://github.com/oparisblue"><code>@​oparisblue</code></a> for this PR!</li>
</ul>
<h2>[4.1.1] - 2022-11-30</h2>
<h3>Fixed</h3>
<ul>
<li>Skip stat call / throwing an exception when source files don't exist. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/225">#225</a>. Thanks to <a href="https://github.com/robstolarz"><code>@​robstolarz</code></a> for this PR!</li>
</ul>
<h2>[4.1.0] - 2022-08-06</h2>
<ul>
<li>Add support for nested main field selectors #. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/218">#218</a>. Thanks to <a href="https://github.com/aaronadamsCA"><code>@​aaronadamsCA</code></a> for this PR!</li>
</ul>
<h2>[4.0.0] - 2022-05-02</h2>
<h3>Changed</h3>
<ul>
<li>Ignore <code>--project</code>/<code>-P</code> CLI flag when explicit options are passed to <code>register</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/206">#206</a>.</li>
<li>Tolerate an undefined <code>baseUrl</code> compiler option. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/208">#208</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>cwd</code> option to <code>register</code> function that overrides where the <code>tsconfig.json</code> search begins. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/205">#205</a>.</li>
<li>Add support for <code>jsconfig.json</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/199">#199</a>. Thanks to <a href="https://github.com/F3n67u"><code>@​F3n67u</code></a> for this PR!</li>
<li>Let <code>paths</code> mappings be absolute paths. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/184">#184</a>.</li>
<li>Allow <code>baseUrl</code> in <code>tsconfig.json</code> to be an absolute path. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/174">#174</a>. Thanks to <a href="https://github.com/nwalters512"><code>@​nwalters512</code></a> for this PR!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/76dab7661d3cc158c751eba64b363b1d5e032e0f"><code>76dab76</code></a> v4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/4a5bfeed6a3bc4a0f34ae4a16ad376529e03a6a0"><code>4a5bfee</code></a> Update changelog for 4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9721a98718c9f6a35bb4029292204aaa90474bab"><code>9721a98</code></a> Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175 (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/232">#232</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/1b71683fa7d48a2e7b9cbae4825410594a1c7c81"><code>1b71683</code></a> v4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/73fdd5991d6542df4da0a6d22dbb18f5656b091d"><code>73fdd59</code></a> Update changelog for 4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/b732fcf0b894a65af5e997b284c40fc3e155837d"><code>b732fcf</code></a> Skip stat call / throwing when files don't exist (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/225">#225</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/206e49a4dd016e9f7086c8a938266f74f9301568"><code>206e49a</code></a> v4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/e71c964000808500a34d7ac4ced6c8b7e98b99b3"><code>e71c964</code></a> Update changelog for 4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9124aa60f18efb52562431d0ec8dd03b4b36ba6a"><code>9124aa6</code></a> Add support for nested main field selectors (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/218">#218</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f42003925f4d56458d41daed80013c8ad23c88ea"><code>f420039</code></a> Explicitly specify minimum Node.js version (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/212">#212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.14.1...v4.1.2">compare view</a></li>
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
        Created At 2023-01-03 04:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies need to be updated together.

Updates `json5` from 1.0.1 to 2.2.3
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
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v1.0.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.14.1 to 4.1.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[4.1.2] - 2023-01-02</h2>
<h3>Fixed</h3>
<ul>
<li>Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/232">#232</a>. Thanks to <a href="https://github.com/oparisblue"><code>@​oparisblue</code></a> for this PR!</li>
</ul>
<h2>[4.1.1] - 2022-11-30</h2>
<h3>Fixed</h3>
<ul>
<li>Skip stat call / throwing an exception when source files don't exist. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/225">#225</a>. Thanks to <a href="https://github.com/robstolarz"><code>@​robstolarz</code></a> for this PR!</li>
</ul>
<h2>[4.1.0] - 2022-08-06</h2>
<ul>
<li>Add support for nested main field selectors #. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/218">#218</a>. Thanks to <a href="https://github.com/aaronadamsCA"><code>@​aaronadamsCA</code></a> for this PR!</li>
</ul>
<h2>[4.0.0] - 2022-05-02</h2>
<h3>Changed</h3>
<ul>
<li>Ignore <code>--project</code>/<code>-P</code> CLI flag when explicit options are passed to <code>register</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/206">#206</a>.</li>
<li>Tolerate an undefined <code>baseUrl</code> compiler option. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/208">#208</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>cwd</code> option to <code>register</code> function that overrides where the <code>tsconfig.json</code> search begins. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/205">#205</a>.</li>
<li>Add support for <code>jsconfig.json</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/199">#199</a>. Thanks to <a href="https://github.com/F3n67u"><code>@​F3n67u</code></a> for this PR!</li>
<li>Let <code>paths</code> mappings be absolute paths. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/184">#184</a>.</li>
<li>Allow <code>baseUrl</code> in <code>tsconfig.json</code> to be an absolute path. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/174">#174</a>. Thanks to <a href="https://github.com/nwalters512"><code>@​nwalters512</code></a> for this PR!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/76dab7661d3cc158c751eba64b363b1d5e032e0f"><code>76dab76</code></a> v4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/4a5bfeed6a3bc4a0f34ae4a16ad376529e03a6a0"><code>4a5bfee</code></a> Update changelog for 4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9721a98718c9f6a35bb4029292204aaa90474bab"><code>9721a98</code></a> Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175 (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/232">#232</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/1b71683fa7d48a2e7b9cbae4825410594a1c7c81"><code>1b71683</code></a> v4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/73fdd5991d6542df4da0a6d22dbb18f5656b091d"><code>73fdd59</code></a> Update changelog for 4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/b732fcf0b894a65af5e997b284c40fc3e155837d"><code>b732fcf</code></a> Skip stat call / throwing when files don't exist (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/225">#225</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/206e49a4dd016e9f7086c8a938266f74f9301568"><code>206e49a</code></a> v4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/e71c964000808500a34d7ac4ced6c8b7e98b99b3"><code>e71c964</code></a> Update changelog for 4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9124aa60f18efb52562431d0ec8dd03b4b36ba6a"><code>9124aa6</code></a> Add support for nested main field selectors (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/218">#218</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f42003925f4d56458d41daed80013c8ad23c88ea"><code>f420039</code></a> Explicitly specify minimum Node.js version (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/212">#212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.14.1...v4.1.2">compare view</a></li>
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
        Created At 2023-01-03 04:56:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies need to be updated together.

Updates `json5` from 1.0.1 to 2.2.3
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
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v1.0.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.14.1 to 4.1.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[4.1.2] - 2023-01-02</h2>
<h3>Fixed</h3>
<ul>
<li>Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/232">#232</a>. Thanks to <a href="https://github.com/oparisblue"><code>@​oparisblue</code></a> for this PR!</li>
</ul>
<h2>[4.1.1] - 2022-11-30</h2>
<h3>Fixed</h3>
<ul>
<li>Skip stat call / throwing an exception when source files don't exist. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/225">#225</a>. Thanks to <a href="https://github.com/robstolarz"><code>@​robstolarz</code></a> for this PR!</li>
</ul>
<h2>[4.1.0] - 2022-08-06</h2>
<ul>
<li>Add support for nested main field selectors #. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/218">#218</a>. Thanks to <a href="https://github.com/aaronadamsCA"><code>@​aaronadamsCA</code></a> for this PR!</li>
</ul>
<h2>[4.0.0] - 2022-05-02</h2>
<h3>Changed</h3>
<ul>
<li>Ignore <code>--project</code>/<code>-P</code> CLI flag when explicit options are passed to <code>register</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/206">#206</a>.</li>
<li>Tolerate an undefined <code>baseUrl</code> compiler option. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/208">#208</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>cwd</code> option to <code>register</code> function that overrides where the <code>tsconfig.json</code> search begins. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/205">#205</a>.</li>
<li>Add support for <code>jsconfig.json</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/199">#199</a>. Thanks to <a href="https://github.com/F3n67u"><code>@​F3n67u</code></a> for this PR!</li>
<li>Let <code>paths</code> mappings be absolute paths. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/184">#184</a>.</li>
<li>Allow <code>baseUrl</code> in <code>tsconfig.json</code> to be an absolute path. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/174">#174</a>. Thanks to <a href="https://github.com/nwalters512"><code>@​nwalters512</code></a> for this PR!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/76dab7661d3cc158c751eba64b363b1d5e032e0f"><code>76dab76</code></a> v4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/4a5bfeed6a3bc4a0f34ae4a16ad376529e03a6a0"><code>4a5bfee</code></a> Update changelog for 4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9721a98718c9f6a35bb4029292204aaa90474bab"><code>9721a98</code></a> Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175 (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/232">#232</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/1b71683fa7d48a2e7b9cbae4825410594a1c7c81"><code>1b71683</code></a> v4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/73fdd5991d6542df4da0a6d22dbb18f5656b091d"><code>73fdd59</code></a> Update changelog for 4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/b732fcf0b894a65af5e997b284c40fc3e155837d"><code>b732fcf</code></a> Skip stat call / throwing when files don't exist (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/225">#225</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/206e49a4dd016e9f7086c8a938266f74f9301568"><code>206e49a</code></a> v4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/e71c964000808500a34d7ac4ced6c8b7e98b99b3"><code>e71c964</code></a> Update changelog for 4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9124aa60f18efb52562431d0ec8dd03b4b36ba6a"><code>9124aa6</code></a> Add support for nested main field selectors (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/218">#218</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f42003925f4d56458d41daed80013c8ad23c88ea"><code>f420039</code></a> Explicitly specify minimum Node.js version (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/212">#212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.14.1...v4.1.2">compare view</a></li>
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
        Created At 2023-01-03 04:56:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths in /platform/backend/src/packages/application/api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies need to be updated together.

Updates `json5` from 1.0.1 to 2.2.3
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
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v1.0.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.12.0 to 4.1.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[4.1.2] - 2023-01-02</h2>
<h3>Fixed</h3>
<ul>
<li>Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/232">#232</a>. Thanks to <a href="https://github.com/oparisblue"><code>@​oparisblue</code></a> for this PR!</li>
</ul>
<h2>[4.1.1] - 2022-11-30</h2>
<h3>Fixed</h3>
<ul>
<li>Skip stat call / throwing an exception when source files don't exist. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/225">#225</a>. Thanks to <a href="https://github.com/robstolarz"><code>@​robstolarz</code></a> for this PR!</li>
</ul>
<h2>[4.1.0] - 2022-08-06</h2>
<ul>
<li>Add support for nested main field selectors #. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/218">#218</a>. Thanks to <a href="https://github.com/aaronadamsCA"><code>@​aaronadamsCA</code></a> for this PR!</li>
</ul>
<h2>[4.0.0] - 2022-05-02</h2>
<h3>Changed</h3>
<ul>
<li>Ignore <code>--project</code>/<code>-P</code> CLI flag when explicit options are passed to <code>register</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/206">#206</a>.</li>
<li>Tolerate an undefined <code>baseUrl</code> compiler option. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/208">#208</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>cwd</code> option to <code>register</code> function that overrides where the <code>tsconfig.json</code> search begins. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/205">#205</a>.</li>
<li>Add support for <code>jsconfig.json</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/199">#199</a>. Thanks to <a href="https://github.com/F3n67u"><code>@​F3n67u</code></a> for this PR!</li>
<li>Let <code>paths</code> mappings be absolute paths. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/184">#184</a>.</li>
<li>Allow <code>baseUrl</code> in <code>tsconfig.json</code> to be an absolute path. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/174">#174</a>. Thanks to <a href="https://github.com/nwalters512"><code>@​nwalters512</code></a> for this PR!</li>
</ul>
<h2>[3.14.1] - 2022-03-22</h2>
<h3>Fixed</h3>
<ul>
<li>Use minimist 1.2.6 for all depencencies becuase of pollution vulnerability. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/197">#197</a>. Thanks to <a href="https://github.com/gopijaganthan"><code>@​gopijaganthan</code></a> for this fix!</li>
</ul>
<h2>[3.14.0] - 2022-03-13</h2>
<h3>Added</h3>
<ul>
<li>Support for path mapping starting with <code>/</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/180">#180</a>, issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/113">#113</a>, and issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/128">#128</a>. Thanks to <a href="https://github.com/benevbright"><code>@​benevbright</code></a> for this fix!</li>
</ul>
<h2>[3.13.0] - 2022-03-03</h2>
<h3>Added</h3>
<ul>
<li>Include file extension in paths resolved from package.json &quot;main&quot; field. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/135">#135</a> and issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/133">#133</a>. Thanks to <a href="https://github.com/katywings"><code>@​katywings</code></a> for this fix!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/76dab7661d3cc158c751eba64b363b1d5e032e0f"><code>76dab76</code></a> v4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/4a5bfeed6a3bc4a0f34ae4a16ad376529e03a6a0"><code>4a5bfee</code></a> Update changelog for 4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9721a98718c9f6a35bb4029292204aaa90474bab"><code>9721a98</code></a> Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175 (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/232">#232</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/1b71683fa7d48a2e7b9cbae4825410594a1c7c81"><code>1b71683</code></a> v4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/73fdd5991d6542df4da0a6d22dbb18f5656b091d"><code>73fdd59</code></a> Update changelog for 4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/b732fcf0b894a65af5e997b284c40fc3e155837d"><code>b732fcf</code></a> Skip stat call / throwing when files don't exist (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/225">#225</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/206e49a4dd016e9f7086c8a938266f74f9301568"><code>206e49a</code></a> v4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/e71c964000808500a34d7ac4ced6c8b7e98b99b3"><code>e71c964</code></a> Update changelog for 4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9124aa60f18efb52562431d0ec8dd03b4b36ba6a"><code>9124aa6</code></a> Add support for nested main field selectors (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/218">#218</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f42003925f4d56458d41daed80013c8ad23c88ea"><code>f420039</code></a> Explicitly specify minimum Node.js version (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/212">#212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.12.0...v4.1.2">compare view</a></li>
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
        Created At 2023-01-03 04:56:07 +0000 UTC
    </div>
</div>

