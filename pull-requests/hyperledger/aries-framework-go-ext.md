---
layout: default
title: aries-framework-go-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go-ext
---

# aries-framework-go-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    chore(deps): bump go.mongodb.org/mongo-driver from 1.4.2 to 1.5.1 in /component/storage/mongodb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [go.mongodb.org/mongo-driver](https://github.com/mongodb/mongo-go-driver) from 1.4.2 to 1.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mongodb/mongo-go-driver/releases">go.mongodb.org/mongo-driver's releases</a>.</em></p>
<blockquote>
<h2>MongoDB Go Driver 1.5.1</h2>
<p>The MongoDB Go driver team is pleased to release 1.5.1 of the official Go driver.</p>
<p>This release contains several bug fixes. Due to the issue below, we recommend all users upgrade to this version of the driver.</p>
<p>Documentation can be found on <a href="https://pkg.go.dev/go.mongodb.org/mongo-driver/mongo?tab=doc">pkg.go.dev</a> and the <a href="https://docs.mongodb.com/ecosystem/drivers/go/">MongoDB documentation site</a>. BSON library documentation is also available on <a href="https://pkg.go.dev/go.mongodb.org/mongo-driver/bson?tab=doc">pkg.go.dev</a>. Questions and inquiries can be asked on the <a href="https://community.mongodb.com/">MongoDB Developer Community</a>. Bugs can be reported in the <a href="https://jira.mongodb.org/secure/CreateIssue!default.jspa">Go Driver Jira</a> where a list of <a href="https://jira.mongodb.org/browse/GODRIVER">current issues</a> can be found.</p>
<!-- raw HTML omitted -->
<p>This CVE describes a security issue with the driver's BSON marshalling system. BSON marshalling functions would incorrectly handle null bytes embedded in BSON key names and the pattern/options fields of a BSON regex value. BSON marshalling functions now correctly validate and error if there is an embedded null byte in BSON key names or the pattern/options fields of a BSON regex value. We recommend all users of the driver upgrade to this version.</p>
<p><!-- raw HTML omitted -->CVE ID<!-- raw HTML omitted -->: CVE-2021-20329
<!-- raw HTML omitted -->Title<!-- raw HTML omitted -->: Specific cstrings input may not be properly validated in the MongoDB Go Driver
<!-- raw HTML omitted -->Description<!-- raw HTML omitted -->: Specific cstrings input may not be properly validated in the MongoDB Go Driver when marshalling Go objects into BSON. A malicious user could use a Go object with specific string to potentially inject additional fields into marshalled documents. This issue affects all MongoDB GO Drivers up to (and including) 1.5.0.
<!-- raw HTML omitted -->CVSS score<!-- raw HTML omitted -->: 6.8
CVSS:3.1/AV:N/AC:H/PR:L/UI:N/S:U/C:H/I:H/A:N
<!-- raw HTML omitted -->Affected products and versions, MongoDB Go Driver versions<!-- raw HTML omitted --> &lt;= 1.5.0
<!-- raw HTML omitted -->Underlying operating systems affected: All<!-- raw HTML omitted --></p>
<!-- raw HTML omitted -->
<p>For a full list of tickets included in this release, please see the links below:</p>
<p><a href="https://jira.mongodb.org/issues/?jql=project%3DGODRIVER%20and%20type%3DBug%20and%20status%3Dclosed%20and%20fixVersion%3D1.5.1">Bugs</a></p>
<p><a href="https://jira.mongodb.org/issues/?jql=project%20%3D%20GODRIVER%20AND%20issuetype%20%3D%20Task%20AND%20status%20%3D%20Closed%20AND%20fixVersion%20%3D%201.5.1">Tasks</a></p>
<h2>MongoDB Go Driver 1.5.0</h2>
<p>The MongoDB Go driver team is pleased to release 1.5.0 of the official Go driver.</p>
<p>This release contains several new features and usability improvements for the driver.</p>
<p>Documentation can be found on <a href="https://pkg.go.dev/go.mongodb.org/mongo-driver/mongo?tab=doc">pkg.go.dev</a> and the <a href="https://docs.mongodb.com/ecosystem/drivers/go/">MongoDB documentation site</a>. BSON library documentation is also available on <a href="https://pkg.go.dev/go.mongodb.org/mongo-driver/bson?tab=doc">pkg.go.dev</a>. Questions and inquiries can be asked on the <a href="https://community.mongodb.com/">MongoDB Developer Community</a>. Bugs can be reported in the <a href="https://jira.mongodb.org/secure/CreateIssue!default.jspa">Go Driver Jira</a> where a list of <a href="https://jira.mongodb.org/browse/GODRIVER">current issues</a> can be found.</p>
<!-- raw HTML omitted -->
<p>This release contains a new errors API for the primary <code>mongo</code> package. Users can now detect duplicate key errors, timeouts, and network errors via the <code>mongo.IsDuplicateKeyError</code>, <code>mongo.IsTimeout</code>, and <code>mongo.IsNetworkError</code> functions, respectively. Additionally, a new <code>UpdateByID</code> function has been added to the <code>mongo.Collection</code> type to update a single document with a given <code>_id</code> value.</p>
<!-- raw HTML omitted -->
<p>The Go Driver now supports using GCP and Azure key management services with the client-side field level encryption feature. In addition, AWS key management support has been enhanced to allow authenticating with temporary AWS credentials. See the <a href="https://docs.mongodb.com/drivers/security/client-side-field-level-encryption-local-key-to-kms/">MongoDB docs</a> for more information about these improvements. Use of client-side field level encryption requires users to install the latest released version of <a href="https://github.com/mongodb/libmongocrypt">libmongocrypt</a>. <strong>Note</strong>: This means that existing applications that use this feature will need to upgrade the libmongocrypt dependency when upgrading to this driver version; otherwise, the application will fail to compile. Users can upgrade to the latest development release of libmongocrypt  via the OS-specific instructions for <a href="https://github.com/mongodb/libmongocrypt#installing-libmongocrypt-on-macos">macos</a>, <a href="https://github.com/mongodb/libmongocrypt#installing-libmongocrypt-on-windows">Windows</a>, and <a href="https://github.com/mongodb/libmongocrypt#installing-libmongocrypt-from-distribution-packages">Linux</a>.</p>
<!-- raw HTML omitted -->
<p>Monitoring has now been added for various server events. A <code>ServerMonitor</code> set on a <code>mongo.Client</code> monitors changes on the MongoDB deployment it is connected to and reports the changes in the client's representation of the deployment.</p>
<!-- raw HTML omitted -->
<p>The driver will now error if a map with more than one key is used as a hint option, sort option, or for index creation. This is to prevent unexpected behavior, for example, an index being created with the keys in the wrong order.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/40c0e70826f57cf9d942045a014367d9b3c94251"><code>40c0e70</code></a> Update version to v1.5.1</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/3a89e6cde18d6ac5d38f39b54eaa8d4e321fd118"><code>3a89e6c</code></a> GODRIVER-1923 Error if BSON cstrings contain null bytes (<a href="https://github-redirect.dependabot.com/mongodb/mongo-go-driver/issues/622">#622</a>)</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/1a2534c7d5f023dd3a48a353e2421a2d9e3d74a0"><code>1a2534c</code></a> GODRIVER-1935 Update scram/stringprep dependencies (<a href="https://github-redirect.dependabot.com/mongodb/mongo-go-driver/issues/624">#624</a>)</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/6ea353a400000498cf3591dacb61d91478067751"><code>6ea353a</code></a> GODRIVER-1918 Check for zero length in readstring (<a href="https://github-redirect.dependabot.com/mongodb/mongo-go-driver/issues/613">#613</a>)</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/d5e11aa021c6988d1f257b887e8055464662d954"><code>d5e11aa</code></a> GODRIVER-1919 Support decoding ObjectIDs from hex strings in BSON (<a href="https://github-redirect.dependabot.com/mongodb/mongo-go-driver/issues/610">#610</a>)</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/e0ed6d61ab5d313bf6ae5ed518d15d4fed4c3f7f"><code>e0ed6d6</code></a> Update version to v1.5.1+prerelease</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/6760875fa58e0fa5518c992582efa6d807960d6c"><code>6760875</code></a> Update version to v1.5.0</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/19a368cb71ee83c8e2c1474346560a61c26349f9"><code>19a368c</code></a> GODRIVER-1911 Fix Windows/macos test failures for CSFLE (<a href="https://github-redirect.dependabot.com/mongodb/mongo-go-driver/issues/603">#603</a>)</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/2a5f9a4fa2c39e810a954a2d68757a81bc4ed8c1"><code>2a5f9a4</code></a> GODRIVER-1879 Apply connectTimeoutMS to TLS handshake (<a href="https://github-redirect.dependabot.com/mongodb/mongo-go-driver/issues/594">#594</a>)</li>
<li><a href="https://github.com/mongodb/mongo-go-driver/commit/2c5b75be90cc58314d0c124094a143bb0abd83c9"><code>2c5b75b</code></a> GODRIVER-1855 Support AWS authentication with temporary credentials in CSFLE ...</li>
<li>Additional commits viewable in <a href="https://github.com/mongodb/mongo-go-driver/compare/v1.4.2...v1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=go.mongodb.org/mongo-driver&package-manager=go_modules&previous-version=1.4.2&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 16:29:57 +0000 UTC
    </div>
</div>

