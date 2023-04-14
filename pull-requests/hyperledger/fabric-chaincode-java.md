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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    Bump json from 20180813 to 20230227 in /fabric-chaincode-integration-test/src/contracts/wrapper-maven
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json](https://github.com/douglascrockford/JSON-java) from 20180813 to 20230227.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/douglascrockford/JSON-java/releases">json's releases</a>.</em></p>
<blockquote>
<h2>20230227</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/723">#723</a></td>
<td>Protect JSONML from stack overflow exceptions caused by recursion</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/720">#720</a></td>
<td>Limit the XML nesting depth for CVE-2022-45688</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/711">#711</a></td>
<td>Revert pull 707 - interviewbit spam</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/704">#704</a></td>
<td>Move javadoc comments above the interface definition to make it visible</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/703">#703</a></td>
<td>Update Releases.md for JSONObject(Map): Throws NPE if key is null</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/696">#696</a></td>
<td>Update JSONPointerTest for NonDex compatibility</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/694">#694</a></td>
<td>Pretty print XML</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/692">#692</a></td>
<td>Example.md syntax highlight and indentation</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/691">#691</a></td>
<td>Create unit tests for various number formats</td>
</tr>
</tbody>
</table>
<h2>20220924</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/688">#688</a></td>
<td>Update copyright to Public Domain</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/687">#687</a></td>
<td>Fix a typo</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/685">#685</a></td>
<td>JSONObject map type unit tests</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/684">#684</a></td>
<td>Remove v7 build from pipeline</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/682">#682</a></td>
<td>JSONString similarity</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/675">#675</a></td>
<td><a href="https://redirect.github.com/stleary/JSON-java/pull/675">stleary/JSON-java#675</a></td>
</tr>
</tbody>
</table>
<h2>20220320</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/660">#660</a></td>
<td>Wrap StackOverflow with JSONException</td>
</tr>
</tbody>
</table>
<h2>20211205</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/651">#651</a></td>
<td>IdentityHashSet for JSONObject cycle detection</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/646">#646</a></td>
<td>XMLParserConfiguration defined json arrays option</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/645">#645</a></td>
<td>Handle circular references in Java beans</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/640">#640</a></td>
<td>Unit tests for multiple backslashes in JSONPointer</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/637">#637</a></td>
<td>Reorganized README.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/634">#634</a></td>
<td>Update README with Unix examples</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/631">#631</a></td>
<td>Refactor JSONPointerTest</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/626">#626</a></td>
<td>Add CODE_OF_CONDUCT.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/622">#622</a></td>
<td>Clean up readme.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/621">#621</a></td>
<td>Clean up comments</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/617">#617</a></td>
<td>JSONObject.similar() numeric compare bug fix</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/613">#613</a></td>
<td>JsonObject.similar() number entry check bug fix</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/610">#610</a></td>
<td>optJSONObject() add default value</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/607">#607</a></td>
<td>Add Security.md policy page</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/606">#606</a></td>
<td>Clean up comments, add suppressWarning annotation</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/604">#604</a></td>
<td>Fixed incorrect cast getting float from array</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/601">#601</a></td>
<td>Added Examples.md for new users</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/stleary/JSON-java/blob/master/docs/RELEASES.md">json's changelog</a>.</em></p>
<blockquote>
<p>20230227    Fix for CVE-2022-45688 and recent commits</p>
<p>20220924    New License - public domain, and some minor updates</p>
<p>20220320    Wrap StackOverflow with JSONException</p>
<p>20211205    Recent commits and some bug fixes for similar()</p>
<p>20210307    Recent commits and potentially breaking fix to JSONPointer</p>
<p>20201115    Recent commits and first release after project structure change</p>
<p>20200518    Recent commits and snapshot before project structure change</p>
<p>20190722    Recent commits</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/douglascrockford/JSON-java/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=org.json:json&package-manager=maven&previous-version=20180813&new-version=20230227)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-chaincode-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 17:51:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/302" class=".btn">#302</a>
            </td>
            <td>
                <b>
                    Bump json from 20180813 to 20230227 in /fabric-chaincode-integration-test/src/contracts/bare-maven
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json](https://github.com/douglascrockford/JSON-java) from 20180813 to 20230227.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/douglascrockford/JSON-java/releases">json's releases</a>.</em></p>
<blockquote>
<h2>20230227</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/723">#723</a></td>
<td>Protect JSONML from stack overflow exceptions caused by recursion</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/720">#720</a></td>
<td>Limit the XML nesting depth for CVE-2022-45688</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/711">#711</a></td>
<td>Revert pull 707 - interviewbit spam</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/704">#704</a></td>
<td>Move javadoc comments above the interface definition to make it visible</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/703">#703</a></td>
<td>Update Releases.md for JSONObject(Map): Throws NPE if key is null</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/696">#696</a></td>
<td>Update JSONPointerTest for NonDex compatibility</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/694">#694</a></td>
<td>Pretty print XML</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/692">#692</a></td>
<td>Example.md syntax highlight and indentation</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/691">#691</a></td>
<td>Create unit tests for various number formats</td>
</tr>
</tbody>
</table>
<h2>20220924</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/688">#688</a></td>
<td>Update copyright to Public Domain</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/687">#687</a></td>
<td>Fix a typo</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/685">#685</a></td>
<td>JSONObject map type unit tests</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/684">#684</a></td>
<td>Remove v7 build from pipeline</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/682">#682</a></td>
<td>JSONString similarity</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/675">#675</a></td>
<td><a href="https://redirect.github.com/stleary/JSON-java/pull/675">stleary/JSON-java#675</a></td>
</tr>
</tbody>
</table>
<h2>20220320</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/660">#660</a></td>
<td>Wrap StackOverflow with JSONException</td>
</tr>
</tbody>
</table>
<h2>20211205</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/651">#651</a></td>
<td>IdentityHashSet for JSONObject cycle detection</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/646">#646</a></td>
<td>XMLParserConfiguration defined json arrays option</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/645">#645</a></td>
<td>Handle circular references in Java beans</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/640">#640</a></td>
<td>Unit tests for multiple backslashes in JSONPointer</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/637">#637</a></td>
<td>Reorganized README.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/634">#634</a></td>
<td>Update README with Unix examples</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/631">#631</a></td>
<td>Refactor JSONPointerTest</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/626">#626</a></td>
<td>Add CODE_OF_CONDUCT.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/622">#622</a></td>
<td>Clean up readme.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/621">#621</a></td>
<td>Clean up comments</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/617">#617</a></td>
<td>JSONObject.similar() numeric compare bug fix</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/613">#613</a></td>
<td>JsonObject.similar() number entry check bug fix</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/610">#610</a></td>
<td>optJSONObject() add default value</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/607">#607</a></td>
<td>Add Security.md policy page</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/606">#606</a></td>
<td>Clean up comments, add suppressWarning annotation</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/604">#604</a></td>
<td>Fixed incorrect cast getting float from array</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/601">#601</a></td>
<td>Added Examples.md for new users</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/stleary/JSON-java/blob/master/docs/RELEASES.md">json's changelog</a>.</em></p>
<blockquote>
<p>20230227    Fix for CVE-2022-45688 and recent commits</p>
<p>20220924    New License - public domain, and some minor updates</p>
<p>20220320    Wrap StackOverflow with JSONException</p>
<p>20211205    Recent commits and some bug fixes for similar()</p>
<p>20210307    Recent commits and potentially breaking fix to JSONPointer</p>
<p>20201115    Recent commits and first release after project structure change</p>
<p>20200518    Recent commits and snapshot before project structure change</p>
<p>20190722    Recent commits</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/douglascrockford/JSON-java/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=org.json:json&package-manager=maven&previous-version=20180813&new-version=20230227)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-chaincode-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 17:50:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/301" class=".btn">#301</a>
            </td>
            <td>
                <b>
                    Bump json from 20180813 to 20230227 in /examples/fabric-contract-example-maven
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json](https://github.com/douglascrockford/JSON-java) from 20180813 to 20230227.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/douglascrockford/JSON-java/releases">json's releases</a>.</em></p>
<blockquote>
<h2>20230227</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/723">#723</a></td>
<td>Protect JSONML from stack overflow exceptions caused by recursion</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/720">#720</a></td>
<td>Limit the XML nesting depth for CVE-2022-45688</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/711">#711</a></td>
<td>Revert pull 707 - interviewbit spam</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/704">#704</a></td>
<td>Move javadoc comments above the interface definition to make it visible</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/703">#703</a></td>
<td>Update Releases.md for JSONObject(Map): Throws NPE if key is null</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/696">#696</a></td>
<td>Update JSONPointerTest for NonDex compatibility</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/694">#694</a></td>
<td>Pretty print XML</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/692">#692</a></td>
<td>Example.md syntax highlight and indentation</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/691">#691</a></td>
<td>Create unit tests for various number formats</td>
</tr>
</tbody>
</table>
<h2>20220924</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/688">#688</a></td>
<td>Update copyright to Public Domain</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/687">#687</a></td>
<td>Fix a typo</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/685">#685</a></td>
<td>JSONObject map type unit tests</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/684">#684</a></td>
<td>Remove v7 build from pipeline</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/682">#682</a></td>
<td>JSONString similarity</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/675">#675</a></td>
<td><a href="https://redirect.github.com/stleary/JSON-java/pull/675">stleary/JSON-java#675</a></td>
</tr>
</tbody>
</table>
<h2>20220320</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/660">#660</a></td>
<td>Wrap StackOverflow with JSONException</td>
</tr>
</tbody>
</table>
<h2>20211205</h2>
<table>
<thead>
<tr>
<th>Pull Request</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/651">#651</a></td>
<td>IdentityHashSet for JSONObject cycle detection</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/646">#646</a></td>
<td>XMLParserConfiguration defined json arrays option</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/645">#645</a></td>
<td>Handle circular references in Java beans</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/640">#640</a></td>
<td>Unit tests for multiple backslashes in JSONPointer</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/637">#637</a></td>
<td>Reorganized README.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/634">#634</a></td>
<td>Update README with Unix examples</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/631">#631</a></td>
<td>Refactor JSONPointerTest</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/626">#626</a></td>
<td>Add CODE_OF_CONDUCT.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/622">#622</a></td>
<td>Clean up readme.md</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/621">#621</a></td>
<td>Clean up comments</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/617">#617</a></td>
<td>JSONObject.similar() numeric compare bug fix</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/613">#613</a></td>
<td>JsonObject.similar() number entry check bug fix</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/610">#610</a></td>
<td>optJSONObject() add default value</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/607">#607</a></td>
<td>Add Security.md policy page</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/606">#606</a></td>
<td>Clean up comments, add suppressWarning annotation</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/604">#604</a></td>
<td>Fixed incorrect cast getting float from array</td>
</tr>
<tr>
<td><a href="https://redirect.github.com/douglascrockford/JSON-java/issues/601">#601</a></td>
<td>Added Examples.md for new users</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/stleary/JSON-java/blob/master/docs/RELEASES.md">json's changelog</a>.</em></p>
<blockquote>
<p>20230227    Fix for CVE-2022-45688 and recent commits</p>
<p>20220924    New License - public domain, and some minor updates</p>
<p>20220320    Wrap StackOverflow with JSONException</p>
<p>20211205    Recent commits and some bug fixes for similar()</p>
<p>20210307    Recent commits and potentially breaking fix to JSONPointer</p>
<p>20201115    Recent commits and first release after project structure change</p>
<p>20200518    Recent commits and snapshot before project structure change</p>
<p>20190722    Recent commits</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/douglascrockford/JSON-java/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=org.json:json&package-manager=maven&previous-version=20180813&new-version=20230227)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-chaincode-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 17:49:22 +0000 UTC
    </div>
</div>

