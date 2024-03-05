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
                PR <a href="https://github.com/hyperledger/cacti/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    docs(build): change NodeJS version in BUILD.md to v18.18.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix node version in BUILD.md what caused type error in corepack
and prevented yarn from installing packages correctly.
Error message when using node 16: Type Error: URL.canParse is not a function

Signed-off-by: Tomasz Awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 14:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    test(cbdc-example): removed dependency on chai and update tests
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

