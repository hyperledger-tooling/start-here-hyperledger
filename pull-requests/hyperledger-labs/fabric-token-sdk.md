---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    unit-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-19 14:56:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.22.0 to 0.23.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.22.0 to 0.23.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/c48da131589f122489348be5dfbcb6457640046f"><code>c48da13</code></a> http2: fix TestServerContinuationFlood flakes</li>
<li><a href="https://github.com/golang/net/commit/762b58d1cf6e0779780decad89c6c1523386638d"><code>762b58d</code></a> http2: fix tipos in comment</li>
<li><a href="https://github.com/golang/net/commit/ba872109ef2dc8f1da778651bd1fd3792d0e4587"><code>ba87210</code></a> http2: close connections when receiving too many headers</li>
<li><a href="https://github.com/golang/net/commit/ebc8168ac8ac742194df729305175940790c55a2"><code>ebc8168</code></a> all: fix some typos</li>
<li><a href="https://github.com/golang/net/commit/3678185f8a652e52864c44049a9ea96b7bcc066a"><code>3678185</code></a> http2: make TestCanonicalHeaderCacheGrowth faster</li>
<li><a href="https://github.com/golang/net/commit/448c44f9287b6745f958d74aa2a17ec7761c2f13"><code>448c44f</code></a> http2: remove clientTester</li>
<li><a href="https://github.com/golang/net/commit/c7877ac4213b2f859831366f5a35b353e0dc9f66"><code>c7877ac</code></a> http2: convert the remaining clientTester tests to testClientConn</li>
<li><a href="https://github.com/golang/net/commit/d8870b0bf2f2426fc8d19a9332f652da5c25418f"><code>d8870b0</code></a> http2: use synthetic time in TestIdleConnTimeout</li>
<li><a href="https://github.com/golang/net/commit/d73acffdc9493532acb85777105bb4a351eea702"><code>d73acff</code></a> http2: only set up deadline when Server.IdleTimeout is positive</li>
<li><a href="https://github.com/golang/net/commit/89f602b7bbf237abe0467031a18b42fc742ced08"><code>89f602b</code></a> http2: validate client/outgoing trailers</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.22.0...v0.23.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.22.0&new-version=0.23.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-19 13:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/606" class=".btn">#606</a>
            </td>
            <td>
                <b>
                    Draft: enforce foreign key constraints in token transaction db
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                (Draft because it includes the code for the previous PR to remove query executor)

Business logic dictates that validations, transactions and movements all flow from a TokenRequest. This PR enforces that in the ttxdb database schema with foreign keys. It also uses JOINs to get the status and the request itself, instead of duplicating it across the tables.

<img width="436" alt="image" src="https://github.com/hyperledger-labs/fabric-token-sdk/assets/6328508/8e4d3f60-25d0-4ea2-9d63-46a5017e230f">

It doesn't yet include the foreign key constraint for the TransactionEndorseAck, because we don't use JOINs towards the request. But if these also should never exist without a TokenRequest, we should probably add that constraint as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-19 11:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/605" class=".btn">#605</a>
            </td>
            <td>
                <b>
                    fsc dep update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 17:59:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/604" class=".btn">#604</a>
            </td>
            <td>
                <b>
                    remove query executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Breaking API change: instead of opening and closing a query executor:

```
aqe := auditor.NewQueryExecutor()
defer aqe.Done()
 aqe.NewPaymentsFilter()
```
You have to directly:
```
auditor.NewPaymentsFilter()
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 14:21:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/603" class=".btn">#603</a>
            </td>
            <td>
                <b>
                    driver cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following: It refactors the `TokenManagerService` to avoid interface imports.
This makes more modular the implementation of a new driver.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 06:37:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/602" class=".btn">#602</a>
            </td>
            <td>
                <b>
                    core logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following: It removes from the `core` package the package level logging to introduce struct level logging.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 10:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/601" class=".btn">#601</a>
            </td>
            <td>
                <b>
                    network service cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following:
- Remove finality API from network service
- Cleanup ValidationCode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 08:33:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/600" class=".btn">#600</a>
            </td>
            <td>
                <b>
                    add atomic write to ttxdb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                if this is ok, we can do the same for the auditdb and remove the functions that are now on the AtomicWrite (as well as the 'txn' field) from the database struct.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 07:41:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/599" class=".btn">#599</a>
            </td>
            <td>
                <b>
                    Centralize database initialization logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simplifies opening of SQL databases by centralizing the configuration in the database package, similar to how identitydb was already doing it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 10:36:40 +0000 UTC
    </div>
</div>

