---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2547" class=".btn">#2547</a>
            </td>
            <td>
                <b>
                    build(deps): bump tough-cookie from 4.0.0 to 4.1.3 in /weaver/common/policy-dsl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tough-cookie](https://github.com/salesforce/tough-cookie) from 4.0.0 to 4.1.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/salesforce/tough-cookie/releases">tough-cookie's releases</a>.</em></p>
<blockquote>
<h2>4.1.3</h2>
<p>Security fix for Prototype Pollution discovery in <a href="https://redirect.github.com/salesforce/tough-cookie/issues/282">#282</a>. This is a minor release, although output from the <code>inspect</code> utility is affected by this change, we felt this change was important enough to be pushed into the next patch.</p>
<h2>4.1.2 -- Patch and Bugfix Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow set cookies with localhost by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/253">salesforce/tough-cookie#253</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2">https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2</a></p>
<h2>4.1.1</h2>
<h2>Patch Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow special use domains by default by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/249">salesforce/tough-cookie#249</a></li>
<li>4.1.1 Patch -- allow special use domains by default by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/250">salesforce/tough-cookie#250</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1">https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1</a></p>
<h2>4.1.0</h2>
<p>v4.1.0</p>
<p>Minor release, focused mainly on resolving reported issues and some minor feature work.</p>
<h2>What's Changed</h2>
<ul>
<li>Create CHANGELOG.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/189">salesforce/tough-cookie#189</a></li>
<li>Missing param validation issue145 by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/193">salesforce/tough-cookie#193</a></li>
<li>Create SECURITY.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/201">salesforce/tough-cookie#201</a></li>
<li>Create CODE_OF_CONDUCT.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/200">salesforce/tough-cookie#200</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/195">#195</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/202">salesforce/tough-cookie#202</a></li>
<li>Add explanation and more special-use domains by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/203">salesforce/tough-cookie#203</a></li>
<li>Sync of constructor options for serialization by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/204">salesforce/tough-cookie#204</a></li>
<li>Returned null in case of empty cookie value by <a href="https://github.com/vsin12"><code>@​vsin12</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/196">salesforce/tough-cookie#196</a></li>
<li>132 str trim not a function by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/209">salesforce/tough-cookie#209</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/153">#153</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/210">salesforce/tough-cookie#210</a></li>
<li>Fix permuteDomain with trailing dot by <a href="https://github.com/ruoho-sfdc"><code>@​ruoho-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/216">salesforce/tough-cookie#216</a></li>
<li>Issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/213">#213</a> -- added gh-actions flow for building and testing tough-co… by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/218">salesforce/tough-cookie#218</a></li>
<li>Issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/210">#210</a> -- Updated workflow to use npm install. by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/220">salesforce/tough-cookie#220</a></li>
<li>@<a href="https://redirect.github.com/salesforce/tough-cookie/issues/215">GH-215</a> -- Tests that document localhost behavior when set as domain. by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/221">salesforce/tough-cookie#221</a></li>
<li>fix: MemoryCookieStore methods should exist on the prototype, not on the class. by <a href="https://github.com/wjhsf"><code>@​wjhsf</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/226">salesforce/tough-cookie#226</a></li>
<li>Unit test cases for <code>allowSpecialUseDomain</code> option by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/225">salesforce/tough-cookie#225</a></li>
<li>[Snyk] Upgrade universalify from 0.1.2 to 0.2.0 by <a href="https://github.com/snyk-bot"><code>@​snyk-bot</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/228">salesforce/tough-cookie#228</a></li>
<li>React Native Support by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/227">salesforce/tough-cookie#227</a></li>
<li>Adding Updating CODEOWNERS with ECCN as per Export Control Compliance by <a href="https://github.com/svc-scm"><code>@​svc-scm</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/223">salesforce/tough-cookie#223</a></li>
<li>fix: domain match routine by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/236">salesforce/tough-cookie#236</a></li>
<li>Stop using the internal NodeJS punycode module by <a href="https://github.com/gboer"><code>@​gboer</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/238">salesforce/tough-cookie#238</a></li>
<li>Initial documentation review by <a href="https://github.com/mcarey86"><code>@​mcarey86</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/234">salesforce/tough-cookie#234</a></li>
<li>fix: distinguish between no samesite and samesite=none by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/240">salesforce/tough-cookie#240</a></li>
<li>Prepare tough-cookie 4.1 for publishing (updated GitHub actions, move… by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/242">salesforce/tough-cookie#242</a></li>
<li>4.1.0 release to NPM by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/245">salesforce/tough-cookie#245</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4ff4d29f6cefd279a412b8d62a21142ebd410b36"><code>4ff4d29</code></a> 4.1.3 release preparation, update the package and lib/version to 4.1.3. (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/284">#284</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/12d474791bb856004e858fdb1c47b7608d09cf6e"><code>12d4747</code></a> Prevent prototype pollution in cookie memstore (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/283">#283</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/f06b72d1d447f33dfa6222c0a3c0c5e063558248"><code>f06b72d</code></a> Fix documentation for store.findCookies, missing allowSpecialUseDomain proper...</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/b1a8898ee3f8af52c6c1c355555d9f50ebe626ce"><code>b1a8898</code></a> fix: allow set cookies with localhost (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/253">#253</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/ec707966e68a48199e646e2fa6b3055df6a280f0"><code>ec70796</code></a> 4.1.1 Patch -- allow special use domains by default (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/250">#250</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/d4ac5801dd2c2d53eec51329e5380bbffb23bfaf"><code>d4ac580</code></a> fix: allow special use domains by default (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/249">#249</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/79c2f7d373e39918605c270ecd965f507701233d"><code>79c2f7d</code></a> 4.1.0 release to NPM (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/245">#245</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4fafc179a798a570e32fc698034f0480c07d9afa"><code>4fafc17</code></a> Prepare tough-cookie 4.1 for publishing (updated GitHub actions, move Dockerf...</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/aa4396da7abcb2dbe607db7b31606f7dd0f45709"><code>aa4396d</code></a> fix: distinguish between no samesite and samesite=none (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/240">#240</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/b8d751188da697157e5eed81fa1e5f806fdfb541"><code>b8d7511</code></a> Modernize README (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/234">#234</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/salesforce/tough-cookie/compare/v4.0.0...v4.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tough-cookie&package-manager=npm_and_yarn&previous-version=4.0.0&new-version=4.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 20:54:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2540" class=".btn">#2540</a>
            </td>
            <td>
                <b>
                    docs(examples): upgrade Angular to v15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Upgraded from Angular v14 to v15 for both GUI packages that use it.
2. Upgraded the Typescript compiler project-wide to 4.8.4
3. Due to 2) There was a change needed in the file
examples/cactus-example-discounted-asset-trade/transaction-fabric.ts
which introduces a constraint on the T type parameter.
4. Disabled the staged files linting because right now ESLint is broken
due to our Typescript version being >=4.8.0 (and upgrading it was not
an option because then it is broken due to ESM issues...)
5. Cleaned out a lot of the unused dev dependencies of the front-end
packages where angular was upgraded. These dependencies were related to
end-to-end browser testing which we haven't set up yet to be executed
because all the front-end packages are just example code that - while
important to test - does not have the highest priority in this sense.
6. Set the rootDir property in the electricity trade example's tsconfig.json
    file to the standard value (./) because without it the new tsc compiler
    version seems to be putting the compiled source files in a different
    location by default (probably an accidental breaking change on the compiler's
    part or just a lack of my understanding of how the configuration of it
    should work). With the rootDir explicitly specified, it appears to be
    compiling the files in the correct location as before.

Fixes #2229

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 22:47:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2538" class=".btn">#2538</a>
            </td>
            <td>
                <b>
                    refactor(plugin-htlc-eth-besu): stop using the deprecated api.encodePacked
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Add tests to vanilla HashTimeLock
2. Replace abi.encodePacked by abi.encode
3. Compile and replace generated ABIs (for HashTimeLock and PrivateHashTimeLock)

Addresses #2531 
cc @petermetz 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 05:35:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2537" class=".btn">#2537</a>
            </td>
            <td>
                <b>
                    build(deps): bump @grpc/grpc-js from 1.3.6 to 1.8.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.3.6 to 1.8.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<ul>
<li>Continue keepalive pings after receiving a GOAWAY on the client (<a href="https://redirect.github.com/grpc/grpc-node/issues/2308">#2308</a>)</li>
<li>Fix handling of keepalive timers when the timeout is longer than the interval (<a href="https://redirect.github.com/grpc/grpc-node/issues/2304">#2304</a> contributed by <a href="https://github.com/nicknotfun"><code>@​nicknotfun</code></a>, included in <a href="https://redirect.github.com/grpc/grpc-node/issues/2308">#2308</a>)</li>
<li>Ensure the last received message is fully handled before outputting status (<a href="https://redirect.github.com/grpc/grpc-node/issues/2316">#2316</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js-xds</code> 1.8.2</h2>
<ul>
<li>Fix behavior when receiving invalid resources after receiving valid resources for the same resource name (<a href="https://redirect.github.com/grpc/grpc-node/issues/2433">#2433</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.1</h2>
<ul>
<li>Implement support for the <code>grpc.service_config_disable_resolution</code> channel option (<a href="https://redirect.github.com/grpc/grpc-node/issues/2277">#2277</a> contributed by <a href="https://github.com/kleinsch"><code>@​kleinsch</code></a>)</li>
<li>Include standard headers in trailers-only responses (<a href="https://redirect.github.com/grpc/grpc-node/issues/2305">#2305</a>)</li>
<li>Fix a memory leak in the retry implementation (<a href="https://redirect.github.com/grpc/grpc-node/issues/2306">#2306</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js-xds</code> 1.8.1</h2>
<ul>
<li>Populate Node message field user_agent_version (<a href="https://redirect.github.com/grpc/grpc-node/issues/2391">#2391</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js-xds</code> 1.8.0</h2>
<ul>
<li>Add <a href="https://github.com/grpc/proposal/blob/master/A44-xds-retry.md">Retry support</a> (<a href="https://redirect.github.com/grpc/grpc-node/issues/2280">#2280</a>)</li>
<li>Drop support for xDS version 2 following the timeline in <a href="https://github.com/grpc/proposal/blob/master/A30-xds-v3.md">gRFC A30</a> (<a href="https://redirect.github.com/grpc/grpc-node/issues/2244">#2244</a>)</li>
<li>Update xDS Client failure mode behavior as specified in <a href="https://github.com/grpc/proposal/blob/master/A57-xds-client-failure-mode-behavior.md">gRFC A57</a></li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.0</h2>
<ul>
<li>Implement retries (<a href="https://github.com/grpc/proposal/blob/master/A6-client-retries.md">specified in gRFC A6</a>) (<a href="https://redirect.github.com/grpc/grpc-node/issues/2243">#2243</a>, <a href="https://redirect.github.com/grpc/grpc-node/issues/2278">#2278</a>)</li>
<li>Enable servers to send trailers-only responses (<a href="https://redirect.github.com/grpc/grpc-node/issues/2278">#2278</a>)</li>
<li>Add server connection management options (<a href="https://redirect.github.com/grpc/grpc-node/issues/2272">#2272</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.7.3</h2>
<ul>
<li>Server performance improvements (<a href="https://redirect.github.com/grpc/grpc-node/issues/2249">#2249</a> contributed by <a href="https://github.com/AVVS"><code>@​AVVS</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.7.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/7ab5368a6e5863fa58ac36b3a0a7d7a07d82eed8"><code>7ab5368</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a> from murgatroid99/grpc-js_retry_commit_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/2b7f296680f30fd9822f2183b2280ce0db8a6d7f"><code>2b7f296</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a> from murgatroid99/grpc-js_export_interceptor_types</li>
<li><a href="https://github.com/grpc/grpc-node/commit/9bf74d9d5973102e5da9bb0feb97c5d06c40ab00"><code>9bf74d9</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a> from murgatroid99/grpc-js_retry_clean_status</li>
<li><a href="https://github.com/grpc/grpc-node/commit/18c803e6dd458b762fa5fe7361b4abc59d263382"><code>18c803e</code></a> grpc-js: Export InterceptingListener and NextCall types</li>
<li><a href="https://github.com/grpc/grpc-node/commit/3596c4f65518b1f0e8aae841b255a98e68dfe608"><code>3596c4f</code></a> grpc-js: Remove progress field in status from retrying call</li>
<li><a href="https://github.com/grpc/grpc-node/commit/cf090c7f5075452d322ead84496b7f0ed0bb1868"><code>cf090c7</code></a> grpc-js: Fix commitCallWithMostMessages trying to commit completed attempts</li>
<li><a href="https://github.com/grpc/grpc-node/commit/cea545dd7763a260130bf178b8838792c5283fb7"><code>cea545d</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a> from murgatroid99/grpc-js_transport_fix_active_call_...</li>
<li><a href="https://github.com/grpc/grpc-node/commit/3efdc7b58c0910075659982603e850cc883e019b"><code>3efdc7b</code></a> grpc-js: Bump version to 1.8.7</li>
<li><a href="https://github.com/grpc/grpc-node/commit/0d177a818f83cd9de6fc1f5e4bd343de4538e35a"><code>0d177a8</code></a> grpc-js: Fix tracking of active calls in transport</li>
<li><a href="https://github.com/grpc/grpc-node/commit/f29e99d0c6cf350dfc0006440ad9c417f90d7d48"><code>f29e99d</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a> from murgatroid99/grpc-js_transport_garbage_collection</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.3.6...@grpc/grpc-js@1.8.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.3.6&new-version=1.8.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:40:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2536" class=".btn">#2536</a>
            </td>
            <td>
                <b>
                    build(deps): bump google.golang.org/grpc from 1.30.0 to 1.53.0 in /packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/fixtures/go/asset-transfer-private-data/chaincode-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.30.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.30.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.30.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 20:59:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2535" class=".btn">#2535</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add new connector plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add new plugin for connecting with Ethereum ledgers. New connector is based on already existing quorum connector. The main reason for introducing yet another plugin is a need for web3js upgrade (to 4.X) which is imposible in current quorum / besu connectors due to dependency to `web3js-quorum` which requires web3js 1.X.

We have plans to make web3js library pluggable and reduce code duplication among other connectors in the future, but it will be delivered later on in a separate PR.

Changes:
- Add new plugin based on quorum connector.
- Removed private transaction and other quorum related functionalities.
- Update web3js to 1.10 - will be updated to 4.X in a separate commit.
- Add missing `web3-eth-contract` dependencies to besu and xdai connectors.
- Add new connector to cactus-verifier-client
- Add integration tests in `cactus-test-plugin-ledger-connector-ethereum` (based on similar ones for quorum connector.)
- Add new connector to CI.
- Add `web3*` 1.5.2 dependencies to root `package.json` because they are already required in a root level (by `typings/web3js-quorum`). Ideally this could be put into another package (quorum connector?) and have the dependencies there, but for now I think it's important to be explicit about it since it's easy to mess up if wrong web3js library is hoisted up from any monorepo package.
- Sort main `package.json`
- Remove tap test scripts from the root `package.json` - they don't use `.taprc` and cause bunch of errors when they try to execute jest tests. This is confusing for the users because of all false negative errors printed.
- Reorganize jest config and taprc to keep tests from quorum and ethereum conenctors grouped.

Closes: #2534
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 15:17:44 +0000 UTC
    </div>
</div>

