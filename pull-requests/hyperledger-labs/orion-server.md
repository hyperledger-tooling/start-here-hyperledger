---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    Update goleveldb version to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                There a many bug fixes since the first release of goleveldb.
One of which, is fixing crashes when using released snapshots.

For the full update list, see: https://github.com/syndtr/goleveldb/compare/v1...master

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 13:17:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/495" class=".btn">#495</a>
            </td>
            <td>
                <b>
                    Allow setting different go version from the command line
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                E.g., `make GO=go1.19.4 binary`

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 12:53:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    Bump github.com/gogo/protobuf from 1.3.0 to 1.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/gogo/protobuf](https://github.com/gogo/protobuf) from 1.3.0 to 1.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gogo/protobuf/releases">github.com/gogo/protobuf's releases</a>.</em></p>
<blockquote>
<h2>Release v.1.3.2</h2>
<h2>Tested versions:</h2>
<p>go 1.15.6
protoc 3.14.0</p>
<h2>Bug fixes:</h2>
<p>skippy peanut butter</p>
<h2>Release v1.3.1</h2>
<h4>Tested versions:</h4>
<p>go 1.12.10
protoc 3.9.1</p>
<h2>Bug fixes:</h2>
<ul>
<li>proto/buffer: fix proto.Buffer marshaling.
<ul>
<li>Thanks: <a href="https://github.com/apelisse">https://github.com/apelisse</a></li>
</ul>
</li>
<li>plugin/gostring: generate values instead of pointers when a field is repeated and non-nullable.
<ul>
<li>Thanks <a href="https://github.com/godfried">https://github.com/godfried</a></li>
</ul>
</li>
<li>protoc-gen-gogo/generator: Generate json and custom tags for oneof
<ul>
<li>Thanks: <a href="https://github.com/krhubert">https://github.com/krhubert</a></li>
</ul>
</li>
<li>plugin/marshalto: Use ProtoSize() in MarshalTo when enabled for oneof fields.
<ul>
<li>Thanks: <a href="https://github.com/gaffneyc">https://github.com/gaffneyc</a></li>
</ul>
</li>
</ul>
<h2>Upstream commits:</h2>
<ul>
<li>4c88cc3f1a34ffade77b79abc53335d1e511f25b - all: fix reflect.Value.Interface races.</li>
<li>6c65a5562fc06764971b7c5d05c76c75e84bdbf7 -  jsonpb: fix marshaling of Duration</li>
<li>b285ee9cfc6c881bb20c0d8dc73370ea9b9ec90f - Log parsing errors using log pkg</li>
</ul>
<h2>Misc:</h2>
<ul>
<li>add github workflow config</li>
<li>protoc update - Updated to protoc 3.9.1</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gogo/protobuf/commit/b03c65ea87cdc3521ede29f62fe3ce239267c1bc"><code>b03c65e</code></a> skippy peanut butter</li>
<li><a href="https://github.com/gogo/protobuf/commit/550e88954e617545f49920b752c154d72abf1d8d"><code>550e889</code></a> update to go version 1.15.6 and protoc 3.14.0 (<a href="https://github-redirect.dependabot.com/gogo/protobuf/issues/717">#717</a>)</li>
<li><a href="https://github.com/gogo/protobuf/commit/deb6fe8ca7c6d06584bfbd40ca407bf69d9fd2aa"><code>deb6fe8</code></a> Update Readme.md</li>
<li><a href="https://github.com/gogo/protobuf/commit/5628607bb4c51c3157aacc3a50f0ab707582b805"><code>5628607</code></a> github/workflow - update protoc version to 3.9.1 (<a href="https://github-redirect.dependabot.com/gogo/protobuf/issues/637">#637</a>)</li>
<li><a href="https://github.com/gogo/protobuf/commit/09ab7735f7757c093f5b0a2285bff3998d684a61"><code>09ab773</code></a> Issue619safer (<a href="https://github-redirect.dependabot.com/gogo/protobuf/issues/627">#627</a>)</li>
<li><a href="https://github.com/gogo/protobuf/commit/8142193b881b41b9b93dae1124dd99e619b8941f"><code>8142193</code></a> GoString plugin: generate values instead of pointers when a field is repeated...</li>
<li><a href="https://github.com/gogo/protobuf/commit/627c0c9b4094c6cd02b3cb49e22420455e97e64c"><code>627c0c9</code></a> umarshal - refactor skip from recursive calls to a loop. (<a href="https://github-redirect.dependabot.com/gogo/protobuf/issues/636">#636</a>)</li>
<li><a href="https://github.com/gogo/protobuf/commit/69adf3ecd52d1754cc42d7464c449e50d4b79521"><code>69adf3e</code></a> Ghworkflow (<a href="https://github-redirect.dependabot.com/gogo/protobuf/issues/632">#632</a>)</li>
<li><a href="https://github.com/gogo/protobuf/commit/8a5ed79f688836cf007ca23aefe0299791e7bea5"><code>8a5ed79</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/gogo/protobuf/issues/622">#622</a> from jmarais/master</li>
<li><a href="https://github.com/gogo/protobuf/commit/33d47608f2cc12f4c1e590655e6175596f05e6bf"><code>33d4760</code></a> merged in golang/protobuf commit 4c88cc3f1a34ffade77b79abc53335d1e511f25b - a...</li>
<li>Additional commits viewable in <a href="https://github.com/gogo/protobuf/compare/v1.3.0...v1.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/gogo/protobuf&package-manager=go_modules&previous-version=1.3.0&new-version=1.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/orion-server/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 11:19:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    Avoid instantiating the default marshaller before each use
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span>
            </td>
            <td>
                - Fix typo in class name

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 10:25:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Go 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">security</span>
            </td>
            <td>
                Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 08:22:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Allow issuing cert with URI instead of IP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                This is used by Orion's benchmark to issue certificates for the servers.

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 13:50:03 +0000 UTC
    </div>
</div>

