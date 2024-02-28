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
                PR <a href="https://github.com/hyperledger/cacti/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    fix(cbdc-example): removed dependency on chai and update tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Chai was removed as dependency of the cbdc-backend package
* A test scenario was removed in the 'bridge-back' feature due to having duplicated logic with another one in the same file
* Some tests were failing due to timeouts, so we added an explicit and generous timeout limit for each step

closes #3034
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 17:07:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3033" class=".btn">#3033</a>
            </td>
            <td>
                <b>
                    chore: make spellcheck script less noisy with --no-progress flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A quality of life improvement for contributors.

Prior to this the cspell tool that we invoke for spellchecking had listed every single file as a separate log line on standard output during it's execution and the files that had issues were marked in that list, but since we have more than a thousand files, it was a lot of scrolling and scanning to find the files that had spelling mistakes in them during development time.

With the `--no-progress` flag now passed in to cspell it will only print the files that were found to have spelling mistakes in them which makes contributor productivity a little better.

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
        Created At 2024-02-28 01:54:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3032" class=".btn">#3032</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump axios from 0.22.0 to 1.6.0 in /packages/cactus-plugin-ledger-connector-polkadot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.22.0 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v0.28.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li>fix(security): fixed CVE-2023-45857 by backporting <code>withXSRFToken</code> option to v0.x (<a href="https://redirect.github.com/axios/axios/issues/6091">#6091</a>)</li>
</ul>
<h3>Backports from v1.x:</h3>
<ul>
<li>Allow null indexes on formSerializer and paramsSerializer v0.x (<a href="https://redirect.github.com/axios/axios/issues/4961">#4961</a>)</li>
<li>Fixing content-type header repeated <a href="https://redirect.github.com/axios/axios/issues/4745">#4745</a></li>
<li>Fixed timeout error message for HTTP 4738</li>
<li>Added <code>axios.formToJSON</code> method (<a href="https://redirect.github.com/axios/axios/issues/4735">#4735</a>)</li>
<li>URL params serializer (<a href="https://redirect.github.com/axios/axios/issues/4734">#4734</a>)</li>
<li>Fixed toFormData Blob issue on node&gt;v17 <a href="https://redirect.github.com/axios/axios/issues/4728">#4728</a></li>
<li>Adding types for progress event callbacks <a href="https://redirect.github.com/axios/axios/issues/4675">#4675</a></li>
<li>Fixed max body length defaults <a href="https://redirect.github.com/axios/axios/issues/4731">#4731</a></li>
<li>Added data URL support for node.js (<a href="https://redirect.github.com/axios/axios/issues/4725">#4725</a>)</li>
<li>Added isCancel type assert (<a href="https://redirect.github.com/axios/axios/issues/4293">#4293</a>)</li>
<li>Added the ability for the <code>url-encoded-form</code> serializer to respect the <code>formSerializer</code> config (<a href="https://redirect.github.com/axios/axios/issues/4721">#4721</a>)</li>
<li>Add <code>string[]</code> to <code>AxiosRequestHeaders</code> type (<a href="https://redirect.github.com/axios/axios/issues/4322">#4322</a>)</li>
<li>Allow type definition for axios instance methods (<a href="https://redirect.github.com/axios/axios/issues/4224">#4224</a>)</li>
<li>Fixed <code>AxiosError</code> stack capturing; (<a href="https://redirect.github.com/axios/axios/issues/4718">#4718</a>)</li>
<li>Fixed <code>AxiosError</code> status code type; (<a href="https://redirect.github.com/axios/axios/issues/4717">#4717</a>)</li>
<li>Adding Canceler parameters config and request (<a href="https://redirect.github.com/axios/axios/issues/4711">#4711</a>)</li>
<li>fix(types): allow to specify partial default headers for instance creation (<a href="https://redirect.github.com/axios/axios/issues/4185">#4185</a>)</li>
<li>Added <code>blob</code> to the list of protocols supported by the browser (<a href="https://redirect.github.com/axios/axios/issues/4678">#4678</a>)</li>
<li>Fixing Z_BUF_ERROR when no content (<a href="https://redirect.github.com/axios/axios/issues/4701">#4701</a>)</li>
<li>Fixed race condition on immediate requests cancellation (<a href="https://redirect.github.com/axios/axios/issues/4261">#4261</a>)</li>
<li>Added a clear() function to the request and response interceptors object so a user can ensure that all interceptors have been removed from an Axios instance <a href="https://redirect.github.com/axios/axios/pull/4248">axios/axios#4248</a></li>
<li>Added generic AxiosAbortSignal TS interface to avoid importing AbortController polyfill (<a href="https://redirect.github.com/axios/axios/issues/4229">#4229</a>)</li>
<li>Fix TS definition for AxiosRequestTransformer (<a href="https://redirect.github.com/axios/axios/issues/4201">#4201</a>)</li>
<li>Use type alias instead of interface for AxiosPromise (<a href="https://redirect.github.com/axios/axios/issues/4505">#4505</a>)</li>
<li>Include request and config when creating a CanceledError instance (<a href="https://redirect.github.com/axios/axios/issues/4659">#4659</a>)</li>
<li>Added generic TS types for the exposed toFormData helper (<a href="https://redirect.github.com/axios/axios/issues/4668">#4668</a>)</li>
<li>Optimized the code that checks cancellation (<a href="https://redirect.github.com/axios/axios/issues/4587">#4587</a>)</li>
<li>Replaced webpack with rollup (<a href="https://redirect.github.com/axios/axios/issues/4596">#4596</a>)</li>
<li>Added stack trace to AxiosError (<a href="https://redirect.github.com/axios/axios/issues/4624">#4624</a>)</li>
<li>Updated AxiosError.config to be optional in the type definition (<a href="https://redirect.github.com/axios/axios/issues/4665">#4665</a>)</li>
<li>Removed incorrect argument for NetworkError constructor (<a href="https://redirect.github.com/axios/axios/issues/4656">#4656</a>)</li>
</ul>
<h2>v0.27.2</h2>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed FormData posting in browser environment by reverting <a href="https://redirect.github.com/axios/axios/issues/3785">#3785</a> (<a href="https://redirect.github.com/axios/axios/pull/4640">#4640</a>)</li>
<li>Enhanced protocol parsing implementation (<a href="https://redirect.github.com/axios/axios/pull/4639">#4639</a>)</li>
<li>Fixed bundle size</li>
</ul>
<h2>v0.27.1</h2>
<h3>Fixes and Functionality:</h3>
<ul>
<li>Removed import of url module in browser build due to huge size overhead and builds being broken (<a href="https://redirect.github.com/axios/axios/pull/4594">#4594</a>)</li>
<li>Bumped follow-redirects to ^1.14.9 (<a href="https://redirect.github.com/axios/axios/pull/4615">#4615</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v0.28.0/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/axios/axios/compare/v0.27.2...v0.28.0">0.28.0</a> (2024-02-12)</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li>fix(security): fixed CVE-2023-45857 by backporting <code>withXSRFToken</code> option to v0.x (<a href="https://redirect.github.com/axios/axios/issues/6091">#6091</a>)</li>
</ul>
<h3>Backports from v1.x:</h3>
<ul>
<li>Allow null indexes on formSerializer and paramsSerializer v0.x (<a href="https://redirect.github.com/axios/axios/issues/4961">#4961</a>)</li>
<li>Fixing content-type header repeated <a href="https://redirect.github.com/axios/axios/issues/4745">#4745</a></li>
<li>Fixed timeout error message for HTTP 4738</li>
<li>Added <code>axios.formToJSON</code> method (<a href="https://redirect.github.com/axios/axios/issues/4735">#4735</a>)</li>
<li>URL params serializer (<a href="https://redirect.github.com/axios/axios/issues/4734">#4734</a>)</li>
<li>Fixed toFormData Blob issue on node&gt;v17 <a href="https://redirect.github.com/axios/axios/issues/4728">#4728</a></li>
<li>Adding types for progress event callbacks <a href="https://redirect.github.com/axios/axios/issues/4675">#4675</a></li>
<li>Fixed max body length defaults <a href="https://redirect.github.com/axios/axios/issues/4731">#4731</a></li>
<li>Added data URL support for node.js (<a href="https://redirect.github.com/axios/axios/issues/4725">#4725</a>)</li>
<li>Added isCancel type assert (<a href="https://redirect.github.com/axios/axios/issues/4293">#4293</a>)</li>
<li>Added the ability for the <code>url-encoded-form</code> serializer to respect the <code>formSerializer</code> config (<a href="https://redirect.github.com/axios/axios/issues/4721">#4721</a>)</li>
<li>Add <code>string[]</code> to <code>AxiosRequestHeaders</code> type (<a href="https://redirect.github.com/axios/axios/issues/4322">#4322</a>)</li>
<li>Allow type definition for axios instance methods (<a href="https://redirect.github.com/axios/axios/issues/4224">#4224</a>)</li>
<li>Fixed <code>AxiosError</code> stack capturing; (<a href="https://redirect.github.com/axios/axios/issues/4718">#4718</a>)</li>
<li>Fixed <code>AxiosError</code> status code type; (<a href="https://redirect.github.com/axios/axios/issues/4717">#4717</a>)</li>
<li>Adding Canceler parameters config and request (<a href="https://redirect.github.com/axios/axios/issues/4711">#4711</a>)</li>
<li>fix(types): allow to specify partial default headers for instance creation (<a href="https://redirect.github.com/axios/axios/issues/4185">#4185</a>)</li>
<li>Added <code>blob</code> to the list of protocols supported by the browser (<a href="https://redirect.github.com/axios/axios/issues/4678">#4678</a>)</li>
<li>Fixing Z_BUF_ERROR when no content (<a href="https://redirect.github.com/axios/axios/issues/4701">#4701</a>)</li>
<li>Fixed race condition on immediate requests cancellation (<a href="https://redirect.github.com/axios/axios/issues/4261">#4261</a>)</li>
<li>Added a clear() function to the request and response interceptors object so a user can ensure that all interceptors have been removed from an Axios instance <a href="https://redirect.github.com/axios/axios/pull/4248">axios/axios#4248</a></li>
<li>Added generic AxiosAbortSignal TS interface to avoid importing AbortController polyfill (<a href="https://redirect.github.com/axios/axios/issues/4229">#4229</a>)</li>
<li>Fix TS definition for AxiosRequestTransformer (<a href="https://redirect.github.com/axios/axios/issues/4201">#4201</a>)</li>
<li>Use type alias instead of interface for AxiosPromise (<a href="https://redirect.github.com/axios/axios/issues/4505">#4505</a>)</li>
<li>Include request and config when creating a CanceledError instance (<a href="https://redirect.github.com/axios/axios/issues/4659">#4659</a>)</li>
<li>Added generic TS types for the exposed toFormData helper (<a href="https://redirect.github.com/axios/axios/issues/4668">#4668</a>)</li>
<li>Optimized the code that checks cancellation (<a href="https://redirect.github.com/axios/axios/issues/4587">#4587</a>)</li>
<li>Replaced webpack with rollup (<a href="https://redirect.github.com/axios/axios/issues/4596">#4596</a>)</li>
<li>Added stack trace to AxiosError (<a href="https://redirect.github.com/axios/axios/issues/4624">#4624</a>)</li>
<li>Updated AxiosError.config to be optional in the type definition (<a href="https://redirect.github.com/axios/axios/issues/4665">#4665</a>)</li>
<li>Removed incorrect argument for NetworkError constructor (<a href="https://redirect.github.com/axios/axios/issues/4656">#4656</a>)</li>
</ul>
<h2>0.27.2 (April 27, 2022)</h2>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed FormData posting in browser environment by reverting <a href="https://redirect.github.com/axios/axios/issues/3785">#3785</a> (<a href="https://redirect.github.com/axios/axios/pull/4640">#4640</a>)</li>
<li>Enhanced protocol parsing implementation (<a href="https://redirect.github.com/axios/axios/pull/4639">#4639</a>)</li>
<li>Fixed bundle size</li>
</ul>
<h2>0.27.1 (April 26, 2022)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/3b7635aefc842c05da0ec8c90e8bd09cb54616b8"><code>3b7635a</code></a> [Release] v0.28.0 (<a href="https://redirect.github.com/axios/axios/issues/6211">#6211</a>)</li>
<li><a href="https://github.com/axios/axios/commit/27c007656d8d7ffe780248edc531949d744450b7"><code>27c0076</code></a> feat(backport): added ability for paramsSerializer to handle function; (<a href="https://redirect.github.com/axios/axios/issues/6227">#6227</a>)</li>
<li><a href="https://github.com/axios/axios/commit/80c3d74544197e83ee268b24f9cc1428e04d766c"><code>80c3d74</code></a> chore(ci): backported publish action; (<a href="https://redirect.github.com/axios/axios/issues/6224">#6224</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2755df562b9c194fba6d8b609a383443f6a6e967"><code>2755df5</code></a> fix(security): fixed CVE-2023-45857 by backporting <code>withXSRFToken</code> option to ...</li>
<li><a href="https://github.com/axios/axios/commit/880b42e2b8cdd467ce0c6ecd1cf522ef6ef65682"><code>880b42e</code></a> docs: Fix a typo in README</li>
<li><a href="https://github.com/axios/axios/commit/c4bf0a4afcac9a49e9b58d3ea64570110cba34f8"><code>c4bf0a4</code></a> Allow null indexes on formSerializer and paramsSerializer v0.x (<a href="https://redirect.github.com/axios/axios/issues/4961">#4961</a>)</li>
<li><a href="https://github.com/axios/axios/commit/1e2679f75b2030dd62c661e3292ab265c89497b8"><code>1e2679f</code></a> fix: [Types] Type of header in AxiosRequestConfig / for Axios.create is incor...</li>
<li><a href="https://github.com/axios/axios/commit/80b546c3f1982852aa0047dac5ddde38426e25cb"><code>80b546c</code></a> fix: loosing request header (<a href="https://redirect.github.com/axios/axios/issues/4858">#4858</a>) (<a href="https://redirect.github.com/axios/axios/issues/4871">#4871</a>)</li>
<li><a href="https://github.com/axios/axios/commit/6acb5ef8ff127db65da85189b3ccaeb10b93121a"><code>6acb5ef</code></a> feat: brower platform add data protocol. (<a href="https://redirect.github.com/axios/axios/issues/4814">#4814</a>)</li>
<li><a href="https://github.com/axios/axios/commit/bbb2264614befdce107449baa8a3102d9043a527"><code>bbb2264</code></a> fix(typing): axios response headers can be undefined (<a href="https://redirect.github.com/axios/axios/issues/4813">#4813</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.22.0...v0.28.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.22.0&new-version=0.28.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-27 21:31:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3031" class=".btn">#3031</a>
            </td>
            <td>
                <b>
                    test(test-tooling): fix FabricTestLedger INVALID_ENDORSER_TRANSACTION
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * reverts changes of commit 3371772c582389f6ee0c6fb66af875dd93cc94c6,
which seems to be breaking the Fabric Test Ledger

Results of further investigation into the root cause done by Peter:
1. The URLs we specify have the `grpcs://` protocol specified meaning that
TLS is used for securing the connection.
2. Certificates that are generated by the Fabric-provided boostrap scripts
when setting up crypto materials for the ledger are generated with `localhost`
as the hostname instead of the IP address of localhost.
3. The C++ gRPC implementation does not support mixing IP addresses and
hostnames when it comes to connections that are using TLS, e.g. if the
certificate we are using was made out for `localhost` then it won't work
for `127.0.0.1` even though technically from our perspective they meaning
the same thing (do note however that technically localhost could be set
up to resolve to something other than 127.0.0.1 in a DNS server so the 
difference is meaningful).

Source: https://github.com/grpc/grpc/issues/2691

closes #3009

Co-authored-by: Peter Somogyvari <peter.somogyvari@accenture.com>

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 17:33:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3030" class=".btn">#3030</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump vite from 5.0.8 to 5.0.12 in /packages/cacti-ledger-browser-react
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite) from 5.0.8 to 5.0.12.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/v5.0.12/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->5.0.12 (2024-01-19)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: await <code>configResolved</code> hooks of worker plugins (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15597">#15597</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15605">#15605</a>) (<a href="https://github.com/vitejs/vite/commit/ef89f80">ef89f80</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15597">#15597</a> <a href="https://redirect.github.com/vitejs/vite/issues/15605">#15605</a></li>
<li>fix: fs deny for case insensitive systems (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15653">#15653</a>) (<a href="https://github.com/vitejs/vite/commit/91641c4">91641c4</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15653">#15653</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.0.11 (2024-01-05)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: don't pretransform classic script links (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15361">#15361</a>) (<a href="https://github.com/vitejs/vite/commit/19e3c9a">19e3c9a</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15361">#15361</a></li>
<li>fix: inject <code>__vite__mapDeps</code> code before sourcemap file comment (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15483">#15483</a>) (<a href="https://github.com/vitejs/vite/commit/d2aa096">d2aa096</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15483">#15483</a></li>
<li>fix(assets): avoid splitting <code>,</code> inside base64 value of <code>srcset</code> attribute (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15422">#15422</a>) (<a href="https://github.com/vitejs/vite/commit/8de7bd2">8de7bd2</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15422">#15422</a></li>
<li>fix(html): handle offset magic-string slice error (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15435">#15435</a>) (<a href="https://github.com/vitejs/vite/commit/5ea9edb">5ea9edb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15435">#15435</a></li>
<li>chore(deps): update dependency strip-literal to v2 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15475">#15475</a>) (<a href="https://github.com/vitejs/vite/commit/49d21fe">49d21fe</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15475">#15475</a></li>
<li>chore(deps): update tj-actions/changed-files action to v41 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15476">#15476</a>) (<a href="https://github.com/vitejs/vite/commit/2a540ee">2a540ee</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15476">#15476</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.0.10 (2023-12-15)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: omit protocol does not require pre-transform (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15355">#15355</a>) (<a href="https://github.com/vitejs/vite/commit/d9ae1b2">d9ae1b2</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15355">#15355</a></li>
<li>fix(build): use base64 for inline SVG if it contains both single and double quotes (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15271">#15271</a>) (<a href="https://github.com/vitejs/vite/commit/1bbff16">1bbff16</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15271">#15271</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.0.9 (2023-12-14)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: htmlFallbackMiddleware for favicon (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15301">#15301</a>) (<a href="https://github.com/vitejs/vite/commit/c902545">c902545</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15301">#15301</a></li>
<li>fix: more stable hash calculation for depsOptimize (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15337">#15337</a>) (<a href="https://github.com/vitejs/vite/commit/2b39fe6">2b39fe6</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15337">#15337</a></li>
<li>fix(scanner): catch all external files for glob imports (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15286">#15286</a>) (<a href="https://github.com/vitejs/vite/commit/129d0d0">129d0d0</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15286">#15286</a></li>
<li>fix(server): avoid chokidar throttling on startup (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15347">#15347</a>) (<a href="https://github.com/vitejs/vite/commit/56a5740">56a5740</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15347">#15347</a></li>
<li>fix(worker): replace <code>import.meta</code> correctly for IIFE worker (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15321">#15321</a>) (<a href="https://github.com/vitejs/vite/commit/08d093c">08d093c</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15321">#15321</a></li>
<li>feat: log re-optimization reasons (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15339">#15339</a>) (<a href="https://github.com/vitejs/vite/commit/b1a6c84">b1a6c84</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15339">#15339</a></li>
<li>chore: temporary typo (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15329">#15329</a>) (<a href="https://github.com/vitejs/vite/commit/7b71854">7b71854</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15329">#15329</a></li>
<li>perf: avoid computing paths on each request (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15318">#15318</a>) (<a href="https://github.com/vitejs/vite/commit/0506812">0506812</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15318">#15318</a></li>
<li>perf: temporary hack to avoid fs checks for /<a href="https://github.com/react-refresh"><code>@​react-refresh</code></a> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15299">#15299</a>) (<a href="https://github.com/vitejs/vite/commit/b1d6211">b1d6211</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15299">#15299</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/ee81e196769c102a6b1bf30f8444ccde236e71d5"><code>ee81e19</code></a> release: v5.0.12</li>
<li><a href="https://github.com/vitejs/vite/commit/91641c4da0a011d4c5352e88fc68389d4e1289a5"><code>91641c4</code></a> fix: fs deny for case insensitive systems (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15653">#15653</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/ef89f8092f0eb1d8fd7d21256e6af8c4e64fe9b2"><code>ef89f80</code></a> fix: await <code>configResolved</code> hooks of worker plugins (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15597">#15597</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15605">#15605</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/b44c49302ffbf0c82f984f6219ed6376d1e4552a"><code>b44c493</code></a> release: v5.0.11</li>
<li><a href="https://github.com/vitejs/vite/commit/d2aa0969ee316000d3b957d7e879f001e85e369e"><code>d2aa096</code></a> fix: inject <code>__vite__mapDeps</code> code before sourcemap file comment (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15483">#15483</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/2a540eee82f9a31deff8215bdbdccfa46d494a06"><code>2a540ee</code></a> chore(deps): update tj-actions/changed-files action to v41 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15476">#15476</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/5ea9edbc9ceb991e85f893fe62d68ed028677451"><code>5ea9edb</code></a> fix(html): handle offset magic-string slice error (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15435">#15435</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/49d21fe1feaac30dee0196bd484480a8000a4363"><code>49d21fe</code></a> chore(deps): update dependency strip-literal to v2 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15475">#15475</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/8de7bd2b68db27b83d9484cc8d4e26436615168e"><code>8de7bd2</code></a> fix(assets): avoid splitting <code>,</code> inside base64 value of <code>srcset</code> attribute (#...</li>
<li><a href="https://github.com/vitejs/vite/commit/19e3c9a8a16847486fbad8a8cd48fc771b1538bb"><code>19e3c9a</code></a> fix: don't pretransform classic script links (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15361">#15361</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vitejs/vite/commits/v5.0.12/packages/vite">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=vite&package-manager=npm_and_yarn&previous-version=5.0.8&new-version=5.0.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-24 02:28:37 +0000 UTC
    </div>
</div>

