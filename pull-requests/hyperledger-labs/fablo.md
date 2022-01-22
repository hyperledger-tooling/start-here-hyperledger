---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Bump nanoid from 3.1.22 to 3.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [nanoid](https://github.com/ai/nanoid) from 3.1.22 to 3.2.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ai/nanoid/blob/main/CHANGELOG.md">nanoid's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<p>This project adheres to <a href="http://semver.org/">Semantic Versioning</a>.</p>
<h2>3.2</h2>
<ul>
<li>Added <code>--size</code> and <code>--alphabet</code> arguments to binary (by Vitaly Baev).</li>
</ul>
<h2>3.1.32</h2>
<ul>
<li>Reduced <code>async</code> exports size (by Artyom Arutyunyan).</li>
<li>Moved from Jest to uvu (by Vitaly Baev).</li>
</ul>
<h2>3.1.31</h2>
<ul>
<li>Fixed collision vulnerability on object in <code>size</code> (by Artyom Arutyunyan).</li>
</ul>
<h2>3.1.30</h2>
<ul>
<li>Reduced size for project with <code>brotli</code> compression (by Anton Khlynovskiy).</li>
</ul>
<h2>3.1.29</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.28</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.27</h2>
<ul>
<li>Cleaned <code>dependencies</code> from development tools.</li>
</ul>
<h2>3.1.26</h2>
<ul>
<li>Improved performance (by Eitan Har-Shoshanim).</li>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.25</h2>
<ul>
<li>Fixed <code>browserify</code> support.</li>
</ul>
<h2>3.1.24</h2>
<ul>
<li>Fixed <code>browserify</code> support (by Artur Paikin).</li>
</ul>
<h2>3.1.23</h2>
<ul>
<li>Fixed <code>esbuild</code> support.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ai/nanoid/commit/23b136929a6d58f32e31b269534a3ce3f680a086"><code>23b1369</code></a> Release 3.2 version</li>
<li><a href="https://github.com/ai/nanoid/commit/967788efce880960512f969a56f8f22f3fc20bae"><code>967788e</code></a> Remove TS test tools</li>
<li><a href="https://github.com/ai/nanoid/commit/27eaa90cd207a7782bbcf17343092ae87dd62164"><code>27eaa90</code></a> Simplify new binary tool</li>
<li><a href="https://github.com/ai/nanoid/commit/a9d91239931dc77506381874826d297aee71d6ef"><code>a9d9123</code></a> Update dependencies</li>
<li><a href="https://github.com/ai/nanoid/commit/32b9bdaab1fbc28576b17de8516164ce0360f292"><code>32b9bda</code></a> Allows passing size or custom alphabet via cli as args (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/334">#334</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/246d5f87b6b34e23b5e401bdf3da1f80c810ac4c"><code>246d5f8</code></a> Update vite</li>
<li><a href="https://github.com/ai/nanoid/commit/afdf9c92b41427f35476fbe14b5af5d73dd7fbdb"><code>afdf9c9</code></a> doc: Fixed Typo (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/335">#335</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/90a446fef3ecaac78e5af2ea01025c4f40182e2b"><code>90a446f</code></a> Update benchmark results</li>
<li><a href="https://github.com/ai/nanoid/commit/8ba2319b579895cc1f9060b9946a44852f97c509"><code>8ba2319</code></a> bench: add <code>@​napi-rs/uuid</code> v4 (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/333">#333</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/f4257780ece488734a65c176e80c2fd8ab6aab8e"><code>f425778</code></a> Release 3.1.32 version</li>
<li>Additional commits viewable in <a href="https://github.com/ai/nanoid/compare/3.1.22...3.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nanoid&package-manager=npm_and_yarn&previous-version=3.1.22&new-version=3.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-22 01:42:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.1 to 1.14.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.1 to 1.14.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ede36d7c60d3acdcd324dcd99a9dbd52e4fb3a6"><code>2ede36d</code></a> Release version 1.14.7 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8b347cbcef7c7b72a6e9be20f5710c17d6163c22"><code>8b347cb</code></a> Drop Cookie header across domains.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/6f5029ae1a0fdab4dc25f6379a5ee303c2319070"><code>6f5029a</code></a> Release version 1.14.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/af706bee57de954414c0bde0a9f33e62beea3e52"><code>af706be</code></a> Ignore null headers.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d01ab7a5c5df3617c7a40a03de7af6427fdfac55"><code>d01ab7a</code></a> Release version 1.14.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/40052ea8aa13559becee5795715c1d45b1f0eb76"><code>40052ea</code></a> Make compatible with Node 17.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/86f7572f9365dadc39f85916259b58973819617f"><code>86f7572</code></a> Fix: clear internal timer on request abort to avoid leakage</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2e1eaf0218c5315a2ab27f53964d0535d4dafb51"><code>2e1eaf0</code></a> Keep Authorization header on subdomain redirects.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ad9e82b6277ae2104f7770e9ff1186cc6da29d4"><code>2ad9e82</code></a> Carry over Host header on relative redirects (<a href="https://github-redirect.dependabot.com/follow-redirects/follow-redirects/issues/172">#172</a>)</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/77e2a581e1d1811674b7b74745a9c20a5b939488"><code>77e2a58</code></a> Release version 1.14.4 of the npm package.</li>
<li>Additional commits viewable in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.1...v1.14.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.1&new-version=1.14.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 07:43:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Bump shelljs from 0.8.4 to 0.8.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shelljs](https://github.com/shelljs/shelljs) from 0.8.4 to 0.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/shelljs/shelljs/releases">shelljs's releases</a>.</em></p>
<blockquote>
<h2>v0.8.5</h2>
<p>This was a small security fix for <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1058">#1058</a>.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/shelljs/shelljs/commit/70668a4555c7d49c4f67d53ea063b899be4d6d40"><code>70668a4</code></a> 0.8.5</li>
<li><a href="https://github.com/shelljs/shelljs/commit/d919d22dd6de385edaa9d90313075a77f74b338c"><code>d919d22</code></a> fix(exec): lockdown file permissions (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1060">#1060</a>)</li>
<li>See full diff in <a href="https://github.com/shelljs/shelljs/compare/v0.8.4...v0.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=shelljs&package-manager=npm_and_yarn&previous-version=0.8.4&new-version=0.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 07:00:33 +0000 UTC
    </div>
</div>

