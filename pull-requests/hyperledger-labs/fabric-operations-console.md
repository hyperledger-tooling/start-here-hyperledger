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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Bump github.com/emicklei/go-restful from 2.9.5+incompatible to 2.16.0+incompatible in /packages/fabric-deployer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/emicklei/go-restful](https://github.com/emicklei/go-restful) from 2.9.5+incompatible to 2.16.0+incompatible.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/emicklei/go-restful/blob/v3/CHANGES.md">github.com/emicklei/go-restful's changelog</a>.</em></p>
<blockquote>
<h1>Change history of go-restful</h1>
<h2>[v3.10.2] - 2023-03-09</h2>
<ul>
<li>introduced MergePathStrategy to be able to revert behaviour of path concatenation to 3.9.0
see comment in Readme how to customize this behaviour.</li>
</ul>
<h2>[v3.10.1] - 2022-11-19</h2>
<ul>
<li>fix broken 3.10.0 by using path package for joining paths</li>
</ul>
<h2>[v3.10.0] - 2022-10-11 - BROKEN</h2>
<ul>
<li>changed tokenizer to match std route match behavior; do not trimright the path (<a href="https://redirect.github.com/emicklei/go-restful/issues/511">#511</a>)</li>
<li>Add MIME_ZIP (<a href="https://redirect.github.com/emicklei/go-restful/issues/512">#512</a>)</li>
<li>Add MIME_ZIP and HEADER_ContentDisposition (<a href="https://redirect.github.com/emicklei/go-restful/issues/513">#513</a>)</li>
<li>Changed how to get query parameter issue <a href="https://redirect.github.com/emicklei/go-restful/issues/510">#510</a></li>
</ul>
<h2>[v3.9.0] - 2022-07-21</h2>
<ul>
<li>add support for http.Handler implementations to work as FilterFunction, issue <a href="https://redirect.github.com/emicklei/go-restful/issues/504">#504</a> (thanks to <a href="https://github.com/ggicci">https://github.com/ggicci</a>)</li>
</ul>
<h2>[v3.8.0] - 2022-06-06</h2>
<ul>
<li>use exact matching of allowed domain entries, issue <a href="https://redirect.github.com/emicklei/go-restful/issues/489">#489</a> (<a href="https://redirect.github.com/emicklei/go-restful/issues/493">#493</a>)
<ul>
<li>this changes fixes [security] Authorization Bypass Through User-Controlled Key
by changing the behaviour of the AllowedDomains setting in the CORS filter.
To support the previous behaviour, the CORS filter type now has a AllowedDomainFunc
callback mechanism which is called when a simple domain match fails.</li>
</ul>
</li>
<li>add test and fix for POST without body and Content-type, issue <a href="https://redirect.github.com/emicklei/go-restful/issues/492">#492</a> (<a href="https://redirect.github.com/emicklei/go-restful/issues/496">#496</a>)</li>
<li>[Minor] Bad practice to have a mix of Receiver types. (<a href="https://redirect.github.com/emicklei/go-restful/issues/491">#491</a>)</li>
</ul>
<h2>[v3.7.2] - 2021-11-24</h2>
<ul>
<li>restored FilterChain (<a href="https://redirect.github.com/emicklei/go-restful/issues/482">#482</a> by SVilgelm)</li>
</ul>
<h2>[v3.7.1] - 2021-10-04</h2>
<ul>
<li>fix problem with contentEncodingEnabled setting (<a href="https://redirect.github.com/emicklei/go-restful/issues/479">#479</a>)</li>
</ul>
<h2>[v3.7.0] - 2021-09-24</h2>
<ul>
<li>feat(parameter): adds additional openapi mappings (<a href="https://redirect.github.com/emicklei/go-restful/issues/478">#478</a>)</li>
</ul>
<h2>[v3.6.0] - 2021-09-18</h2>
<ul>
<li>add support for vendor extensions (<a href="https://redirect.github.com/emicklei/go-restful/issues/477">#477</a> thx erraggy)</li>
</ul>
<h2>[v3.5.2] - 2021-07-14</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/emicklei/go-restful/commit/ac666c045e035603f2704c98c59e979fccbfa94f"><code>ac666c0</code></a> update changes</li>
<li><a href="https://github.com/emicklei/go-restful/commit/926662532deb450272956c7bc573978464aae74e"><code>9266625</code></a> use exact matching of allowed domain entries, issue <a href="https://redirect.github.com/emicklei/go-restful/issues/489">#489</a> (<a href="https://redirect.github.com/emicklei/go-restful/issues/493">#493</a>) (<a href="https://redirect.github.com/emicklei/go-restful/issues/503">#503</a>)</li>
<li><a href="https://github.com/emicklei/go-restful/commit/d9c71e118c95f152ff2e0d884d7504aa726d3618"><code>d9c71e1</code></a> support multipart/form-data (<a href="https://redirect.github.com/emicklei/go-restful/issues/502">#502</a>)</li>
<li><a href="https://github.com/emicklei/go-restful/commit/1e8c63ce7906ee023956e8068ce4c54d634c2d2b"><code>1e8c63c</code></a> add access to Route from Request, issue <a href="https://redirect.github.com/emicklei/go-restful/issues/459">#459</a> (<a href="https://redirect.github.com/emicklei/go-restful/issues/462">#462</a>)</li>
<li><a href="https://github.com/emicklei/go-restful/commit/0d68a53f8da6e2fcdf2ba7ffd90305ee037e5467"><code>0d68a53</code></a> fix typo (<a href="https://redirect.github.com/emicklei/go-restful/issues/465">#465</a>)</li>
<li><a href="https://github.com/emicklei/go-restful/commit/a22b51de949f628f359177cff8d8975261b3292f"><code>a22b51d</code></a> add check for wildcard (<a href="https://redirect.github.com/emicklei/go-restful/issues/463">#463</a>)</li>
<li><a href="https://github.com/emicklei/go-restful/commit/8dd9eb88e2526fab4b4768e46d6b75e72d471fb9"><code>8dd9eb8</code></a> update chg</li>
<li><a href="https://github.com/emicklei/go-restful/commit/e5d317549b87950b816947cbba10142378c328e6"><code>e5d3175</code></a> add options shortcut (<a href="https://redirect.github.com/emicklei/go-restful/issues/455">#455</a>)</li>
<li><a href="https://github.com/emicklei/go-restful/commit/1f7f1def5cb588c5bd7e8b9e23b1df771a749c7f"><code>1f7f1de</code></a> fix link to example</li>
<li><a href="https://github.com/emicklei/go-restful/commit/601692bdb9017788c3b10d573c5b4473eba505bc"><code>601692b</code></a> examples use v3</li>
<li>Additional commits viewable in <a href="https://github.com/emicklei/go-restful/compare/v2.9.5...v2.16.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/emicklei/go-restful&package-manager=go_modules&previous-version=2.9.5+incompatible&new-version=2.16.0+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 16:20:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Updating fabric v251 dependent APIs from operator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)


#### Description

updating fabric v251 API dependencies from fabric-operator repo / api branch

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 16:07:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/489" class=".btn">#489</a>
            </td>
            <td>
                <b>
                    use absolute paths for logout/login links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- changes the logout/login links from a url + path, to just an absolute path. more robust this way


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 19:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    fix the deployer sync timing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- fixes the component data sync with deployer, now waits for the deployer changes to write to the db before rebuilding the url safelist


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 19:46:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/487" class=".btn">#487</a>
            </td>
            <td>
                <b>
                    Fix button size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Fixes the width of the button container to match the side panel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 20:07:16 +0000 UTC
    </div>
</div>

