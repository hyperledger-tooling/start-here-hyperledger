---
layout: default
title: aries-endorser-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-endorser-service
---

# aries-endorser-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-endorser-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Bump black from 21.12b0 to 24.3.0 in /bdd-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 21.12b0 to 24.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<p>This release is a milestone: it fixes Black's first CVE security vulnerability. If you
run Black on untrusted input, or if you habitually put thousands of leading tab
characters in your docstrings, you are strongly encouraged to upgrade immediately to fix
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.</p>
<p>This release also fixes a bug in Black's AST safety check that allowed Black to make
incorrect changes to certain f-strings that are valid in Python 3.12 and higher.</p>
<h3>Stable style</h3>
<ul>
<li>Don't move comments along with delimiters, which could cause crashes (<a href="https://redirect.github.com/psf/black/issues/4248">#4248</a>)</li>
<li>Strengthen AST safety check to catch more unsafe changes to strings. Previous versions
of Black would incorrectly format the contents of certain unusual f-strings containing
nested strings with the same quote type. Now, Black will crash on such strings until
support for the new f-string syntax is implemented. (<a href="https://redirect.github.com/psf/black/issues/4270">#4270</a>)</li>
<li>Fix a bug where line-ranges exceeding the last code line would not work as expected
(<a href="https://redirect.github.com/psf/black/issues/4273">#4273</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix catastrophic performance on docstrings that contain large numbers of leading tab
characters. This fixes
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.
(<a href="https://redirect.github.com/psf/black/issues/4278">#4278</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Note what happens when <code>--check</code> is used with <code>--quiet</code> (<a href="https://redirect.github.com/psf/black/issues/4236">#4236</a>)</li>
</ul>
<h2>24.2.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fixed a bug where comments where mistakenly removed along with redundant parentheses
(<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li>Move the <code>hug_parens_with_braces_and_square_brackets</code> feature to the unstable style
due to an outstanding crash and proposed formatting tweaks (<a href="https://redirect.github.com/psf/black/issues/4198">#4198</a>)</li>
<li>Fixed a bug where base expressions caused inconsistent formatting of ** in tenary
expression (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li>Checking for newline before adding one on docstring that is almost at the line limit
(<a href="https://redirect.github.com/psf/black/issues/4185">#4185</a>)</li>
<li>Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>).</li>
</ul>
<h3>Configuration</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<p>This release is a milestone: it fixes Black's first CVE security vulnerability. If you
run Black on untrusted input, or if you habitually put thousands of leading tab
characters in your docstrings, you are strongly encouraged to upgrade immediately to fix
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.</p>
<p>This release also fixes a bug in Black's AST safety check that allowed Black to make
incorrect changes to certain f-strings that are valid in Python 3.12 and higher.</p>
<h3>Stable style</h3>
<ul>
<li>Don't move comments along with delimiters, which could cause crashes (<a href="https://redirect.github.com/psf/black/issues/4248">#4248</a>)</li>
<li>Strengthen AST safety check to catch more unsafe changes to strings. Previous versions
of Black would incorrectly format the contents of certain unusual f-strings containing
nested strings with the same quote type. Now, Black will crash on such strings until
support for the new f-string syntax is implemented. (<a href="https://redirect.github.com/psf/black/issues/4270">#4270</a>)</li>
<li>Fix a bug where line-ranges exceeding the last code line would not work as expected
(<a href="https://redirect.github.com/psf/black/issues/4273">#4273</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix catastrophic performance on docstrings that contain large numbers of leading tab
characters. This fixes
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.
(<a href="https://redirect.github.com/psf/black/issues/4278">#4278</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Note what happens when <code>--check</code> is used with <code>--quiet</code> (<a href="https://redirect.github.com/psf/black/issues/4236">#4236</a>)</li>
</ul>
<h2>24.2.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fixed a bug where comments where mistakenly removed along with redundant parentheses
(<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li>Move the <code>hug_parens_with_braces_and_square_brackets</code> feature to the unstable style
due to an outstanding crash and proposed formatting tweaks (<a href="https://redirect.github.com/psf/black/issues/4198">#4198</a>)</li>
<li>Fixed a bug where base expressions caused inconsistent formatting of ** in tenary
expression (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li>Checking for newline before adding one on docstring that is almost at the line limit
(<a href="https://redirect.github.com/psf/black/issues/4185">#4185</a>)</li>
<li>Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>).</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/psf/black/commits/24.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=21.12b0&new-version=24.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-endorser-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 11:49:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Bump starlette from 0.17.1 to 0.36.2 in /endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                [//]: # (dependabot-start)
⚠️  **Dependabot is rebasing this PR** ⚠️ 

Rebasing might not happen immediately, so don't worry if this takes some time.

Note: if you make any changes to this PR yourself, they will take precedence over the rebase.

---

[//]: # (dependabot-end)

Bumps [starlette](https://github.com/encode/starlette) from 0.17.1 to 0.36.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/encode/starlette/releases">starlette's releases</a>.</em></p>
<blockquote>
<h2>Version 0.36.2</h2>
<h2>Fixed</h2>
<ul>
<li>Upgrade <code>python-multipart</code> to <code>0.0.7</code> <a href="https://github.com/encode/starlette/blob/HEAD/13e5c26a27f4903924624736abd6131b2da80cc5">13e5c26</a>.</li>
<li>Avoid duplicate charset on <code>Content-Type</code> <a href="https://github.com/encode/starlette/2443">#2443</a>.</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/starlette/compare/0.36.1...0.36.2">https://github.com/encode/starlette/compare/0.36.1...0.36.2</a></p>
<h2>Version 0.36.1</h2>
<h2>Fixed</h2>
<ul>
<li>Check if &quot;extensions&quot; in scope before checking the extension <a href="http://redirect.github.com/encode/starlette/pull/2438">#2438</a>.</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/starlette/compare/0.36.0...0.36.1">https://github.com/encode/starlette/compare/0.36.0...0.36.1</a></p>
<h2>Version 0.36.0</h2>
<h2>Added</h2>
<ul>
<li>Add support for ASGI <code>pathsend</code> extension <a href="http://redirect.github.com/encode/starlette/pull/2435">#2435</a>.</li>
<li>Cancel <code>WebSocketTestSession</code> on close <a href="http://redirect.github.com/encode/starlette/pull/2427">#2427</a>.</li>
<li>Raise <code>WebSocketDisconnect</code> when <code>WebSocket.send()</code> excepts <code>IOError</code> <a href="http://redirect.github.com/encode/starlette/pull/2425">#2425</a>.</li>
<li>Raise <code>FileNotFoundError</code> when the <code>env_file</code> parameter on <code>Config</code> is not valid <a href="http://redirect.github.com/encode/starlette/pull/2422">#2422</a>.</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/starlette/compare/0.35.1...0.36.0">https://github.com/encode/starlette/compare/0.35.1...0.36.0</a></p>
<h2>Version 0.35.1</h2>
<h2>Fixed</h2>
<ul>
<li>Stop using the deprecated &quot;method&quot; parameter in <code>FileResponse</code> inside of <code>StaticFiles</code> <a href="https://redirect.github.com/encode/starlette/pull/2406">#2406</a>.</li>
<li>Make <code>typing-extensions</code> optional again <a href="https://redirect.github.com/encode/starlette/pull/2409">#2409</a>.</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/starlette/compare/0.35.0...0.35.1">https://github.com/encode/starlette/compare/0.35.0...0.35.1</a></p>
<h2>Version 0.35.0</h2>
<h2>Added</h2>
<ul>
<li>Add <code>*args</code> to <code>Middleware</code> and improve its type hints <a href="https://redirect.github.com/encode/starlette/pull/2381">#2381</a>.</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>Use <code>Iterable</code> instead <code>Iterator</code> on <code>iterate_in_threadpool</code> <a href="https://redirect.github.com/encode/starlette/pull/2362">#2362</a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/encode/starlette/blob/master/docs/release-notes.md">starlette's changelog</a>.</em></p>
<blockquote>
<h2>0.36.2</h2>
<p>February 3, 2024</p>
<h4>Fixed</h4>
<ul>
<li>Upgrade <code>python-multipart</code> to <code>0.0.7</code> <a href="https://github.com/encode/starlette/blob/master/docs/13e5c26a27f4903924624736abd6131b2da80cc5">13e5c26</a>.</li>
<li>Avoid duplicate charset on <code>Content-Type</code> <a href="https://github.com/encode/starlette/2443">#2443</a>.</li>
</ul>
<h2>0.36.1</h2>
<p>January 23, 2024</p>
<h4>Fixed</h4>
<ul>
<li>Check if &quot;extensions&quot; in scope before checking the extension <a href="http://redirect.github.com/encode/starlette/pull/2438">#2438</a>.</li>
</ul>
<h2>0.36.0</h2>
<p>January 22, 2024</p>
<h4>Added</h4>
<ul>
<li>Add support for ASGI <code>pathsend</code> extension <a href="http://redirect.github.com/encode/starlette/pull/2435">#2435</a>.</li>
<li>Cancel <code>WebSocketTestSession</code> on close <a href="http://redirect.github.com/encode/starlette/pull/2427">#2427</a>.</li>
<li>Raise <code>WebSocketDisconnect</code> when <code>WebSocket.send()</code> excepts <code>IOError</code> <a href="http://redirect.github.com/encode/starlette/pull/2425">#2425</a>.</li>
<li>Raise <code>FileNotFoundError</code> when the <code>env_file</code> parameter on <code>Config</code> is not valid <a href="http://redirect.github.com/encode/starlette/pull/2422">#2422</a>.</li>
</ul>
<h2>0.35.1</h2>
<p>January 11, 2024</p>
<h4>Fixed</h4>
<ul>
<li>Stop using the deprecated &quot;method&quot; parameter in <code>FileResponse</code> inside of <code>StaticFiles</code> <a href="https://redirect.github.com/encode/starlette/pull/2406">#2406</a>.</li>
<li>Make <code>typing-extensions</code> optional again <a href="https://redirect.github.com/encode/starlette/pull/2409">#2409</a>.</li>
</ul>
<h2>0.35.0</h2>
<p>January 11, 2024</p>
<h4>Added</h4>
<ul>
<li>Add <code>*args</code> to <code>Middleware</code> and improve its type hints <a href="https://redirect.github.com/encode/starlette/pull/2381">#2381</a>.</li>
</ul>
<h4>Fixed</h4>
<ul>
<li>Use <code>Iterable</code> instead <code>Iterator</code> on <code>iterate_in_threadpool</code> <a href="https://redirect.github.com/encode/starlette/pull/2362">#2362</a>.</li>
</ul>
<h4>Changes</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/encode/starlette/commit/04a7d9d8d1db3734c028d89a6a3fd636ddcafedf"><code>04a7d9d</code></a> Version 0.36.2 (<a href="https://redirect.github.com/encode/starlette/issues/2456">#2456</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/13e5c26a27f4903924624736abd6131b2da80cc5"><code>13e5c26</code></a> Merge pull request from GHSA-93gm-qmq6-w238</li>
<li><a href="https://github.com/encode/starlette/commit/b8eebef38711902769fc1846c9bb2a1fcd26960d"><code>b8eebef</code></a> Avoid duplicate charset on <code>Content-Type</code> (<a href="https://redirect.github.com/encode/starlette/issues/2443">#2443</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/8da52c2243b8855426c40c16ae24b27734824078"><code>8da52c2</code></a> Bump the python-packages group with 4 updates (<a href="https://redirect.github.com/encode/starlette/issues/2455">#2455</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/4355e6bc288e14dea9597ad9c9265c0f9cad33c0"><code>4355e6b</code></a> Fix nav override for newer version of Mkdocs Material (<a href="https://redirect.github.com/encode/starlette/issues/2444">#2444</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/433da65fc1431754dae0c3c87290b0421aa4a6f9"><code>433da65</code></a> Version 0.36.1 (<a href="https://redirect.github.com/encode/starlette/issues/2440">#2440</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/4ca0a8757a6ac5938c64f8ce925e3abe95625468"><code>4ca0a87</code></a> Downgrade mkdocs-material (<a href="https://redirect.github.com/encode/starlette/issues/2439">#2439</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/e54be85aba48201b0f1c061c892bdc380efb754d"><code>e54be85</code></a> Check if &quot;extensions&quot; in scope before checking the extension (<a href="https://redirect.github.com/encode/starlette/issues/2438">#2438</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/8d09cf4b692a8e28a2f52c7cfa108c80471ffc21"><code>8d09cf4</code></a> Version 0.36.0 (<a href="https://redirect.github.com/encode/starlette/issues/2432">#2432</a>)</li>
<li><a href="https://github.com/encode/starlette/commit/7936e86f0a0eb7494aee8a1094b0ccda31c67a72"><code>7936e86</code></a> Add support for ASGI <code>pathsend</code> extension (<a href="https://redirect.github.com/encode/starlette/issues/2435">#2435</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/encode/starlette/compare/0.17.1...0.36.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=starlette&package-manager=pip&previous-version=0.17.1&new-version=0.36.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-endorser-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 11:49:25 +0000 UTC
    </div>
</div>

