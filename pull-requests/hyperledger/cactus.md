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
                PR <a href="https://github.com/hyperledger/cactus/pull/1005" class=".btn">#1005</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): upgrade Fabric AIO image tag used for test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span>
            </td>
            <td>
                Upgraded from the image build in March 2021 to the one in April which
is believed to be more stable making this change potentially viable as
a soltuion to the flakes that we've been observing during test execution
when the AIO image fails to boot.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 17:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1004" class=".btn">#1004</a>
            </td>
            <td>
                <b>
                    fix(readthedocs): updated readthedocs file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #981 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 08:41:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    fix(validator,verifier): delete some minor duplicated documents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1002 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 10:50:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/999" class=".btn">#999</a>
            </td>
            <td>
                <b>
                    fix(tools): fix a typo of README on iroha-testnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1000 
cc: @tkyonezu 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 10:08:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/998" class=".btn">#998</a>
            </td>
            <td>
                <b>
                    refactor(examples): refactor electricity-trade in order to allow BLP connects ledgers only via Verifier and Validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #970 

contents:
 - modify electricity-trade in order to allow BLP not to direcly call getNonceHex but to call getNonceHex via Verifier and Validator

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 09:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/996" class=".btn">#996</a>
            </td>
            <td>
                <b>
                    build: migrate dev container to Ubuntu 20; add nvm to image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                Primary change:
--------------

The Debian 10 to Ubuntu 20.04 LTS move

This came up when I tried to install the DFINITY SDK which failed due to
some GLIB C version mismatch which was not possible to get resolved
on Debian Buster (v10) without upgrading to the not-yet-stable version
11 (Bullseye).

While going through the above, I also realized that our CI uses
Ubuntu 20.04 so it would be great to have consistency across the board
when it comes OS versions. This will become even more important when
we start adding microk8s in the mix as well (hopefully soon).

Secondary change:
-----------------

build: include node version manager (nvm) to .devcontainer

The need for this dawned on me when I pulled up a fresh dev
container, tried to run the configure script that failed because
the current latest NodeJS (v16) was installed by apk and the
build could not handle that
We have a pending PR for this separately at the time of this
writing, but to make it easier to work around issues like this
in the future, nvm should be in the image should that people
can just do nvm use 14 for example. (which is what the fix
was in my case).

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 21:27:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/994" class=".btn">#994</a>
            </td>
            <td>
                <b>
                    test: container shutdown hook prior to starting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                ## Dependencies

Depends on #993 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Date: Fri May 28 2021 00:04:09 GMT-0700 (Pacific Daylight Time) 

test: container shutdown hook prior to starting

Figured out from the additional logs we recently added that
the reason why the Fabric 1.4.x AIO image fails to start for
the 1.4.x tests is because a previously ran test (2.x)
crashes and never stops it's container which then ends up
hogging the ports which cannot be randomized for the
Fabric AIO images yet.

So, adding more logging here and also ensuring that the
test finish hooks that are responsible for shutting down
the containers are registered prior to calling
the start method on the test container classes so that
if the start method hangs the container will still go
away as it should.

This is what gave me the clue from the CI logs:

    # BEFORE runs tx on a Fabric v2.2.0 ledger
    Detected current process to be running inside a Github Action. Pruning all docker resources...
    [2021-05-28T01:23:31.310Z] DEBUG (Containers#pruneDockerResources()): Finished pruning all docker resources. Outcome: {
      containers: { ContainersDeleted: null, SpaceReclaimed: 0 },
      images: { ImagesDeleted: null, SpaceReclaimed: 0 },
      networks: { NetworksDeleted: null },
      volumes: {
        VolumesDeleted: [
          '10afa6c6071a4e362324ec7eaabedbbee088dedc0b0e182880ca4ccc6430b998',
          [length]: 1
        ],
        SpaceReclaimed: 1915254089
      }
    }
    ok 1 Pruning didn't throw OK
    # runs tx on a Fabric v2.2.0 ledger
    # test count(1) != plan(null)
    # failed 1 test
not ok 62 - packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/integration/fabric-v2-2-x/run-transaction-endpoint-v1.test.ts # time=3600276.779ms

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 07:13:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/993" class=".btn">#993</a>
            </td>
            <td>
                <b>
                    ci: delete Android SDK, .NET in GitHub Action runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                This is a workaround for the warnings that we've been getting
about the disk of the GHA runners being full. 

The trick is to delete the Android SDK and .NET from the runner
because we don't need any of those and it gives us a cozy 30 GB
extra space to play with which should be more than enough for
the foreseeable future.

The idea comes from:
https://github.com/actions/virtual-environments/issues/2606#issuecomment-772683150

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 21:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/991" class=".btn">#991</a>
            </td>
            <td>
                <b>
                    feat(azure-kv): added keychain plugin for azure keyvault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
------------------------------
feat(azure-kv): added keychain plugin for azure keyvault

        Primary Change
        ---
        1. Added new package cactus-plugin-keychain-azure-kv under packages/
        2. Added PluginKeychainAzureKvMock class to mock the functions of SecretClient under packages/cactus-plugin-keychain-azure-kv/src/test/typescript/mock/plugin-keychain-azure-kv-mock.ts

Resolves #971

Signed-off-by: Jagpreet Singh Sasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 09:49:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/990" class=".btn">#990</a>
            </td>
            <td>
                <b>
                    chore(deps): bump browserslist from 4.16.3 to 4.16.6 in /packages/cactus-cockpit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [browserslist](https://github.com/browserslist/browserslist) from 4.16.3 to 4.16.6.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/browserslist/browserslist/blob/main/CHANGELOG.md">browserslist's changelog</a>.</em></p>
<blockquote>
<h2>4.16.6</h2>
<ul>
<li>Fixed <code>npm-shrinkwrap.json</code> support in <code>--update-db</code> (by Geoff Newman).</li>
</ul>
<h2>4.16.5</h2>
<ul>
<li>Fixed unsafe RegExp (by Yeting Li).</li>
</ul>
<h2>4.16.4</h2>
<ul>
<li>Fixed unsafe RegExp.</li>
<li>Added artifactory support to <code>--update-db</code> (by Ittai Baratz).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/browserslist/browserslist/commit/6fe3614db05b40f9dc1c63588a83d2ada05bae75"><code>6fe3614</code></a> Release 4.16.6 version</li>
<li><a href="https://github.com/browserslist/browserslist/commit/33ebac933839847a62ede680273449f6cdca1e18"><code>33ebac9</code></a> Update dependencies</li>
<li><a href="https://github.com/browserslist/browserslist/commit/2128170f231a6c9f462276006e09f302d811df31"><code>2128170</code></a> Add support for npm-shrinkwrap files alongside package-lock (<a href="https://github-redirect.dependabot.com/browserslist/browserslist/issues/595">#595</a>)</li>
<li><a href="https://github.com/browserslist/browserslist/commit/7cc2aedd0047d800d44aa0259c02b6db1414105c"><code>7cc2aed</code></a> Release 4.16.5 version</li>
<li><a href="https://github.com/browserslist/browserslist/commit/27e4afdc68798ca93f8c01c5ea6208b4b361a704"><code>27e4afd</code></a> Update dependencies</li>
<li><a href="https://github.com/browserslist/browserslist/commit/1013a1847931a209c34a704aebc85a8c091286e7"><code>1013a18</code></a> Fix version RegExp</li>
<li><a href="https://github.com/browserslist/browserslist/commit/b879a1a304def2563f42cc3d3f5711e760662be3"><code>b879a1a</code></a> Use Node.js 16 on CI</li>
<li><a href="https://github.com/browserslist/browserslist/commit/bd1e9e01c95cad24be706fb11be7d151cd99ed0a"><code>bd1e9e0</code></a> Fix ReDoS (<a href="https://github-redirect.dependabot.com/browserslist/browserslist/issues/593">#593</a>)</li>
<li><a href="https://github.com/browserslist/browserslist/commit/209adf9e0051fa39a2b25354cffd493300f34b02"><code>209adf9</code></a> Release 4.16.4 version</li>
<li><a href="https://github.com/browserslist/browserslist/commit/3e2ae3b52daf7f5203247fd4f583b3bda66ea57d"><code>3e2ae3b</code></a> Fix types</li>
<li>Additional commits viewable in <a href="https://github.com/browserslist/browserslist/compare/4.16.3...4.16.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=browserslist&package-manager=npm_and_yarn&previous-version=4.16.3&new-version=4.16.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-26 20:13:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/989" class=".btn">#989</a>
            </td>
            <td>
                <b>
                    Cleanup electricity-trade example docker containers and fix readme. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span><span class="chip">documentation</span><span class="chip">enhancement</span>
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 18:01:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/988" class=".btn">#988</a>
            </td>
            <td>
                <b>
                    test(cmd-api-server): refactor mTLS test to use tape-promise
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 14:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/987" class=".btn">#987</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): drop URI type alt name from self signed TLS cert
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">Security</span><span class="chip">bug</span>
            </td>
            <td>
                The test verifying mTLS support was failing on NodeJS v16
with the error below which was traced back to the fact that
the URL constructor fails with "localhost" as an input at the
verify server identity phase.
This seems like a bug in NodeJS, but maybe it works as intended.

TypeError [ERR_INVALID_URL]: Invalid URL: localhost
    at new NodeError (node:internal/errors:363:5)
    at onParseError (node:internal/url:537:9)
    at new URL (node:internal/url:613:5)
    at node:tls:247:21
    at Array.forEach (<anonymous>)
    at Object.checkServerIdentity (node:tls:243:5)
    at TLSSocket.onConnectSecure (node:_tls_wrap:1551:27)
    at TLSSocket.emit (node:events:365:28)
    at TLSSocket._finishInit (node:_tls_wrap:952:8)
    at TLSWrap.ssl.onhandshakedone (node:_tls_wrap:723:12)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 14:24:34 +0000 UTC
    </div>
</div>

