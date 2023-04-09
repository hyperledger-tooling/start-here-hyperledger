---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/395" class=".btn">#395</a>
            </td>
            <td>
                <b>
                    build(deps): Bump golang.org/x/crypto from 0.0.0-20200622213623-75b288015ac9 to 0.1.0 in /samples/fabric/go-cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/crypto](https://github.com/golang/crypto) from 0.0.0-20200622213623-75b288015ac9 to 0.1.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/crypto/commits/v0.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/crypto&package-manager=go_modules&previous-version=0.0.0-20200622213623-75b288015ac9&new-version=0.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 16:39:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/394" class=".btn">#394</a>
            </td>
            <td>
                <b>
                    Fix Go Publish workflows and relay, driver changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Fix Go publish workflows by changing go version 1.20 in those workflows.
2. Relay: Added configurable variable `DB_OPEN_MAX_RETRIES`, to remove hard coded 10 re-try db open attempts.
3. Fabric Driver: Added configurable variable `LEVELDB_LOCKED_MAX_RETRIES`, to remove hard coded 10 re-try db open attempts.
4. Version Bump for relay and fabric-driver to `v1.5.12`
5. Fix docs vulnerability: [CVE-2020-28477 ](https://github.com/advisories/GHSA-9qmh-276g-x5pj)
6. Fix relay vulnerability: https://github.com/hyperledger-labs/weaver-dlt-interoperability/security/dependabot/93
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 18:12:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    build(deps): Bump golang.org/x/net from 0.0.0-20200822124328-c89045814202 to 0.7.0 in /samples/fabric/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.0.0-20200822124328-c89045814202 to 0.7.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/net/commits/v0.7.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.0.0-20200822124328-c89045814202&new-version=0.7.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    build(deps): Bump golang.org/x/text from 0.3.2 to 0.3.8 in /samples/fabric/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/text](https://github.com/golang/text) from 0.3.2 to 0.3.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/text/commit/434eadcdbc3b0256971992e8c70027278364c72c"><code>434eadc</code></a> language: reject excessively large Accept-Language strings</li>
<li><a href="https://github.com/golang/text/commit/23407e72ed5b895a2dfd230aec777f4fbe026d6a"><code>23407e7</code></a> go.mod: ignore cyclic dependency for tagging</li>
<li><a href="https://github.com/golang/text/commit/b18d3dd8a4b426ebedcf279b593e85ac4985b9d3"><code>b18d3dd</code></a> secure/precis: replace bytes.Compare with bytes.Equal</li>
<li><a href="https://github.com/golang/text/commit/795e854ff348c9cac4fd0033ce04c417705dd0bb"><code>795e854</code></a> all: replace io/ioutil with io and os package</li>
<li><a href="https://github.com/golang/text/commit/b0ca10ff35f1325c7d0ac7830fe3f036bd72d8f9"><code>b0ca10f</code></a> internal/language: bump script types to uint16 and update registry</li>
<li><a href="https://github.com/golang/text/commit/ba9b0e1d4b03523c708709935fbc961124b6967b"><code>ba9b0e1</code></a> go.mod: update x/tools to HEAD</li>
<li><a href="https://github.com/golang/text/commit/d03b41800055b01e3895b1e047af09733c93bf63"><code>d03b418</code></a> A+C: delete AUTHORS and CONTRIBUTORS</li>
<li><a href="https://github.com/golang/text/commit/b4bca84b03619dba00657375259024a7f8ae6712"><code>b4bca84</code></a> language/display: fix Tag method comment</li>
<li><a href="https://github.com/golang/text/commit/ea49e3e2d5b3f1518081d8bc53ffefc8bc60ecec"><code>ea49e3e</code></a> go.mod: update x/tools to HEAD</li>
<li><a href="https://github.com/golang/text/commit/78819d01d041a94e055bbaa2d95e5e4d49e8f8a0"><code>78819d0</code></a> go.mod: update to golang.org/x/text v0.1.10</li>
<li>Additional commits viewable in <a href="https://github.com/golang/text/compare/v0.3.2...v0.3.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/text&package-manager=go_modules&previous-version=0.3.2&new-version=0.3.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    build(deps): Bump golang.org/x/sys from 0.0.0-20200323222414-85ca7c5b95cd to 0.1.0 in /samples/fabric/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/sys](https://github.com/golang/sys) from 0.0.0-20200323222414-85ca7c5b95cd to 0.1.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/sys/commits/v0.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/sys&package-manager=go_modules&previous-version=0.0.0-20200323222414-85ca7c5b95cd&new-version=0.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:56:11 +0000 UTC
    </div>
</div>

