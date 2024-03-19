---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2844" class=".btn">#2844</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the all-actions group with 1 update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps the all-actions group with 1 update: [psf/black](https://github.com/psf/black).

Updates `psf/black` from 24.2.0 to 24.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">psf/black's releases</a>.</em></p>
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
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">psf/black's changelog</a>.</em></p>
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/24.2.0...24.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=psf/black&package-manager=github_actions&previous-version=24.2.0&new-version=24.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 21:46:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2843" class=".btn">#2843</a>
            </td>
            <td>
                <b>
                    Update to run_demo script to support Apple M1 CPUs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2842 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 19:50:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2840" class=".btn">#2840</a>
            </td>
            <td>
                <b>
                    Add anoncreds upgrade via api endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is WIP. More testing and refactoring.

This includes feature https://github.com/hyperledger/aries-cloudagent-python/pull/2822 as it was built off of it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 19:27:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2836" class=".btn">#2836</a>
            </td>
            <td>
                <b>
                    Remove requirement for write ledger in read-only mode.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2829 

This change removes the requirement for the list of ledgers to specify at least a ledger with attribute `is_write` when running the agent in read-only mode.

I initially tried to mock the parsed argument in the tests as one was failing, however having attributes from different groups made mocking very complicated so I opted for moving this setting onto `LedgerGroup` as well, as it seems appropriate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 01:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2835" class=".btn">#2835</a>
            </td>
            <td>
                <b>
                    feat: external suite provider interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a pluggable component enabling usage of an externally provided signature suite. This is a refinement on previous attempts to make this aspect of ACA-Py more flexible; namely, #2706 which was later reverted due to issues with including profile in the context and multi-tenancy. This approach minimizes the "surface area" of the interface that the plugin must fulfill (at least when compared to what was proposed in #2706).

This is an advanced use case requiring some fairly deep knowledge of the management of DIDs and VCs. I have an example implementation of using an external KMS for signing JSON-LD creds that I may push to the open as a starting point for interested parties.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 21:59:33 +0000 UTC
    </div>
</div>

