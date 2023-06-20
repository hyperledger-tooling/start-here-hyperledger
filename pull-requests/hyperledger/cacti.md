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
                PR <a href="https://github.com/hyperledger/cacti/pull/2513" class=".btn">#2513</a>
            </td>
            <td>
                <b>
                    fix(dockerfile): changed the dockerfile to remove erroneous setup.py, to install all dependencies seperately.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issue #2500 
Changed the line 24 of the dockerfile, to remove the use of the erroneous setup.py to replace it with a full line of all the dependencies modeled from the same file. 

@VRamakrishna Kindly check 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 14:36:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2512" class=".btn">#2512</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.9.1 to 4.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.9.1 to 4.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.2</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p</a>.</p>
</blockquote>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.9.2/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.2 (2023-06-16)</h2>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e50c24f5839db17f46991478384bfda14acfb830"><code>e50c24f</code></a> Release v4.9.2 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4364">#4364</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4d2383e17186be3e8ccf5a442e9686ecc7de1c55"><code>4d2383e</code></a> Merge pull request from GHSA-wprv-93r4-jj2p</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/f03420b5c77ae3cfa73fce4ffc7f4778cfa2b503"><code>f03420b</code></a> Remove automatic conflict resolution for merge from release branch (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4362">#4362</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ded8c9eedb9a03b0703b65d430e6d0076cb0e444"><code>ded8c9e</code></a> Update index.adoc (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4336">#4336</a>)</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.9.1...v4.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.9.1&new-version=4.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-06-19 20:16:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2511" class=".btn">#2511</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.9.1 to 4.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.9.1 to 4.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.2</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p</a>.</p>
</blockquote>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/v4.9.2/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.2 (2023-06-16)</h2>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/bc95521e34dcd49792065e264a7ad2b5a86f0091"><code>bc95521</code></a> Transpile e50c24f5</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/e7d20ee1cecbfa36bd75ffb4b2e5dad4c47801f1"><code>e7d20ee</code></a> Transpile 4d2383e1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/8aac85b00f7f0a96b431a85ab96db81d356514a7"><code>8aac85b</code></a> Transpile f03420b5</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/953a201b0b60f70337ea4d2245500552f58fb5d5"><code>953a201</code></a> Transpile ded8c9ee</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.9.1...v4.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.9.1&new-version=4.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-06-19 19:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2466" class=".btn">#2466</a>
            </td>
            <td>
                <b>
                    ci(github): evaluate cache viability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WORK IN PROGRESS

Fixes #2117

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-17 05:55:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2465" class=".btn">#2465</a>
            </td>
            <td>
                <b>
                    test(fabric-all-in-one): fix sed write error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgrade the base images to docker:24.0.2-dind
which contain the fix for the cgroup v2 problems.

The images built locally from this commit are pushed to ghcr.io as

ghcr.io/hyperledger/cactus-fabric-all-in-one:2023-06-16-d436ef26e-issue2464-dind-v24
and
ghcr.io/hyperledger/cactus-fabric2-all-in-one:2023-06-16-d436ef26e-issue2464-dind-v24

Additional context:

The root cause analysis can be found here [1][2]
which states that the solution is to upgrade the
dind image to a version of at least 20.10.16

[1] docker-library/docker#308
[2] testcontainers/dind-drone-plugin#18

Fixes #2464

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-17 03:06:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2462" class=".btn">#2462</a>
            </td>
            <td>
                <b>
                    build(codegen): fix openapi concurrent jar download
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a script to  warm up the file-system cache where the
.jar files are downloaded (which contain the OpenAPI generator)

This way the .jar download does not happen concurrently for 26
packages but instead just the one time right before the codegen
script is executed.

IMPORTANT NOTE: If you change the OpenAPI generator version
that is being used by the project from the current v5.2.1 and v6.3.0
then these warm-up scripts must also be updated at the same time
otherwise the same issue that we are fixing here now will creep back
in immediately.

 Fixes #2461

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 05:10:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2460" class=".btn">#2460</a>
            </td>
            <td>
                <b>
                    docs ( update ) update FAQ.md file 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                adding Alternative cacti install guide for developers using local machines in FAQ.md

Signed-off-by: Barnaba Pawelczak <barnaba.pawelczak@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 08:41:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2457" class=".btn">#2457</a>
            </td>
            <td>
                <b>
                    ci(custom-checks): fix sibling pkg dependency version inconsistencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - replace old packages verions in package.json files printed after $npm run custom-checks

Closes: #2431
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 18:13:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2456" class=".btn">#2456</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-cdl-socketio): add new connector plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add new plugin for connecting with Fujitsu CDL.
- Add test script for checking connector operations manually.

Closes: #2455
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 13:09:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2454" class=".btn">#2454</a>
            </td>
            <td>
                <b>
                    CI Scan
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
        Created At 2023-06-14 06:58:09 +0000 UTC
    </div>
</div>

