---
layout: default
title: karma-charity-platform
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/karma-charity-platform
---

# karma-charity-platform <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/karma-charity-platform){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Bump @nestjs/core and @ts-core/backend-nestjs in /chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@nestjs/core](https://github.com/nestjs/nest) to 9.4.0 and updates ancestor dependency [@ts-core/backend-nestjs](https://github.com/ManhattanDoctor/ts-core-backend-nestjs). These dependencies need to be updated together.

Updates `@nestjs/core` from 8.4.7 to 9.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/nest/releases"><code>@​nestjs/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v9.4.0 (2023-04-05)</h2>
<h4>Features</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/10628">#10628</a> feat(microservice): TCP microservice over TLS (<a href="https://github.com/nomaxg"><code>@​nomaxg</code></a>)</li>
</ul>
</li>
</ul>
<h4>Bug fixes</h4>
<ul>
<li><code>platform-ws</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11188">#11188</a> fix(ws): mount multi <code>ws</code> servers on different paths (<a href="https://github.com/CodyTseng"><code>@​CodyTseng</code></a>)</li>
</ul>
</li>
<li><code>platform-express</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11325">#11325</a> fix(express): remove body-parser types and ship these types our own (<a href="https://github.com/tolgap"><code>@​tolgap</code></a>)</li>
</ul>
</li>
</ul>
<h4>Enhancements</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11426">#11426</a> feat: allow extension of microservice event and message extras (<a href="https://github.com/effervescentia"><code>@​effervescentia</code></a>)</li>
</ul>
</li>
</ul>
<h4>Dependencies</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11394">#11394</a> chore(deps-dev): bump sinon from 15.0.2 to 15.0.3 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11406">#11406</a> chore(deps-dev): bump <code>@​types/node</code> from 18.15.6 to 18.15.11 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11418">#11418</a> chore(deps-dev): bump <code>@​fastify/static</code> from 6.9.0 to 6.10.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11419">#11419</a> chore(deps): bump fast-json-stringify from 5.6.2 to 5.7.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11422">#11422</a> chore(deps-dev): bump <code>@​apollo/server</code> from 4.5.0 to 4.6.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11423">#11423</a> chore(deps-dev): bump amqp-connection-manager from 4.1.11 to 4.1.12 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11424">#11424</a> chore(deps-dev): bump core-js from 3.29.1 to 3.30.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11405">#11405</a> chore(deps-dev): bump ts-morph from 17.0.1 to 18.0.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11403">#11403</a> fix(deps): update dependency <code>@​nestjs/apollo</code> to v11.0.4 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11402">#11402</a> chore(deps): update dependency <code>@​types/cache-manager</code> to v4.0.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11401">#11401</a> chore(deps): update dependency <code>@​babel/core</code> to v7.21.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11407">#11407</a> chore(deps-dev): bump concurrently from 7.6.0 to 8.0.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11408">#11408</a> chore(deps-dev): bump <code>@​commitlint/cli</code> from 17.5.0 to 17.5.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11347">#11347</a> fix(deps): update dependency sequelize-typescript to v2.1.5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11344">#11344</a> fix(deps): update dependency <code>@​nestjs/typeorm</code> to v9.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11343">#11343</a> fix(deps): update dependency <code>@​nestjs/serve-static</code> to v3.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11342">#11342</a> fix(deps): update dependency <code>@​nestjs/mongoose</code> to v9.2.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11340">#11340</a> fix(deps): update dependency <code>@​nestjs/bull</code> to v0.6.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11351">#11351</a> chore(deps): update dependency <code>@​types/amqplib</code> to v0.10.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11323">#11323</a> chore(deps-dev): bump <code>@​grpc/proto-loader</code> from 0.7.5 to 0.7.6 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11395">#11395</a> chore(deps-dev): bump prettier from 2.8.6 to 2.8.7 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11336">#11336</a> chore(deps): update dependency nodemon to v2.0.22 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11339">#11339</a> chore(deps): update mysql docker tag to v8.0.32 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11348">#11348</a> fix(deps): update dependency typeorm to v0.3.12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11349">#11349</a> chore(deps): update confluentinc/cp-kafka docker tag to v7.3.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11366">#11366</a> fix(deps): update dependency <code>@​fastify/view</code> to v7.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11376">#11376</a> fix(deps): update dependency socket.io to v4.6.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11381">#11381</a> chore(deps): update mongo docker tag to v6 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11384">#11384</a> fix(deps): update dependency mercurius to v12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11385">#11385</a> fix(deps): update dependency mongodb to v5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11387">#11387</a> fix(deps): update dependency mysql2 to v3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11389">#11389</a> fix(deps): update dependency rimraf to v4.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/nest/commit/676c98ca91212a8fd81ab37f7d7f8d12ad3dd005"><code>676c98c</code></a> chore(<a href="https://github.com/nestjs"><code>@​nestjs</code></a>) publish v9.4.0 release</li>
<li><a href="https://github.com/nestjs/nest/commit/11f512c7db19fe02dcde4c42fbdadd98a408ea89"><code>11f512c</code></a> sample: update 20-cache sample</li>
<li><a href="https://github.com/nestjs/nest/commit/4be791ffca7b99593fc81bbedb24346cb463a5d0"><code>4be791f</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11426">#11426</a> from voiceflow/feat/extend-microservice-extras</li>
<li><a href="https://github.com/nestjs/nest/commit/e990336deb411319b90f74fcd53591601fd7aaa6"><code>e990336</code></a> Merge branch 'master' of <a href="https://github.com/nestjs/nest">https://github.com/nestjs/nest</a></li>
<li><a href="https://github.com/nestjs/nest/commit/06da94bca513cd3d93859fbc175840514b09c995"><code>06da94b</code></a> chore: assert type of route info objects</li>
<li><a href="https://github.com/nestjs/nest/commit/402a389e54908351cc5702b609ff0e031d529169"><code>402a389</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/10228">#10228</a> from nathanArseneau/test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/c885a89dec2ad2b867331b6c2ff511b2b9e50cf7"><code>c885a89</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11188">#11188</a> from CodyTseng/fix-ws-multi-servers-on-different-paths</li>
<li><a href="https://github.com/nestjs/nest/commit/718e70476b763ba01cf22c14d3801a444cc9383b"><code>718e704</code></a> chore: upgrade typescript</li>
<li><a href="https://github.com/nestjs/nest/commit/9b6b00f0debcedaec1b2ca2d6be56f2cb0216e57"><code>9b6b00f</code></a> Merge branch 'master' into test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/e46147ebcbbea565a4e59e480ec0e413d2a0f29f"><code>e46147e</code></a> Merge branch 'master' into fix-ws-multi-servers-on-different-paths</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/nest/compare/v8.4.7...v9.4.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@ts-core/backend-nestjs` from 8.1.8 to 9.0.2
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/ManhattanDoctor/ts-core-backend-nestjs/commits">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 17:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Bump @nestjs/core, @nestjs/platform-express, @nestjs/swagger and @ts-core/backend-nestjs in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@nestjs/core](https://github.com/nestjs/nest) to 9.4.0 and updates ancestor dependencies [@nestjs/core](https://github.com/nestjs/nest), [@nestjs/platform-express](https://github.com/nestjs/nest), [@nestjs/swagger](https://github.com/nestjs/swagger) and [@ts-core/backend-nestjs](https://github.com/ManhattanDoctor/ts-core-backend-nestjs). These dependencies need to be updated together.

Updates `@nestjs/core` from 8.4.7 to 9.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/nest/releases"><code>@​nestjs/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v9.4.0 (2023-04-05)</h2>
<h4>Features</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/10628">#10628</a> feat(microservice): TCP microservice over TLS (<a href="https://github.com/nomaxg"><code>@​nomaxg</code></a>)</li>
</ul>
</li>
</ul>
<h4>Bug fixes</h4>
<ul>
<li><code>platform-ws</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11188">#11188</a> fix(ws): mount multi <code>ws</code> servers on different paths (<a href="https://github.com/CodyTseng"><code>@​CodyTseng</code></a>)</li>
</ul>
</li>
<li><code>platform-express</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11325">#11325</a> fix(express): remove body-parser types and ship these types our own (<a href="https://github.com/tolgap"><code>@​tolgap</code></a>)</li>
</ul>
</li>
</ul>
<h4>Enhancements</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11426">#11426</a> feat: allow extension of microservice event and message extras (<a href="https://github.com/effervescentia"><code>@​effervescentia</code></a>)</li>
</ul>
</li>
</ul>
<h4>Dependencies</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11394">#11394</a> chore(deps-dev): bump sinon from 15.0.2 to 15.0.3 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11406">#11406</a> chore(deps-dev): bump <code>@​types/node</code> from 18.15.6 to 18.15.11 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11418">#11418</a> chore(deps-dev): bump <code>@​fastify/static</code> from 6.9.0 to 6.10.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11419">#11419</a> chore(deps): bump fast-json-stringify from 5.6.2 to 5.7.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11422">#11422</a> chore(deps-dev): bump <code>@​apollo/server</code> from 4.5.0 to 4.6.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11423">#11423</a> chore(deps-dev): bump amqp-connection-manager from 4.1.11 to 4.1.12 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11424">#11424</a> chore(deps-dev): bump core-js from 3.29.1 to 3.30.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11405">#11405</a> chore(deps-dev): bump ts-morph from 17.0.1 to 18.0.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11403">#11403</a> fix(deps): update dependency <code>@​nestjs/apollo</code> to v11.0.4 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11402">#11402</a> chore(deps): update dependency <code>@​types/cache-manager</code> to v4.0.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11401">#11401</a> chore(deps): update dependency <code>@​babel/core</code> to v7.21.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11407">#11407</a> chore(deps-dev): bump concurrently from 7.6.0 to 8.0.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11408">#11408</a> chore(deps-dev): bump <code>@​commitlint/cli</code> from 17.5.0 to 17.5.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11347">#11347</a> fix(deps): update dependency sequelize-typescript to v2.1.5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11344">#11344</a> fix(deps): update dependency <code>@​nestjs/typeorm</code> to v9.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11343">#11343</a> fix(deps): update dependency <code>@​nestjs/serve-static</code> to v3.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11342">#11342</a> fix(deps): update dependency <code>@​nestjs/mongoose</code> to v9.2.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11340">#11340</a> fix(deps): update dependency <code>@​nestjs/bull</code> to v0.6.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11351">#11351</a> chore(deps): update dependency <code>@​types/amqplib</code> to v0.10.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11323">#11323</a> chore(deps-dev): bump <code>@​grpc/proto-loader</code> from 0.7.5 to 0.7.6 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11395">#11395</a> chore(deps-dev): bump prettier from 2.8.6 to 2.8.7 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11336">#11336</a> chore(deps): update dependency nodemon to v2.0.22 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11339">#11339</a> chore(deps): update mysql docker tag to v8.0.32 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11348">#11348</a> fix(deps): update dependency typeorm to v0.3.12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11349">#11349</a> chore(deps): update confluentinc/cp-kafka docker tag to v7.3.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11366">#11366</a> fix(deps): update dependency <code>@​fastify/view</code> to v7.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11376">#11376</a> fix(deps): update dependency socket.io to v4.6.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11381">#11381</a> chore(deps): update mongo docker tag to v6 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11384">#11384</a> fix(deps): update dependency mercurius to v12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11385">#11385</a> fix(deps): update dependency mongodb to v5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11387">#11387</a> fix(deps): update dependency mysql2 to v3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11389">#11389</a> fix(deps): update dependency rimraf to v4.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/nest/commit/676c98ca91212a8fd81ab37f7d7f8d12ad3dd005"><code>676c98c</code></a> chore(<a href="https://github.com/nestjs"><code>@​nestjs</code></a>) publish v9.4.0 release</li>
<li><a href="https://github.com/nestjs/nest/commit/11f512c7db19fe02dcde4c42fbdadd98a408ea89"><code>11f512c</code></a> sample: update 20-cache sample</li>
<li><a href="https://github.com/nestjs/nest/commit/4be791ffca7b99593fc81bbedb24346cb463a5d0"><code>4be791f</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11426">#11426</a> from voiceflow/feat/extend-microservice-extras</li>
<li><a href="https://github.com/nestjs/nest/commit/e990336deb411319b90f74fcd53591601fd7aaa6"><code>e990336</code></a> Merge branch 'master' of <a href="https://github.com/nestjs/nest">https://github.com/nestjs/nest</a></li>
<li><a href="https://github.com/nestjs/nest/commit/06da94bca513cd3d93859fbc175840514b09c995"><code>06da94b</code></a> chore: assert type of route info objects</li>
<li><a href="https://github.com/nestjs/nest/commit/402a389e54908351cc5702b609ff0e031d529169"><code>402a389</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/10228">#10228</a> from nathanArseneau/test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/c885a89dec2ad2b867331b6c2ff511b2b9e50cf7"><code>c885a89</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11188">#11188</a> from CodyTseng/fix-ws-multi-servers-on-different-paths</li>
<li><a href="https://github.com/nestjs/nest/commit/718e70476b763ba01cf22c14d3801a444cc9383b"><code>718e704</code></a> chore: upgrade typescript</li>
<li><a href="https://github.com/nestjs/nest/commit/9b6b00f0debcedaec1b2ca2d6be56f2cb0216e57"><code>9b6b00f</code></a> Merge branch 'master' into test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/e46147ebcbbea565a4e59e480ec0e413d2a0f29f"><code>e46147e</code></a> Merge branch 'master' into fix-ws-multi-servers-on-different-paths</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/nest/compare/v8.4.7...v9.4.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@nestjs/platform-express` from 8.4.7 to 9.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/nest/releases"><code>@​nestjs/platform-express</code>'s releases</a>.</em></p>
<blockquote>
<h2>v9.4.0 (2023-04-05)</h2>
<h4>Features</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/10628">#10628</a> feat(microservice): TCP microservice over TLS (<a href="https://github.com/nomaxg"><code>@​nomaxg</code></a>)</li>
</ul>
</li>
</ul>
<h4>Bug fixes</h4>
<ul>
<li><code>platform-ws</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11188">#11188</a> fix(ws): mount multi <code>ws</code> servers on different paths (<a href="https://github.com/CodyTseng"><code>@​CodyTseng</code></a>)</li>
</ul>
</li>
<li><code>platform-express</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11325">#11325</a> fix(express): remove body-parser types and ship these types our own (<a href="https://github.com/tolgap"><code>@​tolgap</code></a>)</li>
</ul>
</li>
</ul>
<h4>Enhancements</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11426">#11426</a> feat: allow extension of microservice event and message extras (<a href="https://github.com/effervescentia"><code>@​effervescentia</code></a>)</li>
</ul>
</li>
</ul>
<h4>Dependencies</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11394">#11394</a> chore(deps-dev): bump sinon from 15.0.2 to 15.0.3 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11406">#11406</a> chore(deps-dev): bump <code>@​types/node</code> from 18.15.6 to 18.15.11 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11418">#11418</a> chore(deps-dev): bump <code>@​fastify/static</code> from 6.9.0 to 6.10.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11419">#11419</a> chore(deps): bump fast-json-stringify from 5.6.2 to 5.7.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11422">#11422</a> chore(deps-dev): bump <code>@​apollo/server</code> from 4.5.0 to 4.6.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11423">#11423</a> chore(deps-dev): bump amqp-connection-manager from 4.1.11 to 4.1.12 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11424">#11424</a> chore(deps-dev): bump core-js from 3.29.1 to 3.30.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11405">#11405</a> chore(deps-dev): bump ts-morph from 17.0.1 to 18.0.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11403">#11403</a> fix(deps): update dependency <code>@​nestjs/apollo</code> to v11.0.4 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11402">#11402</a> chore(deps): update dependency <code>@​types/cache-manager</code> to v4.0.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11401">#11401</a> chore(deps): update dependency <code>@​babel/core</code> to v7.21.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11407">#11407</a> chore(deps-dev): bump concurrently from 7.6.0 to 8.0.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11408">#11408</a> chore(deps-dev): bump <code>@​commitlint/cli</code> from 17.5.0 to 17.5.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11347">#11347</a> fix(deps): update dependency sequelize-typescript to v2.1.5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11344">#11344</a> fix(deps): update dependency <code>@​nestjs/typeorm</code> to v9.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11343">#11343</a> fix(deps): update dependency <code>@​nestjs/serve-static</code> to v3.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11342">#11342</a> fix(deps): update dependency <code>@​nestjs/mongoose</code> to v9.2.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11340">#11340</a> fix(deps): update dependency <code>@​nestjs/bull</code> to v0.6.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11351">#11351</a> chore(deps): update dependency <code>@​types/amqplib</code> to v0.10.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11323">#11323</a> chore(deps-dev): bump <code>@​grpc/proto-loader</code> from 0.7.5 to 0.7.6 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11395">#11395</a> chore(deps-dev): bump prettier from 2.8.6 to 2.8.7 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11336">#11336</a> chore(deps): update dependency nodemon to v2.0.22 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11339">#11339</a> chore(deps): update mysql docker tag to v8.0.32 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11348">#11348</a> fix(deps): update dependency typeorm to v0.3.12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11349">#11349</a> chore(deps): update confluentinc/cp-kafka docker tag to v7.3.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11366">#11366</a> fix(deps): update dependency <code>@​fastify/view</code> to v7.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11376">#11376</a> fix(deps): update dependency socket.io to v4.6.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11381">#11381</a> chore(deps): update mongo docker tag to v6 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11384">#11384</a> fix(deps): update dependency mercurius to v12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11385">#11385</a> fix(deps): update dependency mongodb to v5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11387">#11387</a> fix(deps): update dependency mysql2 to v3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11389">#11389</a> fix(deps): update dependency rimraf to v4.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/nest/commit/676c98ca91212a8fd81ab37f7d7f8d12ad3dd005"><code>676c98c</code></a> chore(<a href="https://github.com/nestjs"><code>@​nestjs</code></a>) publish v9.4.0 release</li>
<li><a href="https://github.com/nestjs/nest/commit/11f512c7db19fe02dcde4c42fbdadd98a408ea89"><code>11f512c</code></a> sample: update 20-cache sample</li>
<li><a href="https://github.com/nestjs/nest/commit/4be791ffca7b99593fc81bbedb24346cb463a5d0"><code>4be791f</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11426">#11426</a> from voiceflow/feat/extend-microservice-extras</li>
<li><a href="https://github.com/nestjs/nest/commit/e990336deb411319b90f74fcd53591601fd7aaa6"><code>e990336</code></a> Merge branch 'master' of <a href="https://github.com/nestjs/nest">https://github.com/nestjs/nest</a></li>
<li><a href="https://github.com/nestjs/nest/commit/06da94bca513cd3d93859fbc175840514b09c995"><code>06da94b</code></a> chore: assert type of route info objects</li>
<li><a href="https://github.com/nestjs/nest/commit/402a389e54908351cc5702b609ff0e031d529169"><code>402a389</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/10228">#10228</a> from nathanArseneau/test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/c885a89dec2ad2b867331b6c2ff511b2b9e50cf7"><code>c885a89</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11188">#11188</a> from CodyTseng/fix-ws-multi-servers-on-different-paths</li>
<li><a href="https://github.com/nestjs/nest/commit/718e70476b763ba01cf22c14d3801a444cc9383b"><code>718e704</code></a> chore: upgrade typescript</li>
<li><a href="https://github.com/nestjs/nest/commit/9b6b00f0debcedaec1b2ca2d6be56f2cb0216e57"><code>9b6b00f</code></a> Merge branch 'master' into test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/e46147ebcbbea565a4e59e480ec0e413d2a0f29f"><code>e46147e</code></a> Merge branch 'master' into fix-ws-multi-servers-on-different-paths</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/nest/compare/v8.4.7...v9.4.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@nestjs/swagger` from 5.2.1 to 6.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/swagger/releases"><code>@​nestjs/swagger</code>'s releases</a>.</em></p>
<blockquote>
<h2>Release 6.3.0</h2>
<ul>
<li>test: check ts version and compare diff output if v5 (508a206)</li>
<li>fix(plugin): hotfix ts version condition (4858616)</li>
<li>fix(plugin): hotfix ts version condition (9e82747)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2296">#2296</a> from bojovypstros/refactor-intersection (ae495fc)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2303">#2303</a> from Dracks/master (6f02ee2)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2308">#2308</a> from nestjs/renovate/swagger-ui-dist-4.x (5b02c68)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2145">#2145</a> from timoklingenhoefer/master (46c5fae)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2283">#2283</a> from nestjs/renovate/cimg-node-19.x (804d2b5)</li>
<li>chore(deps): upgrade typescript (35043f9)</li>
<li>fix(deps): update dependency swagger-ui-dist to v4.18.2 (8dc7920)</li>
<li>chore(deps): update dependency eslint to v8.37.0 (132fbac)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.11 (9ac9348)</li>
<li>chore(deps): update dependency <code>@​commitlint/cli</code> to v17.5.1 (f2c9e4f)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.57.0 (8e1d529)</li>
<li>chore(deps): update dependency <code>@​types/lodash</code> to v4.14.192 (0cd083a)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.10 (56b4054)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.9 (c8d5174)</li>
<li>chore(deps): update dependency release-it to v15.9.3 (6653b68)</li>
<li>chore(deps): update dependency prettier to v2.8.7 (5c6e615)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.7 (8d0c28c)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.6 (07db689)</li>
<li>chore(deps): update dependency <code>@​commitlint/cli</code> to v17.5.0 (f797487)</li>
<li>chore(deps): update nest monorepo to v9.3.12 (82f49cb)</li>
<li>chore(deps): update nest monorepo to v9.3.11 (47fe4b5)</li>
<li>chore(deps): update dependency release-it to v15.9.1 (8b3cdd8)</li>
<li>chore(deps): update dependency prettier to v2.8.6 (2c6c3a0)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.5 (f9aea9f)</li>
<li>chore(deps): update dependency eslint-config-prettier to v8.8.0 (52cc234)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.56.0 (83699ee)</li>
<li>chore(deps): update node.js to v19.8 (6f15fa8)</li>
<li>chore(deps): update dependency prettier to v2.8.5 (72cc7aa)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.5.0 (d399b18)</li>
<li>chore(deps): update dependency release-it to v15.9.0 (6f82f87)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.4.4 (423ee60)</li>
<li>chore(deps): update nest monorepo to v9.3.10 (e37f568)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.4.2 (44277ac)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.3 (1a71715)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.55.0 (906f720)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.2 (e0c8d19)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.4.1 (259f783)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.1 (19a8750)</li>
<li>chore(deps): update dependency eslint to v8.36.0 (b9fcf4a)</li>
<li>chore(deps): update dependency lint-staged to v13.2.0 (e4b5312)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.0 (6eb3e4c)</li>
<li>chore(deps): update dependency release-it to v15.8.0 (329b54c)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.54.1 (fa542f7)</li>
<li>chore(deps): update dependency jest to v29.5.0 (bf25252)</li>
<li>chore(deps): update dependency eslint-config-prettier to v8.7.0 (3c952d3)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.14.6 (3a6ce81)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/swagger/commit/2a80ffcf824a826d34947d30a6fdf67165a958d7"><code>2a80ffc</code></a> chore(): release v6.3.0</li>
<li><a href="https://github.com/nestjs/swagger/commit/508a206ca8b3e133660c9bef6e489439552ce548"><code>508a206</code></a> test: check ts version and compare diff output if v5</li>
<li><a href="https://github.com/nestjs/swagger/commit/4858616f7721c83f1246eda1e83fe42855a728c6"><code>4858616</code></a> fix(plugin): hotfix ts version condition</li>
<li><a href="https://github.com/nestjs/swagger/commit/9e82747370d5449943f7046e0f417a706c9c6c69"><code>9e82747</code></a> fix(plugin): hotfix ts version condition</li>
<li><a href="https://github.com/nestjs/swagger/commit/ae495fc6e48f5d7b79ef4cce493fbb5372c1514b"><code>ae495fc</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2296">#2296</a> from bojovypstros/refactor-intersection</li>
<li><a href="https://github.com/nestjs/swagger/commit/6f02ee28a8d2b530f6ae92229aa865627eef5886"><code>6f02ee2</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2303">#2303</a> from Dracks/master</li>
<li><a href="https://github.com/nestjs/swagger/commit/5b02c686def7f445285132970d1150ba98e0f13e"><code>5b02c68</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2308">#2308</a> from nestjs/renovate/swagger-ui-dist-4.x</li>
<li><a href="https://github.com/nestjs/swagger/commit/46c5fae21a8fd0881ea894a7c97b89649a5dd7fc"><code>46c5fae</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2145">#2145</a> from timoklingenhoefer/master</li>
<li><a href="https://github.com/nestjs/swagger/commit/804d2b5f7bde947cf872da8b49d8c6cf40420f78"><code>804d2b5</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2283">#2283</a> from nestjs/renovate/cimg-node-19.x</li>
<li><a href="https://github.com/nestjs/swagger/commit/35043f9d7fee38a8a35b3cbca1ec234a95c5a20c"><code>35043f9</code></a> chore(deps): upgrade typescript</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/swagger/compare/5.2.1...6.3.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@ts-core/backend-nestjs` from 8.1.8 to 9.0.2
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/ManhattanDoctor/ts-core-backend-nestjs/commits">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 17:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Bump @nestjs/core, @nestjs/platform-express, @nestjs/swagger and @ts-core/backend-nestjs in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@nestjs/core](https://github.com/nestjs/nest) to 9.4.0 and updates ancestor dependencies [@nestjs/core](https://github.com/nestjs/nest), [@nestjs/platform-express](https://github.com/nestjs/nest), [@nestjs/swagger](https://github.com/nestjs/swagger) and [@ts-core/backend-nestjs](https://github.com/ManhattanDoctor/ts-core-backend-nestjs). These dependencies need to be updated together.

Updates `@nestjs/core` from 8.4.7 to 9.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/nest/releases"><code>@​nestjs/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v9.4.0 (2023-04-05)</h2>
<h4>Features</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/10628">#10628</a> feat(microservice): TCP microservice over TLS (<a href="https://github.com/nomaxg"><code>@​nomaxg</code></a>)</li>
</ul>
</li>
</ul>
<h4>Bug fixes</h4>
<ul>
<li><code>platform-ws</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11188">#11188</a> fix(ws): mount multi <code>ws</code> servers on different paths (<a href="https://github.com/CodyTseng"><code>@​CodyTseng</code></a>)</li>
</ul>
</li>
<li><code>platform-express</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11325">#11325</a> fix(express): remove body-parser types and ship these types our own (<a href="https://github.com/tolgap"><code>@​tolgap</code></a>)</li>
</ul>
</li>
</ul>
<h4>Enhancements</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11426">#11426</a> feat: allow extension of microservice event and message extras (<a href="https://github.com/effervescentia"><code>@​effervescentia</code></a>)</li>
</ul>
</li>
</ul>
<h4>Dependencies</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11394">#11394</a> chore(deps-dev): bump sinon from 15.0.2 to 15.0.3 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11406">#11406</a> chore(deps-dev): bump <code>@​types/node</code> from 18.15.6 to 18.15.11 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11418">#11418</a> chore(deps-dev): bump <code>@​fastify/static</code> from 6.9.0 to 6.10.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11419">#11419</a> chore(deps): bump fast-json-stringify from 5.6.2 to 5.7.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11422">#11422</a> chore(deps-dev): bump <code>@​apollo/server</code> from 4.5.0 to 4.6.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11423">#11423</a> chore(deps-dev): bump amqp-connection-manager from 4.1.11 to 4.1.12 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11424">#11424</a> chore(deps-dev): bump core-js from 3.29.1 to 3.30.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11405">#11405</a> chore(deps-dev): bump ts-morph from 17.0.1 to 18.0.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11403">#11403</a> fix(deps): update dependency <code>@​nestjs/apollo</code> to v11.0.4 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11402">#11402</a> chore(deps): update dependency <code>@​types/cache-manager</code> to v4.0.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11401">#11401</a> chore(deps): update dependency <code>@​babel/core</code> to v7.21.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11407">#11407</a> chore(deps-dev): bump concurrently from 7.6.0 to 8.0.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11408">#11408</a> chore(deps-dev): bump <code>@​commitlint/cli</code> from 17.5.0 to 17.5.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11347">#11347</a> fix(deps): update dependency sequelize-typescript to v2.1.5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11344">#11344</a> fix(deps): update dependency <code>@​nestjs/typeorm</code> to v9.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11343">#11343</a> fix(deps): update dependency <code>@​nestjs/serve-static</code> to v3.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11342">#11342</a> fix(deps): update dependency <code>@​nestjs/mongoose</code> to v9.2.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11340">#11340</a> fix(deps): update dependency <code>@​nestjs/bull</code> to v0.6.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11351">#11351</a> chore(deps): update dependency <code>@​types/amqplib</code> to v0.10.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11323">#11323</a> chore(deps-dev): bump <code>@​grpc/proto-loader</code> from 0.7.5 to 0.7.6 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11395">#11395</a> chore(deps-dev): bump prettier from 2.8.6 to 2.8.7 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11336">#11336</a> chore(deps): update dependency nodemon to v2.0.22 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11339">#11339</a> chore(deps): update mysql docker tag to v8.0.32 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11348">#11348</a> fix(deps): update dependency typeorm to v0.3.12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11349">#11349</a> chore(deps): update confluentinc/cp-kafka docker tag to v7.3.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11366">#11366</a> fix(deps): update dependency <code>@​fastify/view</code> to v7.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11376">#11376</a> fix(deps): update dependency socket.io to v4.6.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11381">#11381</a> chore(deps): update mongo docker tag to v6 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11384">#11384</a> fix(deps): update dependency mercurius to v12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11385">#11385</a> fix(deps): update dependency mongodb to v5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11387">#11387</a> fix(deps): update dependency mysql2 to v3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11389">#11389</a> fix(deps): update dependency rimraf to v4.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/nest/commit/676c98ca91212a8fd81ab37f7d7f8d12ad3dd005"><code>676c98c</code></a> chore(<a href="https://github.com/nestjs"><code>@​nestjs</code></a>) publish v9.4.0 release</li>
<li><a href="https://github.com/nestjs/nest/commit/11f512c7db19fe02dcde4c42fbdadd98a408ea89"><code>11f512c</code></a> sample: update 20-cache sample</li>
<li><a href="https://github.com/nestjs/nest/commit/4be791ffca7b99593fc81bbedb24346cb463a5d0"><code>4be791f</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11426">#11426</a> from voiceflow/feat/extend-microservice-extras</li>
<li><a href="https://github.com/nestjs/nest/commit/e990336deb411319b90f74fcd53591601fd7aaa6"><code>e990336</code></a> Merge branch 'master' of <a href="https://github.com/nestjs/nest">https://github.com/nestjs/nest</a></li>
<li><a href="https://github.com/nestjs/nest/commit/06da94bca513cd3d93859fbc175840514b09c995"><code>06da94b</code></a> chore: assert type of route info objects</li>
<li><a href="https://github.com/nestjs/nest/commit/402a389e54908351cc5702b609ff0e031d529169"><code>402a389</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/10228">#10228</a> from nathanArseneau/test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/c885a89dec2ad2b867331b6c2ff511b2b9e50cf7"><code>c885a89</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11188">#11188</a> from CodyTseng/fix-ws-multi-servers-on-different-paths</li>
<li><a href="https://github.com/nestjs/nest/commit/718e70476b763ba01cf22c14d3801a444cc9383b"><code>718e704</code></a> chore: upgrade typescript</li>
<li><a href="https://github.com/nestjs/nest/commit/9b6b00f0debcedaec1b2ca2d6be56f2cb0216e57"><code>9b6b00f</code></a> Merge branch 'master' into test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/e46147ebcbbea565a4e59e480ec0e413d2a0f29f"><code>e46147e</code></a> Merge branch 'master' into fix-ws-multi-servers-on-different-paths</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/nest/compare/v8.4.7...v9.4.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@nestjs/platform-express` from 8.4.7 to 9.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/nest/releases"><code>@​nestjs/platform-express</code>'s releases</a>.</em></p>
<blockquote>
<h2>v9.4.0 (2023-04-05)</h2>
<h4>Features</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/10628">#10628</a> feat(microservice): TCP microservice over TLS (<a href="https://github.com/nomaxg"><code>@​nomaxg</code></a>)</li>
</ul>
</li>
</ul>
<h4>Bug fixes</h4>
<ul>
<li><code>platform-ws</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11188">#11188</a> fix(ws): mount multi <code>ws</code> servers on different paths (<a href="https://github.com/CodyTseng"><code>@​CodyTseng</code></a>)</li>
</ul>
</li>
<li><code>platform-express</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11325">#11325</a> fix(express): remove body-parser types and ship these types our own (<a href="https://github.com/tolgap"><code>@​tolgap</code></a>)</li>
</ul>
</li>
</ul>
<h4>Enhancements</h4>
<ul>
<li><code>microservices</code>
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11426">#11426</a> feat: allow extension of microservice event and message extras (<a href="https://github.com/effervescentia"><code>@​effervescentia</code></a>)</li>
</ul>
</li>
</ul>
<h4>Dependencies</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11394">#11394</a> chore(deps-dev): bump sinon from 15.0.2 to 15.0.3 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11406">#11406</a> chore(deps-dev): bump <code>@​types/node</code> from 18.15.6 to 18.15.11 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11418">#11418</a> chore(deps-dev): bump <code>@​fastify/static</code> from 6.9.0 to 6.10.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11419">#11419</a> chore(deps): bump fast-json-stringify from 5.6.2 to 5.7.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11422">#11422</a> chore(deps-dev): bump <code>@​apollo/server</code> from 4.5.0 to 4.6.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11423">#11423</a> chore(deps-dev): bump amqp-connection-manager from 4.1.11 to 4.1.12 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11424">#11424</a> chore(deps-dev): bump core-js from 3.29.1 to 3.30.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11405">#11405</a> chore(deps-dev): bump ts-morph from 17.0.1 to 18.0.0 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11403">#11403</a> fix(deps): update dependency <code>@​nestjs/apollo</code> to v11.0.4 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11402">#11402</a> chore(deps): update dependency <code>@​types/cache-manager</code> to v4.0.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11401">#11401</a> chore(deps): update dependency <code>@​babel/core</code> to v7.21.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11407">#11407</a> chore(deps-dev): bump concurrently from 7.6.0 to 8.0.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11408">#11408</a> chore(deps-dev): bump <code>@​commitlint/cli</code> from 17.5.0 to 17.5.1 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11347">#11347</a> fix(deps): update dependency sequelize-typescript to v2.1.5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11344">#11344</a> fix(deps): update dependency <code>@​nestjs/typeorm</code> to v9.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11343">#11343</a> fix(deps): update dependency <code>@​nestjs/serve-static</code> to v3.0.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11342">#11342</a> fix(deps): update dependency <code>@​nestjs/mongoose</code> to v9.2.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11340">#11340</a> fix(deps): update dependency <code>@​nestjs/bull</code> to v0.6.3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11351">#11351</a> chore(deps): update dependency <code>@​types/amqplib</code> to v0.10.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11323">#11323</a> chore(deps-dev): bump <code>@​grpc/proto-loader</code> from 0.7.5 to 0.7.6 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11395">#11395</a> chore(deps-dev): bump prettier from 2.8.6 to 2.8.7 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11336">#11336</a> chore(deps): update dependency nodemon to v2.0.22 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11339">#11339</a> chore(deps): update mysql docker tag to v8.0.32 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11348">#11348</a> fix(deps): update dependency typeorm to v0.3.12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11349">#11349</a> chore(deps): update confluentinc/cp-kafka docker tag to v7.3.2 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11366">#11366</a> fix(deps): update dependency <code>@​fastify/view</code> to v7.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11376">#11376</a> fix(deps): update dependency socket.io to v4.6.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11381">#11381</a> chore(deps): update mongo docker tag to v6 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11384">#11384</a> fix(deps): update dependency mercurius to v12 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11385">#11385</a> fix(deps): update dependency mongodb to v5 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11387">#11387</a> fix(deps): update dependency mysql2 to v3 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
<li><a href="https://redirect.github.com/nestjs/nest/pull/11389">#11389</a> fix(deps): update dependency rimraf to v4.4.1 (<a href="https://github.com/apps/renovate"><code>@​renovate[bot]</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/nest/commit/676c98ca91212a8fd81ab37f7d7f8d12ad3dd005"><code>676c98c</code></a> chore(<a href="https://github.com/nestjs"><code>@​nestjs</code></a>) publish v9.4.0 release</li>
<li><a href="https://github.com/nestjs/nest/commit/11f512c7db19fe02dcde4c42fbdadd98a408ea89"><code>11f512c</code></a> sample: update 20-cache sample</li>
<li><a href="https://github.com/nestjs/nest/commit/4be791ffca7b99593fc81bbedb24346cb463a5d0"><code>4be791f</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11426">#11426</a> from voiceflow/feat/extend-microservice-extras</li>
<li><a href="https://github.com/nestjs/nest/commit/e990336deb411319b90f74fcd53591601fd7aaa6"><code>e990336</code></a> Merge branch 'master' of <a href="https://github.com/nestjs/nest">https://github.com/nestjs/nest</a></li>
<li><a href="https://github.com/nestjs/nest/commit/06da94bca513cd3d93859fbc175840514b09c995"><code>06da94b</code></a> chore: assert type of route info objects</li>
<li><a href="https://github.com/nestjs/nest/commit/402a389e54908351cc5702b609ff0e031d529169"><code>402a389</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/10228">#10228</a> from nathanArseneau/test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/c885a89dec2ad2b867331b6c2ff511b2b9e50cf7"><code>c885a89</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/nest/issues/11188">#11188</a> from CodyTseng/fix-ws-multi-servers-on-different-paths</li>
<li><a href="https://github.com/nestjs/nest/commit/718e70476b763ba01cf22c14d3801a444cc9383b"><code>718e704</code></a> chore: upgrade typescript</li>
<li><a href="https://github.com/nestjs/nest/commit/9b6b00f0debcedaec1b2ca2d6be56f2cb0216e57"><code>9b6b00f</code></a> Merge branch 'master' into test/sample-02-gateways</li>
<li><a href="https://github.com/nestjs/nest/commit/e46147ebcbbea565a4e59e480ec0e413d2a0f29f"><code>e46147e</code></a> Merge branch 'master' into fix-ws-multi-servers-on-different-paths</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/nest/compare/v8.4.7...v9.4.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@nestjs/swagger` from 5.2.1 to 6.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nestjs/swagger/releases"><code>@​nestjs/swagger</code>'s releases</a>.</em></p>
<blockquote>
<h2>Release 6.3.0</h2>
<ul>
<li>test: check ts version and compare diff output if v5 (508a206)</li>
<li>fix(plugin): hotfix ts version condition (4858616)</li>
<li>fix(plugin): hotfix ts version condition (9e82747)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2296">#2296</a> from bojovypstros/refactor-intersection (ae495fc)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2303">#2303</a> from Dracks/master (6f02ee2)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2308">#2308</a> from nestjs/renovate/swagger-ui-dist-4.x (5b02c68)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2145">#2145</a> from timoklingenhoefer/master (46c5fae)</li>
<li>Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2283">#2283</a> from nestjs/renovate/cimg-node-19.x (804d2b5)</li>
<li>chore(deps): upgrade typescript (35043f9)</li>
<li>fix(deps): update dependency swagger-ui-dist to v4.18.2 (8dc7920)</li>
<li>chore(deps): update dependency eslint to v8.37.0 (132fbac)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.11 (9ac9348)</li>
<li>chore(deps): update dependency <code>@​commitlint/cli</code> to v17.5.1 (f2c9e4f)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.57.0 (8e1d529)</li>
<li>chore(deps): update dependency <code>@​types/lodash</code> to v4.14.192 (0cd083a)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.10 (56b4054)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.9 (c8d5174)</li>
<li>chore(deps): update dependency release-it to v15.9.3 (6653b68)</li>
<li>chore(deps): update dependency prettier to v2.8.7 (5c6e615)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.7 (8d0c28c)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.6 (07db689)</li>
<li>chore(deps): update dependency <code>@​commitlint/cli</code> to v17.5.0 (f797487)</li>
<li>chore(deps): update nest monorepo to v9.3.12 (82f49cb)</li>
<li>chore(deps): update nest monorepo to v9.3.11 (47fe4b5)</li>
<li>chore(deps): update dependency release-it to v15.9.1 (8b3cdd8)</li>
<li>chore(deps): update dependency prettier to v2.8.6 (2c6c3a0)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.5 (f9aea9f)</li>
<li>chore(deps): update dependency eslint-config-prettier to v8.8.0 (52cc234)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.56.0 (83699ee)</li>
<li>chore(deps): update node.js to v19.8 (6f15fa8)</li>
<li>chore(deps): update dependency prettier to v2.8.5 (72cc7aa)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.5.0 (d399b18)</li>
<li>chore(deps): update dependency release-it to v15.9.0 (6f82f87)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.4.4 (423ee60)</li>
<li>chore(deps): update nest monorepo to v9.3.10 (e37f568)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.4.2 (44277ac)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.3 (1a71715)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.55.0 (906f720)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.2 (e0c8d19)</li>
<li>chore(deps): update dependency <code>@​types/jest</code> to v29.4.1 (259f783)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.1 (19a8750)</li>
<li>chore(deps): update dependency eslint to v8.36.0 (b9fcf4a)</li>
<li>chore(deps): update dependency lint-staged to v13.2.0 (e4b5312)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.15.0 (6eb3e4c)</li>
<li>chore(deps): update dependency release-it to v15.8.0 (329b54c)</li>
<li>chore(deps): update typescript-eslint monorepo to v5.54.1 (fa542f7)</li>
<li>chore(deps): update dependency jest to v29.5.0 (bf25252)</li>
<li>chore(deps): update dependency eslint-config-prettier to v8.7.0 (3c952d3)</li>
<li>chore(deps): update dependency <code>@​types/node</code> to v18.14.6 (3a6ce81)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nestjs/swagger/commit/2a80ffcf824a826d34947d30a6fdf67165a958d7"><code>2a80ffc</code></a> chore(): release v6.3.0</li>
<li><a href="https://github.com/nestjs/swagger/commit/508a206ca8b3e133660c9bef6e489439552ce548"><code>508a206</code></a> test: check ts version and compare diff output if v5</li>
<li><a href="https://github.com/nestjs/swagger/commit/4858616f7721c83f1246eda1e83fe42855a728c6"><code>4858616</code></a> fix(plugin): hotfix ts version condition</li>
<li><a href="https://github.com/nestjs/swagger/commit/9e82747370d5449943f7046e0f417a706c9c6c69"><code>9e82747</code></a> fix(plugin): hotfix ts version condition</li>
<li><a href="https://github.com/nestjs/swagger/commit/ae495fc6e48f5d7b79ef4cce493fbb5372c1514b"><code>ae495fc</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2296">#2296</a> from bojovypstros/refactor-intersection</li>
<li><a href="https://github.com/nestjs/swagger/commit/6f02ee28a8d2b530f6ae92229aa865627eef5886"><code>6f02ee2</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2303">#2303</a> from Dracks/master</li>
<li><a href="https://github.com/nestjs/swagger/commit/5b02c686def7f445285132970d1150ba98e0f13e"><code>5b02c68</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2308">#2308</a> from nestjs/renovate/swagger-ui-dist-4.x</li>
<li><a href="https://github.com/nestjs/swagger/commit/46c5fae21a8fd0881ea894a7c97b89649a5dd7fc"><code>46c5fae</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2145">#2145</a> from timoklingenhoefer/master</li>
<li><a href="https://github.com/nestjs/swagger/commit/804d2b5f7bde947cf872da8b49d8c6cf40420f78"><code>804d2b5</code></a> Merge pull request <a href="https://redirect.github.com/nestjs/swagger/issues/2283">#2283</a> from nestjs/renovate/cimg-node-19.x</li>
<li><a href="https://github.com/nestjs/swagger/commit/35043f9d7fee38a8a35b3cbca1ec234a95c5a20c"><code>35043f9</code></a> chore(deps): upgrade typescript</li>
<li>Additional commits viewable in <a href="https://github.com/nestjs/swagger/compare/5.2.1...6.3.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@ts-core/backend-nestjs` from 8.1.8 to 9.0.2
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/ManhattanDoctor/ts-core-backend-nestjs/commits">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 17:27:00 +0000 UTC
    </div>
</div>

