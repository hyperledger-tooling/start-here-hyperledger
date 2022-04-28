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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3232" class=".btn">#3232</a>
            </td>
            <td>
                <b>
                    feat: add HealthCheck for remote kms
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
        Created At 2022-04-27 13:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3231" class=".btn">#3231</a>
            </td>
            <td>
                <b>
                    chore(deps): bump axios from 0.23.0 to 0.27.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.23.0 to 0.27.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>v0.27.1</h2>
<h3>0.27.1 (April 26, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Removed import of url module in browser build due to huge size overhead and builds being broken (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4594">#4594</a>)</li>
<li>Bumped follow-redirects to ^1.14.9 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4615">#4615</a>)</li>
</ul>
<h2>v0.27.0</h2>
<h3>0.27.0 (April 25, 2022)</h3>
<p>Breaking changes:</p>
<ul>
<li>New toFormData helper function that allows the implementor to pass an object and allow axios to convert it to FormData (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3757">#3757</a>)</li>
<li>Removed functionality that removed the the <code>Content-Type</code> request header when passing FormData (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3785">#3785</a>)</li>
<li><strong>(*)</strong> Refactored error handling implementing AxiosError as a constructor, this is a large change to error handling on the whole (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3645">#3645</a>)</li>
<li>Separated responsibility for FormData instantiation between <code>transformRequest</code> and <code>toFormData</code> (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4470">#4470</a>)</li>
<li><strong>(*)</strong> Improved and fixed multiple issues with FormData support (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4448">#4448</a>)</li>
</ul>
<p>QOL and DevX improvements:</p>
<ul>
<li>Added a multipart/form-data testing playground allowing contributors to debug changes easily (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4465">#4465</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Refactored project file structure to avoid circular imports (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4516">#4515</a>) &amp; (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4516">#4516</a>)</li>
<li>Bumped follow-redirects to ^1.14.9 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4562">#4562</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Updated dev dependencies to latest version</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Fixing incorrect link in changelog (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4551">#4551</a>)</li>
</ul>
<p>Notes:</p>
<ul>
<li><strong>(*)</strong> Please read these pull requests before updating, these changes are very impactful and far reaching.</li>
</ul>
<h2>v0.26.1</h2>
<h3>0.26.1 (March 9, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Refactored project file structure to avoid circular imports (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4220">#4220</a>)</li>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/master/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h3>0.27.1 (April 26, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Removed import of url module in browser build due to huge size overhead and builds being broken (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4594">#4594</a>)</li>
<li>Bumped follow-redirects to ^1.14.9 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4615">#4615</a>)</li>
</ul>
<h3>0.27.0 (April 25, 2022)</h3>
<p>Breaking changes:</p>
<ul>
<li>New toFormData helper function that allows the implementor to pass an object and allow axios to convert it to FormData (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3757">#3757</a>)</li>
<li>Removed functionality that removed the the <code>Content-Type</code> request header when passing FormData (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3785">#3785</a>)</li>
<li><strong>(*)</strong> Refactored error handling implementing AxiosError as a constructor, this is a large change to error handling on the whole (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3645">#3645</a>)</li>
<li>Separated responsibility for FormData instantiation between <code>transformRequest</code> and <code>toFormData</code> (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4470">#4470</a>)</li>
<li><strong>(*)</strong> Improved and fixed multiple issues with FormData support (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4448">#4448</a>)</li>
</ul>
<p>QOL and DevX improvements:</p>
<ul>
<li>Added a multipart/form-data testing playground allowing contributors to debug changes easily (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4465">#4465</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Refactored project file structure to avoid circular imports (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4516">#4515</a>) &amp; (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4516">#4516</a>)</li>
<li>Bumped follow-redirects to ^1.14.9 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4562">#4562</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Updated dev dependencies to latest version</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Fixing incorrect link in changelog (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4551">#4551</a>)</li>
</ul>
<p>Notes:</p>
<ul>
<li><strong>(*)</strong> Please read these pull requests before updating, these changes are very impactful and far reaching.</li>
</ul>
<h3>0.26.1 (March 9, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Refactored project file structure to avoid circular imports (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4220">#4220</a>)</li>
</ul>
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
<h3>0.25.0 (January 18, 2022)</h3>
<p>Breaking changes:</p>
<ul>
<li>Fixing maxBodyLength enforcement (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/838f53b4bb6616d8ec8efdae0612c9c74b8c3804"><code>838f53b</code></a> Merge branch 'master' of github.com:axios/axios</li>
<li><a href="https://github.com/axios/axios/commit/cb9c534963a99292f1d0c6137a7d32d9c859f6d5"><code>cb9c534</code></a> Releasing v0.27.1</li>
<li><a href="https://github.com/axios/axios/commit/91d21fc5fb0eeb4c60f6a75ab6db303c5d23f3c5"><code>91d21fc</code></a> Releasing v0.72.1</li>
<li><a href="https://github.com/axios/axios/commit/167cb8b8e7dbef7acd0be9b05bd50e4af2335291"><code>167cb8b</code></a> Remove eslint-g package as this seems have been added in error</li>
<li><a href="https://github.com/axios/axios/commit/4f7e3e3a7a9b91579faa328964c3d5fe30e661d7"><code>4f7e3e3</code></a> Removed import of url module in browser build due to significant size overhea...</li>
<li><a href="https://github.com/axios/axios/commit/cdd7add9b05c2c651de197a54d6a51172a6655a3"><code>cdd7add</code></a> Fixed date on chnagelog</li>
<li><a href="https://github.com/axios/axios/commit/f94dda9c76442ac097923fdfc02199e72c20f083"><code>f94dda9</code></a> Bump async from 2.6.3 to 2.6.4 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4615">#4615</a>)</li>
<li><a href="https://github.com/axios/axios/commit/008dd9d466167e97727bdba13f4937bb9d7f3baa"><code>008dd9d</code></a> Releaseing version 0.27.0</li>
<li><a href="https://github.com/axios/axios/commit/ee151a7356ec4498af045dd830312822637890c9"><code>ee151a7</code></a> Revert some changes that are only required when we actually release</li>
<li><a href="https://github.com/axios/axios/commit/499d3bee543b55877b8458aeb56ce71969720333"><code>499d3be</code></a> follow-redirects to ^1.14.9 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4562">#4562</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.23.0...v0.27.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.23.0&new-version=0.27.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-26 08:17:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3230" class=".btn">#3230</a>
            </td>
            <td>
                <b>
                    feat: In-memory store "ping" method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The method always returns nil. It's there just to allow it to implement a "Pinger" sort of interface which may be defined somewhere.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 17:51:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3229" class=".btn">#3229</a>
            </td>
            <td>
                <b>
                    externalize agent parameters + router
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Allow External Usage of `agentParameters` and `mux.Router`

**Description:**
To allow for another server framework than golang's `http`, we need to externalize the creation of `mux.NewRouter()`.

**Summary:**
Related: #3224 

When @borancar and I first authored #3224, we copied and pasted `start.go` and named it `aires.go` to gain access to `mux.NewRouter()`, so we could plug it into another server framework, as Lambda does not use golang's `http` package, however it is compatible with gorillamux.

So this PR allows us to import `startcmd` and leverage a couple new functions:
 - `NewAgentParameters()`
    - `AgentParameters` is now an exported type
    - `AgentParameters` has a new method: `NewRouter()`
 - nil-safety on helper functions for `cobra.Command`
   - Our lambda integration will use environment variables exclusively, so we pass `nil` when constructing `AgentParameters`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 17:46:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3227" class=".btn">#3227</a>
            </td>
            <td>
                <b>
                    refactor: web-redirector with underscore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following this DIDcomm V2 spec udpate:
https://github.com/decentralized-identity/didcomm-messaging/pull/363
web-redirect is now web_redirect.

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 13:35:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3226" class=".btn">#3226</a>
            </td>
            <td>
                <b>
                    fix: vc-revocation-list-2021 context
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
        Created At 2022-04-22 11:50:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3225" class=".btn">#3225</a>
            </td>
            <td>
                <b>
                    chore: add revocation list 2021 context
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
        Created At 2022-04-22 10:54:20 +0000 UTC
    </div>
</div>

