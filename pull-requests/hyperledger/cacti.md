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
                PR <a href="https://github.com/hyperledger/cacti/pull/2589" class=".btn">#2589</a>
            </td>
            <td>
                <b>
                    build(openapi): license presence check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Adds a custom check that ensures that all the properties of the
license object are specified (name, identifier, url).
2. Optimized the custom-check that verifies the opan API json specs so
that it ignores **/node_modules/ not just node_modules (meaning that it
was only excluding the root dir not all sub-dirs of the packages as well)

Fixes #490

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 00:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2588" class=".btn">#2588</a>
            </td>
            <td>
                <b>
                    test(test-geth-ledger): add test for test-geth-ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add tests for geth-test-ledger
- fix small errors in GethTestLedger class
    
Closes: #2579 
Depends on: #2577
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 15:41:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2587" class=".btn">#2587</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in example-carbon-accounting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2062
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 06:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2586" class=".btn">#2586</a>
            </td>
            <td>
                <b>
                    build(cmd-api-server): upgrade to Artillery v2.x or migrate to loadtest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2234
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 04:40:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2585" class=".btn">#2585</a>
            </td>
            <td>
                <b>
                    chore: fix package.json#name properties to have scope and project name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2570

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 23:14:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2584" class=".btn">#2584</a>
            </td>
            <td>
                <b>
                    build(deps): bump certifi from 2022.12.7 to 2023.7.22 in /packages-python/cactus_validator_socketio_indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [certifi](https://github.com/certifi/python-certifi) from 2022.12.7 to 2023.7.22.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/8fb96ed81f71e7097ed11bc4d9b19afd7ea5c909"><code>8fb96ed</code></a> 2023.07.22</li>
<li><a href="https://github.com/certifi/python-certifi/commit/afe77220e0eaa722593fc5d294213ff5275d1b40"><code>afe7722</code></a> Bump actions/setup-python from 4.6.1 to 4.7.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/230">#230</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2038739ad56abec7aaddfa90ad2ce6b3ed7f5c7b"><code>2038739</code></a> Bump dessant/lock-threads from 3.0.0 to 4.0.1 (<a href="https://redirect.github.com/certifi/python-certifi/issues/229">#229</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/44df761f4c09d19f32b3cc09208a739043a5e25b"><code>44df761</code></a> Hash pin Actions and enable dependabot (<a href="https://redirect.github.com/certifi/python-certifi/issues/228">#228</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/8b3d7bae85bbc87c9181cc1d39548db3d31627f0"><code>8b3d7ba</code></a> 2023.05.07</li>
<li><a href="https://github.com/certifi/python-certifi/commit/53da2405b1af430f6bafa21ba45d8dd8dfc726b8"><code>53da240</code></a> ci: Add Python 3.12-dev to the testing (<a href="https://redirect.github.com/certifi/python-certifi/issues/224">#224</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2fc3b1f64d6946f1057971ee897ea828ae848d8"><code>c2fc3b1</code></a> Create a Security Policy (<a href="https://redirect.github.com/certifi/python-certifi/issues/222">#222</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c211ef482a01aff5f1bc92c4128bfa0c955f4a01"><code>c211ef4</code></a> Set up permissions to github workflows (<a href="https://redirect.github.com/certifi/python-certifi/issues/218">#218</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2087de5d0aa1d472145fc1dbdfece3fe652bbac5"><code>2087de5</code></a> Don't let deprecation warning fail CI (<a href="https://redirect.github.com/certifi/python-certifi/issues/219">#219</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e0b9fc5c8f52ac8c300da502e5760ce3d41429ec"><code>e0b9fc5</code></a> remove paragraphs about 1024-bit roots from README</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2022.12.07...2023.07.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2022.12.7&new-version=2023.7.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-07-25 20:59:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2583" class=".btn">#2583</a>
            </td>
            <td>
                <b>
                    build(deps): bump certifi from 2022.12.7 to 2023.7.22 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [certifi](https://github.com/certifi/python-certifi) from 2022.12.7 to 2023.7.22.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/8fb96ed81f71e7097ed11bc4d9b19afd7ea5c909"><code>8fb96ed</code></a> 2023.07.22</li>
<li><a href="https://github.com/certifi/python-certifi/commit/afe77220e0eaa722593fc5d294213ff5275d1b40"><code>afe7722</code></a> Bump actions/setup-python from 4.6.1 to 4.7.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/230">#230</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2038739ad56abec7aaddfa90ad2ce6b3ed7f5c7b"><code>2038739</code></a> Bump dessant/lock-threads from 3.0.0 to 4.0.1 (<a href="https://redirect.github.com/certifi/python-certifi/issues/229">#229</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/44df761f4c09d19f32b3cc09208a739043a5e25b"><code>44df761</code></a> Hash pin Actions and enable dependabot (<a href="https://redirect.github.com/certifi/python-certifi/issues/228">#228</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/8b3d7bae85bbc87c9181cc1d39548db3d31627f0"><code>8b3d7ba</code></a> 2023.05.07</li>
<li><a href="https://github.com/certifi/python-certifi/commit/53da2405b1af430f6bafa21ba45d8dd8dfc726b8"><code>53da240</code></a> ci: Add Python 3.12-dev to the testing (<a href="https://redirect.github.com/certifi/python-certifi/issues/224">#224</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2fc3b1f64d6946f1057971ee897ea828ae848d8"><code>c2fc3b1</code></a> Create a Security Policy (<a href="https://redirect.github.com/certifi/python-certifi/issues/222">#222</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c211ef482a01aff5f1bc92c4128bfa0c955f4a01"><code>c211ef4</code></a> Set up permissions to github workflows (<a href="https://redirect.github.com/certifi/python-certifi/issues/218">#218</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2087de5d0aa1d472145fc1dbdfece3fe652bbac5"><code>2087de5</code></a> Don't let deprecation warning fail CI (<a href="https://redirect.github.com/certifi/python-certifi/issues/219">#219</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e0b9fc5c8f52ac8c300da502e5760ce3d41429ec"><code>e0b9fc5</code></a> remove paragraphs about 1024-bit roots from README</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2022.12.07...2023.07.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2022.12.7&new-version=2023.7.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-07-25 20:59:16 +0000 UTC
    </div>
</div>

