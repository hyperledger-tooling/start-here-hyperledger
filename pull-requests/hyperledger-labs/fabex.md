---
layout: default
title: fabex
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabex
---

# fabex <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabex){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabex/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Bump go.mongodb.org/mongo-driver from 1.1.0 to 1.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [go.mongodb.org/mongo-driver](https://github.com/mongodb/mongo-go-driver) from 1.1.0 to 1.5.1.
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
<li>Additional commits viewable in <a href="https://github.com/mongodb/mongo-go-driver/compare/v1.1.0...v1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=go.mongodb.org/mongo-driver&package-manager=go_modules&previous-version=1.1.0&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabex/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 19:53:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabex/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Bump github.com/gin-gonic/gin from 1.6.3 to 1.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/gin-gonic/gin](https://github.com/gin-gonic/gin) from 1.6.3 to 1.7.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gin-gonic/gin/releases">github.com/gin-gonic/gin's releases</a>.</em></p>
<blockquote>
<h2>Release v1.7.0</h2>
<h3>BUGFIXES</h3>
<ul>
<li>fix compile error from <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2572">#2572</a> (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2600">#2600</a>)</li>
<li>fix: print headers without Authorization header on broken pipe (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2528">#2528</a>)</li>
<li>fix(tree): reassign fullpath when register new node (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2366">#2366</a>)</li>
</ul>
<h3>ENHANCEMENTS</h3>
<ul>
<li>Support params and exact routes without creating conflicts (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2663">#2663</a>)</li>
<li>chore: improve render string performance (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2365">#2365</a>)</li>
<li>Sync route tree to httprouter latest code (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2368">#2368</a>)</li>
<li>chore: rename getQueryCache/getFormCache to initQueryCache/initFormCa (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2375">#2375</a>)</li>
<li>chore(performance): improve countParams (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2378">#2378</a>)</li>
<li>Remove some functions that have the same effect as the bytes package (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2387">#2387</a>)</li>
<li>update:SetMode function (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2321">#2321</a>)</li>
<li>remove a unused type SecureJSONPrefix (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2391">#2391</a>)</li>
<li>Add a redirect sample for POST method (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2389">#2389</a>)</li>
<li>Add CustomRecovery builtin middleware (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2322">#2322</a>)</li>
<li>binding: avoid 2038 problem on 32-bit architectures (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2450">#2450</a>)</li>
<li>Prevent panic in Context.GetQuery() when there is no Request (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2412">#2412</a>)</li>
<li>Add GetUint and GetUint64 method on gin.context (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2487">#2487</a>)</li>
<li>update content-disposition header to MIME-style (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2512">#2512</a>)</li>
<li>reduce allocs and improve the render <code>WriteString</code> (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2508">#2508</a>)</li>
<li>implement &quot;.Unwrap() error&quot; on Error type (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2525">#2525</a>) (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2526">#2526</a>)</li>
<li>Allow bind with a map[string]string (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2484">#2484</a>)</li>
<li>chore: update tree (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2371">#2371</a>)</li>
<li>Support binding for slice/array obj [Rewrite] (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2302">#2302</a>)</li>
<li>basic auth: fix timing oracle (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2609">#2609</a>)</li>
<li>Add mixed param and non-param paths (port of httprouter<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/329">#329</a>) (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2663">#2663</a>)</li>
<li>feat(engine): add trustedproxies and remoteIP (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2632">#2632</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/gin-gonic/gin/blob/master/CHANGELOG.md">github.com/gin-gonic/gin's changelog</a>.</em></p>
<blockquote>
<h2>Gin v1.7.0</h2>
<h3>BUGFIXES</h3>
<ul>
<li>fix compile error from <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2572">#2572</a> (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2600">#2600</a>)</li>
<li>fix: print headers without Authorization header on broken pipe (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2528">#2528</a>)</li>
<li>fix(tree): reassign fullpath when register new node (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2366">#2366</a>)</li>
</ul>
<h3>ENHANCEMENTS</h3>
<ul>
<li>Support params and exact routes without creating conflicts (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2663">#2663</a>)</li>
<li>chore: improve render string performance (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2365">#2365</a>)</li>
<li>Sync route tree to httprouter latest code (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2368">#2368</a>)</li>
<li>chore: rename getQueryCache/getFormCache to initQueryCache/initFormCa (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2375">#2375</a>)</li>
<li>chore(performance): improve countParams (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2378">#2378</a>)</li>
<li>Remove some functions that have the same effect as the bytes package (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2387">#2387</a>)</li>
<li>update:SetMode function (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2321">#2321</a>)</li>
<li>remove a unused type SecureJSONPrefix (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2391">#2391</a>)</li>
<li>Add a redirect sample for POST method (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2389">#2389</a>)</li>
<li>Add CustomRecovery builtin middleware (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2322">#2322</a>)</li>
<li>binding: avoid 2038 problem on 32-bit architectures (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2450">#2450</a>)</li>
<li>Prevent panic in Context.GetQuery() when there is no Request (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2412">#2412</a>)</li>
<li>Add GetUint and GetUint64 method on gin.context (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2487">#2487</a>)</li>
<li>update content-disposition header to MIME-style (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2512">#2512</a>)</li>
<li>reduce allocs and improve the render <code>WriteString</code> (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2508">#2508</a>)</li>
<li>implement &quot;.Unwrap() error&quot; on Error type (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2525">#2525</a>) (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2526">#2526</a>)</li>
<li>Allow bind with a map[string]string (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2484">#2484</a>)</li>
<li>chore: update tree (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2371">#2371</a>)</li>
<li>Support binding for slice/array obj [Rewrite] (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2302">#2302</a>)</li>
<li>basic auth: fix timing oracle (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2609">#2609</a>)</li>
<li>Add mixed param and non-param paths (port of httprouter<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/329">#329</a>) (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2663">#2663</a>)</li>
<li>feat(engine): add trustedproxies and remoteIP (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2632">#2632</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gin-gonic/gin/commit/d496f64540b6707602de50ab57aeea8ff4080b74"><code>d496f64</code></a> bump to v1.7.0 version (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2672">#2672</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/bfc8ca285eb46dad60e037d57c545cd260636711"><code>bfc8ca2</code></a> feat(engine): add trustedproxies and remoteIP (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2632">#2632</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/f3de8132c5d955784deeadb9bcf5752e9fdf0d8c"><code>f3de813</code></a> Add mixed param and non-param paths (port of httprouter#329) (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2663">#2663</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/a331dc6a31473b7208c57ec32e14bfcec3062dbb"><code>a331dc6</code></a> chore: remove duplicate test 'assert.Equal' (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2617">#2617</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/ed6f85c478ba00e5168be1f29ffcdc9a983568b8"><code>ed6f85c</code></a> build: convert to go:build directives (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2664">#2664</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/1bdf86b722026fd650fddfef7fe9bd8342b51b7a"><code>1bdf86b</code></a> Remove the tedious named return value (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2620">#2620</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/e899771392ecf35de8ce10a030ed8fed2207e9cb"><code>e899771</code></a> chore: Deleted spaces (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2622">#2622</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/b01605bb5b43dbf33781970af5ad6633e5549fd1"><code>b01605b</code></a> basic auth: fix timing oracle (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2609">#2609</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/46ddd4259cac975be1eb11b4f1192264f582db16"><code>46ddd42</code></a> Fixes to the graceful shutdown example (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2552">#2552</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/f4bc259de33c561fd3b0ae3e7aaa849c1d251c0b"><code>f4bc259</code></a> fix error gin support min Go version (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2584">#2584</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/gin-gonic/gin/compare/v1.6.3...v1.7.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/gin-gonic/gin&package-manager=go_modules&previous-version=1.6.3&new-version=1.7.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabex/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 19:52:29 +0000 UTC
    </div>
</div>

