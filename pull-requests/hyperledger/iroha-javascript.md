---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/minimistjs/minimist) from 1.2.5 to 1.2.8.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/minimistjs/minimist/blob/main/CHANGELOG.md">minimist's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.7...v1.2.8">v1.2.8</a> - 2023-02-09</h2>
<h3>Merged</h3>
<ul>
<li>[Fix] Fix long option followed by single dash <a href="https://github-redirect.dependabot.com/minimistjs/minimist/pull/17"><code>[#17](https://github.com/minimistjs/minimist/issues/17)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://github-redirect.dependabot.com/minimistjs/minimist/pull/12"><code>[#12](https://github.com/minimistjs/minimist/issues/12)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://github-redirect.dependabot.com/minimistjs/minimist/pull/10"><code>[#10](https://github.com/minimistjs/minimist/issues/10)</code></a></li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[Fix] Fix long option followed by single dash (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/17">#17</a>) <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Tests] Remove duplicate test (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/12">#12</a>) <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] Fix long option followed by single dash <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Fix] opt.string works with multiple aliases (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/10">#10</a>) <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
<li>[Fix] Fix handling of short option with non-trivial equals <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/5"><code>[#5](https://github.com/minimistjs/minimist/issues/5)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>Merge tag 'v0.2.3' <a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/5368ca4147e974138a54cc0dc4cea8f756546b70"><code>5368ca4</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/e5f5067259ceeaf0b098d14bec910f87e58708c7"><code>e5f5067</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/62fde7d935f83417fb046741531a9e2346a36976"><code>62fde7d</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/36ac5d0d95e4947d074e5737d94814034ca335d1"><code>36ac5d0</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/minimistjs/minimist/commit/73923d223553fca08b1ba77e3fbc2a492862ae4c"><code>73923d2</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/minimistjs/minimist/commit/d80727df77bfa9e631044d7f16368d8f09242c91"><code>d80727d</code></a></li>
<li>[eslint] add eslint; rules to enable later are warnings <a href="https://github.com/minimistjs/minimist/commit/48bc06a1b41f00e9cdf183db34f7a51ba70e98d4"><code>48bc06a</code></a></li>
<li>[eslint] fix indentation <a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a></li>
<li>[readme] rename and add badges <a href="https://github.com/minimistjs/minimist/commit/5df0fe49211bd09a3636f8686a7cb3012c3e98f0"><code>5df0fe4</code></a></li>
<li>[Dev Deps] switch from <code>covert</code> to <code>nyc</code> <a href="https://github.com/minimistjs/minimist/commit/a48b128fdb8d427dfb20a15273f83e38d97bef07"><code>a48b128</code></a></li>
<li>[Dev Deps] update <code>covert</code>, <code>tape</code>; remove unnecessary <code>tap</code> <a href="https://github.com/minimistjs/minimist/commit/f0fb958e9a1fe980cdffc436a211b0bda58f621b"><code>f0fb958</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/minimistjs/minimist/commit/3639e0c819359a366387e425ab6eabf4c78d3caa"><code>3639e0c</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/minimistjs/minimist/commit/be2e038c342d8333b32f0fde67a0026b79c8150e"><code>be2e038</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/minimistjs/minimist/commit/282b570e7489d01b03f2d6d3dabf79cd3e5f84cf"><code>282b570</code></a></li>
<li>isConstructorOrProto adapted from PR <a href="https://github.com/minimistjs/minimist/commit/ef9153fc52b6cea0744b2239921c5dcae4697f11"><code>ef9153f</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/3124ed3e46306301ebb3c834874ce0241555c2c4"><code>3124ed3</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/minimistjs/minimist/commit/4b927de696d561c636b4f43bf49d4597cb36d6d6"><code>4b927de</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/minimistjs/minimist/commit/b32d9bd0ab340f4e9f8c3a97ff2a4424f25fab8c"><code>b32d9bd</code></a></li>
<li>[meta] update repo URLs <a href="https://github.com/minimistjs/minimist/commit/f9fdfc032c54884d9a9996a390c63cd0719bbe1a"><code>f9fdfc0</code></a></li>
<li>[actions] Avoid 0.6 tests due to build failures <a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/minimistjs/minimist/commit/950eaa74f112e04d23e9c606c67472c46739b473"><code>950eaa7</code></a></li>
<li>[Dev Deps] add missing <code>npmignore</code> dev dep <a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a></li>
<li>Merge tag 'v0.2.2' <a href="https://github.com/minimistjs/minimist/commit/980d7ac61a0b4bd552711251ac107d506b23e41f"><code>980d7ac</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.6...v1.2.7">v1.2.7</a> - 2022-10-10</h2>
<h3>Commits</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/minimistjs/minimist/commit/6901ee286bc4c16da6830b48b46ce1574703cea1"><code>6901ee2</code></a> v1.2.8</li>
<li><a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a> Merge tag 'v0.2.3'</li>
<li><a href="https://github.com/minimistjs/minimist/commit/c0b26618322e94adea26c68e613ef0be482c6c63"><code>c0b2661</code></a> v0.2.3</li>
<li><a href="https://github.com/minimistjs/minimist/commit/63b8fee87b8e7a003216d5d77ba5d6decf3cfb0d"><code>63b8fee</code></a> [Fix] Fix long option followed by single dash (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/17">#17</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/72239e6f0ea77d8be0ad4f682b7ae7d142144395"><code>72239e6</code></a> [Tests] Remove duplicate test (<a href="https://github-redirect.dependabot.com/minimistjs/minimist/issues/12">#12</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a> [eslint] fix indentation</li>
<li><a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a> [Dev Deps] add missing <code>npmignore</code> dev dep</li>
<li><a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a> [Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/9ec4d279ced72ea2f60237218e71cc03aa0dfdd6"><code>9ec4d27</code></a> [Fix] Fix long option followed by single dash</li>
<li><a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a> [actions] Avoid 0.6 tests due to build failures</li>
<li>Additional commits viewable in <a href="https://github.com/minimistjs/minimist/compare/v1.2.5...v1.2.8">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for minimist since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-04 03:29:01 +0000 UTC
    </div>
</div>

