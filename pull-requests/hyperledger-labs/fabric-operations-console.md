---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/548" class=".btn">#548</a>
            </td>
            <td>
                <b>
                    Bump browserify-sign from 4.2.1 to 4.2.2 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [browserify-sign](https://github.com/crypto-browserify/browserify-sign) from 4.2.1 to 4.2.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/browserify/browserify-sign/blob/main/CHANGELOG.md">browserify-sign's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/browserify/browserify-sign/compare/v4.2.1...v4.2.2">v4.2.2</a> - 2023-10-25</h2>
<h3>Fixed</h3>
<ul>
<li>[Tests] log when openssl doesn't support cipher <a href="https://redirect.github.com/browserify/browserify-sign/issues/37"><code>[#37](https://github.com/crypto-browserify/browserify-sign/issues/37)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>Only apps should have lockfiles <a href="https://github.com/browserify/browserify-sign/commit/09a89959393b3c89fedd4f7f3bafa4fec44371d7"><code>09a8995</code></a></li>
<li>[eslint] switch to eslint <a href="https://github.com/browserify/browserify-sign/commit/83fe46374b819e959d56d2c0b931308f7451a664"><code>83fe463</code></a></li>
<li>[meta] add <code>npmignore</code> and <code>auto-changelog</code> <a href="https://github.com/browserify/browserify-sign/commit/44181838e7dcc4d5d0c568f74312ea28f0bcdfd5"><code>4418183</code></a></li>
<li>[meta] fix package.json indentation <a href="https://github.com/browserify/browserify-sign/commit/9ac5a5eaaac8a11eb70ec2febd13745c8764ae02"><code>9ac5a5e</code></a></li>
<li>[Tests] migrate from travis to github actions <a href="https://github.com/browserify/browserify-sign/commit/d845d855def38e2085d5a21e447a48300f99fa60"><code>d845d85</code></a></li>
<li>[Fix] <code>sign</code>: throw on unsupported padding scheme <a href="https://github.com/browserify/browserify-sign/commit/8767739a4516289568bcce9fed8a3b7e23478de9"><code>8767739</code></a></li>
<li>[Fix] properly check the upper bound for DSA signatures <a href="https://github.com/browserify/browserify-sign/commit/85994cd6348b50f2fd1b73c54e20881416f44a30"><code>85994cd</code></a></li>
<li>[Tests] handle openSSL not supporting a scheme <a href="https://github.com/browserify/browserify-sign/commit/f5f17c27f9824de40b5ce8ebd8502111203fd6af"><code>f5f17c2</code></a></li>
<li>[Deps] update <code>bn.js</code>, <code>browserify-rsa</code>, <code>elliptic</code>, <code>parse-asn1</code>, <code>readable-stream</code>, <code>safe-buffer</code> <a href="https://github.com/browserify/browserify-sign/commit/a67d0eb4ffceabb366b69da69ce9a223e9d5e96b"><code>a67d0eb</code></a></li>
<li>[Dev Deps] update <code>nyc</code>, <code>standard</code>, <code>tape</code> <a href="https://github.com/browserify/browserify-sign/commit/cc5350b96702fcba930e0662cf763844fd2f59bf"><code>cc5350b</code></a></li>
<li>[Tests] always run coverage; downgrade <code>nyc</code> <a href="https://github.com/browserify/browserify-sign/commit/75ce1d5c49a6591dd13422016c07f8f9cae13371"><code>75ce1d5</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/browserify/browserify-sign/commit/dcf49ce85a1a66a6fb31689508d916d7894286a9"><code>dcf49ce</code></a></li>
<li>[Tests] add <code>npm run posttest</code> <a href="https://github.com/browserify/browserify-sign/commit/75dd8fd6ce56eb37b12e30807e5f913867b21733"><code>75dd8fd</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/browserify/browserify-sign/commit/3aec0386dc8dfba8698be756ec770df863867c84"><code>3aec038</code></a></li>
<li>[Tests] skip unsupported schemes <a href="https://github.com/browserify/browserify-sign/commit/703c83ea72db2f45714fe749c6f04b05243ca9a8"><code>703c83e</code></a></li>
<li>[Tests] node &lt; 6 lacks array <code>includes</code> <a href="https://github.com/browserify/browserify-sign/commit/3aa43cfbc1fdde8481bcdd3bff581574159b869a"><code>3aa43cf</code></a></li>
<li>[Dev Deps] fix eslint range <a href="https://github.com/browserify/browserify-sign/commit/98d4e0d7ff18871b0ca07415f758a610ccf8ebbe"><code>98d4e0d</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/browserify/browserify-sign/commit/4af5a90bf8acd9e76e5671dc0497f6ba71968a2c"><code>4af5a90</code></a> v4.2.2</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/3aec0386dc8dfba8698be756ec770df863867c84"><code>3aec038</code></a> [Dev Deps] update <code>tape</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/85994cd6348b50f2fd1b73c54e20881416f44a30"><code>85994cd</code></a> [Fix] properly check the upper bound for DSA signatures</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/9ac5a5eaaac8a11eb70ec2febd13745c8764ae02"><code>9ac5a5e</code></a> [meta] fix package.json indentation</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/dcf49ce85a1a66a6fb31689508d916d7894286a9"><code>dcf49ce</code></a> [meta] add <code>safe-publish-latest</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/44181838e7dcc4d5d0c568f74312ea28f0bcdfd5"><code>4418183</code></a> [meta] add <code>npmignore</code> and <code>auto-changelog</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/8767739a4516289568bcce9fed8a3b7e23478de9"><code>8767739</code></a> [Fix] <code>sign</code>: throw on unsupported padding scheme</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/5f6fb1755917851a40249db7d834da4265ed5950"><code>5f6fb17</code></a> [Tests] log when openssl doesn't support cipher</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/f5f17c27f9824de40b5ce8ebd8502111203fd6af"><code>f5f17c2</code></a> [Tests] handle openSSL not supporting a scheme</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/d845d855def38e2085d5a21e447a48300f99fa60"><code>d845d85</code></a> [Tests] migrate from travis to github actions</li>
<li>Additional commits viewable in <a href="https://github.com/crypto-browserify/browserify-sign/compare/v4.2.1...v4.2.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for browserify-sign since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=browserify-sign&package-manager=npm_and_yarn&previous-version=4.2.1&new-version=4.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-27 19:18:36 +0000 UTC
    </div>
</div>

