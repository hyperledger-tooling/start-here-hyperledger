---
layout: default
title: sawtooth-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-java
---

# sawtooth-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-java/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Bump protobuf-java from 3.16.1 to 3.16.3 in /examples/xo_java
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobuf-java](https://github.com/protocolbuffers/protobuf) from 3.16.1 to 3.16.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf-java's releases</a>.</em></p>
<blockquote>
<h2>Protobuf Release v3.16.3</h2>
<h1>Java</h1>
<ul>
<li>Refactoring java full runtime to reuse sub-message builders and prepare to
migrate parsing logic from parse constructor to builder.</li>
<li>Move proto wireformat parsing functionality from the private &quot;parsing
constructor&quot; to the Builder class.</li>
<li>Change the Lite runtime to prefer merging from the wireformat into mutable
messages rather than building up a new immutable object before merging. This
way results in fewer allocations and copy operations.</li>
<li>Make message-type extensions merge from wire-format instead of building up
instances and merging afterwards. This has much better performance.</li>
<li>Fix TextFormat parser to build up recurring (but supposedly not repeated)
sub-messages directly from text rather than building a new sub-message and
merging the fully formed message into the existing field.</li>
<li>This release addresses a <a href="https://github.com/protocolbuffers/protobuf/security/advisories/GHSA-h4h5-3hr4-j3g2">Security Advisory for Java users</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/b8c2488f480bbe3d66b9874c2fcd434201caa48a"><code>b8c2488</code></a> Updating version.json and repo version numbers to: 16.3</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/42e47e5a3fa7219b136f6a5de7c74a89a79245c6"><code>42e47e5</code></a> Refactoring Java parsing (3.16.x) (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10668">#10668</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/98884a8a293488375e10480e5ff1c1f76de9ec8f"><code>98884a8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10556">#10556</a> from deannagarcia/3.16.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/450b648f288f9a6def073f08e3300233bb46c5dd"><code>450b648</code></a> Cherrypick ruby fixes for monterey</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/b17bb392b46a7bc9d09ae075dc5e8557e246698d"><code>b17bb39</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10548">#10548</a> from protocolbuffers/3.16.x-202209131829</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/c18f5e71d86063fd6cea2c47cd7ab4131db5c9e2"><code>c18f5e7</code></a> Updating changelog</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/6f4e81791d390cba199184c378e75da40a4965f0"><code>6f4e817</code></a> Updating version.json and repo version numbers to: 16.2</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/a7d4e94a4666b722695d9c55ac842d4a3735699e"><code>a7d4e94</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10547">#10547</a> from deannagarcia/3.16.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/55815e423bb82cc828836bbd60c79c1f9a195763"><code>55815e4</code></a> Apply patch</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/152d7bf809dcb24fd9d417d66cf2b270b3654369"><code>152d7bf</code></a> Update version.json with &quot;lts&quot;: true (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10535">#10535</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.16.1...v3.16.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.google.protobuf:protobuf-java&package-manager=maven&previous-version=3.16.1&new-version=3.16.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/sawtooth-sdk-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-05 01:01:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-java/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Bump protobuf-java from 3.16.1 to 3.16.3 in /examples/intkey_java
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobuf-java](https://github.com/protocolbuffers/protobuf) from 3.16.1 to 3.16.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf-java's releases</a>.</em></p>
<blockquote>
<h2>Protobuf Release v3.16.3</h2>
<h1>Java</h1>
<ul>
<li>Refactoring java full runtime to reuse sub-message builders and prepare to
migrate parsing logic from parse constructor to builder.</li>
<li>Move proto wireformat parsing functionality from the private &quot;parsing
constructor&quot; to the Builder class.</li>
<li>Change the Lite runtime to prefer merging from the wireformat into mutable
messages rather than building up a new immutable object before merging. This
way results in fewer allocations and copy operations.</li>
<li>Make message-type extensions merge from wire-format instead of building up
instances and merging afterwards. This has much better performance.</li>
<li>Fix TextFormat parser to build up recurring (but supposedly not repeated)
sub-messages directly from text rather than building a new sub-message and
merging the fully formed message into the existing field.</li>
<li>This release addresses a <a href="https://github.com/protocolbuffers/protobuf/security/advisories/GHSA-h4h5-3hr4-j3g2">Security Advisory for Java users</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/b8c2488f480bbe3d66b9874c2fcd434201caa48a"><code>b8c2488</code></a> Updating version.json and repo version numbers to: 16.3</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/42e47e5a3fa7219b136f6a5de7c74a89a79245c6"><code>42e47e5</code></a> Refactoring Java parsing (3.16.x) (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10668">#10668</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/98884a8a293488375e10480e5ff1c1f76de9ec8f"><code>98884a8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10556">#10556</a> from deannagarcia/3.16.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/450b648f288f9a6def073f08e3300233bb46c5dd"><code>450b648</code></a> Cherrypick ruby fixes for monterey</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/b17bb392b46a7bc9d09ae075dc5e8557e246698d"><code>b17bb39</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10548">#10548</a> from protocolbuffers/3.16.x-202209131829</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/c18f5e71d86063fd6cea2c47cd7ab4131db5c9e2"><code>c18f5e7</code></a> Updating changelog</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/6f4e81791d390cba199184c378e75da40a4965f0"><code>6f4e817</code></a> Updating version.json and repo version numbers to: 16.2</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/a7d4e94a4666b722695d9c55ac842d4a3735699e"><code>a7d4e94</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10547">#10547</a> from deannagarcia/3.16.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/55815e423bb82cc828836bbd60c79c1f9a195763"><code>55815e4</code></a> Apply patch</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/152d7bf809dcb24fd9d417d66cf2b270b3654369"><code>152d7bf</code></a> Update version.json with &quot;lts&quot;: true (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10535">#10535</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.16.1...v3.16.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.google.protobuf:protobuf-java&package-manager=maven&previous-version=3.16.1&new-version=3.16.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/sawtooth-sdk-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-05 01:00:25 +0000 UTC
    </div>
</div>

