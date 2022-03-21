---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1938" class=".btn">#1938</a>
            </td>
            <td>
                <b>
                    feat(plugin-odap): addition of client endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Until now, the protocol was implemented using only the server endpoints.

The changes can be summarized as follows:
- Implementation of client endpoints
- Adapted and added more tests (now divided into unit and integration tests)
- Addition of more checks regarding the validity of the messages received on the server side

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-20 23:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1936" class=".btn">#1936</a>
            </td>
            <td>
                <b>
                    fix: resolve some CodeQL warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix CodeQL warnings:
- Reflected cross-site scripting
- Exception text reinterpreted as HTML

In following files:
- `examples/cactus-check-connection-ethereum-validator/check-ethereum-validator.ts`
- `examples/discounted-cartrade/trades.ts`
- `examples/electricity-trade/electricity-trade.ts`
- `examples/test-run-transaction/test-run-transaction.ts`
- `packages/cactus-cmd-socketio-server/src/main/typescript/routing-interface/routes/index.ts`

Also, sample apps in `example/` did not build after last socketio upgrade, had to upgrade typescript to make them build again.

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 15:35:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1934" class=".btn">#1934</a>
            </td>
            <td>
                <b>
                    docs(plugin-object-store-ipfs): added README.md description
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added some instructions for the usage of the package `plugin-object-store-ipfs` in the README.md.

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 02:29:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1933" class=".btn">#1933</a>
            </td>
            <td>
                <b>
                    feat(quorum-connector): implement validator interface on go-quorum-connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add three new endpoints to quorum ledger connector achieve legacy verifier compatibility.
  - `InvokeRawWeb3EthContractEndpoint` can be used to form any call to deployed contract.
  - `InvokeRawWeb3EthMethodEndpoint` can be used to call any web3.eth function. Both are marked as low-level functions, should be used only when there's no designated endpoint for given functionality yet.
  - `WatchBlocksV1Endpoint` can be used to monitor new block headers / data from the ledger. Type of the output is determined from input option flag.
- Extend `QuorumApiClient` to support Verifier interface, that is: block monitoring, and sending sync/async requests. Sending requests is marked as deprecated, because user can use direct REST calls from generated ApiClient, nevertheless this API was requested by one of the teams.
- Added functional tests for two new, request based endpoints.
- Moved verifier-besu integration test to besu-test package.
- Added verifier-quorum integration test, it supplements direct endpoint tests and provides a reference for API usage.
- Added support for `QuorumApiClient` in Verifier.

Closes: https://github.com/hyperledger/cactus/issues/1604
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

### Notes
- I can't make CodeQL to cooperate, it reports dynamic call errors, even though I explicitly check if methods are defined on a contract / object (also assert they type is a function). Tried different methods to make the scanner notice it but did not succeed. Please double check and mark as false positive if possible.

Depends on https://github.com/hyperledger/cactus/pull/1928
Depends on https://github.com/hyperledger/cactus/pull/1926
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 19:08:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1931" class=".btn">#1931</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">dependencies</span>
            </td>
            <td>
                The current 1.0.0 release is undergoing a being security audited by a
third-party security audit company at the time of this writing. and the
process will take about 6 to 8 weeks to complete, but we are planning
to keep the 1.0.0 API stability in place as dictated by the semantic
versioning rules.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com> 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 09:34:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1930" class=".btn">#1930</a>
            </td>
            <td>
                <b>
                    ci: add fuzzer tests for our APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                Fixes #495

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 06:22:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1929" class=".btn">#1929</a>
            </td>
            <td>
                <b>
                    build(deps): bump underscore from 1.9.1 to 1.13.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [underscore](https://github.com/jashkenas/underscore) from 1.9.1 to 1.13.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jashkenas/underscore/commit/33383fe35cdaf90ff1aa12e20067f44cbe267e87"><code>33383fe</code></a> Update generated sources, tag 1.13.2 release</li>
<li><a href="https://github.com/jashkenas/underscore/commit/cd03f4c08e7f49592d88de83dfc3630762e376dc"><code>cd03f4c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2946">#2946</a> from jgonggrijp/prepare-1.13.2</li>
<li><a href="https://github.com/jashkenas/underscore/commit/5463692bfd2b6024c6aa3f87b33bd724886a993d"><code>5463692</code></a> Add a change log entry for 1.13.2</li>
<li><a href="https://github.com/jashkenas/underscore/commit/315c2df4b82a1c2fb378441d62f906c72f9501ba"><code>315c2df</code></a> Bump the version to 1.13.2</li>
<li><a href="https://github.com/jashkenas/underscore/commit/8cd397b70a1eb9c72daba7f07ed0f94931f039a3"><code>8cd397b</code></a> Use statically.io for the 1.13.x series doc archives</li>
<li><a href="https://github.com/jashkenas/underscore/commit/92db0d9df4c22068a992a62ac543b5216095badb"><code>92db0d9</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2937">#2937</a> from zheng-kai/master</li>
<li><a href="https://github.com/jashkenas/underscore/commit/7c2db70ff0464ae01fa4b486d5ef5f0aa8f6a103"><code>7c2db70</code></a> Clarify that _.bind and _.partial can be used together (<a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2328">#2328</a>)</li>
<li><a href="https://github.com/jashkenas/underscore/commit/d9e00911565df587792b45f1213639b6aba0dcb0"><code>d9e0091</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2944">#2944</a> from jgonggrijp/fix-sample-string</li>
<li><a href="https://github.com/jashkenas/underscore/commit/72173baf348b5d21853aceab632ef92b3c93c911"><code>72173ba</code></a> Properly convert _.sample input collection _.toArray (fix <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2927">#2927</a>)</li>
<li><a href="https://github.com/jashkenas/underscore/commit/354337ac9689bb82c098d11dabb85204cc09e31a"><code>354337a</code></a> Add a regression test for <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2927">#2927</a> (caused in <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2158">#2158</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/jashkenas/underscore/compare/1.9.1...1.13.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jgonggrijp">jgonggrijp</a>, a new releaser for underscore since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=underscore&package-manager=npm_and_yarn&previous-version=1.9.1&new-version=1.13.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 07:00:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1928" class=".btn">#1928</a>
            </td>
            <td>
                <b>
                    refactor(quorum-multi-party-all-in-one): enhance quorum-mp image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span>
            </td>
            <td>
                Current Quorum-MP WS endpoints are not available outside of docker, fix
it. Use upstream npm setup package instead of contributor branch. Test
all members in healthcheck. Update readme. Add test tooling to setup
multi party ledger in functional tests. Cleanup and simplify dockerfile.
Publish MP image to ghcr.

Closes: #1927
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

Notes
- I've added a new image publish in this PR, but there's ongoing issue with package publish - https://github.com/hyperledger/cactus/issues/1881
- Since I'm not sure when the image will be published, I've used my personal ghcr for now, since I'm already using it in some functional tests on another branch. I will change it to hyperledger ghcr when the publish completes correctly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 13:06:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1926" class=".btn">#1926</a>
            </td>
            <td>
                <b>
                    fix(api-server): allow no authorization on socketio endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                authorizeSocket middleware will be installed only if AuthorizationProtocol different than NONE was provided.

Closes:  #1925
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

Note
- This change work on my other local branch (not PR ready yet).
- This can be refactored, so that all authorization middleware creation would be handled by `AuthorizerFactory.createMiddleware`, but I didn't want to touch it without test coverage. I will probably introduce some tests with of socketio authorization as part of other PR, we can think about improvements then.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 12:40:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1923" class=".btn">#1923</a>
            </td>
            <td>
                <b>
                    fix(security): upgrade to yarn > 1.22.0 - CVE-2019-10773, CVE-2020-8131
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                Fixes #1922

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 07:30:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1921" class=".btn">#1921</a>
            </td>
            <td>
                <b>
                    fix(security): ensure ansi-html > 0.0.8 - CVE-2021-23424
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                Fixes #1920

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 07:15:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1919" class=".btn">#1919</a>
            </td>
            <td>
                <b>
                    fix(security): force lodash > 4.17.20 - CVE-2020-8203
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                TODO: Longer term we should take care to upgrade the top level
dependencies instead (as patched releases become available)

Fixes #1918

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 07:08:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1917" class=".btn">#1917</a>
            </td>
            <td>
                <b>
                    fix(deps): ensure glob-parent is above 5.1.2 - CVE-2020-28469
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                1. Upgrade cpy-cli to 4.1.0
2. Force glob-parent to be on 5.1.2

TODO: The proper solution to 2) is to upgrade Angular to 13
so we do need to do that later when more time is available.

Fixes #1916

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 06:46:49 +0000 UTC
    </div>
</div>

