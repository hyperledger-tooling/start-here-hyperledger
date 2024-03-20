---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.3.0 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.3.0.
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
<li><a href="https://github.com/psf/black/commit/552baf822992936134cbd31a38f69c8cfe7c0f05"><code>552baf8</code></a> Prepare release 24.3.0 (<a href="https://redirect.github.com/psf/black/issues/4279">#4279</a>)</li>
<li><a href="https://github.com/psf/black/commit/f00093672628d212b8965a8993cee8bedf5fe9b8"><code>f000936</code></a> Fix catastrophic performance in lines_with_leading_tabs_expanded() (<a href="https://redirect.github.com/psf/black/issues/4278">#4278</a>)</li>
<li><a href="https://github.com/psf/black/commit/7b5a657285f38126bf28483478bbd9ea928077ec"><code>7b5a657</code></a> Fix --line-ranges behavior when ranges are at EOF (<a href="https://redirect.github.com/psf/black/issues/4273">#4273</a>)</li>
<li><a href="https://github.com/psf/black/commit/1abcffc81816257985678f08c61584ed4287f22a"><code>1abcffc</code></a> Use regex where we ignore case on windows (<a href="https://redirect.github.com/psf/black/issues/4252">#4252</a>)</li>
<li><a href="https://github.com/psf/black/commit/719e67462c80574c81a96faa144886de6da84489"><code>719e674</code></a> Fix 4227: Improve documentation for --quiet --check (<a href="https://redirect.github.com/psf/black/issues/4236">#4236</a>)</li>
<li><a href="https://github.com/psf/black/commit/e5510afc06cd238cd0cba4095283943a870a7e7b"><code>e5510af</code></a> update plugin url for Thonny (<a href="https://redirect.github.com/psf/black/issues/4259">#4259</a>)</li>
<li><a href="https://github.com/psf/black/commit/6af7d1109693c4ad3af08ecbc34649c232b47a6d"><code>6af7d11</code></a> Fix AST safety check false negative (<a href="https://redirect.github.com/psf/black/issues/4270">#4270</a>)</li>
<li><a href="https://github.com/psf/black/commit/f03ee113c9f3dfeb477f2d4247bfb7de2e5f465c"><code>f03ee11</code></a> Ensure <code>blib2to3.pygram</code> is initialized before use (<a href="https://redirect.github.com/psf/black/issues/4224">#4224</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4bfedbec2e8b10cc6b7b31442478f05db0ce06d"><code>e4bfedb</code></a> fix: Don't move comments while splitting delimiters (<a href="https://redirect.github.com/psf/black/issues/4248">#4248</a>)</li>
<li><a href="https://github.com/psf/black/commit/d0287e1f7558d97e6c0ebd6dc5bcb5b970e2bf8c"><code>d0287e1</code></a> Make trailing comma logic more concise (<a href="https://redirect.github.com/psf/black/issues/4202">#4202</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 04:15:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.3.0 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.3.0.
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
<li><a href="https://github.com/psf/black/commit/552baf822992936134cbd31a38f69c8cfe7c0f05"><code>552baf8</code></a> Prepare release 24.3.0 (<a href="https://redirect.github.com/psf/black/issues/4279">#4279</a>)</li>
<li><a href="https://github.com/psf/black/commit/f00093672628d212b8965a8993cee8bedf5fe9b8"><code>f000936</code></a> Fix catastrophic performance in lines_with_leading_tabs_expanded() (<a href="https://redirect.github.com/psf/black/issues/4278">#4278</a>)</li>
<li><a href="https://github.com/psf/black/commit/7b5a657285f38126bf28483478bbd9ea928077ec"><code>7b5a657</code></a> Fix --line-ranges behavior when ranges are at EOF (<a href="https://redirect.github.com/psf/black/issues/4273">#4273</a>)</li>
<li><a href="https://github.com/psf/black/commit/1abcffc81816257985678f08c61584ed4287f22a"><code>1abcffc</code></a> Use regex where we ignore case on windows (<a href="https://redirect.github.com/psf/black/issues/4252">#4252</a>)</li>
<li><a href="https://github.com/psf/black/commit/719e67462c80574c81a96faa144886de6da84489"><code>719e674</code></a> Fix 4227: Improve documentation for --quiet --check (<a href="https://redirect.github.com/psf/black/issues/4236">#4236</a>)</li>
<li><a href="https://github.com/psf/black/commit/e5510afc06cd238cd0cba4095283943a870a7e7b"><code>e5510af</code></a> update plugin url for Thonny (<a href="https://redirect.github.com/psf/black/issues/4259">#4259</a>)</li>
<li><a href="https://github.com/psf/black/commit/6af7d1109693c4ad3af08ecbc34649c232b47a6d"><code>6af7d11</code></a> Fix AST safety check false negative (<a href="https://redirect.github.com/psf/black/issues/4270">#4270</a>)</li>
<li><a href="https://github.com/psf/black/commit/f03ee113c9f3dfeb477f2d4247bfb7de2e5f465c"><code>f03ee11</code></a> Ensure <code>blib2to3.pygram</code> is initialized before use (<a href="https://redirect.github.com/psf/black/issues/4224">#4224</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4bfedbec2e8b10cc6b7b31442478f05db0ce06d"><code>e4bfedb</code></a> fix: Don't move comments while splitting delimiters (<a href="https://redirect.github.com/psf/black/issues/4248">#4248</a>)</li>
<li><a href="https://github.com/psf/black/commit/d0287e1f7558d97e6c0ebd6dc5bcb5b970e2bf8c"><code>d0287e1</code></a> Make trailing comma logic more concise (<a href="https://redirect.github.com/psf/black/issues/4202">#4202</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 04:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.3.3 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.3.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.3.3</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bandit</code>]: Implement <code>S610</code> rule (<a href="https://redirect.github.com/astral-sh/ruff/pull/10316">#10316</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>blank-line-at-end-of-file</code> (<code>W391</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10243">#10243</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>redundant-backslash</code> (<code>E502</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10292">#10292</a>)</li>
<li>[<code>pylint</code>] - implement <code>redeclared-assigned-name</code> (<code>W0128</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/9268">#9268</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8_comprehensions</code>] Handled special case for <code>C400</code> which also matches <code>C416</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10419">#10419</a>)</li>
<li>[<code>flake8-bandit</code>] Implement upstream updates for <code>S311</code>, <code>S324</code> and <code>S605</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10313">#10313</a>)</li>
<li>[<code>pyflakes</code>] Remove <code>F401</code> fix for <code>__init__</code> imports by default and allow opt-in to unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/10365">#10365</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-bool-return-type</code> (<code>E304</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10377">#10377</a>)</li>
<li>[<code>pylint</code>] Include builtin warnings in useless-exception-statement (<code>PLW0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10394">#10394</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add message on success to <code>ruff check</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/8631">#8631</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>PIE970</code>] Allow trailing ellipsis in <code>typing.TYPE_CHECKING</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10413">#10413</a>)</li>
<li>Avoid <code>TRIO115</code> if the argument is a variable (<a href="https://redirect.github.com/astral-sh/ruff/pull/10376">#10376</a>)</li>
<li>[<code>F811</code>] Avoid removing shadowed imports that point to different symbols (<a href="https://redirect.github.com/astral-sh/ruff/pull/10387">#10387</a>)</li>
<li>Fix <code>F821</code> and <code>F822</code> false positives in <code>.pyi</code> files (<a href="https://redirect.github.com/astral-sh/ruff/pull/10341">#10341</a>)</li>
<li>Fix <code>F821</code> false negatives in <code>.py</code> files when <code>from __future__ import annotations</code> is active (<a href="https://redirect.github.com/astral-sh/ruff/pull/10362">#10362</a>)</li>
<li>Fix case where <code>Indexer</code> fails to identify continuation preceded by newline <a href="https://redirect.github.com/astral-sh/ruff/issues/10351">#10351</a> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10354">#10354</a>)</li>
<li>Sort hash maps in <code>Settings</code> display (<a href="https://redirect.github.com/astral-sh/ruff/pull/10370">#10370</a>)</li>
<li>Track conditional deletions in the semantic model (<a href="https://redirect.github.com/astral-sh/ruff/pull/10415">#10415</a>)</li>
<li>[<code>C413</code>] Wrap expressions in parentheses when negating (<a href="https://redirect.github.com/astral-sh/ruff/pull/10346">#10346</a>)</li>
<li>[<code>pycodestyle</code>] Do not ignore lines before the first logical line in blank lines rules. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10382">#10382</a>)</li>
<li>[<code>pycodestyle</code>] Do not trigger <code>E225</code> and <code>E275</code> when the next token is a ')' (<a href="https://redirect.github.com/astral-sh/ruff/pull/10315">#10315</a>)</li>
<li>[<code>pylint</code>] Avoid false-positive slot non-assignment for <code>__dict__</code> (<code>PLE0237</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10348">#10348</a>)</li>
<li>Gate f-string struct size test for Rustc &lt; 1.76 (<a href="https://redirect.github.com/astral-sh/ruff/pull/10371">#10371</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Use <code>ruff.toml</code> format in README (<a href="https://redirect.github.com/astral-sh/ruff/pull/10393">#10393</a>)</li>
<li>[<code>RUF008</code>] Make it clearer that a mutable default in a dataclass is only valid if it is typed as a ClassVar (<a href="https://redirect.github.com/astral-sh/ruff/pull/10395">#10395</a>)</li>
<li>[<code>pylint</code>] Extend docs and test in <code>invalid-str-return-type</code> (<code>E307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10400">#10400</a>)</li>
<li>Remove <code>.</code> from <code>check</code> and <code>format</code> commands (<a href="https://redirect.github.com/astral-sh/ruff/pull/10217">#10217</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Guilherme-Vasconcelos"><code>@​Guilherme-Vasconcelos</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/anuraaga"><code>@​anuraaga</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.3.3</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bandit</code>]: Implement <code>S610</code> rule (<a href="https://redirect.github.com/astral-sh/ruff/pull/10316">#10316</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>blank-line-at-end-of-file</code> (<code>W391</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10243">#10243</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>redundant-backslash</code> (<code>E502</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10292">#10292</a>)</li>
<li>[<code>pylint</code>] - implement <code>redeclared-assigned-name</code> (<code>W0128</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/9268">#9268</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8_comprehensions</code>] Handled special case for <code>C400</code> which also matches <code>C416</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10419">#10419</a>)</li>
<li>[<code>flake8-bandit</code>] Implement upstream updates for <code>S311</code>, <code>S324</code> and <code>S605</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10313">#10313</a>)</li>
<li>[<code>pyflakes</code>] Remove <code>F401</code> fix for <code>__init__</code> imports by default and allow opt-in to unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/10365">#10365</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-bool-return-type</code> (<code>E304</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10377">#10377</a>)</li>
<li>[<code>pylint</code>] Include builtin warnings in useless-exception-statement (<code>PLW0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10394">#10394</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add message on success to <code>ruff check</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/8631">#8631</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>PIE970</code>] Allow trailing ellipsis in <code>typing.TYPE_CHECKING</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10413">#10413</a>)</li>
<li>Avoid <code>TRIO115</code> if the argument is a variable (<a href="https://redirect.github.com/astral-sh/ruff/pull/10376">#10376</a>)</li>
<li>[<code>F811</code>] Avoid removing shadowed imports that point to different symbols (<a href="https://redirect.github.com/astral-sh/ruff/pull/10387">#10387</a>)</li>
<li>Fix <code>F821</code> and <code>F822</code> false positives in <code>.pyi</code> files (<a href="https://redirect.github.com/astral-sh/ruff/pull/10341">#10341</a>)</li>
<li>Fix <code>F821</code> false negatives in <code>.py</code> files when <code>from __future__ import annotations</code> is active (<a href="https://redirect.github.com/astral-sh/ruff/pull/10362">#10362</a>)</li>
<li>Fix case where <code>Indexer</code> fails to identify continuation preceded by newline <a href="https://redirect.github.com/astral-sh/ruff/issues/10351">#10351</a> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10354">#10354</a>)</li>
<li>Sort hash maps in <code>Settings</code> display (<a href="https://redirect.github.com/astral-sh/ruff/pull/10370">#10370</a>)</li>
<li>Track conditional deletions in the semantic model (<a href="https://redirect.github.com/astral-sh/ruff/pull/10415">#10415</a>)</li>
<li>[<code>C413</code>] Wrap expressions in parentheses when negating (<a href="https://redirect.github.com/astral-sh/ruff/pull/10346">#10346</a>)</li>
<li>[<code>pycodestyle</code>] Do not ignore lines before the first logical line in blank lines rules. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10382">#10382</a>)</li>
<li>[<code>pycodestyle</code>] Do not trigger <code>E225</code> and <code>E275</code> when the next token is a ')' (<a href="https://redirect.github.com/astral-sh/ruff/pull/10315">#10315</a>)</li>
<li>[<code>pylint</code>] Avoid false-positive slot non-assignment for <code>__dict__</code> (<code>PLE0237</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10348">#10348</a>)</li>
<li>Gate f-string struct size test for Rustc &lt; 1.76 (<a href="https://redirect.github.com/astral-sh/ruff/pull/10371">#10371</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Use <code>ruff.toml</code> format in README (<a href="https://redirect.github.com/astral-sh/ruff/pull/10393">#10393</a>)</li>
<li>[<code>RUF008</code>] Make it clearer that a mutable default in a dataclass is only valid if it is typed as a ClassVar (<a href="https://redirect.github.com/astral-sh/ruff/pull/10395">#10395</a>)</li>
<li>[<code>pylint</code>] Extend docs and test in <code>invalid-str-return-type</code> (<code>E307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10400">#10400</a>)</li>
<li>Remove <code>.</code> from <code>check</code> and <code>format</code> commands (<a href="https://redirect.github.com/astral-sh/ruff/pull/10217">#10217</a>)</li>
</ul>
<h2>0.3.2</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/608df9a1bc0e6025049add877d1d833f1739e966"><code>608df9a</code></a> Bump version to 0.3.3 (<a href="https://redirect.github.com/astral-sh/ruff/issues/10425">#10425</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/740c08b033d835f071e4887cea2f608d6cc662c6"><code>740c08b</code></a> [<code>pylint</code>] - implement <code>redeclared-assigned-name</code> (<code>W0128</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/9268">#9268</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7e652e8fcb7e9a4c331d8b8829adbf135154fa0f"><code>7e652e8</code></a> [<code>flake8_comprehensions</code>] Handled special case for <code>C400</code> which also matches ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9675e1867a73e536a609e971f2e823c799771afc"><code>9675e18</code></a> Allow trailing ellipsis in <code>typing.TYPE_CHECKING</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/10413">#10413</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/10ace88e9a7423271441ba314e788daee53e00f0"><code>10ace88</code></a> Track conditional deletions in the semantic model (<a href="https://redirect.github.com/astral-sh/ruff/issues/10415">#10415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a8e50a7f40b2883b904d9ba347ef01c466179a75"><code>a8e50a7</code></a> [RUF008] Make it clearer that a mutable default in a dataclass is only valid ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e944c16c4601af3b503f2ac19d3f9266aae7660d"><code>e944c16</code></a> [<code>pycodestyle</code>] Do not ignore lines before the first logical line in blank li...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f40371ffc2073fec7e66c3014bb1f765845bfd1"><code>5f40371</code></a> Use <code>ExprFString</code> for <code>StringLike::FString</code> variant (<a href="https://redirect.github.com/astral-sh/ruff/issues/10311">#10311</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f7802ad5dea287f3c853ffaf14a8b2c5dd7daa67"><code>f7802ad</code></a> [<code>pylint</code>] Extend docs and test in <code>invalid-str-return-type</code> (<code>E307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/10400">#10400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e832327a56be73d48733506863711a3740f15877"><code>e832327</code></a> Require --preview for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/10368">#10368</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.3.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 04:12:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.3.3 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.3.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.3.3</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bandit</code>]: Implement <code>S610</code> rule (<a href="https://redirect.github.com/astral-sh/ruff/pull/10316">#10316</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>blank-line-at-end-of-file</code> (<code>W391</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10243">#10243</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>redundant-backslash</code> (<code>E502</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10292">#10292</a>)</li>
<li>[<code>pylint</code>] - implement <code>redeclared-assigned-name</code> (<code>W0128</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/9268">#9268</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8_comprehensions</code>] Handled special case for <code>C400</code> which also matches <code>C416</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10419">#10419</a>)</li>
<li>[<code>flake8-bandit</code>] Implement upstream updates for <code>S311</code>, <code>S324</code> and <code>S605</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10313">#10313</a>)</li>
<li>[<code>pyflakes</code>] Remove <code>F401</code> fix for <code>__init__</code> imports by default and allow opt-in to unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/10365">#10365</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-bool-return-type</code> (<code>E304</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10377">#10377</a>)</li>
<li>[<code>pylint</code>] Include builtin warnings in useless-exception-statement (<code>PLW0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10394">#10394</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add message on success to <code>ruff check</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/8631">#8631</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>PIE970</code>] Allow trailing ellipsis in <code>typing.TYPE_CHECKING</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10413">#10413</a>)</li>
<li>Avoid <code>TRIO115</code> if the argument is a variable (<a href="https://redirect.github.com/astral-sh/ruff/pull/10376">#10376</a>)</li>
<li>[<code>F811</code>] Avoid removing shadowed imports that point to different symbols (<a href="https://redirect.github.com/astral-sh/ruff/pull/10387">#10387</a>)</li>
<li>Fix <code>F821</code> and <code>F822</code> false positives in <code>.pyi</code> files (<a href="https://redirect.github.com/astral-sh/ruff/pull/10341">#10341</a>)</li>
<li>Fix <code>F821</code> false negatives in <code>.py</code> files when <code>from __future__ import annotations</code> is active (<a href="https://redirect.github.com/astral-sh/ruff/pull/10362">#10362</a>)</li>
<li>Fix case where <code>Indexer</code> fails to identify continuation preceded by newline <a href="https://redirect.github.com/astral-sh/ruff/issues/10351">#10351</a> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10354">#10354</a>)</li>
<li>Sort hash maps in <code>Settings</code> display (<a href="https://redirect.github.com/astral-sh/ruff/pull/10370">#10370</a>)</li>
<li>Track conditional deletions in the semantic model (<a href="https://redirect.github.com/astral-sh/ruff/pull/10415">#10415</a>)</li>
<li>[<code>C413</code>] Wrap expressions in parentheses when negating (<a href="https://redirect.github.com/astral-sh/ruff/pull/10346">#10346</a>)</li>
<li>[<code>pycodestyle</code>] Do not ignore lines before the first logical line in blank lines rules. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10382">#10382</a>)</li>
<li>[<code>pycodestyle</code>] Do not trigger <code>E225</code> and <code>E275</code> when the next token is a ')' (<a href="https://redirect.github.com/astral-sh/ruff/pull/10315">#10315</a>)</li>
<li>[<code>pylint</code>] Avoid false-positive slot non-assignment for <code>__dict__</code> (<code>PLE0237</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10348">#10348</a>)</li>
<li>Gate f-string struct size test for Rustc &lt; 1.76 (<a href="https://redirect.github.com/astral-sh/ruff/pull/10371">#10371</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Use <code>ruff.toml</code> format in README (<a href="https://redirect.github.com/astral-sh/ruff/pull/10393">#10393</a>)</li>
<li>[<code>RUF008</code>] Make it clearer that a mutable default in a dataclass is only valid if it is typed as a ClassVar (<a href="https://redirect.github.com/astral-sh/ruff/pull/10395">#10395</a>)</li>
<li>[<code>pylint</code>] Extend docs and test in <code>invalid-str-return-type</code> (<code>E307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10400">#10400</a>)</li>
<li>Remove <code>.</code> from <code>check</code> and <code>format</code> commands (<a href="https://redirect.github.com/astral-sh/ruff/pull/10217">#10217</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Guilherme-Vasconcelos"><code>@​Guilherme-Vasconcelos</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/anuraaga"><code>@​anuraaga</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.3.3</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bandit</code>]: Implement <code>S610</code> rule (<a href="https://redirect.github.com/astral-sh/ruff/pull/10316">#10316</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>blank-line-at-end-of-file</code> (<code>W391</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10243">#10243</a>)</li>
<li>[<code>pycodestyle</code>] Implement <code>redundant-backslash</code> (<code>E502</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10292">#10292</a>)</li>
<li>[<code>pylint</code>] - implement <code>redeclared-assigned-name</code> (<code>W0128</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/9268">#9268</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8_comprehensions</code>] Handled special case for <code>C400</code> which also matches <code>C416</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10419">#10419</a>)</li>
<li>[<code>flake8-bandit</code>] Implement upstream updates for <code>S311</code>, <code>S324</code> and <code>S605</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10313">#10313</a>)</li>
<li>[<code>pyflakes</code>] Remove <code>F401</code> fix for <code>__init__</code> imports by default and allow opt-in to unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/10365">#10365</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-bool-return-type</code> (<code>E304</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10377">#10377</a>)</li>
<li>[<code>pylint</code>] Include builtin warnings in useless-exception-statement (<code>PLW0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10394">#10394</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add message on success to <code>ruff check</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/8631">#8631</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>PIE970</code>] Allow trailing ellipsis in <code>typing.TYPE_CHECKING</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10413">#10413</a>)</li>
<li>Avoid <code>TRIO115</code> if the argument is a variable (<a href="https://redirect.github.com/astral-sh/ruff/pull/10376">#10376</a>)</li>
<li>[<code>F811</code>] Avoid removing shadowed imports that point to different symbols (<a href="https://redirect.github.com/astral-sh/ruff/pull/10387">#10387</a>)</li>
<li>Fix <code>F821</code> and <code>F822</code> false positives in <code>.pyi</code> files (<a href="https://redirect.github.com/astral-sh/ruff/pull/10341">#10341</a>)</li>
<li>Fix <code>F821</code> false negatives in <code>.py</code> files when <code>from __future__ import annotations</code> is active (<a href="https://redirect.github.com/astral-sh/ruff/pull/10362">#10362</a>)</li>
<li>Fix case where <code>Indexer</code> fails to identify continuation preceded by newline <a href="https://redirect.github.com/astral-sh/ruff/issues/10351">#10351</a> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10354">#10354</a>)</li>
<li>Sort hash maps in <code>Settings</code> display (<a href="https://redirect.github.com/astral-sh/ruff/pull/10370">#10370</a>)</li>
<li>Track conditional deletions in the semantic model (<a href="https://redirect.github.com/astral-sh/ruff/pull/10415">#10415</a>)</li>
<li>[<code>C413</code>] Wrap expressions in parentheses when negating (<a href="https://redirect.github.com/astral-sh/ruff/pull/10346">#10346</a>)</li>
<li>[<code>pycodestyle</code>] Do not ignore lines before the first logical line in blank lines rules. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10382">#10382</a>)</li>
<li>[<code>pycodestyle</code>] Do not trigger <code>E225</code> and <code>E275</code> when the next token is a ')' (<a href="https://redirect.github.com/astral-sh/ruff/pull/10315">#10315</a>)</li>
<li>[<code>pylint</code>] Avoid false-positive slot non-assignment for <code>__dict__</code> (<code>PLE0237</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10348">#10348</a>)</li>
<li>Gate f-string struct size test for Rustc &lt; 1.76 (<a href="https://redirect.github.com/astral-sh/ruff/pull/10371">#10371</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Use <code>ruff.toml</code> format in README (<a href="https://redirect.github.com/astral-sh/ruff/pull/10393">#10393</a>)</li>
<li>[<code>RUF008</code>] Make it clearer that a mutable default in a dataclass is only valid if it is typed as a ClassVar (<a href="https://redirect.github.com/astral-sh/ruff/pull/10395">#10395</a>)</li>
<li>[<code>pylint</code>] Extend docs and test in <code>invalid-str-return-type</code> (<code>E307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10400">#10400</a>)</li>
<li>Remove <code>.</code> from <code>check</code> and <code>format</code> commands (<a href="https://redirect.github.com/astral-sh/ruff/pull/10217">#10217</a>)</li>
</ul>
<h2>0.3.2</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/608df9a1bc0e6025049add877d1d833f1739e966"><code>608df9a</code></a> Bump version to 0.3.3 (<a href="https://redirect.github.com/astral-sh/ruff/issues/10425">#10425</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/740c08b033d835f071e4887cea2f608d6cc662c6"><code>740c08b</code></a> [<code>pylint</code>] - implement <code>redeclared-assigned-name</code> (<code>W0128</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/9268">#9268</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7e652e8fcb7e9a4c331d8b8829adbf135154fa0f"><code>7e652e8</code></a> [<code>flake8_comprehensions</code>] Handled special case for <code>C400</code> which also matches ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9675e1867a73e536a609e971f2e823c799771afc"><code>9675e18</code></a> Allow trailing ellipsis in <code>typing.TYPE_CHECKING</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/10413">#10413</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/10ace88e9a7423271441ba314e788daee53e00f0"><code>10ace88</code></a> Track conditional deletions in the semantic model (<a href="https://redirect.github.com/astral-sh/ruff/issues/10415">#10415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a8e50a7f40b2883b904d9ba347ef01c466179a75"><code>a8e50a7</code></a> [RUF008] Make it clearer that a mutable default in a dataclass is only valid ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e944c16c4601af3b503f2ac19d3f9266aae7660d"><code>e944c16</code></a> [<code>pycodestyle</code>] Do not ignore lines before the first logical line in blank li...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f40371ffc2073fec7e66c3014bb1f765845bfd1"><code>5f40371</code></a> Use <code>ExprFString</code> for <code>StringLike::FString</code> variant (<a href="https://redirect.github.com/astral-sh/ruff/issues/10311">#10311</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f7802ad5dea287f3c853ffaf14a8b2c5dd7daa67"><code>f7802ad</code></a> [<code>pylint</code>] Extend docs and test in <code>invalid-str-return-type</code> (<code>E307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/10400">#10400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e832327a56be73d48733506863711a3740f15877"><code>e832327</code></a> Require --preview for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/10368">#10368</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.3.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 04:11:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:32:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.1 to 1.5.6 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.1 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
<h2>v1.5.4</h2>
<p>One more release bump to address issues with typing_extensions minimum required version</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.3...v1.5.4">https://github.com/latchset/jwcrypto/compare/v1.5.3...v1.5.4</a></p>
<h2>v1.5.3</h2>
<p>Bumping release due to inconsistency in python 3.6 support that affected pypi
<a href="https://github.com/latchset/jwcrypto/files/14201083/jwcrypto-1.5.3.tar.gz.sha512sum.txt">jwcrypto-1.5.3.tar.gz.sha512sum.txt</a>
<a href="https://github.com/latchset/jwcrypto/files/14201084/jwcrypto-1.5.3.tar.gz">jwcrypto-1.5.3.tar.gz</a></p>
<h2>What's Changed</h2>
<ul>
<li>Drop python 3.6 and 3.7 and add 3.11 support by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/340">latchset/jwcrypto#340</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.2...v1.5.3">https://github.com/latchset/jwcrypto/compare/v1.5.2...v1.5.3</a></p>
<h2>Version 1.5.2 -  maintenance release</h2>
<p>This is a minor maintenance release to improve interoperability with debuggers
<strong>Note: yanked from pypi due to 3.6 incompatibility, use 1.5.3</strong></p>
<h2>What's Changed</h2>
<ul>
<li>replace deprecated package with typing_extensions by <a href="https://github.com/david-homelend"><code>@​david-homelend</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/337">latchset/jwcrypto#337</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/david-homelend"><code>@​david-homelend</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/337">latchset/jwcrypto#337</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.1...v1.5.2">https://github.com/latchset/jwcrypto/compare/v1.5.1...v1.5.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/b9432ef46fc8ee90c813469440ea86b049916e52"><code>b9432ef</code></a> Version 1.5.4</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/e7ef80f286883f6710df54c2b7ef78f528d95ee8"><code>e7ef80f</code></a> Set a minimum version for typing_extensions</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/a06b84a1281a2cd6a27eeed3b38ae38e74938d86"><code>a06b84a</code></a> Version 1.5.3</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/c659e385883e3067acf1bf4503d244e95eba4a3d"><code>c659e38</code></a> Drop python 3.6 and 3.7 and add 3.11 support</li>
<li>Additional commits viewable in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.1...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.1&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:32:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:31:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:31:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-17 13:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump follow-redirects from 1.15.4 to 1.15.6 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.15.4 to 1.15.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/35a517c5861d79dc8bff7db8626013d20b711b06"><code>35a517c</code></a> Release version 1.15.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/c4f847f85176991f95ab9c88af63b1294de8649b"><code>c4f847f</code></a> Drop Proxy-Authorization across hosts.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8526b4a1b2ab3a2e4044299377df623a661caa76"><code>8526b4a</code></a> Use GitHub for disclosure.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/b1677ce00110ee50dc5da576751d39b281fc4944"><code>b1677ce</code></a> Release version 1.15.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d8914f7982403ea096b39bd594a00ee9d3b7e224"><code>d8914f7</code></a> Preserve fragment in responseUrl.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.15.4...v1.15.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.15.4&new-version=1.15.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-16 22:45:00 +0000 UTC
    </div>
</div>

