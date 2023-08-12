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
                PR <a href="https://github.com/hyperledger/cacti/pull/2604" class=".btn">#2604</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.9.2 to 4.9.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.9.2 to 4.9.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.3</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-g4vp-m682-qqmp">GHSA-g4vp-m682-qqmp</a>.</p>
</blockquote>
<ul>
<li><code>ERC2771Context</code>: Return the forwarder address whenever the <code>msg.data</code> of a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes), as specified by ERC-2771. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4481">#4481</a>)</li>
<li><code>ERC2771Context</code>: Prevent revert in <code>_msgData()</code> when a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes). Return the full calldata in that case. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4484">#4484</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.9.3/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.3 (2023-07-28)</h2>
<ul>
<li><code>ERC2771Context</code>: Return the forwarder address whenever the <code>msg.data</code> of a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes), as specified by ERC-2771. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4481">#4481</a>)</li>
<li><code>ERC2771Context</code>: Prevent revert in <code>_msgData()</code> when a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes). Return the full calldata in that case. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4484">#4484</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/fd81a96f01cc42ef1c9a5399364968d0e07e9e90"><code>fd81a96</code></a> Release v4.9.3 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4482">#4482</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/70dea74ac7d969321d56cebdb96cf31cd9f1fb8a"><code>70dea74</code></a> Add changeset PR numbers</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e4435eed757d4309436b1e06608e97b6d6e2fdb5"><code>e4435ee</code></a> Adjust ERC2771Context._msgData for msg.data.length &lt; 20 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4484">#4484</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/7ec712baa50525353360a43700f953912bebef9c"><code>7ec712b</code></a> Make ERC2771Context return original sender address if <code>msg.data.length &lt;= 20</code>...</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/d26025b4103b8d053684a75129a16852d1ae95c0"><code>d26025b</code></a> Fix error when running hardhat test with parameters (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4265">#4265</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a54f6398e5463081909e1d24248942c953b272a3"><code>a54f639</code></a> Update docs for <code>SafeERC20.forceApprove</code> (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4231">#4231</a>)</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.9.2...v4.9.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.9.2&new-version=4.9.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 19:33:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2603" class=".btn">#2603</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.9.2 to 4.9.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.9.2 to 4.9.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.3</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-g4vp-m682-qqmp">GHSA-g4vp-m682-qqmp</a>.</p>
</blockquote>
<ul>
<li><code>ERC2771Context</code>: Return the forwarder address whenever the <code>msg.data</code> of a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes), as specified by ERC-2771. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4481">#4481</a>)</li>
<li><code>ERC2771Context</code>: Prevent revert in <code>_msgData()</code> when a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes). Return the full calldata in that case. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4484">#4484</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/v4.9.3/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.3 (2023-07-28)</h2>
<ul>
<li><code>ERC2771Context</code>: Return the forwarder address whenever the <code>msg.data</code> of a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes), as specified by ERC-2771. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4481">#4481</a>)</li>
<li><code>ERC2771Context</code>: Prevent revert in <code>_msgData()</code> when a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes). Return the full calldata in that case. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4484">#4484</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/3d4c0d5741b131c231e558d7a6213392ab3672a5"><code>3d4c0d5</code></a> Transpile fd81a96f</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/54bd6e3b8feff65dd623d86f4f3e1ca3351d8920"><code>54bd6e3</code></a> Transpile 70dea74a</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/1c13b8134f4216a1df353956ab8d8364c9882f7b"><code>1c13b81</code></a> Transpile e4435eed</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/231affb7723504f323d742a5d6079a646c82a3d4"><code>231affb</code></a> Transpile 7ec712ba</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/2a2bda2d295ef79541c5645b8aa9ac3c193c6f78"><code>2a2bda2</code></a> Transpile d26025b4</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/b87a6bf321fff890d7bd7b0c99d3f03e9d8cd886"><code>b87a6bf</code></a> Transpile a54f6398</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.9.2...v4.9.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.9.2&new-version=4.9.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 19:15:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2602" class=".btn">#2602</a>
            </td>
            <td>
                <b>
                    fix: use common package convention
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - change package.json and tsconfig.json files to follow common convention

Closes: #2216
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 09:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2599" class=".btn">#2599</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): fix tests - package io/fs is not in GOROOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                  The simple answer was to upgrade to go v1.20.x from v1.15.x, but
  this caused a series of other problems that also needed to address
  so the complete list of changes and their motivations are below:
  
  1. The upgrade to go v1.20.6
  1.1. We no longer install docker-compose via pip because since v2
  it ships with the main docker package itself (they rewrote it in go)
  1.2. Added a new "gcompat" apk package which is necessary because
  of go v1.20.6 as well. Details on this can be found here:
  https://github.com/golang/go/issues/59305#issuecomment-1488478737
  1.3. As  part of installing the OpenSSH server, we now must first wipe all
  openssh* packages due to newly surfaced package version conflicts due
  to the ones that are prepackaged with the alpine image.
  Without the purge step it fails like this:
```
        => ERROR [17/64] RUN apk add --no-cache openssh augeas                   1.1s
       ------
        > [17/64] RUN apk add --no-cache openssh augeas:
       0.300 fetch https://dl-cdn.alpinelinux.org/alpine/v3.18/main/x86_64/APKINDEX.tar.gz
       0.560 fetch https://dl-cdn.alpinelinux.org/alpine/v3.18/community/x86_64/APKINDEX.tar.gz
       1.041 ERROR: unable to select packages:
       1.043   openssh-client-common-9.3_p1-r3:
       1.043     breaks: openssh-client-default-9.3_p2-r0[openssh-client-common=9.3_p2-r0]
```
  2. Upgraded the node-ssh library to v13 because v12 was broken due to
  changes introduced by the new OpenSSH server.
  3. Modified the container image definition so that we have the ability
  to customize the version of fabric-nodeenv images used internally by the
  peers of the fabric-samples repository. This was needed so that we can
  control what version of npm and NodeJS are being used when the chain code
  installation process is happening (which is just the peer running the
  `npm install --production` command within the fabric-nodeenv container)
  4. The default Fabric version used by the testing infrastructure is now
  Fabric v2.2.13 and for the NodeJS chain code it is 2.4.2
  5. Slightly rearranged the imports & constants in some of the tests
  which made it easier to verify that the new image is working as intended.
  6. The new image built from this dockerfile for Fabric AIO 2.x is tagged
  on the registry as:
  `ghcr.io/hyperledger/cactus-fabric2-all-in-one:2023-08-05-issue2358`
  
  Fixes #2358
  
  Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-08 22:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2598" class=".btn">#2598</a>
            </td>
            <td>
                <b>
                    fix(indy-validator): fix package dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update indy validator python dependencies.
- Add README chapter on updating python dependencies to simplify this process in the future.
- Use pinend ubuntu base image in indy-sdk-cli dockerfile.
- Do some minor README improvements and cleanups.

Tested with `discounted-asset-trade` (should work without an issue now, at least dockerless one)

Depends on: #2596

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 09:36:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2597" class=".btn">#2597</a>
            </td>
            <td>
                <b>
                    test(jest): reduce Jest log verbosity - make logs more compact
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Configure jest to override it's internal console logger with the
regular console object provided by the JS runtime.
This way it does not have the extra information printed that is
not useful for 99% of our use-cases (100% of the known ones).

Fixes #2595

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-05 19:44:45 +0000 UTC
    </div>
</div>

