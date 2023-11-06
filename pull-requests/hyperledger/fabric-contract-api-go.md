---
layout: default
title: fabric-contract-api-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-contract-api-go
---

# fabric-contract-api-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-contract-api-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    Bump github.com/stretchr/testify from 1.8.2 to 1.8.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/stretchr/testify](https://github.com/stretchr/testify) from 1.8.2 to 1.8.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/stretchr/testify/commit/f97607b89807936ac4ff96748d766cf4b9711f78"><code>f97607b</code></a> Create GitHub release when new release tag is pushed (<a href="https://redirect.github.com/stretchr/testify/issues/1354">#1354</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/4c93d8f201cb46ed50de949ee65804f944b570f8"><code>4c93d8f</code></a> EqualExportedValues: Handle nested pointer, slice and map fields (<a href="https://redirect.github.com/stretchr/testify/issues/1379">#1379</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/4b2f4d2bcff3848b6a4e63d462da6ce3c21e9c78"><code>4b2f4d2</code></a> add EventuallyWithT assertion (<a href="https://redirect.github.com/stretchr/testify/issues/1264">#1264</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/b3106d772c7aa439743e1a3f4de81149e323cf70"><code>b3106d7</code></a> allow testing for functional options (<a href="https://redirect.github.com/stretchr/testify/issues/1023">#1023</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/437071b948cd89bdbaaf43a41f19fbe1a0945f6f"><code>437071b</code></a> assert: fix error message formatting for NotContains (<a href="https://redirect.github.com/stretchr/testify/issues/1362">#1362</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/c5fc9d6b6b21ea89be8480c0dc35e2977ab988f6"><code>c5fc9d6</code></a> Compare public elements of struct (<a href="https://redirect.github.com/stretchr/testify/issues/1309">#1309</a>)</li>
<li>See full diff in <a href="https://github.com/stretchr/testify/compare/v1.8.2...v1.8.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/stretchr/testify&package-manager=go_modules&previous-version=1.8.2&new-version=1.8.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 15:19:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Bump github.com/hyperledger/fabric-protos-go from 0.3.0 to 0.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/hyperledger/fabric-protos-go](https://github.com/hyperledger/fabric-protos-go) from 0.3.0 to 0.3.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/212400245d309cf319fd0734ac18d60783d3a746"><code>2124002</code></a> Extend lifecycle protos to checkcommitreadiness to provide discrepancy details</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/b03edb47a905a20294e668e937d2035659852564"><code>b03edb4</code></a> system channel cleanup - make HeaderType_ORDERER_TRANSACTION deprecated (<a href="https://redirect.github.com/hyperledger/fabric-protos-go/issues/184">#184</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/8f302041c2e296480a3755906f72f5aab9bcc3ba"><code>8f30204</code></a> Bump Go to 1.19 (<a href="https://redirect.github.com/hyperledger/fabric-protos-go/issues/178">#178</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/8b7f1c52afc671f1e64c3c18bf192078facaace2"><code>8b7f1c5</code></a> Update Go bindings build</li>
<li>See full diff in <a href="https://github.com/hyperledger/fabric-protos-go/compare/v0.3.0...v0.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/hyperledger/fabric-protos-go&package-manager=go_modules&previous-version=0.3.0&new-version=0.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 15:19:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    Bump github.com/go-openapi/spec from 0.20.8 to 0.20.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/go-openapi/spec](https://github.com/go-openapi/spec) from 0.20.8 to 0.20.9.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/go-openapi/spec/commit/832384d4ee1b2aa2479009d732f42866b63ed5f6"><code>832384d</code></a> Merge pull request <a href="https://redirect.github.com/go-openapi/spec/issues/163">#163</a> from ChandanChainani/fix/162/x-order_not_working_with...</li>
<li><a href="https://github.com/go-openapi/spec/commit/b123375b48daebf61f70cd51443f95c51e4b64eb"><code>b123375</code></a> Fix <code>x-order</code> not working with number value <a href="https://redirect.github.com/go-openapi/spec/issues/162">#162</a></li>
<li><a href="https://github.com/go-openapi/spec/commit/7ee5140616c37284180358d92c6f8ed40a85af4d"><code>7ee5140</code></a> Merge pull request <a href="https://redirect.github.com/go-openapi/spec/issues/166">#166</a> from Aven30/fix-spec-parser-ignoring-response-entries...</li>
<li><a href="https://github.com/go-openapi/spec/commit/f85abf4bfd5ab9fc74d26bc5c0674fbf4bb7ff54"><code>f85abf4</code></a> Fix <a href="https://redirect.github.com/go-openapi/spec/issues/165">#165</a></li>
<li>See full diff in <a href="https://github.com/go-openapi/spec/compare/v0.20.8...v0.20.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/go-openapi/spec&package-manager=go_modules&previous-version=0.20.8&new-version=0.20.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 15:19:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Bump github.com/cucumber/godog from 0.12.6 to 0.13.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/cucumber/godog](https://github.com/cucumber/godog) from 0.12.6 to 0.13.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cucumber/godog/releases">github.com/cucumber/godog's releases</a>.</em></p>
<blockquote>
<h2>v0.13.0</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(*): BREAKING CHANGE, use new repos for cucumber and messages by <a href="https://github.com/otrava7"><code>@​otrava7</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/515">cucumber/godog#515</a></li>
<li>Configure Renovate by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/512">cucumber/godog#512</a></li>
<li>fix(deps): update module github.com/cucumber/godog to v0.12.6 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/520">cucumber/godog#520</a></li>
<li>chore(deps): update codecov/codecov-action action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/530">cucumber/godog#530</a></li>
<li>chore(deps): update actions/checkout action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/528">cucumber/godog#528</a></li>
<li>chore(deps): update actions/setup-go action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/529">cucumber/godog#529</a></li>
<li>chore(deps): update actions/cache action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/527">cucumber/godog#527</a></li>
<li>fix(deps): update module github.com/cucumber/gherkin/go/v26 to v26.0.3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/519">cucumber/godog#519</a></li>
<li>fix(deps): update module github.com/data-dog/go-txdb to v0.1.5 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/522">cucumber/godog#522</a></li>
<li>fix(deps): update module github.com/go-sql-driver/mysql to v1.7.0 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/524">cucumber/godog#524</a></li>
<li>fix(deps): update module github.com/hashicorp/go-memdb to v1.3.4 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/523">cucumber/godog#523</a></li>
<li>fix(deps): update module github.com/spf13/cobra to v1.6.1 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/526">cucumber/godog#526</a></li>
<li>fix(deps): update module github.com/smartystreets/goconvey to v1.7.2 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/525">cucumber/godog#525</a></li>
<li>Setup Renovate with default Configs by <a href="https://github.com/mpkorstanje"><code>@​mpkorstanje</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/531">cucumber/godog#531</a></li>
<li>Implement unambiguous keywords by <a href="https://github.com/otrava7"><code>@​otrava7</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/509">cucumber/godog#509</a></li>
<li>docs(*): correct example by <a href="https://github.com/otrava7"><code>@​otrava7</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/538">cucumber/godog#538</a></li>
<li>fix(deps): update module github.com/data-dog/go-txdb to v0.1.6 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/540">cucumber/godog#540</a></li>
<li>fix(deps): update module github.com/stretchr/testify to v1.8.2 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/541">cucumber/godog#541</a></li>
<li>chore(deps): update actions/setup-go action to v4 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/546">cucumber/godog#546</a></li>
<li>docs: prefer go test to use of godog cli in README by <a href="https://github.com/danielhelfand"><code>@​danielhelfand</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/548">cucumber/godog#548</a></li>
<li>Use <code>fs.FS</code> abstraction for filesystem by <a href="https://github.com/tigh-latte"><code>@​tigh-latte</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/550">cucumber/godog#550</a></li>
<li>Result of testing.T respect strict option by <a href="https://github.com/eiel"><code>@​eiel</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/539">cucumber/godog#539</a></li>
<li>Update CI for go1.20 by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/552">cucumber/godog#552</a></li>
<li>fix(deps): update module github.com/cucumber/gherkin/go/v26 to v26.1.0 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/549">cucumber/godog#549</a></li>
<li>cancel context for each scenario by <a href="https://github.com/draganm"><code>@​draganm</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/514">cucumber/godog#514</a></li>
<li>Use staticcheck GitHub Action by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/563">cucumber/godog#563</a></li>
<li>refactor: test_context.go by <a href="https://github.com/longyue0521"><code>@​longyue0521</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/564">cucumber/godog#564</a></li>
<li>Improve hooks invocation flow by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/568">cucumber/godog#568</a></li>
<li>fix(examples): update api example by <a href="https://github.com/forward32"><code>@​forward32</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/532">cucumber/godog#532</a></li>
<li>Improve example with concurrency support by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/573">cucumber/godog#573</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/otrava7"><code>@​otrava7</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/515">cucumber/godog#515</a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/512">cucumber/godog#512</a></li>
<li><a href="https://github.com/mpkorstanje"><code>@​mpkorstanje</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/531">cucumber/godog#531</a></li>
<li><a href="https://github.com/danielhelfand"><code>@​danielhelfand</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/548">cucumber/godog#548</a></li>
<li><a href="https://github.com/tigh-latte"><code>@​tigh-latte</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/550">cucumber/godog#550</a></li>
<li><a href="https://github.com/eiel"><code>@​eiel</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/539">cucumber/godog#539</a></li>
<li><a href="https://github.com/draganm"><code>@​draganm</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/514">cucumber/godog#514</a></li>
<li><a href="https://github.com/longyue0521"><code>@​longyue0521</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/564">cucumber/godog#564</a></li>
<li><a href="https://github.com/forward32"><code>@​forward32</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/532">cucumber/godog#532</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cucumber/godog/compare/v0.12.6...v0.13.0">https://github.com/cucumber/godog/compare/v0.12.6...v0.13.0</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cucumber/godog/blob/main/CHANGELOG.md">github.com/cucumber/godog's changelog</a>.</em></p>
<blockquote>
<h2>[v0.13.0]</h2>
<h3>Added</h3>
<ul>
<li>Support for reading feature files from an <code>fs.FS</code> (<a href="https://redirect.github.com/cucumber/godog/pull/550">550</a> - <a href="https://github.com/tigh-latte">tigh-latte</a>)</li>
<li>Added keyword functions. (<a href="https://redirect.github.com/cucumber/godog/pull/509">509</a> - <a href="https://github.com/otrava7">otrava7</a>)</li>
<li>Prefer go test to use of godog cli in README (<a href="https://redirect.github.com/cucumber/godog/pull/548">548</a> - <a href="https://github.com/danielhelfand">danielhelfand</a>)</li>
<li>Use <code>fs.FS</code> abstraction for filesystem (<a href="https://redirect.github.com/cucumber/godog/pull/550">550</a> - <a href="https://github.com/tigh-latte">tigh-latte</a>)</li>
<li>Cancel context for each scenario (<a href="https://redirect.github.com/cucumber/godog/pull/514">514</a> - <a href="https://github.com/draganm">draganm</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Improve hooks invocation flow (<a href="https://redirect.github.com/cucumber/godog/pull/568">568</a> - <a href="https://github.com/vearutop">vearutop</a>)</li>
<li>Result of testing.T respect strict option (<a href="https://redirect.github.com/cucumber/godog/pull/539">539</a> - <a href="https://github.com/eiel">eiel</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>BREAKING CHANGE, upgraded cucumber and messages dependencies = (<a href="https://redirect.github.com/cucumber/godog/pull/515">515</a> - <a href="https://github.com/otrava7">otrava7</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cucumber/godog/commit/6b96d47e70b95ff62bb240aff3e588569b7d19b2"><code>6b96d47</code></a> Prepare CHANGELOG.md for new release</li>
<li><a href="https://github.com/cucumber/godog/commit/d3aec7142e95ad5a0c9ec849e72d3accef089040"><code>d3aec71</code></a> Improve example with concurrency support (<a href="https://redirect.github.com/cucumber/godog/issues/573">#573</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/75d5cab90d0443b1eff2903a4fbfbdb6e594a139"><code>75d5cab</code></a> fix(examples): update api example (<a href="https://redirect.github.com/cucumber/godog/issues/532">#532</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/3e0f9026f3ddb697b9e4e82b0e770fbbe0e966b7"><code>3e0f902</code></a> Improve hooks invocation flow (<a href="https://redirect.github.com/cucumber/godog/issues/568">#568</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/51d164ff5789b10ad013c6db4099f4499f1a31a0"><code>51d164f</code></a> Print verbose error to enable traces</li>
<li><a href="https://github.com/cucumber/godog/commit/72db47c51993eb6d29378cbda01e24fae4156c7f"><code>72db47c</code></a> refactor: test_context.go (<a href="https://redirect.github.com/cucumber/godog/issues/564">#564</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/ea50e4bdfcd911252e39f303b9327197079be1e4"><code>ea50e4b</code></a> Use staticcheck GitHub Action (<a href="https://redirect.github.com/cucumber/godog/issues/563">#563</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/7f75c5d4ee9cd2e9d86b7ff62ebf38b9172d2c88"><code>7f75c5d</code></a> Remove redundant return</li>
<li><a href="https://github.com/cucumber/godog/commit/35820ff9fee90f20afdc1c20a7e5e7c4d6c59ebb"><code>35820ff</code></a> Reduce deps, fix CI for go1.16, format imports</li>
<li><a href="https://github.com/cucumber/godog/commit/3eae6c04373960d397e20e1d24cc8ee4210af72e"><code>3eae6c0</code></a> Update dependencies</li>
<li>Additional commits viewable in <a href="https://github.com/cucumber/godog/compare/v0.12.6...v0.13.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/cucumber/godog&package-manager=go_modules&previous-version=0.12.6&new-version=0.13.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 15:19:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Update dependencies to address GO-2023-2153
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
        Created At 2023-11-05 10:25:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.53.0 to 1.56.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.53.0 to 1.56.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.56.3</h2>
<h1>Security</h1>
<ul>
<li>
<p>server: prohibit more than MaxConcurrentStreams handlers from running at once (CVE-2023-44487)</p>
<p>In addition to this change, applications should ensure they do not leave running tasks behind related to the RPC before returning from method handlers, or should enforce appropriate limits on any such work.</p>
</li>
</ul>
<h2>Release 1.56.2</h2>
<ul>
<li>status: To fix a panic, <code>status.FromError</code> now returns an error with <code>codes.Unknown</code> when the error implements the <code>GRPCStatus()</code> method, and calling <code>GRPCStatus()</code> returns <code>nil</code>. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6374">#6374</a>)</li>
</ul>
<h2>Release 1.56.1</h2>
<ul>
<li>client: handle empty address lists correctly in addrConn.updateAddrs</li>
</ul>
<h2>Release 1.56.0</h2>
<h1>New Features</h1>
<ul>
<li>client: support channel idleness using <code>WithIdleTimeout</code> dial option (<a href="https://redirect.github.com/grpc/grpc-go/issues/6263">#6263</a>)
<ul>
<li>This feature is currently disabled by default, but will be enabled with a 30 minute default in the future.</li>
</ul>
</li>
<li>client: when using pickfirst, keep channel state in TRANSIENT_FAILURE until it becomes READY (<a href="https://github.com/grpc/proposal/blob/master/A62-pick-first.md">gRFC A62</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6306">#6306</a>)</li>
<li>xds: Add support for Custom LB Policies (<a href="https://github.com/grpc/proposal/blob/master/A52-xds-custom-lb-policies.md">gRFC A52</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6224">#6224</a>)</li>
<li>xds: support pick_first Custom LB policy (<a href="https://github.com/grpc/proposal/blob/master/A62-pick-first.md">gRFC A62</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6314">#6314</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6317">#6317</a>)</li>
<li>client: add support for pickfirst address shuffling (<a href="https://github.com/grpc/proposal/blob/master/A62-pick-first.md">gRFC A62</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6311">#6311</a>)</li>
<li>xds: Add support for String Matcher Header Matcher in RDS (<a href="https://redirect.github.com/grpc/grpc-go/issues/6313">#6313</a>)</li>
<li>xds/outlierdetection: Add Channelz Logger to Outlier Detection LB (<a href="https://redirect.github.com/grpc/grpc-go/issues/6145">#6145</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/s-matyukevich"><code>@​s-matyukevich</code></a></li>
</ul>
</li>
<li>xds: enable RLS in xDS by default (<a href="https://redirect.github.com/grpc/grpc-go/issues/6343">#6343</a>)</li>
<li>orca: add support for application_utilization field and missing range checks on several metrics setters</li>
<li>balancer/weightedroundrobin: add new LB policy for balancing between backends based on their load reports (<a href="https://github.com/grpc/proposal/blob/master/A58-client-side-weighted-round-robin-lb-policy.md">gRFC A58</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6241">#6241</a>)</li>
<li>authz: add conversion of json to RBAC Audit Logging config (<a href="https://redirect.github.com/grpc/grpc-go/issues/6192">#6192</a>)</li>
<li>authz: add support for stdout logger (<a href="https://redirect.github.com/grpc/grpc-go/issues/6230">#6230</a> and <a href="https://redirect.github.com/grpc/grpc-go/issues/6298">#6298</a>)</li>
<li>authz: support customizable audit functionality for authorization policy (<a href="https://redirect.github.com/grpc/grpc-go/issues/6192">#6192</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6230">#6230</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6298">#6298</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6158">#6158</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6304">#6304</a> and <a href="https://redirect.github.com/grpc/grpc-go/issues/6225">#6225</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>orca: fix a race at startup of out-of-band metric subscriptions that would cause the report interval to request 0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6245">#6245</a>)</li>
<li>xds/xdsresource: Fix Outlier Detection Config Handling and correctly set xDS Defaults (<a href="https://redirect.github.com/grpc/grpc-go/issues/6361">#6361</a>)</li>
<li>xds/outlierdetection: Fix Outlier Detection Config Handling by setting defaults in ParseConfig() (<a href="https://redirect.github.com/grpc/grpc-go/issues/6361">#6361</a>)</li>
</ul>
<h1>API Changes</h1>
<ul>
<li>orca: allow a ServerMetricsProvider to be passed to the ORCA service and ServerOption (<a href="https://redirect.github.com/grpc/grpc-go/issues/6223">#6223</a>)</li>
</ul>
<h2>Release 1.55.1</h2>
<ul>
<li>status: To fix a panic, <code>status.FromError</code> now returns an error with <code>codes.Unknown</code> when the error implements the <code>GRPCStatus()</code> method, and calling <code>GRPCStatus()</code> returns <code>nil</code>. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6374">#6374</a>)</li>
</ul>
<h2>Release 1.55.0</h2>
<h1>Behavior Changes</h1>
<ul>
<li>xds: enable federation support by default (<a href="https://redirect.github.com/grpc/grpc-go/issues/6151">#6151</a>)</li>
<li>status: <code>status.Code</code> and <code>status.FromError</code> handle wrapped errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/6031">#6031</a> and <a href="https://redirect.github.com/grpc/grpc-go/issues/6150">#6150</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/1055b481ed2204a29d233286b9b50c42b63f8825"><code>1055b48</code></a> Update version.go to 1.56.3 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6713">#6713</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/5efd7bd73e11fea58d1c7f1c110902e78a286299"><code>5efd7bd</code></a> server: prohibit more than MaxConcurrentStreams handlers from running at once...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bd1f038e7234580c2694e433bec5cd97e7b7f662"><code>bd1f038</code></a> Upgrade version.go to 1.56.3-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6434">#6434</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/faab8736bf73291f92b867d5dae31c927d53d508"><code>faab873</code></a> Update version.go to v1.56.2 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6432">#6432</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6b0b291d79831b1c8caafceec268b82c92253f96"><code>6b0b291</code></a> status: fix panic when servers return a wrapped error with status OK (<a href="https://redirect.github.com/grpc/grpc-go/issues/6374">#6374</a>) ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ed56401aa514462d5371713b8ec5c889da33953c"><code>ed56401</code></a> [PSM interop] Don't fail target if sub-target already failed (<a href="https://redirect.github.com/grpc/grpc-go/issues/6390">#6390</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6405">#6405</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/cd6a794f0bdcf9a216e8f4d3c5717faf96d9fd78"><code>cd6a794</code></a> Update version.go to v1.56.2-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6387">#6387</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/5b67e5ea449ef0686a0c0b6de48cd4cb63e3db2a"><code>5b67e5e</code></a> Update version.go to v1.56.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6386">#6386</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d0f5150384a87f9fcac488a9c18727a55b7354c1"><code>d0f5150</code></a> client: handle empty address lists correctly in addrConn.updateAddrs (<a href="https://redirect.github.com/grpc/grpc-go/issues/6354">#6354</a>) ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/997c1ea101cc5d496d2b148388f1df49632a9171"><code>997c1ea</code></a> Change version to 1.56.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6345">#6345</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.53.0...v1.56.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.53.0&new-version=1.56.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-contract-api-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 00:39:21 +0000 UTC
    </div>
</div>

