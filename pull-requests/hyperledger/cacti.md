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
                PR <a href="https://github.com/hyperledger/cacti/pull/3361" class=".btn">#3361</a>
            </td>
            <td>
                <b>
                    enable useUnknownInCatchVariables typescript compiler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - enable useUnknownInCatchVariables flag in tsconfig

Closes: #2463
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-26 11:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3360" class=".btn">#3360</a>
            </td>
            <td>
                <b>
                    chore(examples): update versions in discounted-asset-trade example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the versions in the discounted-asset-trade example to ensure
compatibility and proper functionality.

The Fabric version was upgraded from 2.4.4 to 2.5.6 as the internal image
being used required v2_5 capability.

Additionally, as per the Hyperledger Fabric documentation
(https://hyperledger-fabric.readthedocs.io/en/release-2.5/prereqs.html),
Go version 1.22.4 is needed for the example to work in its entirety.

Signed-off-by: Rajat Sharma <rajat.sharma@ril.com>

**Pull Request Requirements**
- [X] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [X] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [X] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [X] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [X] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-25 14:49:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3359" class=".btn">#3359</a>
            </td>
            <td>
                <b>
                    build: bump the npm_and_yarn group across 1 directory with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 4 updates in the / directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node), [bl](https://github.com/rvagg/bl), [qs](https://github.com/ljharb/qs) and [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite).

Updates `@grpc/grpc-js` from 1.10.9 to 1.10.10
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.10.10</h2>
<ul>
<li>Various improvements to handling of keepalive timers (<a href="https://redirect.github.com/grpc/grpc-node/issues/2760">#2760</a> by <a href="https://github.com/davidfiala"><code>@​davidfiala</code></a>)</li>
<li>Fix a bug causing unary response client requests to hang when unexpectedly receiving multiple messages (<a href="https://redirect.github.com/grpc/grpc-node/issues/2772">#2772</a>)</li>
<li>Fix a bug causing some requests to fail when making requests through a local proxy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2746">#2746</a> contributed by <a href="https://github.com/mjameswh"><code>@​mjameswh</code></a>, backported in <a href="https://redirect.github.com/grpc/grpc-node/issues/2777">#2777</a>)</li>
<li>Fix handling of URL-encoded user credentials in proxy configuration (<a href="https://redirect.github.com/grpc/grpc-node/issues/2761">#2761</a> contributed by <a href="https://github.com/brendan-myers"><code>@​brendan-myers</code></a>, backported in <a href="https://redirect.github.com/grpc/grpc-node/issues/2777">#2777</a>)</li>
<li>Fix missing client-side handling of the <code>grpc.max_send_message_length</code> channel option (<a href="https://redirect.github.com/grpc/grpc-node/issues/2779">#2779</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/c9342572aa0eaff181ec0fae34b73bb1b65cc75d"><code>c934257</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2778">#2778</a> from murgatroid99/grpc-js_1.10.10</li>
<li><a href="https://github.com/grpc/grpc-node/commit/3c55b5b7b577c0368dddd84a1c9435c0a14c0d98"><code>3c55b5b</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2777">#2777</a> from murgatroid99/grpc-js_1.10_backports</li>
<li><a href="https://github.com/grpc/grpc-node/commit/97c4cdac48c11135dbca94efe06470fb737c5980"><code>97c4cda</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2779">#2779</a> from murgatroid99/grpc-js_max_send_message_size_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/42844cffd2d5f27eb7dbac7b5da1dd05b3de5a95"><code>42844cf</code></a> grpc-js: Re-add client-side max send message size checking</li>
<li><a href="https://github.com/grpc/grpc-node/commit/cbab4e51cdecbc1cff1d27c46d29ae915c4554fb"><code>cbab4e5</code></a> grpc-js: Bump to 1.10.10</li>
<li><a href="https://github.com/grpc/grpc-node/commit/5ae551445452ccf1db1d4ed8f3890f6b0dfc0c35"><code>5ae5514</code></a> fix: add decoding for url encoded user credentials</li>
<li><a href="https://github.com/grpc/grpc-node/commit/e7590295327b1bbd6dae812cf45f4c5c5b181985"><code>e759029</code></a> HTTP CONNECT: handle early server packets</li>
<li><a href="https://github.com/grpc/grpc-node/commit/5c0226d0dbd55030f366a0597e2496e2a18d507a"><code>5c0226d</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2760">#2760</a> from davidfiala/@grpc/<a href="mailto:grpc-js@1.10.x">grpc-js@1.10.x</a></li>
<li><a href="https://github.com/grpc/grpc-node/commit/52fe8e94e7e31528b54f994bda97b7a969eb415f"><code>52fe8e9</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2772">#2772</a> from murgatroid99/grpc-js_cardinality_error_hang</li>
<li><a href="https://github.com/grpc/grpc-node/commit/98cd87f7512c95cd48bf04c3225f0fa22b5dcb78"><code>98cd87f</code></a> ensure that client keepalive timers are always cleared when they trigger. thi...</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.10.9...@grpc/grpc-js@1.10.10">compare view</a></li>
</ul>
</details>
<br />

Updates `bl` from 5.1.0 to 6.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/releases">bl's releases</a>.</em></p>
<blockquote>
<h2>v6.0.0</h2>
<h2><a href="https://github.com/rvagg/bl/compare/v5.1.0...v6.0.0">6.0.0</a> (2022-10-19)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li><strong>deps:</strong> bump readable-stream from 3.6.0 to 4.2.0</li>
<li>added bigint (Int64) support</li>
</ul>
<h3>Features</h3>
<ul>
<li>added bigint (Int64) support (<a href="https://github.com/rvagg/bl/commit/131ad3217b91090323513a8ea3ef179e8427cf47">131ad32</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>add TypeScript definitions for BigInt (<a href="https://github.com/rvagg/bl/commit/78c5ff489235a4e4233086c364133123c71acef4">78c5ff4</a>)</li>
<li><strong>deps-dev:</strong> bump typescript from 4.7.4 to 4.8.4 (<a href="https://github.com/rvagg/bl/commit/dba13e1cadc5857dde6a9425e975faf2abbb270f">dba13e1</a>)</li>
<li><strong>deps:</strong> bump readable-stream from 3.6.0 to 4.2.0 (<a href="https://github.com/rvagg/bl/commit/fa03eda54b4412c0fdfc9053bd0b0bebaf80bfd9">fa03eda</a>)</li>
<li><strong>docs:</strong> BigInt in API docs (<a href="https://github.com/rvagg/bl/commit/c68af500a04b2c3a14132ae6946412d2e39402d0">c68af50</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/blob/master/CHANGELOG.md">bl's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/rvagg/bl/compare/v5.1.0...v6.0.0">6.0.0</a> (2022-10-19)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li><strong>deps:</strong> bump readable-stream from 3.6.0 to 4.2.0</li>
<li>added bigint (Int64) support</li>
</ul>
<h3>Features</h3>
<ul>
<li>added bigint (Int64) support (<a href="https://github.com/rvagg/bl/commit/131ad3217b91090323513a8ea3ef179e8427cf47">131ad32</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>add TypeScript definitions for BigInt (<a href="https://github.com/rvagg/bl/commit/78c5ff489235a4e4233086c364133123c71acef4">78c5ff4</a>)</li>
<li><strong>deps-dev:</strong> bump typescript from 4.7.4 to 4.8.4 (<a href="https://github.com/rvagg/bl/commit/dba13e1cadc5857dde6a9425e975faf2abbb270f">dba13e1</a>)</li>
<li><strong>deps:</strong> bump readable-stream from 3.6.0 to 4.2.0 (<a href="https://github.com/rvagg/bl/commit/fa03eda54b4412c0fdfc9053bd0b0bebaf80bfd9">fa03eda</a>)</li>
<li><strong>docs:</strong> BigInt in API docs (<a href="https://github.com/rvagg/bl/commit/c68af500a04b2c3a14132ae6946412d2e39402d0">c68af50</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rvagg/bl/commit/a59710d5abddf33e7ed71963b9071d53926156aa"><code>a59710d</code></a> chore(release): 6.0.0 [skip ci]</li>
<li><a href="https://github.com/rvagg/bl/commit/dba13e1cadc5857dde6a9425e975faf2abbb270f"><code>dba13e1</code></a> chore(deps-dev): bump typescript from 4.7.4 to 4.8.4</li>
<li><a href="https://github.com/rvagg/bl/commit/c68af500a04b2c3a14132ae6946412d2e39402d0"><code>c68af50</code></a> chore(docs): BigInt in API docs</li>
<li><a href="https://github.com/rvagg/bl/commit/fa03eda54b4412c0fdfc9053bd0b0bebaf80bfd9"><code>fa03eda</code></a> chore(deps)!: bump readable-stream from 3.6.0 to 4.2.0</li>
<li><a href="https://github.com/rvagg/bl/commit/78c5ff489235a4e4233086c364133123c71acef4"><code>78c5ff4</code></a> chore: add TypeScript definitions for BigInt</li>
<li><a href="https://github.com/rvagg/bl/commit/131ad3217b91090323513a8ea3ef179e8427cf47"><code>131ad32</code></a> feat!: added bigint (Int64) support</li>
<li>See full diff in <a href="https://github.com/rvagg/bl/compare/v5.1.0...v6.0.0">compare view</a></li>
</ul>
</details>
<br />

Updates `qs` from 6.8.3 to 6.9.7
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.9.7</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://redirect.github.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li>Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
<li>[actions] backport actions from main</li>
<li>[Dev Deps] backport updates from main</li>
</ul>
<h2><strong>6.9.6</strong></h2>
<ul>
<li>[Fix] restore <code>dist</code> dir; mistakenly removed in d4f6c32</li>
</ul>
<h2><strong>6.9.5</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: do not encode parens for RFC1738</li>
<li>[Fix] <code>stringify</code>: fix arrayFormat comma with empty array/objects (<a href="https://redirect.github.com/ljharb/qs/issues/350">#350</a>)</li>
<li>[Refactor] <code>format</code>: remove <code>util.assign</code> call</li>
<li>[meta] add &quot;Allow Edits&quot; workflow; update rebase workflow</li>
<li>[actions] switch Automatic Rebase workflow to <code>pull_request_target</code> event</li>
<li>[Tests] <code>stringify</code>: add tests for <a href="https://redirect.github.com/ljharb/qs/issues/378">#378</a></li>
<li>[Tests] migrate tests to Github Actions</li>
<li>[Tests] run <code>nyc</code> on all tests; use <code>tape</code> runner</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>browserify</code>, <code>mkdirp</code>, <code>object-inspect</code>, <code>tape</code>; add <code>aud</code></li>
</ul>
<h2><strong>6.9.4</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: when <code>arrayFormat</code> is <code>comma</code>, respect <code>serializeDate</code> (<a href="https://redirect.github.com/ljharb/qs/issues/364">#364</a>)</li>
<li>[Refactor] <code>stringify</code>: reduce branching (part of <a href="https://redirect.github.com/ljharb/qs/issues/350">#350</a>)</li>
<li>[Refactor] move <code>maybeMap</code> to <code>utils</code></li>
<li>[Dev Deps] update <code>browserify</code>, <code>tape</code></li>
</ul>
<h2><strong>6.9.3</strong></h2>
<ul>
<li>[Fix] proper comma parsing of URL-encoded commas (<a href="https://redirect.github.com/ljharb/qs/issues/361">#361</a>)</li>
<li>[Fix] parses comma delimited array while having percent-encoded comma treated as normal text (<a href="https://redirect.github.com/ljharb/qs/issues/336">#336</a>)</li>
</ul>
<h2><strong>6.9.2</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: Fix parsing array from object with <code>comma</code> true (<a href="https://redirect.github.com/ljharb/qs/issues/359">#359</a>)</li>
<li>[Fix] <code>parse</code>: throw a TypeError instead of an Error for bad charset (<a href="https://redirect.github.com/ljharb/qs/issues/349">#349</a>)</li>
<li>[meta] ignore eclint transitive audit warning</li>
<li>[meta] fix indentation in package.json</li>
<li>[meta] add tidelift marketing copy</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>object-inspect</code>, <code>has-symbols</code>, <code>tape</code>, <code>mkdirp</code>, <code>iconv-lite</code></li>
<li>[actions] add automatic rebasing / merge commit blocking</li>
</ul>
<h2><strong>6.9.1</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: with comma true, handle field that holds an array of arrays (<a href="https://redirect.github.com/ljharb/qs/issues/335">#335</a>)</li>
<li>[Fix] <code>parse</code>: with comma true, do not split non-string values (<a href="https://redirect.github.com/ljharb/qs/issues/334">#334</a>)</li>
<li>[meta] add <code>funding</code> field</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/4cd003291fe3b347884f797e548b58a12150a0e3"><code>4cd0032</code></a> v6.9.7</li>
<li><a href="https://github.com/ljharb/qs/commit/e799ba57e573a30c14b67c1889c7c04d508b9105"><code>e799ba5</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/02ca358155297dc68fcc4c2ac312c26e10524e47"><code>02ca358</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/4a17709e71ae510a7195ff57b969a2bf9cde139f"><code>4a17709</code></a> [Fix] <code>stringify</code>: avoid encoding arrayformat comma when `encodeValuesOnly = ...</li>
<li><a href="https://github.com/ljharb/qs/commit/c0e13e9fc80aab01ef777cc06d7411c0df1676a7"><code>c0e13e9</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/4113a5f245987800ef2a8166f809a941661f1542"><code>4113a5f</code></a> [Tests] clean up stringify tests slightly</li>
<li><a href="https://github.com/ljharb/qs/commit/749a58467c1a28744de66d5193a1a19c079927e0"><code>749a584</code></a> [Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/cce2082f095b29903549ef43bddb509c5ba893c2"><code>cce2082</code></a> [meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/c44f0c59bb508ef22563ca07d9d3000c742fbee2"><code>c44f0c5</code></a> Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
<li><a href="https://github.com/ljharb/qs/commit/e6cfd8bda02143678f57a7eb441cca2183620dfc"><code>e6cfd8b</code></a> [actions] backport actions from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.8.3...v6.9.7">compare view</a></li>
</ul>
</details>
<br />

Updates `vite` from 5.1.7 to 5.2.6
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/releases">vite's releases</a>.</em></p>
<blockquote>
<h2>create-vite@5.2.3</h2>
<p>Please refer to <a href="https://github.com/vitejs/vite/blob/create-vite@5.2.3/packages/create-vite/CHANGELOG.md">CHANGELOG.md</a> for details.</p>
<h2>create-vite@5.2.2</h2>
<p>Please refer to <a href="https://github.com/vitejs/vite/blob/create-vite@5.2.2/packages/create-vite/CHANGELOG.md">CHANGELOG.md</a> for details.</p>
<h2>create-vite@5.2.1</h2>
<p>Please refer to <a href="https://github.com/vitejs/vite/blob/create-vite@5.2.1/packages/create-vite/CHANGELOG.md">CHANGELOG.md</a> for details.</p>
<h2>create-vite@5.2.0</h2>
<p>Please refer to <a href="https://github.com/vitejs/vite/blob/create-vite@5.2.0/packages/create-vite/CHANGELOG.md">CHANGELOG.md</a> for details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/main/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->5.2.6 (2024-03-24)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>) (<a href="https://github.com/vitejs/vite/commit/ba5269c">ba5269c</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16250">#16250</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.2.5 (2024-03-24)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: avoid SSR requests in waitForRequestIdle (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16246">#16246</a>) (<a href="https://github.com/vitejs/vite/commit/7093f77">7093f77</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16246">#16246</a></li>
<li>docs: clarify enforce vs hook.order (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16226">#16226</a>) (<a href="https://github.com/vitejs/vite/commit/3a73e48">3a73e48</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16226">#16226</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.2.4 (2024-03-23)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: dont resolve imports with malformed URI (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16244">#16244</a>) (<a href="https://github.com/vitejs/vite/commit/fbf69d5">fbf69d5</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16244">#16244</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.2.3 (2024-03-22)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: handle warmup request error correctly (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16223">#16223</a>) (<a href="https://github.com/vitejs/vite/commit/d7c5256">d7c5256</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16223">#16223</a></li>
<li>fix: skip encode if is data uri (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16233">#16233</a>) (<a href="https://github.com/vitejs/vite/commit/8617e76">8617e76</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16233">#16233</a></li>
<li>fix(optimizer): fix <code>optimizeDeps.include</code> glob syntax for <code>./*</code> exports (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16230">#16230</a>) (<a href="https://github.com/vitejs/vite/commit/f184c80">f184c80</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16230">#16230</a></li>
<li>fix(runtime): fix sourcemap with <code>prepareStackTrace</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16220">#16220</a>) (<a href="https://github.com/vitejs/vite/commit/dad7f4f">dad7f4f</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16220">#16220</a></li>
<li>chore: <code>utf8</code> replaced with <code>utf-8</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16232">#16232</a>) (<a href="https://github.com/vitejs/vite/commit/9800c73">9800c73</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16232">#16232</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.2.2 (2024-03-20)<!-- raw HTML omitted --></h2>
<ul>
<li>fix(importAnalysis): skip encode in ssr (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16213">#16213</a>) (<a href="https://github.com/vitejs/vite/commit/e4d2d60">e4d2d60</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16213">#16213</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.2.1 (2024-03-20)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: encode path uri only (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16212">#16212</a>) (<a href="https://github.com/vitejs/vite/commit/0b2e40b">0b2e40b</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16212">#16212</a></li>
</ul>
<h2>5.2.0 (2024-03-20)</h2>
<ul>
<li>fix: update client.ts@cleanUrl to accomodate blob protocol (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16182">#16182</a>) (<a href="https://github.com/vitejs/vite/commit/1a3b1d7">1a3b1d7</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16182">#16182</a></li>
<li>fix(assets): avoid splitting <code>,</code> inside query parameter of image URI in srcset property (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16081">#16081</a>) (<a href="https://github.com/vitejs/vite/commit/50caf67">50caf67</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16081">#16081</a></li>
<li>chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16186">#16186</a>) (<a href="https://github.com/vitejs/vite/commit/842643d">842643d</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16186">#16186</a></li>
<li>perf(transformRequest): fast-path watch and sourcemap handling (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16170">#16170</a>) (<a href="https://github.com/vitejs/vite/commit/de60f1e">de60f1e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16170">#16170</a></li>
<li>docs: add <code>@shikiji/vitepress-twoslash</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16168">#16168</a>) (<a href="https://github.com/vitejs/vite/commit/6f8a320">6f8a320</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16168">#16168</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/7369016d8a0f26ad9200cf7fd0e2045ca9fd1a41"><code>7369016</code></a> release: v5.2.6</li>
<li><a href="https://github.com/vitejs/vite/commit/ba5269cca81de3f5fbb0f49d58a1c55688043258"><code>ba5269c</code></a> fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/7a2791ce174933ae3afc29f596491cc0c67b9618"><code>7a2791c</code></a> release: v5.2.5</li>
<li><a href="https://github.com/vitejs/vite/commit/7093f779b7db2e0fdcb3f41affd76696b783a5fc"><code>7093f77</code></a> fix: avoid SSR requests in waitForRequestIdle (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16246">#16246</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/3a73e485cd4c08954fcb06698b5f721dea6e9f44"><code>3a73e48</code></a> docs: clarify enforce vs hook.order (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16226">#16226</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/6a07243a0ecc06a81e87d5b3de7b88023a045e6b"><code>6a07243</code></a> release: v5.2.4</li>
<li><a href="https://github.com/vitejs/vite/commit/fbf69d5f6cef335fc18640fed7da16593b13c9b3"><code>fbf69d5</code></a> fix: dont resolve imports with malformed URI (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16244">#16244</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/a67f9f69456439baa727823ac604a68f7279b3bb"><code>a67f9f6</code></a> release: v5.2.3</li>
<li><a href="https://github.com/vitejs/vite/commit/8617e7638ec105c7a6019a7ebac3b3185297b90d"><code>8617e76</code></a> fix: skip encode if is data uri (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16233">#16233</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/f184c8032bec6e668265a98d254a442e1024b6f3"><code>f184c80</code></a> fix(optimizer): fix <code>optimizeDeps.include</code> glob syntax for <code>./*</code> exports (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16">#16</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/vitejs/vite/commits/v5.2.6/packages/vite">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-25 00:30:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3358" class=".btn">#3358</a>
            </td>
            <td>
                <b>
                    test(weaver-fabric-examples): use docker compose v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the weaver fabric example network.sh file to use docker compose v2 syntax.  docker-compose
v1 will be dropped on the github runners in a few weeks. (ref: https://github.com/actions/runner-images/blob/main/images/ubuntu/Ubuntu2204-Readme.md)

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 14:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3357" class=".btn">#3357</a>
            </td>
            <td>
                <b>
                    feat(connector-corda): add initial set of JvmObject factory functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. These functions are used so more easily construct the JSON representation
of JVM objects (references and primitive values) that we need to define when
interacting with the Corda JVM connector (which is used for Corda v4 ledgers)
2. This is not a comprehensive set but more like a trailblazing initial
implementation to showcase how to create and use these factory functions.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-22 06:55:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3356" class=".btn">#3356</a>
            </td>
            <td>
                <b>
                    build(deps): upgrade Yarn to v4.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quality of life improvement and some minor performance improvements in the
new version from what I understood.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 23:35:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3355" class=".btn">#3355</a>
            </td>
            <td>
                <b>
                    test(test-tooling: add negotiation-cordapp support from kotlin-samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This way we can have examples and test cases developed that use either
the negotiation or the obligation cordapps. Earlier we could only use
the obligation cordapp as it was the hardcoded directory path for contract
deployments.
2. Not an actual feature just an extension to the testing infrastructure
that we have and we need the additional possibilities here because of the
new Harmonia Labs examples coming up.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 22:34:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3354" class=".btn">#3354</a>
            </td>
            <td>
                <b>
                    build(devcontainer): upgrade docker engine to v26.x.y in the image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This will help us with newer features and also potential CVEs in the
(now) quite outdated version we were using before.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 19:00:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3353" class=".btn">#3353</a>
            </td>
            <td>
                <b>
                    chore(docs): add openapi specs to docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create project documentation reference page of all open api specs produced by monorepo projects.

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 18:43:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3352" class=".btn">#3352</a>
            </td>
            <td>
                <b>
                    test(connector-corda): fix deploy-cordapp-jars-to-nodes-v4.8-express
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Upgrading the images that were being used made it so that now the test
is no longer flaky/broken (or at least that's what a series of executions
of it made it looked like on my local machine)
2. Based on the above it might be worthwhile to put this test back into the
ones that are running (previously it was marked to be skipped).
3. We should keep an eye on it to make sure it's not flaky on the CI either
(which has resources much more constrained than my local development machine)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 18:39:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3351" class=".btn">#3351</a>
            </td>
            <td>
                <b>
                    feat(connector-corda): add JSON classname->JVM class object deserialize
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This allows the API clients to specify a class name from which the backend
will retrieve the JVM Class<?> object.
2. It is very simple under the hood it just uses `Class.forName(x)`
3. It is needed to be able to do this because when passing in flow parameters
sometimes the arguments are Class<?> objects and so this was a feature gap.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 18:26:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3350" class=".btn">#3350</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): expose API client and OpenAPI code for web builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. We were only exporting the API client and the related data model type
definitions for NodeJS builds but not for the web.
2. This made it so that you couldn't import/use the Besu API client from
a front-end application such as Angular or React.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 17:46:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3349" class=".btn">#3349</a>
            </td>
            <td>
                <b>
                    build(typescript): upgrade compiler to v5.5.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Brings in size and performance improvements.
2. Also adds support for some new features such as Ecmascript setters

https://www.infoworld.com/article/3715246/typescript-adds-support-for-ecmascripts-set-methods.html

Fixes #3326

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 16:48:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3348" class=".btn">#3348</a>
            </td>
            <td>
                <b>
                    ci(cacti) - Proof of concept using lerna in matrix job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proof of concept to demonstrate a matrix test job which can be used for all cacti packages.

Intention is to simplify monorepo ci by pushing package logic to the individual packages and make use of the lerna toolset to identify changes and run a shared set of lifecycle targets defined in the package, for instance:

 - test
 - build-docker
 - deploy
 - etc

This way, CI can be agnostic to the internals of each package, simplifying logic considerably and ensuring new packages do not further complicate CI.  

The existing ci.yaml file can be refactored via a script to ensure no changes are lost, please see included parsing file for an example python script which (for now) just reports which jobs are redundant.  This script can be a base for pushing logic to the component packages by adding commands to the package.json.  The 80+ ci.yaml file jobs really follow only 5 or 6 basic patterns which can be handled by parsing.

Since the branch is a proof of concept and not for commit, the pull request requirements are ignored.  

Please see here for an example output CI:
https://github.com/jenniferlianne/cacti/actions/runs/9615156170



**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 15:22:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3347" class=".btn">#3347</a>
            </td>
            <td>
                <b>
                    feat(persistence-ethereum): migrate to separate db schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Move all database entities relating to ethereum persistence plugin to
  a seprate schema. Adjust all the files the test to work as expected after
  that change.
- Remove sample SQL data from GUI package, one from persistence packages should
  be used instead.
- Add `sample-persistence-plugin-setup` script for performing end-to-end tests
  of the persistence ethereum plugin.
- Upgrade web3-utils in persistence-ethereum to fix a bug when running the
  standalone script.

Depends on #3340

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 13:20:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3346" class=".btn">#3346</a>
            </td>
            <td>
                <b>
                    ci(custom-checks): fix depcheck not detecting missing dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The depcheck tool we use have not correctly discovered some of the
missing dependencies that we have because it only verifies that the
imported dependency is present SOMEwhere in the package.json file, not that
it is specifically present in the production dependencies section which
leads to crashes and broken packages due to the API server not installing
dev dependencies when instantiating a plugin and therefore missing a few
of the dependencies that are otherwise very much needed at runtime in
production.
2. The solution to the problem was to implement our own typescript parsing
with babel and then double check the work of depcheck to make sure that
the dependencies that it marks as "no issues" are actually OK and have no
issues.
3. The hardest edge case was type imports e.g. `import type { Express } from "express";`
because the import was there, but we did not actually need that dependency
in the production dependencies as long as ALL of the imports to it in the
given package were type imports. To robustly verify this being the case or not
we had to pull out the big guns and parse all the typescript code per package
to make sure that we've looked at every single import of the dependency in
question at every single code file of the package in question.

Depends on #3345

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 01:28:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3345" class=".btn">#3345</a>
            </td>
            <td>
                <b>
                    fix(deps): fix batch of missing production dependencies v2.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Huge diff, simple changes:
1. Where applicable, I added `import type {..}` instead of `import {...}`
so that we do not need the dependency in the production dependencies.
2. For imports where the code imported was actually used at runtime I
altered the package.json file so that the dependency is marked as a production
dependency and therefore won't crash anymore when being imported in isolation
(e.g. outside of the mono-repo dev build).

Fixes #3344

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [X] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [X] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [X] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [X] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [X] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 01:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3343" class=".btn">#3343</a>
            </td>
            <td>
                <b>
                    ci: fix weaver nodejs publish ignore local .npmrc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the issue identified in previous release, here is the error log screenshot, where it was ignoring local `.npmrc` required for publishing, and then later on `npm publish` is unable to authenticate:
<img width="1154" alt="Screenshot 2024-06-21 at 1 31 25 AM" src="https://github.com/hyperledger/cacti/assets/17192099/293d76fa-2eaf-4685-8324-3109495c56bd">
<img width="933" alt="Screenshot 2024-06-21 at 1 43 51 AM" src="https://github.com/hyperledger/cacti/assets/17192099/07f870e9-efd9-416f-b6ee-8ee2d83b8ffd">


**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 20:04:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3342" class=".btn">#3342</a>
            </td>
            <td>
                <b>
                    feat(tcs-huawei-socketio): remove deprecated connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove `cactus-plugin-ledger-connector-tcs-huawei-socketio` connector and any reference to it.
- This is not permanent - we'd love to bring the package back once the necessary refactors are done!
- See issue #3155 on github for more details on context and reasoning of this decision.

Part of #3155

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 15:59:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3341" class=".btn">#3341</a>
            </td>
            <td>
                <b>
                    feat(go-ethereum-socketio): remove deprecated connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove `cactus-plugin-ledger-connector-go-ethereum-socketio` connector and any reference to it.
- Remove `SocketIOApiClient` from `cactus-api-client` since it is the last connector that was linked to it.
- Remove `legacy-socketio` option from `cactus-verifier-client`.

Part of #3155

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 15:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3340" class=".btn">#3340</a>
            </td>
            <td>
                <b>
                    feat(ledger-browser): refactor home page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Remove status apps, its functionality has been moved to the home page.
- Add status components for persistence apps.
- Add home page that contains cards for each configured app. Clicking on it
  naviagtes to specific app, clicking on Status button shows status component.
- Remove app drawer, replace it with a button that navigates to root path 
  (i.e. the home app, navigation between apps is handled here).
- Remove all the remaining dead and legacy code, apply small structure upgrades.
- Since this PR removes all old code, and all the current code was written by
  me and Tomasz, I've also removed previous inactive package contributors.

Depends on #3320

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 14:35:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    fix(go-sdk): use protos v1 api for fabric-protos-go unmarshal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    - ci(release-go-sdk): use make build to test build of go-sdk
    - chore: fix update-weaver-version script typo with quotes
    - chore: bug fix in release script go-gen-checksum

Previous release of `weaver-go-sdk` failed because of a bug in CI.
Also fixed the script `go-gen-checksum` identified in previous release and tested it on Ubuntu and Mac both.

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 08:32:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3338" class=".btn">#3338</a>
            </td>
            <td>
                <b>
                    feat(connector): remove hard dependency on keychain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Commit to be reviewed

feat(connector): remove hard dependency on keychain

    Primary Changes
    ---------------
    1. Updated besu connector to remove hard
       dependency on keychain

    Changes required to incorporate 1)
    2. Updated openapi.json file of the above mentioned connectors
       to include the new no-keychain endpoints
    3. Generated code and updated related web-services for the same

Fixes #963

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 07:22:52 +0000 UTC
    </div>
</div>

