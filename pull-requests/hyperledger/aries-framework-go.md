---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3016" class=".btn">#3016</a>
            </td>
            <td>
                <b>
                    chore(deps): bump axios from 0.21.4 to 0.23.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.21.4 to 0.23.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>v0.23.0</h2>
<h3>0.23.0 (October 12, 2021)</h3>
<p>Breaking changes:</p>
<ul>
<li>Distinguish request and response data types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4116">#4116</a>)</li>
<li>Change never type to unknown (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4142">#4142</a>)</li>
<li>Fixed TransitionalOptions typings (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4147">#4147</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Adding globalObject: 'this' to webpack config (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3176">#3176</a>)</li>
<li>Adding insecureHTTPParser type to AxiosRequestConfig (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4066">#4066</a>)</li>
<li>Fix missing semicolon in typings (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4115">#4115</a>)</li>
<li>Fix response headers types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4136">#4136</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Improve timeout error when timeout is browser default (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3209">#3209</a>)</li>
<li>Fix node version on CI (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4069">#4069</a>)</li>
<li>Added testing to TypeScript portion of project (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4140">#4140</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Rename Angular to AngularJS (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4114">#4114</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/HEAD/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/Evan-Finkelstein">Evan-Finkelstein</a></li>
<li><a href="https://github.com/Jezorko">Paweł Szymański</a></li>
<li><a href="https://github.com/dobesv">Dobes Vandermeer</a></li>
<li><a href="https://github.com/caugner">Claas Augner</a></li>
<li><a href="https://github.com/remcohaszing">Remco Haszing</a></li>
<li><a href="https://github.com/egmen">Evgeniy</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
</ul>
<h2>v0.22.0</h2>
<h3>0.22.0 (October 01, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Caseless header comparing in HTTP adapter (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2880">#2880</a>)</li>
<li>Avoid package.json import fixing issues and warnings related to this (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4041">#4041</a>), (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4065">#4065</a>)</li>
<li>Fixed cancelToken leakage and added AbortController support (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3305">#3305</a>)</li>
<li>Updating CI to run on release branches</li>
<li>Bump follow redirects version</li>
<li>Fixed default transitional config for custom Axios instance; (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4052">#4052</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/HEAD/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/mastermatt">Matt R. Wilson</a></li>
<li><a href="https://github.com/chinesedfan">Xianming Zhong</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/master/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h3>0.23.0 (October 12, 2021)</h3>
<p>Breaking changes:</p>
<ul>
<li>Distinguish request and response data types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4116">#4116</a>)</li>
<li>Change never type to unknown (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4142">#4142</a>)</li>
<li>Fixed TransitionalOptions typings (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4147">#4147</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Adding globalObject: 'this' to webpack config (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3176">#3176</a>)</li>
<li>Adding insecureHTTPParser type to AxiosRequestConfig (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4066">#4066</a>)</li>
<li>Fix missing semicolon in typings (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4115">#4115</a>)</li>
<li>Fix response headers types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4136">#4136</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Improve timeout error when timeout is browser default (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3209">#3209</a>)</li>
<li>Fix node version on CI (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4069">#4069</a>)</li>
<li>Added testing to TypeScript portion of project (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4140">#4140</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Rename Angular to AngularJS (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4114">#4114</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/master/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/Evan-Finkelstein">Evan-Finkelstein</a></li>
<li><a href="https://github.com/Jezorko">Paweł Szymański</a></li>
<li><a href="https://github.com/dobesv">Dobes Vandermeer</a></li>
<li><a href="https://github.com/caugner">Claas Augner</a></li>
<li><a href="https://github.com/remcohaszing">Remco Haszing</a></li>
<li><a href="https://github.com/egmen">Evgeniy</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
</ul>
<h3>0.22.0 (October 01, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Caseless header comparing in HTTP adapter (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2880">#2880</a>)</li>
<li>Avoid package.json import fixing issues and warnings related to this (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4041">#4041</a>), (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4065">#4065</a>)</li>
<li>Fixed cancelToken leakage and added AbortController support (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3305">#3305</a>)</li>
<li>Updating CI to run on release branches</li>
<li>Bump follow redirects version</li>
<li>Fixed default transitional config for custom Axios instance; (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4052">#4052</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/master/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/mastermatt">Matt R. Wilson</a></li>
<li><a href="https://github.com/chinesedfan">Xianming Zhong</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/1025d1231a7747503188459dd5a6d1effdcea928"><code>1025d12</code></a> Release v0.23.0</li>
<li><a href="https://github.com/axios/axios/commit/6d1e30fd80abbf198bca61e7339264e6782dfd73"><code>6d1e30f</code></a> Prepared release notes</li>
<li><a href="https://github.com/axios/axios/commit/20e8b6bc8c27f368ab48241dc14b89bc768ff5f1"><code>20e8b6b</code></a> chore(docs): rename Angular to AngularJS (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4114">#4114</a>)</li>
<li><a href="https://github.com/axios/axios/commit/94a93447992392441f1928dffc9f10529ecec417"><code>94a9344</code></a> Test types (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4140">#4140</a>)</li>
<li><a href="https://github.com/axios/axios/commit/fce210a67e240820cc2c9b146ac80ba6985b8477"><code>fce210a</code></a> Fixed TransitionalOptions typings (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4147">#4147</a>)</li>
<li><a href="https://github.com/axios/axios/commit/547815d9fda524babf9e2b3e9f1648834cb44cb5"><code>547815d</code></a> Mending merge conflict</li>
<li><a href="https://github.com/axios/axios/commit/e462973a4b23e9541efe3e64ca120ae9111a6ad8"><code>e462973</code></a> fix response headers types (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4136">#4136</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7c9a5c5c840b726d621a15f9f859029fff13c961"><code>7c9a5c5</code></a> Fix missing semicolon in typings (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4115">#4115</a>)</li>
<li><a href="https://github.com/axios/axios/commit/6c002323a6bf1efb66942cc130bd8d7cce212930"><code>6c00232</code></a> Change never type to unknown (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4142">#4142</a>)</li>
<li><a href="https://github.com/axios/axios/commit/28a06e6d95b6a8d4f65148743683e85b90719352"><code>28a06e6</code></a> Distinguish request and response data types (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4116">#4116</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.21.4...v0.23.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.21.4&new-version=0.23.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 08:19:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3012" class=".btn">#3012</a>
            </td>
            <td>
                <b>
                    feat: OOB create/accept invitation commands use accept/mediatypeprofile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CreateInvitation:
- Add accept parameter to command
- If accept parameter not present, use agent's first MediaTypeProfile.
  If agent doesn't have any MediaTypeProfile set, default to the aip2 rfc19
  profile, as before.

AcceptInvitation:
- use agent's media type profiles to validate oob accept handshake

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 23:02:39 +0000 UTC
    </div>
</div>

