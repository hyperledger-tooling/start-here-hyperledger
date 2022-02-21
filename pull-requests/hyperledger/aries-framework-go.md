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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3172" class=".btn">#3172</a>
            </td>
            <td>
                <b>
                    chore(deps): bump axios from 0.23.0 to 0.26.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.23.0 to 0.26.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
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
<ul>
<li><a href="https://github.com/axios/axios/blob/HEAD/mailto:jasonsaayman@gmail.com">Jay</a></li>
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
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/master/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
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
<li><a href="https://github.com/fanguangyi">enofan</a></li>
<li><a href="https://github.com/puzpuzpuz">Andrey Pechkurov</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/c9aca7525703ab600eacd9e95fd7f6ecc9942616"><code>c9aca75</code></a> Releasing v0.26.0</li>
<li><a href="https://github.com/axios/axios/commit/3f842e034ec45c6b48247a48160620dfdf9336e4"><code>3f842e0</code></a> Merge branch 'master' of github.com:axios/axios</li>
<li><a href="https://github.com/axios/axios/commit/2f1e8189f2cf2e97f525975a2a609ca5213b6b7a"><code>2f1e818</code></a> Merge branch 'cookieMr-master'</li>
<li><a href="https://github.com/axios/axios/commit/95295f6f291fc7e647e8d3c2960b5d26a2df707d"><code>95295f6</code></a> Fixed conflict in package lock</li>
<li><a href="https://github.com/axios/axios/commit/b3aa79e13818ab6027b43d9aaae491f1ffcec0fe"><code>b3aa79e</code></a> Bump follow-redirects from 1.14.7 to 1.14.8 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4473">#4473</a>)</li>
<li><a href="https://github.com/axios/axios/commit/d660e29c1a0f4af84e2050f1fcfa52eb9715b363"><code>d660e29</code></a> Revert &quot;Fixed isFormData predicate; (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4413">#4413</a>)&quot; (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4472">#4472</a>)</li>
<li><a href="https://github.com/axios/axios/commit/447a24dfc337f93d35b9a8bed7629a76f7aed6bf"><code>447a24d</code></a> Bump karma from 6.3.11 to 6.3.14 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4461">#4461</a>)</li>
<li><a href="https://github.com/axios/axios/commit/c5bdbd436d7ac90d7bac26247cb60752d171e47c"><code>c5bdbd4</code></a> Update follow-redirects dependency due to Vurnerbility</li>
<li><a href="https://github.com/axios/axios/commit/73e3bdb8835ba942096b662e9441f1d85ce4d484"><code>73e3bdb</code></a> Fixed isFormData predicate; (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4413">#4413</a>)</li>
<li><a href="https://github.com/axios/axios/commit/cc86c6c49fdbfd8e2517b191b8833d2f2816ff91"><code>cc86c6c</code></a> Fix/remove url required (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4426">#4426</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.23.0...v0.26.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.23.0&new-version=0.26.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-02-21 08:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3169" class=".btn">#3169</a>
            </td>
            <td>
                <b>
                    fix: didcomm with webkms tests and bugfixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 22:39:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3168" class=".btn">#3168</a>
            </td>
            <td>
                <b>
                    Update package.json with upgraded packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added some core packages to package.json

Signed-off-by: Bhaskar Ram <bhaskar@parrotsec.in>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 17:23:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3166" class=".btn">#3166</a>
            </td>
            <td>
                <b>
                    fix: auth crypt packer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Holovko <andriy.holovko@gmail.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 06:47:07 +0000 UTC
    </div>
</div>

