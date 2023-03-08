---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4081" class=".btn">#4081</a>
            </td>
            <td>
                <b>
                    Updates in main branch for v2.4.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates in main branch for v2.4.9.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 18:05:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4080" class=".btn">#4080</a>
            </td>
            <td>
                <b>
                    Add chaincode initialization guidance to docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add chaincode initialization guidance to docs,
including the option to manage initialization as regular chaincode state rather than with the chaincode lifecycle initialization mechanism.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 17:27:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4078" class=".btn">#4078</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/crypto from 0.0.0-20210921155107-089bfa567519 to 0.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/crypto](https://github.com/golang/crypto) from 0.0.0-20210921155107-089bfa567519 to 0.1.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/crypto/commits/v0.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/crypto&package-manager=go_modules&previous-version=0.0.0-20210921155107-089bfa567519&new-version=0.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 23:15:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4074" class=".btn">#4074</a>
            </td>
            <td>
                <b>
                    Release commit for v2.4.9.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.4.9.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 21:10:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4073" class=".btn">#4073</a>
            </td>
            <td>
                <b>
                    Backport PR 4011 to release-2.4 (fix IsChannelMember)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I7205dbe264248c4ad534499955bb22710d07444d

#### Type of change

- Bug fix

#### Description
PR 4011 addressed a bug (#3998) in IsChannelMember that manifested itself in the test

`integration/raft/cft_test.go` use-case: "disregards certificate renewal if only the validity period changed"

after it was converted to run without the system channel.

Here we
- Backport the fix (in etcdraft/consenter.go)
- Add the same test case which runs without the system channel (w/o the fix this test case fails).
- Backport some test infrastructure that helps running tests without the system channel.


#### Related issues

#3998 the issue describing the bug
#4011 the PR fixing the bug on main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 14:15:16 +0000 UTC
    </div>
</div>

