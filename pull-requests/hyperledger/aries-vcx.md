---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    Make vdrtools wallet usable standalone
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Previously to use wallet in `aries-vcx` you need to import and initialize entire `vdrtools`. This PR should make it possible to setup wallet without all the other vdrtools stuff (ledger zmq, anoncreds, ... )
- Reorganize files in `aries-vcx` such that all wallet APIs are under `aries_vcx_core/wallet` module

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 10:36:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    Default to modular libs
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
        Created At 2023-07-24 07:08:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/908" class=".btn">#908</a>
            </td>
            <td>
                <b>
                    Specify default libvcx feature flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix build for libvcx ios/java artifacts (no features flags are selected for ios/java builds, will fail in runtime)
- fail on compile if no implementation is selected via feature flags
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 15:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/907" class=".btn">#907</a>
            </td>
            <td>
                <b>
                    testing/remove-mixed-breed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                One less thing to worry about - since "mixed breed" testing profile was introduced, we have increased coverage with different profile significantly, and also introduced 4x different testing combinations on `libvcx_core` level. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 13:08:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/906" class=".btn">#906</a>
            </td>
            <td>
                <b>
                    Revert "Added capability of migrating wallet through the node.js wrap…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit be57e49e5fb15c790e68d8f060e8328922a7e7a1 / https://github.com/hyperledger/aries-vcx/pull/895

The PR is causing CI to fail, because it added migrator as dependency of `libvcx_core`. The migrator imports `ariesvcx_core` with `modular_libs` feature, I believe that's the culprit of the issues - as both vdrtool and indyvdr become part of the build - altough seems to work with major scenarios, in tests etc, there are probably some interplay of dependencies during the build process when building for ios/android/linux musl (napi wrapper build)

Strategic way to go about this is to to default to `indy-vdr` ledger client, delete vdrtools based ledger client (and therefore the zmq dependencies coming from `vdrtools`) and then re-apply the changes in reverted commit. 
That might solve the issue, or at least make it simpler to investigate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 12:48:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/905" class=".btn">#905</a>
            </td>
            <td>
                <b>
                    Build artifacts with indy-vdr as ledger client
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
        Created At 2023-07-21 12:36:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/904" class=".btn">#904</a>
            </td>
            <td>
                <b>
                    Bump word-wrap from 1.2.3 to 1.2.4 in /wrappers/node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [word-wrap](https://github.com/jonschlinkert/word-wrap) from 1.2.3 to 1.2.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonschlinkert/word-wrap/releases">word-wrap's releases</a>.</em></p>
<blockquote>
<h2>1.2.4</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove default indent by <a href="https://github.com/mohd-akram"><code>@​mohd-akram</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/24">jonschlinkert/word-wrap#24</a></li>
<li>🔒fix: CVE 2023 26115 (2) by <a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/41">jonschlinkert/word-wrap#41</a></li>
<li>:lock: fix: CVE-2023-26115 by <a href="https://github.com/aashutoshrathi"><code>@​aashutoshrathi</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/33">jonschlinkert/word-wrap#33</a></li>
<li>chore: publish workflow by <a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/42">jonschlinkert/word-wrap#42</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mohd-akram"><code>@​mohd-akram</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/24">jonschlinkert/word-wrap#24</a></li>
<li><a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/41">jonschlinkert/word-wrap#41</a></li>
<li><a href="https://github.com/aashutoshrathi"><code>@​aashutoshrathi</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/33">jonschlinkert/word-wrap#33</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4">https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/f64b188c7261d26b99e1e2075d6b12f21798e83a"><code>f64b188</code></a> run verb to generate README</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/03ea08256ba0c8e8b02b1b304f0f5bd2b1863207"><code>03ea082</code></a> Merge pull request <a href="https://redirect.github.com/jonschlinkert/word-wrap/issues/42">#42</a> from jonschlinkert/chore/publish-workflow</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/420dce9a2412b21881202b73a3c34f0edc53cb2e"><code>420dce9</code></a> Merge pull request <a href="https://redirect.github.com/jonschlinkert/word-wrap/issues/41">#41</a> from jonschlinkert/fix/CVE-2023-26115-2</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/bfa694edf55bb84ff84512f13da6d68bf7593f06"><code>bfa694e</code></a> Update .github/workflows/publish.yml</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/ace0b3c78f81aaf43040bab3bc91d3c5546d3fd2"><code>ace0b3c</code></a> chore: bump version to 1.2.4</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/6fd727594676f3e1b196b08a320908bec2f4ca02"><code>6fd7275</code></a> chore: add publish workflow</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/30d6daf60fce429f5f559252fa86ee78200652c4"><code>30d6daf</code></a> chore: fix test</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/655929cabea6299dddf3b4a21fc3713fca701b48"><code>655929c</code></a> chore: remove package-lock</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/49e08bbc32a84da5d79e6b7e0fa74ff6217f6d81"><code>49e08bb</code></a> chore: added an additional testcase</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/9f626935f3fac6ec0f3c4b26baea4eb9740d9645"><code>9f62693</code></a> fix: cve 2023-26115</li>
<li>Additional commits viewable in <a href="https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=word-wrap&package-manager=npm_and_yarn&previous-version=1.2.3&new-version=1.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-vcx/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 02:44:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/903" class=".btn">#903</a>
            </td>
            <td>
                <b>
                    CI: Do not publish napi wrapper when running in fork PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Should prevent this https://github.com/hyperledger/aries-vcx/pull/884 kind of failures
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 15:46:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/902" class=".btn">#902</a>
            </td>
            <td>
                <b>
                    Feature/anoncreds rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A draft implementation of the `anoncreds-rs` crate. This PR is mainly created as a reference point for the future when the (working) implementation can be done without all kinds of crazy workarounds and code smell.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 12:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/901" class=".btn">#901</a>
            </td>
            <td>
                <b>
                    Rename tails variables in prover code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">breaking</span>
            </td>
            <td>
                - This is breaking change for provers constructing "selected credentials" datastructure when creating proof. While previously they had option to specify field `tails_file`, now they have to use `tails_dir`. It's essentially forced renamed, semantics didn't change. Previously `tails_file` attribute was actually expected to point to a directory (containing tails file)
(eg. see https://github.com/hyperledger/aries-vcx/pull/901/files#diff-7542b0e9db422e41b81fc4f3bf5da974a9e5ec73a1a6a2d08d4698d4a9eb9b89R26 as example of prover accommodating this breaking change)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 11:33:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/900" class=".btn">#900</a>
            </td>
            <td>
                <b>
                    Release 0.57.0
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
        Created At 2023-07-17 13:28:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/899" class=".btn">#899</a>
            </td>
            <td>
                <b>
                    Tweak CI to fix build-docker-android on main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Additional tweak to prevent CI running out of disk space
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 13:28:06 +0000 UTC
    </div>
</div>

