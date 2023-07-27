---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3748" class=".btn">#3748</a>
            </td>
            <td>
                <b>
                    [fix] #3741: Fix tempfile error in `kagami validator`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->
Getting rid of `tempdir` was a driveby fix I did in the CI PR that wasn't merged. Also fixing two other smaller bugs that didn't even have an issue assigned.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3741. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
`kagami validator` and `kagami swarm` working as expected.
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 16:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3747" class=".btn">#3747</a>
            </td>
            <td>
                <b>
                    [fix] #3451: Fix docker build on M1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->
The docker build on M1 was failing because of lacking `platform` tag at first, and then because of some missing links to `wasm-opt`'s musl binaries.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3451. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Finally local docker launching as expected on M1 machines, abysmal build times notwithstanding.
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 16:30:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3746" class=".btn">#3746</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2022.12.7 to 2023.7.22 in /docs/source
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 20:52:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3744" class=".btn">#3744</a>
            </td>
            <td>
                <b>
                    Add removeSignatory cmd to iroha-lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add missing removeSignatory command to iroha_lib_model

## Description

<!-- Just describe what you did. -->

Add missing `removeSignatory`  command implementation to **iroha_lib_model**

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 09:38:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3743" class=".btn">#3743</a>
            </td>
            <td>
                <b>
                    Add GetPeers Query to iroha-lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

Add `GetPeers`  Query to **iroha_lib_model**

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 09:28:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3739" class=".btn">#3739</a>
            </td>
            <td>
                <b>
                    [ci] #3654: Fix iroha2 glibc-based Dockerfiles to be deployed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Fix `Dockerfile.build.glibc` and `Dockerfile.glibc` to be adopted for fully deployment scenario.
2. Bump `alpine` base image version to the stable one iroha2 musl-based image.

### Linked issue

#3654 

Closes #3654 

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 15:57:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3735" class=".btn">#3735</a>
            </td>
            <td>
                <b>
                    [fix] #3445: make `POST configuration` work again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description
Fixed the bug where `GET /configuration` was working, but `POST ..` wasn't.
<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3445. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
All working as expected. Too bad there's no integration test to catch this regression?
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 14:15:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3728" class=".btn">#3728</a>
            </td>
            <td>
                <b>
                    Bump pygments from 2.7.4 to 2.15.0 in /docs/source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pygments](https://github.com/pygments/pygments) from 2.7.4 to 2.15.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pygments/pygments/releases">pygments's releases</a>.</em></p>
<blockquote>
<h2>2.15.0</h2>
<ul>
<li>
<p>Added lexers:</p>
<ul>
<li>Carbon (<a href="https://redirect.github.com/pygments/pygments/issues/2362">#2362</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2365">#2365</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2366">#2366</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2367">#2367</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2368">#2368</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2369">#2369</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2370">#2370</a>)</li>
<li>Dax (<a href="https://redirect.github.com/pygments/pygments/issues/2335">#2335</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2345">#2345</a>)</li>
<li>MediaWiki Wikitext (<a href="https://redirect.github.com/pygments/pygments/issues/2373">#2373</a>, <a href="https://redirect.github.com/pygments/pygments/issues/827">#827</a>)</li>
<li>PostgreSQL Explain (<a href="https://redirect.github.com/pygments/pygments/issues/2398">#2398</a>)</li>
<li>WGSL (WebGPU Shading Language) (<a href="https://redirect.github.com/pygments/pygments/issues/2386">#2386</a>)</li>
<li>X++ (<a href="https://redirect.github.com/pygments/pygments/issues/2339">#2339</a>)</li>
</ul>
</li>
<li>
<p>Updated lexers:</p>
<ul>
<li>
<p>AMDGPU: Add support for <code>scratch_</code> instructions, the <code>attr*.*</code> argument,
as well as the <code>off</code> modifier (<a href="https://redirect.github.com/pygments/pygments/issues/2327">#2327</a>).</p>
</li>
<li>
<p>APDL: Miscellaneous improvements (<a href="https://redirect.github.com/pygments/pygments/issues/2314">#2314</a>)</p>
</li>
<li>
<p>bash/tcsh:</p>
<ul>
<li>Move <code>break</code> to keywords (<a href="https://redirect.github.com/pygments/pygments/issues/2377">#2377</a>)</li>
<li>Improve bash math expansion lexing (<a href="https://redirect.github.com/pygments/pygments/issues/2255">#2255</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2353">#2353</a>)</li>
</ul>
</li>
<li>
<p>Chapel: Support attributes (<a href="https://redirect.github.com/pygments/pygments/issues/2376">#2376</a>)</p>
</li>
<li>
<p>CMake: Implement bracket style comments (<a href="https://redirect.github.com/pygments/pygments/issues/2338">#2338</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2354">#2354</a>)</p>
</li>
<li>
<p>CSS: Improve lexing of numbers inside function calls (<a href="https://redirect.github.com/pygments/pygments/issues/2382">#2382</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2383">#2383</a>)</p>
</li>
<li>
<p>diff: Support normal diff syntax, as opposed to unified diff syntax (<a href="https://redirect.github.com/pygments/pygments/issues/2321">#2321</a>)</p>
</li>
<li>
<p>GLSL, HLSL:</p>
<ul>
<li>Support line continuations in preprocessor code (<a href="https://redirect.github.com/pygments/pygments/issues/2350">#2350</a>)</li>
<li>Improve preprocessor directive handling (<a href="https://redirect.github.com/pygments/pygments/issues/2357">#2357</a>)</li>
</ul>
</li>
<li>
<p>LilyPond: minor update of builtins</p>
</li>
<li>
<p>PHP: support attributes (<a href="https://redirect.github.com/pygments/pygments/issues/2055">#2055</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2347">#2347</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2360">#2360</a>), fix anonymous classes without
parameters (<a href="https://redirect.github.com/pygments/pygments/issues/2359">#2359</a>), improve lexing of variable variable syntax (<a href="https://redirect.github.com/pygments/pygments/issues/2358">#2358</a>)</p>
</li>
<li>
<p>Python:</p>
<ul>
<li>Add missing builtins (<a href="https://redirect.github.com/pygments/pygments/issues/2334">#2334</a>)</li>
<li>Fix inconsistent lexing of <code>None</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2406">#2406</a>)</li>
</ul>
</li>
<li>
<p>Rebol/Red: Don't require script headers (<a href="https://redirect.github.com/pygments/pygments/issues/2348">#2348</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2349">#2349</a>)</p>
</li>
<li>
<p>Spice: Update keywords (<a href="https://redirect.github.com/pygments/pygments/issues/2336">#2336</a>)</p>
</li>
<li>
<p>SQL+Jinja (<code>analyse_text</code> method): Fix catastrophic backtracking (<a href="https://redirect.github.com/pygments/pygments/issues/2355">#2355</a>)</p>
</li>
<li>
<p>Terraform: Add <code>hcl</code> alias (<a href="https://redirect.github.com/pygments/pygments/issues/2375">#2375</a>)</p>
</li>
</ul>
</li>
<li>
<p>Declare support for Python 3.11 and drop support for Python 3.6 (<a href="https://redirect.github.com/pygments/pygments/issues/2324">#2324</a>).</p>
</li>
<li>
<p>Update <code>native</code> style to improve contrast (<a href="https://redirect.github.com/pygments/pygments/issues/2325">#2325</a>).</p>
</li>
<li>
<p>Update `github-dark`` style to match latest Primer style (<a href="https://redirect.github.com/pygments/pygments/issues/2401">#2401</a>)</p>
</li>
<li>
<p>Revert a change that made guessing lexers based on file names slower
on Python 3.10 and older (<a href="https://redirect.github.com/pygments/pygments/issues/2328">#2328</a>).</p>
</li>
<li>
<p>Fix some places where a locale-dependent encoding could unintentionally
be used instead of UTF-8 (<a href="https://redirect.github.com/pygments/pygments/issues/2326">#2326</a>).</p>
</li>
<li>
<p>Fix Python traceback handling (<a href="https://redirect.github.com/pygments/pygments/issues/2226">#2226</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2329">#2329</a>).</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pygments/pygments/blob/master/CHANGES">pygments's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.15.0</h2>
<p>(released April 10th, 2023)</p>
<ul>
<li>
<p>Added lexers:</p>
<ul>
<li>Carbon (<a href="https://redirect.github.com/pygments/pygments/issues/2362">#2362</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2365">#2365</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2366">#2366</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2367">#2367</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2368">#2368</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2369">#2369</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2370">#2370</a>)</li>
<li>Dax (<a href="https://redirect.github.com/pygments/pygments/issues/2335">#2335</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2345">#2345</a>)</li>
<li>MediaWiki Wikitext (<a href="https://redirect.github.com/pygments/pygments/issues/2373">#2373</a>, <a href="https://redirect.github.com/pygments/pygments/issues/827">#827</a>)</li>
<li>PostgreSQL Explain (<a href="https://redirect.github.com/pygments/pygments/issues/2398">#2398</a>)</li>
<li>WGSL (WebGPU Shading Language) (<a href="https://redirect.github.com/pygments/pygments/issues/2386">#2386</a>)</li>
<li>X++ (<a href="https://redirect.github.com/pygments/pygments/issues/2339">#2339</a>)</li>
</ul>
</li>
<li>
<p>Updated lexers:</p>
<ul>
<li>
<p>AMDGPU: Add support for <code>scratch_</code> instructions, the <code>attr*.*</code> argument,
as well as the <code>off</code> modifier (<a href="https://redirect.github.com/pygments/pygments/issues/2327">#2327</a>).</p>
</li>
<li>
<p>APDL: Miscellaneous improvements (<a href="https://redirect.github.com/pygments/pygments/issues/2314">#2314</a>)</p>
</li>
<li>
<p>bash/tcsh:</p>
<ul>
<li>Move <code>break</code> to keywords (<a href="https://redirect.github.com/pygments/pygments/issues/2377">#2377</a>)</li>
<li>Improve bash math expansion lexing (<a href="https://redirect.github.com/pygments/pygments/issues/2255">#2255</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2353">#2353</a>)</li>
</ul>
</li>
<li>
<p>Chapel: Support attributes (<a href="https://redirect.github.com/pygments/pygments/issues/2376">#2376</a>)</p>
</li>
<li>
<p>CMake: Implement bracket style comments (<a href="https://redirect.github.com/pygments/pygments/issues/2338">#2338</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2354">#2354</a>)</p>
</li>
<li>
<p>CSS: Improve lexing of numbers inside function calls (<a href="https://redirect.github.com/pygments/pygments/issues/2382">#2382</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2383">#2383</a>)</p>
</li>
<li>
<p>diff: Support normal diff syntax, as opposed to unified diff syntax (<a href="https://redirect.github.com/pygments/pygments/issues/2321">#2321</a>)</p>
</li>
<li>
<p>GLSL, HLSL:</p>
<ul>
<li>Support line continuations in preprocessor code (<a href="https://redirect.github.com/pygments/pygments/issues/2350">#2350</a>)</li>
<li>Improve preprocessor directive handling (<a href="https://redirect.github.com/pygments/pygments/issues/2357">#2357</a>)</li>
</ul>
</li>
<li>
<p>LilyPond: minor update of builtins</p>
</li>
<li>
<p>PHP: support attributes (<a href="https://redirect.github.com/pygments/pygments/issues/2055">#2055</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2347">#2347</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2360">#2360</a>), fix anonymous classes without
parameters (<a href="https://redirect.github.com/pygments/pygments/issues/2359">#2359</a>), improve lexing of variable variable syntax (<a href="https://redirect.github.com/pygments/pygments/issues/2358">#2358</a>)</p>
</li>
<li>
<p>Python:</p>
<ul>
<li>Add missing builtins (<a href="https://redirect.github.com/pygments/pygments/issues/2334">#2334</a>)</li>
<li>Fix inconsistent lexing of <code>None</code> (<a href="https://redirect.github.com/pygments/pygments/issues/2406">#2406</a>)</li>
</ul>
</li>
<li>
<p>Rebol/Red: Don't require script headers (<a href="https://redirect.github.com/pygments/pygments/issues/2348">#2348</a>, <a href="https://redirect.github.com/pygments/pygments/issues/2349">#2349</a>)</p>
</li>
<li>
<p>Spice: Update keywords (<a href="https://redirect.github.com/pygments/pygments/issues/2336">#2336</a>)</p>
</li>
<li>
<p>SQL+Jinja (<code>analyse_text</code> method): Fix catastrophic backtracking (<a href="https://redirect.github.com/pygments/pygments/issues/2355">#2355</a>)</p>
</li>
<li>
<p>Terraform: Add <code>hcl</code> alias (<a href="https://redirect.github.com/pygments/pygments/issues/2375">#2375</a>)</p>
</li>
</ul>
</li>
<li>
<p>Declare support for Python 3.11 and drop support for Python 3.6 (<a href="https://redirect.github.com/pygments/pygments/issues/2324">#2324</a>).</p>
</li>
<li>
<p>Update <code>native</code> style to improve contrast (<a href="https://redirect.github.com/pygments/pygments/issues/2325">#2325</a>).</p>
</li>
<li>
<p>Update `github-dark`` style to match latest Primer style (<a href="https://redirect.github.com/pygments/pygments/issues/2401">#2401</a>)</p>
</li>
<li>
<p>Revert a change that made guessing lexers based on file names slower
on Python 3.10 and older (<a href="https://redirect.github.com/pygments/pygments/issues/2328">#2328</a>).</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pygments/pygments/commit/6c187ad83267be9ce142af3fd5c9e670339dc7aa"><code>6c187ad</code></a> Prepare 2.15 release.</li>
<li><a href="https://github.com/pygments/pygments/commit/00b9cb022cc9c05784c43c11bd7f73e64008b347"><code>00b9cb0</code></a> Prepare for release.</li>
<li><a href="https://github.com/pygments/pygments/commit/a0824a45f0bd6c45528fa16132f09dd3570a8234"><code>a0824a4</code></a> Update CHANGES</li>
<li><a href="https://github.com/pygments/pygments/commit/26f9f6c852846fe579c37fe936a872b68fa686ba"><code>26f9f6c</code></a> Merge pull request <a href="https://redirect.github.com/pygments/pygments/issues/2406">#2406</a> from rdbende/fix-fromimport-none</li>
<li><a href="https://github.com/pygments/pygments/commit/62b1bbbe6e329268eaa4c68f0e3eb8867c450acc"><code>62b1bbb</code></a> Change token of None after from keyword</li>
<li><a href="https://github.com/pygments/pygments/commit/acee60e4e8dde9ea99fc494740e20b06188791ac"><code>acee60e</code></a> Update CHANGES</li>
<li><a href="https://github.com/pygments/pygments/commit/eaca69091119e0ac5c97e626ba9e3b21b688c5ed"><code>eaca690</code></a> Add lexer for MediaWiki Wikitext (<a href="https://redirect.github.com/pygments/pygments/issues/2373">#2373</a>)</li>
<li><a href="https://github.com/pygments/pygments/commit/0e9c87bcf096908956e031f15a4e589e83be1691"><code>0e9c87b</code></a> Update CHANGES</li>
<li><a href="https://github.com/pygments/pygments/commit/ef0abbaece522732031d61391567c017d48d87b7"><code>ef0abba</code></a> Add PostgreSQL Explain lexer (<a href="https://redirect.github.com/pygments/pygments/issues/2398">#2398</a>)</li>
<li><a href="https://github.com/pygments/pygments/commit/3c6e2af8fbc44bb1ef77389d09118c37faea8746"><code>3c6e2af</code></a> Update CHANGES</li>
<li>Additional commits viewable in <a href="https://github.com/pygments/pygments/compare/2.7.4...2.15.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pygments&package-manager=pip&previous-version=2.7.4&new-version=2.15.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 13:11:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3727" class=".btn">#3727</a>
            </td>
            <td>
                <b>
                    [refactor]: introduce syn 2.0, manyhow and darling for proc-macros
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR adds `syn` 2.0 to the workspace (under the name of `syn2`, to allow co-existence of different versions).

It then updates `iroha_version_derive`, `iroha_primitives_derive` and `iroha_derive` to use syn2, as well as moving from unmaintained `proc-macro-error` to `manyhow`.

It also changes some macro APIs:

I also propose the following changes for `VariantCount` macro (not yet implemented): 
   - confusingly, attributes for `VariantCount` are placed on fields instead of enum variants. I suggest we move them to variants, as it's really a property of the variant
   - the naming of `#[skip_try_from]` is confusing in the context of #[skip_from]: the different in names is in the try, but they correspond to different directions of the generated conversions: from is for `Variant` -> `Enum` and `try_from` is for `Enum` -> `Variant`. I suggest changing the name to `#[skip_into]` or `#[skip_try_into]` to properly represent the change of conversion direction, even if the actual generated trait is `From`
   - Maybe change `#[skip_container]` to `#[skip_from_container]`?

### Benefits

Unlike `proc-macro-error`, `manyhow` is actively maintained and has cleaner API that does not rely on global state.

Using `darling` streamlines parsing of (most) attributes by using a declarative serde-like model, also providing reasonable error messages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 11:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3724" class=".btn">#3724</a>
            </td>
            <td>
                <b>
                    [feature] #3651: WSV snapshots
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Implement `Serialize`/`Deserialize` for `WorldStateView` and down the tree.
Initial implementation of `Fast` init mode for Kura - for now just saves serialized WSV on Kura shutdown, restore when Kura is in `Fast` init mode. In the future this behaviour could be expanded to save snapshots periodically and/or on request, snapshot pruning, etc.

### Linked issue

#3651

### Benefits

Faster start-up time.
Possibly useful for debugging of block stores - WSV snapshot is easier to inspect than a blockchain.

### Drawbacks

Contains manual implementations of serde traits that will need to be maintained. Deriving doesn't seem possible, since there's no support for `DeserializeSeed` in `serde_derive` (and [not planned](https://github.com/serde-rs/serde/issues/881#issuecomment-1627865581)). 

### Alternate designs

Instead of `serde` we could possibly use Parity SCALE, but I believe writing `Decode`/`Encode` implementations would require significant effort.
Instead of serializing `WorldStateView` directly we could use some sort of proxy struct. That would come with performance overhead.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 05:20:01 +0000 UTC
    </div>
</div>

