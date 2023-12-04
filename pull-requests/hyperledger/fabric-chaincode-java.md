---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/321" class=".btn">#321</a>
            </td>
            <td>
                <b>
                    Use OSV-Scanner instead of dependency-check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The existing dependency-check version is no longer supported and might fail after the NVD data feeds it uses are deprecated on 2023-12-15. The updated version requires an API key to interact with the newer NVD APIs. For details see:

- https://github.com/jeremylong/DependencyCheck#900-upgrade-notice

It also requires periodic triage and suppression of false positive detections. OSV-Scanner appears less prone to false positives and does not require an API key to be maintained.

Implement a scheduled vulnerability scan (using OSV-Scanner) so that vulnerabilities are more visible than the current (dependency-check) implementation, which runs in PR builds but does not fail builds or make the results very visible.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 17:25:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/320" class=".btn">#320</a>
            </td>
            <td>
                <b>
                    Bump ch.qos.logback:logback-classic from 1.3.11 to 1.3.12 in /examples/fabric-contract-example-maven
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [ch.qos.logback:logback-classic](https://github.com/qos-ch/logback) from 1.3.11 to 1.3.12.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/qos-ch/logback/commit/0df4ec15d45301b5d0a6e2de6466a17944c3a871"><code>0df4ec1</code></a> prepare release 1.3.12</li>
<li><a href="https://github.com/qos-ch/logback/commit/189af5029addc72c91300e3e53466de5a1ca9894"><code>189af50</code></a> ensure JDK 8 compatibility</li>
<li><a href="https://github.com/qos-ch/logback/commit/14a71d02102bc5365398ff388cee065eb99ce141"><code>14a71d0</code></a> cater for array size marked with -1</li>
<li><a href="https://github.com/qos-ch/logback/commit/b8eac23a9de9e05fb6d51160b3f46acd91af9731"><code>b8eac23</code></a> prevent DOS attacks using on malicious serialized input</li>
<li><a href="https://github.com/qos-ch/logback/commit/d87dd1221eb23732f4400cb60de725765539a274"><code>d87dd12</code></a> further support for Virtual threads, issues 737</li>
<li><a href="https://github.com/qos-ch/logback/commit/034aaee06785b817d41807ea756ce765ed9c8fb3"><code>034aaee</code></a> add support for Virtual threads</li>
<li><a href="https://github.com/qos-ch/logback/commit/d6294e579848e5c3cd179d495c3c668d5c642f32"><code>d6294e5</code></a> parameterizable invocation gate delay</li>
<li><a href="https://github.com/qos-ch/logback/commit/3b91f6d5137814b89a7c9277279ca630292f17c2"><code>3b91f6d</code></a> minor refactoring</li>
<li><a href="https://github.com/qos-ch/logback/commit/d94ebec6edfdd6e7e3737e9e4c3cd1551e8cdec0"><code>d94ebec</code></a> fix guthub issue 715</li>
<li><a href="https://github.com/qos-ch/logback/commit/c76b3030ce618b8c361f39c09779b0a738baf8a6"><code>c76b303</code></a> minor refactoring for better readability</li>
<li>Additional commits viewable in <a href="https://github.com/qos-ch/logback/compare/v_1.3.11...v_1.3.12">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ch.qos.logback:logback-classic&package-manager=maven&previous-version=1.3.11&new-version=1.3.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-chaincode-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 22:46:49 +0000 UTC
    </div>
</div>

