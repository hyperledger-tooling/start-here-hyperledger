---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3076" class=".btn">#3076</a>
            </td>
            <td>
                <b>
                    feat: Credential Fulfillment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added a library that allows you to parse Credential Fulfillment objects and resolve VCs from them based on an Issue Credential Message's attachment. This Credential Fulfillment implementation is based on the specification at https://identity.foundation/credential-manifest/#credential-fulfillment.

- Refactored the CredentialManifest.ResolveOutputDescriptors method to take in a *verifiable.Credential object instead of a []byte, in order to make the expected type more explicit.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 03:19:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3075" class=".btn">#3075</a>
            </td>
            <td>
                <b>
                    feat: command controllers for wallet issuance flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added JS, REST command controllers for wallet issuance interfaces.
- Part of  #3073

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 21:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3074" class=".btn">#3074</a>
            </td>
            <td>
                <b>
                    feat: WACI issuance flow interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                based on [WACI Issuance in Universal
Wallet](https://github.com/w3c-ccg/universal-wallet-interop-spec/issues/101)

- added propose credential interface
- added request credential interface
- added tests
- Closes #3073

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 16:24:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3072" class=".btn">#3072</a>
            </td>
            <td>
                <b>
                    feat: connectionRecord in OOBV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change includes ConnectionRecord creation in OOBV2 and requires invitation attachment messages to include `from`
header representing the sender's DID.


Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 15:24:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3071" class=".btn">#3071</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.64.4 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.64.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.64.4</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix tagged template literal evaluation</li>
<li>fix ModuleFederation with ESM</li>
<li>fix outputModule with intial splitChunks</li>
</ul>
<h1>Performance</h1>
<ul>
<li>upgrade watchpack for faster watcher updating</li>
<li>track file and directory timestamps separately in watchpack and webpack</li>
</ul>
<h1>Developer Experience</h1>
<ul>
<li>show origin of singleton shared module in mismatch warning</li>
</ul>
<h2>v5.64.3</h2>
<h1>Performance</h1>
<ul>
<li>allow to use pre-compiled schema when <code>Infinity</code> is used in configuration</li>
<li>allow to use pre-compiled schema for configuration arrays</li>
</ul>
<h2>v5.64.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>avoid double initial compilation due to invalid dependencies with managedPaths</li>
</ul>
<h2>v5.64.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix regexp in managedPaths to exclude additional slash</li>
<li>make module.accept errorHandler optional in typings</li>
<li>correctly create an async chunk when using a <code>require(...).property</code> in <code>require.ensure</code></li>
<li>fix cleaning of symlinks in <code>output.clean: true</code></li>
<li>fix change detection with <code>unsafeCache</code> within <code>managedPaths</code> (node_modules)</li>
<li>bump webpack-sources for Stack Overflow bugfix</li>
</ul>
<h2>v5.64.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>asyncChunks: boolean</code> option to disable creation of async chunks</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix ProfilingPlugin for <code>experiments.backCompat: false</code></li>
</ul>
<h1>Performance</h1>
<ul>
<li>avoid running regexp twice over the file list</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/d3cd4cb6e38338237fe722d4b7feae2244c425c5"><code>d3cd4cb</code></a> 5.64.4</li>
<li><a href="https://github.com/webpack/webpack/commit/4f9fafc73e46b1b08fa0d3e7551b5ab6b94d1441"><code>4f9fafc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14829">#14829</a> from webpack/bugfix/split-chunks-esm</li>
<li><a href="https://github.com/webpack/webpack/commit/093eadfdb45c3e94bab7057971debba093cb39a9"><code>093eadf</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14827">#14827</a> from webpack/bugfix/mf-module</li>
<li><a href="https://github.com/webpack/webpack/commit/c69e37c39d12c8e3c761c883069d89f90cac817c"><code>c69e37c</code></a> fix outputModule with initial splitChunks</li>
<li><a href="https://github.com/webpack/webpack/commit/041287ff589701f288d6baafe150002529317ca9"><code>041287f</code></a> fix test problem</li>
<li><a href="https://github.com/webpack/webpack/commit/c3691df74064ec2a591b3c0beefe3565f84cb71b"><code>c3691df</code></a> fix CI problems</li>
<li><a href="https://github.com/webpack/webpack/commit/d91248711b63818a4e935294dec290a760fcca5d"><code>d912487</code></a> fix and test module federation with ESM</li>
<li><a href="https://github.com/webpack/webpack/commit/ac9a2c87ed732adaf9dfe307c7690c43609d06a2"><code>ac9a2c8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14782">#14782</a> from tanhauhau/tanhauhau/show-which-container-loade...</li>
<li><a href="https://github.com/webpack/webpack/commit/ce0f0b3a164591da1b8edcee038b9e81d0bf4909"><code>ce0f0b3</code></a> update test case</li>
<li><a href="https://github.com/webpack/webpack/commit/68c4a2a0a9a9c12c55e2ba2a5273dd26958e4027"><code>68c4a2a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14728">#14728</a> from markjm/markjm/context-timestamps</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.64.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.64.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 08:14:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3070" class=".btn">#3070</a>
            </td>
            <td>
                <b>
                    wip: merge present proof v2/v3 client APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 03:34:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3068" class=".btn">#3068</a>
            </td>
            <td>
                <b>
                    feat: support mediator bdd tests with didcomm v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 04:17:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3067" class=".btn">#3067</a>
            </td>
            <td>
                <b>
                    fix: OOB V2 db name can't use . or / for mongodb compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 18:09:34 +0000 UTC
    </div>
</div>

