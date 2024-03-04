---
layout: default
title: fabric-chaincode-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-go
---

# fabric-chaincode-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Bump github.com/stretchr/testify from 1.8.2 to 1.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/stretchr/testify](https://github.com/stretchr/testify) from 1.8.2 to 1.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/stretchr/testify/releases">github.com/stretchr/testify's releases</a>.</em></p>
<blockquote>
<h2>v1.9.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix Go modules version by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1394">stretchr/testify#1394</a></li>
<li>Document that require is not safe to call in created goroutines by <a href="https://github.com/programmer04"><code>@​programmer04</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1392">stretchr/testify#1392</a></li>
<li>Remove myself from MAINTAINERS.md by <a href="https://github.com/mvdkleijn"><code>@​mvdkleijn</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1367">stretchr/testify#1367</a></li>
<li>Correct spelling/grammar by <a href="https://github.com/echarrod"><code>@​echarrod</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1389">stretchr/testify#1389</a></li>
<li>docs: Update URLs in README by <a href="https://github.com/davidjb"><code>@​davidjb</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1349">stretchr/testify#1349</a></li>
<li>Update mockery link to Github Pages in README by <a href="https://github.com/LandonTClipp"><code>@​LandonTClipp</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1346">stretchr/testify#1346</a></li>
<li>docs: Fix typos in tests and comments by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1410">stretchr/testify#1410</a></li>
<li>CI: tests from go1.17 by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1409">stretchr/testify#1409</a></li>
<li>Fix adding ? when no values passed by <a href="https://github.com/lesichkovm"><code>@​lesichkovm</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1320">stretchr/testify#1320</a></li>
<li>codegen: use standard header for generated files by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1406">stretchr/testify#1406</a></li>
<li>mock: AssertExpectations log reason only on failure by <a href="https://github.com/hikyaru-suzuki"><code>@​hikyaru-suzuki</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1360">stretchr/testify#1360</a></li>
<li>assert: fix flaky TestNeverTrue by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1417">stretchr/testify#1417</a></li>
<li>README: fix typos &quot;set up&quot; vs &quot;setup&quot; by <a href="https://github.com/ossan-dev"><code>@​ossan-dev</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1428">stretchr/testify#1428</a></li>
<li>mock: move regexp compilation outside of <code>Called</code> by <a href="https://github.com/aud10slave"><code>@​aud10slave</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/631">stretchr/testify#631</a></li>
<li>assert: refactor internal func getLen() by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1445">stretchr/testify#1445</a></li>
<li>mock: deprecate type AnythingOfTypeArgument (<a href="https://redirect.github.com/stretchr/testify/issues/1434">#1434</a>) by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1441">stretchr/testify#1441</a></li>
<li>Remove no longer needed assert.canConvert by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1470">stretchr/testify#1470</a></li>
<li>assert: ObjectsAreEqual: use time.Equal for time.Time types by <a href="https://github.com/tscales"><code>@​tscales</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1464">stretchr/testify#1464</a></li>
<li>Bump actions/checkout from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1466">stretchr/testify#1466</a></li>
<li>Bump actions/setup-go from 3.2.0 to 4.1.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1451">stretchr/testify#1451</a></li>
<li>fix: make EventuallyWithT concurrency safe by <a href="https://github.com/czeslavo"><code>@​czeslavo</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1395">stretchr/testify#1395</a></li>
<li>assert: fix httpCode and HTTPBody occur panic when http.Handler read Body by <a href="https://github.com/hidu"><code>@​hidu</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1484">stretchr/testify#1484</a></li>
<li>assert.EqualExportedValues: fix handling of arrays by <a href="https://github.com/zrbecker"><code>@​zrbecker</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1473">stretchr/testify#1473</a></li>
<li>.github: use latest Go versions by <a href="https://github.com/kevinburkesegment"><code>@​kevinburkesegment</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1489">stretchr/testify#1489</a></li>
<li>assert: Deprecate EqualExportedValues by <a href="https://github.com/HaraldNordgren"><code>@​HaraldNordgren</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1488">stretchr/testify#1488</a></li>
<li>suite: refactor test assertions by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1474">stretchr/testify#1474</a></li>
<li>suite: fix SetupSubTest and TearDownSubTest execution order by <a href="https://github.com/linusbarth"><code>@​linusbarth</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1471">stretchr/testify#1471</a></li>
<li>docs: Fix deprecation comments for http package by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1335">stretchr/testify#1335</a></li>
<li>Add map support doc comments to Subset and NotSubset by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1306">stretchr/testify#1306</a></li>
<li>TestErrorIs/TestNotErrorIs: check error message contents by <a href="https://github.com/craig65535"><code>@​craig65535</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1435">stretchr/testify#1435</a></li>
<li>suite: fix subtest names (fix <a href="https://redirect.github.com/stretchr/testify/issues/1501">#1501</a>) by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1504">stretchr/testify#1504</a></li>
<li>assert: improve unsafe.Pointer tests by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1505">stretchr/testify#1505</a></li>
<li>assert: simplify isNil implementation by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1506">stretchr/testify#1506</a></li>
<li>assert.InEpsilonSlice: fix expected/actual order and other improvements by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1483">stretchr/testify#1483</a></li>
<li>Fix dependency cycle with objx <a href="https://redirect.github.com/stretchr/testify/issues/1292">#1292</a> by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1453">stretchr/testify#1453</a></li>
<li>mock: refactor TestIsArgsEqual by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1444">stretchr/testify#1444</a></li>
<li>mock: optimize argument matching checks by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1416">stretchr/testify#1416</a></li>
<li>assert: fix TestEventuallyTimeout by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1412">stretchr/testify#1412</a></li>
<li>CI: add go 1.21 in GitHub Actions by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1450">stretchr/testify#1450</a></li>
<li>suite: fix recoverAndFailOnPanic to report test failure at the right location by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1502">stretchr/testify#1502</a></li>
<li>Update maintainers by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1533">stretchr/testify#1533</a></li>
<li>assert: Fix EqualValues to handle overflow/underflow by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1531">stretchr/testify#1531</a></li>
<li>assert: better formatting for Len() error by <a href="https://github.com/kevinburkesegment"><code>@​kevinburkesegment</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1485">stretchr/testify#1485</a></li>
<li>Ensure AssertExpectations does not fail in skipped tests by <a href="https://github.com/ianrose14"><code>@​ianrose14</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1331">stretchr/testify#1331</a></li>
<li>suite: fix deadlock in suite.Require()/Assert() by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1535">stretchr/testify#1535</a></li>
<li>Revert &quot;assert: ObjectsAreEqual: use time.Equal for time.Time type&quot; by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1537">stretchr/testify#1537</a></li>
<li>[chore] Add issue templates by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1538">stretchr/testify#1538</a></li>
<li>Update the build status badge by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1540">stretchr/testify#1540</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/stretchr/testify/commit/bb548d0473d4e1c9b7bbfd6602c7bf12f7a84dd2"><code>bb548d0</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1552">#1552</a> from stretchr/dependabot/go_modules/github.com/stret...</li>
<li><a href="https://github.com/stretchr/testify/commit/814075f391adffd2bf2b5110a74c51827ba132c4"><code>814075f</code></a> build(deps): bump github.com/stretchr/objx from 0.5.1 to 0.5.2</li>
<li><a href="https://github.com/stretchr/testify/commit/e0456122451b1839c8d58d32df6364e4d0f0a709"><code>e045612</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1339">#1339</a> from bogdandrutu/uintptr</li>
<li><a href="https://github.com/stretchr/testify/commit/5b6926d686d412518f50e888b9ae9b938355e011"><code>5b6926d</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1385">#1385</a> from hslatman/not-implements</li>
<li><a href="https://github.com/stretchr/testify/commit/9f97d67703eff02136d487e6c907e76fdea31a8b"><code>9f97d67</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1550">#1550</a> from stretchr/release-notes</li>
<li><a href="https://github.com/stretchr/testify/commit/bcb0d3fe49ff300fb78288cc144bc61a881f58ec"><code>bcb0d3f</code></a> Include the auto-release notes in releases</li>
<li><a href="https://github.com/stretchr/testify/commit/fb770f8238261aa22f8e0c56f18168ccb90f4a09"><code>fb770f8</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1247">#1247</a> from ccoVeille/typos</li>
<li><a href="https://github.com/stretchr/testify/commit/85d8bb6eea715dcbbb68f7c87b50e1956e20f892"><code>85d8bb6</code></a> fix typos in comments, tests and github templates</li>
<li><a href="https://github.com/stretchr/testify/commit/e2741fa4e9bf2fdfe3ed48d976a7eeebe76c5009"><code>e2741fa</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1548">#1548</a> from arjunmahishi/msgAndArgs</li>
<li><a href="https://github.com/stretchr/testify/commit/6e59f20c0d3883d2bdc589a9e48374ea30601851"><code>6e59f20</code></a> http_assertions: assert that the msgAndArgs actually works in tests</li>
<li>Additional commits viewable in <a href="https://github.com/stretchr/testify/compare/v1.8.2...v1.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/stretchr/testify&package-manager=go_modules&previous-version=1.8.2&new-version=1.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-04 04:44:55 +0000 UTC
    </div>
</div>

