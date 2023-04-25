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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    build(deps): Bump golang.org/x/net from 0.0.0-20200822124328-c89045814202 to 0.7.0 in /core/network/fabric-interop-cc/libs/testutils
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
        Created At 2023-04-25 03:33:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    fix(nodesdk): ecies decrypt bug when z is less than 32B
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix decryption bug in `weaver-fabric-interop-sdk`:
Append leading 0 bytes to Z if Z is less than 32 bytes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 18:18:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    fix(driver): monitor to always process events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Monitor should always process events if there is a single block not yet read.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 18:15:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    feat(fabric-driver): Added monitor for missed events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added Monitor in fabric driver for missed events.
2. Removed contract event listener, now block listener serves both block and contract events.
3. Two env variables to configure monitor:
```
MONITOR_ENABLE: Enable or disable monitor
MONITOR_SYNC_PERIOD: time period in seconds for monitor to sleep before running again
```
4. Fix Fabric testnet for Mac
5. Upgrade Fabric testnet to v2.5
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 19:50:06 +0000 UTC
    </div>
</div>

