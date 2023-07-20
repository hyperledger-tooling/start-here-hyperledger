---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4326" class=".btn">#4326</a>
            </td>
            <td>
                <b>
                    Bump pygments from 2.1.3 to 2.15.0 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pygments](https://github.com/pygments/pygments) from 2.1.3 to 2.15.0.
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
<li>Additional commits viewable in <a href="https://github.com/pygments/pygments/compare/2.1.3...2.15.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pygments&package-manager=pip&previous-version=2.1.3&new-version=2.15.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 11:17:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4325" class=".btn">#4325</a>
            </td>
            <td>
                <b>
                    Merge batch size in configtx for both Raft and BFT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge batch size in configtx for both Raft and BFT

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Look at #4294


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 11:02:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4324" class=".btn">#4324</a>
            </td>
            <td>
                <b>
                    [Fix]: Provide a meaningful error for cert sanitization (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit handles the error where the certificate sanitization procedure fails to construct the certificate chain due to misconfiguration. Before this commit, the peer will simply fail with panic without a clear explanation of what exactly was wrong.

Addresses (#4302).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 18:25:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4323" class=".btn">#4323</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.6 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.6.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 17:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4322" class=".btn">#4322</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.6 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.6.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 17:51:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4321" class=".btn">#4321</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.6.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 17:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4320" class=".btn">#4320</a>
            </td>
            <td>
                <b>
                    [Fix]: Provide a meaningful error for cert sanitization (backport #4307)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4307 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 17:33:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4319" class=".btn">#4319</a>
            </td>
            <td>
                <b>
                    Clarify endorsement policy documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The documentation for the default 'majority' endorsement policy was misleading. This commit clarifies it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 21:19:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4318" class=".btn">#4318</a>
            </td>
            <td>
                <b>
                    bft chain unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added unit tests to BFT chain

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 13:13:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4317" class=".btn">#4317</a>
            </td>
            <td>
                <b>
                    Update Homebrew install command in prereq docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Match current install instructions at https://brew.sh/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 20:28:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4316" class=".btn">#4316</a>
            </td>
            <td>
                <b>
                    Update install script for v2.5.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #4300
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 20:21:02 +0000 UTC
    </div>
</div>

