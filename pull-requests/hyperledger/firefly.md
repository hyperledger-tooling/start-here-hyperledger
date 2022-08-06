---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/935" class=".btn">#935</a>
            </td>
            <td>
                <b>
                    Always populate Operation namespace from Managers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also includes some misc cleanup identified while doing E2E and perf test runs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 20:41:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/934" class=".btn">#934</a>
            </td>
            <td>
                <b>
                    Create config migration script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The goal here is to have a script that can detect configuration which was deprecated in a particular version of FireFly and then convert it to the newest format. By progressively iterating through versions, a config file may be brought up to date with the latest expected format.

The secondary goal is for this script to be as easy to maintain as possible. I've prototyped a partial solution in both Python and Go. Both have their advantages, so I'm looking for input on the final choice.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 15:48:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/933" class=".btn">#933</a>
            </td>
            <td>
                <b>
                    Bump tzinfo from 1.2.9 to 1.2.10 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [tzinfo](https://github.com/tzinfo/tzinfo) from 1.2.9 to 1.2.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tzinfo/tzinfo/releases">tzinfo's releases</a>.</em></p>
<blockquote>
<h2>v1.2.10</h2>
<ul>
<li>Fixed a relative path traversal bug that could cause arbitrary files to be loaded with require when used with <code>RubyDataSource</code>. Please refer to
<a href="https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx">https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx</a> for details. CVE-2022-31163.</li>
<li>Ignore the SECURITY file from Arch Linux's tzdata package. <a href="https://github-redirect.dependabot.com/tzinfo/tzinfo/issues/134">#134</a>.</li>
</ul>
<p><a href="https://rubygems.org/gems/tzinfo/versions/1.2.10">TZInfo v1.2.10 on RubyGems.org</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tzinfo/tzinfo/blob/master/CHANGES.md">tzinfo's changelog</a>.</em></p>
<blockquote>
<h2>Version 1.2.10 - 19-Jul-2022</h2>
<ul>
<li>Fixed a relative path traversal bug that could cause arbitrary files to be
loaded with <code>require</code> when used with <code>RubyDataSource</code>. Please refer to
<a href="https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx">https://github.com/tzinfo/tzinfo/security/advisories/GHSA-5cm2-9h8c-rvfx</a> for
details. CVE-2022-31163.</li>
<li>Ignore the SECURITY file from Arch Linux's tzdata package. <a href="https://github-redirect.dependabot.com/tzinfo/tzinfo/issues/134">#134</a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tzinfo/tzinfo/commit/0814dcd6195f247cc90e62a46b86ff0b76e08ed6"><code>0814dcd</code></a> Fix the release date.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/fd05e2a61cc569cef81ebd1a90d0b57f69e401bd"><code>fd05e2a</code></a> Preparing v1.2.10.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/b98c32efd61289fe6f00a50ab8061e95962ea983"><code>b98c32e</code></a> Merge branch 'fix-directory-traversal-1.2' into 1.2</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/ac3ee6828afd67e6a8ee981cba791ee34d20e9fb"><code>ac3ee68</code></a> Remove unnecessary escaping of + within regex character classes.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/9d49bf9728a6d42e55f822c497ebf362e86a65a6"><code>9d49bf9</code></a> Fix relative path loading tests.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/394c381eb6a16eaeafb81196270c363234cf1956"><code>394c381</code></a> Remove <code>private_constant</code> for consistency and compatibility.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/5e9f99086f820573eb43ffe242e074b9a8295027"><code>5e9f990</code></a> Exclude Arch Linux's SECURITY file from the time zone index.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/17fc9e1fa918c24ca8c1915419d4cc15f56b6729"><code>17fc9e1</code></a> Workaround for 'Permission denied - NUL' errors with JRuby on Windows.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/6bd7a5191d9c1ca48a97420652460b8c4dec865d"><code>6bd7a51</code></a> Update copyright years.</li>
<li><a href="https://github.com/tzinfo/tzinfo/commit/9905ca93abf7bf3e387bd592406e403cd18334c7"><code>9905ca9</code></a> Fix directory traversal in Timezone.get when using Ruby data source</li>
<li>Additional commits viewable in <a href="https://github.com/tzinfo/tzinfo/compare/v1.2.9...v1.2.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tzinfo&package-manager=bundler&previous-version=1.2.9&new-version=1.2.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 15:30:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/932" class=".btn">#932</a>
            </td>
            <td>
                <b>
                    Pin golangci-lint to v1.47.3 instead of latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Avoids surprising changes to linter rules.

Also looks like the current "latest" version of golangci-lint is Go 1.19 only, and we don't want to upgrade just yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 19:12:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/930" class=".btn">#930</a>
            </td>
            <td>
                <b>
                    Update Viper to support camelCase nested keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pull in a Viper snapshot containing https://github.com/spf13/viper/pull/1387
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 16:55:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/928" class=".btn">#928</a>
            </td>
            <td>
                <b>
                    Wait up to 1000ms to lock sqlite database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Might fix #925
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 15:21:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    Minor cleanup of namespace comments/struct descriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couple of the minor follow-ups from #898
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 14:58:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/926" class=".btn">#926</a>
            </td>
            <td>
                <b>
                    Destroy sysmessaging package 💥
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was created to stash random interfaces just to avoid circular dependencies - but all of these interfaces can be relocated now without introducing a circle.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 14:56:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    super small typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                discard if you want

Signed-off-by: sebgoa <runseb@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 09:26:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/923" class=".btn">#923</a>
            </td>
            <td>
                <b>
                    Updates for EVMConnect support (with EthConnect cross-compatibility)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Support the `TransactionUpdate` type of websocket payload - which just updates the operation, while leaving it in `Pending` status (rather than marking it success/fail)
- Support events with an `0x12345:` address prefix on the signature
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 21:46:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/922" class=".btn">#922</a>
            </td>
            <td>
                <b>
                    Fixes Incorrect Route in the `broadcast_data`Tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Thank you :) 

Signed-off-by: Jeff <60796676+JeffNeff@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 21:41:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    Add the V1 migration test to integration runs
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
        Created At 2022-08-03 21:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    add E2E test for token plugins with remote names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a new test suite for tokens plugins with remote names. 

Fixes #929 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 22:11:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    E2E test for tokens only namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                * Adds an E2E test for namespaces with only a `tokens` plugin
* Moves `keynormalization` config under `namespaces.predefined[].assets.manager.keynormalization`
* Adds common for code adding namespaces, resetting firefly, etc. to a common package
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 18:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/918" class=".btn">#918</a>
            </td>
            <td>
                <b>
                    Add multi-tenancy E2E test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~~In a chain with #916~~

Includes additional fixes for separating messages/data on different namespaces.

This also includes changes to the NextPins table to add a namespace column.
While it's not possible to populate namespace on any existing entries, we make a best
effort at migration by setting the namespace every time a row is updated. This will allow
legacy environments to migrate over time, as long as they don't immediately add
multi-tenant nodes alongside existing ones.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 17:55:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    Add admin and config fields to E2E testState
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
        Created At 2022-08-02 12:57:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/916" class=".btn">#916</a>
            </td>
            <td>
                <b>
                    Add node-specific suffix to DX endpoint "id"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~~In a chain with #915~~
Depends on https://github.com/hyperledger/firefly-dataexchange-https/pull/62

UPDATE: found a number of bugs while adding E2E tests - so #918 contains everything from this PR, some additional fixes, and an E2E test. The comments below are still relevant though.

FireFly can now support many local namespaces that map to a single remote namespace (for multi-tenancy purposes). Each of these local namespaces may have their own "node" within FireFly, but they may all be sharing a single DX plugin. This change adds a "nodeName" qualifier to many of the dataexchange plugin calls, along with a specific implementation in the FFDX plugin code, to allow many nodes to exist behind a single DX.

Implementation outline:
* For newly created nodes, the FFDX connector will append a suffix to the member ID advertised by the plugin before storing or broadcasting it. This means each node will have a unique verifier ID even if they are sharing a DX member ID and certificate. The FFDX connector and FFDX plugin have agreed on `/` as a separator.
* The FFDX connector will ignore this suffix when routing messages (paying attention only to the member ID before the separator) - but will pass the full recipient string for further routing by FireFly on the far end.
* FireFly will use the combination of the received message's remote namespace and recipient ID to route it uniquely to a single event manager.

Should remain fully backwards compatible for nodes that were already broadcast/stored in the database with a non-suffixed peer ID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 17:44:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/915" class=".btn">#915</a>
            </td>
            <td>
                <b>
                    Allow multiple copies of things on different namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Everything that can be sent (messages, data, all definition types) needs to only be unique within a namespace. The IDs can no longer be considered globally unique, and the database needs to reflect that.

Move "node" configuration to the "multiparty" section (next to "org"), as different namespaces may want to advertise different names for their local node.

Clean up operation handling in DX to make it consistent with other plugins.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-30 17:35:10 +0000 UTC
    </div>
</div>

