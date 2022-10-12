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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3399" class=".btn">#3399</a>
            </td>
            <td>
                <b>
                    Now JWT cred from the presentation is parsed as JWT cred.  Proof not removed.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>


**Title:**
Now JWT cred from the presentation is parsed as JWT cred.  Proof not removed.

**Summary:**

Preliminary jwt decode removed before calling ParseCredential when the presentation is parsed.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-12 13:59:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3398" class=".btn">#3398</a>
            </td>
            <td>
                <b>
                    chore(deps): bump minimist from 1.2.5 to 1.2.7 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/minimistjs/minimist) from 1.2.5 to 1.2.7.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/minimistjs/minimist/blob/main/CHANGELOG.md">minimist's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.6...v1.2.7">v1.2.7</a> - 2022-10-10</h2>
<h3>Commits</h3>
<ul>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/minimistjs/minimist/commit/0ebf4ebcd5f7787a5524d31a849ef41316b83c3c"><code>0ebf4eb</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/minimistjs/minimist/commit/e115b63fa9d3909f33b00a2db647ff79068388de"><code>e115b63</code></a></li>
<li>[eslint] add eslint; rules to enable later are warnings <a href="https://github.com/minimistjs/minimist/commit/f58745b9bb84348e1be72af7dbba5840c7c13013"><code>f58745b</code></a></li>
<li>[Dev Deps] switch from <code>covert</code> to <code>nyc</code> <a href="https://github.com/minimistjs/minimist/commit/ab033567b9c8b31117cb026dc7f1e592ce455c65"><code>ab03356</code></a></li>
<li>[readme] rename and add badges <a href="https://github.com/minimistjs/minimist/commit/236f4a07e4ebe5ee44f1496ec6974991ab293ffd"><code>236f4a0</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/minimistjs/minimist/commit/783a49bfd47e8335d3098a8cac75662cf71eb32a"><code>783a49b</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/minimistjs/minimist/commit/f81ece6aaec2fa14e69ff4f1e0407a8c4e2635a2"><code>f81ece6</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/minimistjs/minimist/commit/56cad44c7f879b9bb5ec18fcc349308024a89bfc"><code>56cad44</code></a></li>
<li>[Dev Deps] update <code>covert</code>, <code>tape</code>; remove unnecessary <code>tap</code> <a href="https://github.com/minimistjs/minimist/commit/49c5f9fb7e6a92db9eb340cc679de92fb3aacded"><code>49c5f9f</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/minimistjs/minimist/commit/228ae938f3cd9db9dfd8bd7458b076a7b2aef280"><code>228ae93</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/minimistjs/minimist/commit/01fc23f5104f85c75059972e01dd33796ab529ff"><code>01fc23f</code></a></li>
<li>[meta] update repo URLs <a href="https://github.com/minimistjs/minimist/commit/6b164c7d68e0b6bf32f894699effdfb7c63041dd"><code>6b164c7</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.5...v1.2.6">v1.2.6</a> - 2022-03-21</h2>
<h3>Commits</h3>
<ul>
<li>test from prototype pollution PR <a href="https://github.com/minimistjs/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a></li>
<li>isConstructorOrProto adapted from PR <a href="https://github.com/minimistjs/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a></li>
<li>security notice for additional prototype pollution issue <a href="https://github.com/minimistjs/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/minimistjs/minimist/commit/c590d75b741a12b5423e2b299f38a7f7c7d25a18"><code>c590d75</code></a> v1.2.7</li>
<li><a href="https://github.com/minimistjs/minimist/commit/0ebf4ebcd5f7787a5524d31a849ef41316b83c3c"><code>0ebf4eb</code></a> [meta] add <code>auto-changelog</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/e115b63fa9d3909f33b00a2db647ff79068388de"><code>e115b63</code></a> [actions] add reusable workflows</li>
<li><a href="https://github.com/minimistjs/minimist/commit/01fc23f5104f85c75059972e01dd33796ab529ff"><code>01fc23f</code></a> [meta] add <code>safe-publish-latest</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/f58745b9bb84348e1be72af7dbba5840c7c13013"><code>f58745b</code></a> [eslint] add eslint; rules to enable later are warnings</li>
<li><a href="https://github.com/minimistjs/minimist/commit/228ae938f3cd9db9dfd8bd7458b076a7b2aef280"><code>228ae93</code></a> [Tests] add <code>aud</code> in <code>posttest</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/236f4a07e4ebe5ee44f1496ec6974991ab293ffd"><code>236f4a0</code></a> [readme] rename and add badges</li>
<li><a href="https://github.com/minimistjs/minimist/commit/ab033567b9c8b31117cb026dc7f1e592ce455c65"><code>ab03356</code></a> [Dev Deps] switch from <code>covert</code> to <code>nyc</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/49c5f9fb7e6a92db9eb340cc679de92fb3aacded"><code>49c5f9f</code></a> [Dev Deps] update <code>covert</code>, <code>tape</code>; remove unnecessary <code>tap</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/783a49bfd47e8335d3098a8cac75662cf71eb32a"><code>783a49b</code></a> [meta] create FUNDING.yml; add <code>funding</code> in package.json</li>
<li>Additional commits viewable in <a href="https://github.com/minimistjs/minimist/compare/v1.2.5...v1.2.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for minimist since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-11 08:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3397" class=".btn">#3397</a>
            </td>
            <td>
                <b>
                    refactor: update ALPINE_VER and GO_VER args in Makefile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Description:**
update default values of ALPINE_VER and GO_VER args in Makefile in order to build project inside suitable image


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 05:33:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3395" class=".btn">#3395</a>
            </td>
            <td>
                <b>
                    refactor: change xeipuuv/gojsonschema to santhosh-tekuri/jsonschema package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Description:**

- Change `xeipuuv/gojsonschema` to `santhosh-tekuri/jsonschema` package inside `verifiable presentation`
- Refactor related unit tests

Related to #3393 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 11:28:30 +0000 UTC
    </div>
</div>

