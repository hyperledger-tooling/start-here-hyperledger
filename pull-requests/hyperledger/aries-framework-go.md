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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3201" class=".btn">#3201</a>
            </td>
            <td>
                <b>
                    feat: add support for ed25519signature2020
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 09:51:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3200" class=".btn">#3200</a>
            </td>
            <td>
                <b>
                    chore(deps): bump axios from 0.23.0 to 0.26.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.23.0 to 0.26.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>v0.26.1</h2>
<h3>0.26.1 (March 9, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Refactored project file structure to avoid circular imports ([#<a href="https://github-redirect.dependabot.com/axios/axios/issues/4220">#4220</a>](<a href="https://github-redirect.dependabot.com/axios/axios/pull/%5B#4220%5D(https://github-redirect.dependabot.com/axios/axios/issues/4220)">axios/axios#4220</a>))</li>
</ul>
<h2>v0.26.0</h2>
<h3>0.26.0 (February 13, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed The timeoutErrorMessage property in config not work with Node.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3581">#3581</a>)</li>
<li>Added errors to be displayed when the query parsing process itself fails (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3961">#3961</a>)</li>
<li>Fix/remove url required (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4426">#4426</a>)</li>
<li>Update follow-redirects dependency due to Vulnerability (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4462">#4462</a>)</li>
<li>Bump karma from 6.3.11 to 6.3.14 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4461">#4461</a>)</li>
<li>Bump follow-redirects from 1.14.7 to 1.14.8 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4473">#4473</a>)</li>
</ul>
<h2>v0.25.0</h2>
<h3>0.25.0 (January 18, 2022)</h3>
<p>Breaking changes:</p>
<ul>
<li>Fixing maxBodyLength enforcement (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Don't rely on strict mode behaviour for arguments (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3470">#3470</a>)</li>
<li>Adding error handling when missing url (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3791">#3791</a>)</li>
<li>Update isAbsoluteURL.js removing escaping of non-special characters (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3809">#3809</a>)</li>
<li>Use native Array.isArray() in utils.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3836">#3836</a>)</li>
<li>Adding error handling inside stream end callback (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3967">#3967</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Added aborted even handler (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3916">#3916</a>)</li>
<li>Header types expanded allowing <code>boolean</code> and <code>number</code> types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4144">#4144</a>)</li>
<li>Fix cancel signature allowing cancel message to be <code>undefined</code> (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3153">#3153</a>)</li>
<li>Updated type checks to be formulated better (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3342">#3342</a>)</li>
<li>Avoid unnecessary buffer allocations (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3321">#3321</a>)</li>
<li>Adding a socket handler to keep TCP connection live when processing long living requests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3422">#3422</a>)</li>
<li>Added toFormData helper function (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3757">#3757</a>)</li>
<li>Adding responseEncoding prop type in AxiosRequestConfig (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3918">#3918</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Adding axios-test-instance to ecosystem (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Optimize the logic of isAxiosError (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3546">#3546</a>)</li>
<li>Add tests and documentation to display how multiple inceptors work (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3564">#3564</a>)</li>
<li>Updating follow-redirects to version 1.14.7 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4379">#4379</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Fixing changelog to show corrext pull request (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4219">#4219</a>)</li>
<li>Update upgrade guide for https proxy setting (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3604">#3604</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/master/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h3>0.26.0 (February 13, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed The timeoutErrorMessage property in config not work with Node.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3581">#3581</a>)</li>
<li>Added errors to be displayed when the query parsing process itself fails (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3961">#3961</a>)</li>
<li>Fix/remove url required (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4426">#4426</a>)</li>
<li>Update follow-redirects dependency due to Vurnerbility (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4462">#4462</a>)</li>
<li>Bump karma from 6.3.11 to 6.3.14 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4461">#4461</a>)</li>
<li>Bump follow-redirects from 1.14.7 to 1.14.8 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4473">#4473</a>)</li>
</ul>
<h3>0.25.0 (January 18, 2022)</h3>
<p>Breaking changes:</p>
<ul>
<li>Fixing maxBodyLength enforcement (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Don't rely on strict mode behaviour for arguments (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3470">#3470</a>)</li>
<li>Adding error handling when missing url (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3791">#3791</a>)</li>
<li>Update isAbsoluteURL.js removing escaping of non-special characters (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3809">#3809</a>)</li>
<li>Use native Array.isArray() in utils.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3836">#3836</a>)</li>
<li>Adding error handling inside stream end callback (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3967">#3967</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Added aborted even handler (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3916">#3916</a>)</li>
<li>Header types expanded allowing <code>boolean</code> and <code>number</code> types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4144">#4144</a>)</li>
<li>Fix cancel signature allowing cancel message to be <code>undefined</code> (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3153">#3153</a>)</li>
<li>Updated type checks to be formulated better (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3342">#3342</a>)</li>
<li>Avoid unnecessary buffer allocations (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3321">#3321</a>)</li>
<li>Adding a socket handler to keep TCP connection live when processing long living requests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3422">#3422</a>)</li>
<li>Added toFormData helper function (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3757">#3757</a>)</li>
<li>Adding responseEncoding prop type in AxiosRequestConfig (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3918">#3918</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Adding axios-test-instance to ecosystem (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Optimize the logic of isAxiosError (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3546">#3546</a>)</li>
<li>Add tests and documentation to display how multiple inceptors work (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3564">#3564</a>)</li>
<li>Updating follow-redirects to version 1.14.7 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4379">#4379</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Fixing changelog to show corrext pull request (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4219">#4219</a>)</li>
<li>Update upgrade guide for https proxy setting (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3604">#3604</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/master/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/rijkvanzanten">Rijk van Zanten</a></li>
<li><a href="https://github.com/koh110">Kohta Ito</a></li>
<li><a href="https://github.com/bfaulk96">Brandon Faulkner</a></li>
<li><a href="https://github.com/NoriSte">Stefano Magni</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/8e67551177990ed067384e1641d6964dcab773f7"><code>8e67551</code></a> Update line on methods, update TS definition to allow strings (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3802">#3802</a>)</li>
<li><a href="https://github.com/axios/axios/commit/224ed940e15b615336bc104b3478b137f7a48b86"><code>224ed94</code></a> Add AxiosInterceptorOptions to d.ts (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3800">#3800</a>)</li>
<li><a href="https://github.com/axios/axios/commit/bdb7d76d40407443dceaf9efa5d5a01ee4ef4da5"><code>bdb7d76</code></a> Adding baseURL to be used in getUri(), also removing question mark trimming s...</li>
<li><a href="https://github.com/axios/axios/commit/195c8e5ff5af6506e5c3e9423cd3c6e839b9cc86"><code>195c8e5</code></a> Returned error treated when requesting uncommon URL (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3544">#3544</a>)</li>
<li><a href="https://github.com/axios/axios/commit/412d3bd6078433dda4a7eb4d86e021dbc57fdeb2"><code>412d3bd</code></a> Adding support for beforeRedirect config option (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3852">#3852</a>)</li>
<li><a href="https://github.com/axios/axios/commit/3d13b67c562d45434536697bb232e2b1fba8e035"><code>3d13b67</code></a> Fix FormData example (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4391">#4391</a>)</li>
<li><a href="https://github.com/axios/axios/commit/45cb5ad7164257a7ad007bc99d1d004205249ab7"><code>45cb5ad</code></a> Updated README example to be coherent with the CommonJS usage (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4418">#4418</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2396fcd7e9b27853670759ee95d8f64156730159"><code>2396fcd</code></a> Bump karma from 6.3.14 to 6.3.16 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4506">#4506</a>)</li>
<li><a href="https://github.com/axios/axios/commit/170588f3d78f855450d1ce50968651a54cda7386"><code>170588f</code></a> Refactored project file structure to avoid circular imports; (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4220">#4220</a>)</li>
<li><a href="https://github.com/axios/axios/commit/6e63edf455b6854feeeb0d2394fe0d1d854b55e0"><code>6e63edf</code></a> Bump url-parse from 1.5.4 to 1.5.10 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4501">#4501</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.23.0...v0.26.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.23.0&new-version=0.26.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-10 08:39:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3199" class=".btn">#3199</a>
            </td>
            <td>
                <b>
                    feat: expose key type in ExportPubKeyBytes()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changes adds the kms.Keytype return value in ExportPubKeyBytes()

closes #3198

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 17:44:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3196" class=".btn">#3196</a>
            </td>
            <td>
                <b>
                    fix: create oobv2 inviter's connection record on v1 messages, with invitation ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add invitation ID to inviter's implicit didcomm v2 connection
- allow all non-didexchange messages to use didcomm v2 handlers

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 23:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3195" class=".btn">#3195</a>
            </td>
            <td>
                <b>
                    Update vcwallet and vdr swagger generation docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #3193

I checked the swagger docs for vcwallet and vdr. Problem might occur in other parts, too.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 20:59:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3194" class=".btn">#3194</a>
            </td>
            <td>
                <b>
                    docs: remove outdated demo app link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Rolson Quadras <rolson.quadras@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 18:14:26 +0000 UTC
    </div>
</div>

