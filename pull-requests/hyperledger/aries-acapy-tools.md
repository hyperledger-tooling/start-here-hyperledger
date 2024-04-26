---
layout: default
title: aries-acapy-tools
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-tools
---

# aries-acapy-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump pydantic from 1.10.5 to 1.10.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [pydantic](https://github.com/pydantic/pydantic) from 1.10.5 to 1.10.13.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>V1.10.13 2023-09-27</h2>
<h2>What's Changed</h2>
<ul>
<li>Update pip commands to install 1.10 by <a href="https://github.com/chbndrhnns"><code>@​chbndrhnns</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6930">pydantic/pydantic#6930</a></li>
<li>Make the v1 mypy plugin work with both v1 and v2 by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6920">pydantic/pydantic#6920</a></li>
<li>[Backport] Add max length check to <code>validate_email</code> by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7673">pydantic/pydantic#7673</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.12...v1.10.13">https://github.com/pydantic/pydantic/compare/v1.10.12...v1.10.13</a></p>
<h2>V1.10.12</h2>
<h2>What's Changed</h2>
<ul>
<li>Deque's maxlen property dropped on V1 validation by <a href="https://github.com/maciekglowka"><code>@​maciekglowka</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6586">pydantic/pydantic#6586</a></li>
<li>Prepare release 1.10.12 by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6825">pydantic/pydantic#6825</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/maciekglowka"><code>@​maciekglowka</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/6586">pydantic/pydantic#6586</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.11...v1.10.12">https://github.com/pydantic/pydantic/compare/v1.10.11...v1.10.12</a></p>
<h2>V1.10.11</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix import of create_model in tools.py by <a href="https://github.com/SharathHuddar"><code>@​SharathHuddar</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6364">pydantic/pydantic#6364</a></li>
<li>Prepare for 1.10.11 by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6420">pydantic/pydantic#6420</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/SharathHuddar"><code>@​SharathHuddar</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/6364">pydantic/pydantic#6364</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.10...v1.10.11">https://github.com/pydantic/pydantic/compare/v1.10.10...v1.10.11</a></p>
<h2>V1.10.10</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix racy doctests by <a href="https://github.com/K900"><code>@​K900</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6103">pydantic/pydantic#6103</a></li>
<li>✅ Update FastAPI test script by <a href="https://github.com/Kludex"><code>@​Kludex</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6117">pydantic/pydantic#6117</a></li>
<li>add roadmap to annoucement by <a href="https://github.com/samuelcolvin"><code>@​samuelcolvin</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6120">pydantic/pydantic#6120</a></li>
<li>Fixed literal validator errors for unhashable values by <a href="https://github.com/markus1978"><code>@​markus1978</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6194">pydantic/pydantic#6194</a></li>
<li>Bug fix for forward refs in generics by <a href="https://github.com/mark-todd"><code>@​mark-todd</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6157">pydantic/pydantic#6157</a></li>
<li>Add Pydantic <code>Json</code> field support to settings management by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/6250">pydantic/pydantic#6250</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/K900"><code>@​K900</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/6103">pydantic/pydantic#6103</a></li>
<li><a href="https://github.com/markus1978"><code>@​markus1978</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/6194">pydantic/pydantic#6194</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.9...v1.10.10">https://github.com/pydantic/pydantic/compare/v1.10.9...v1.10.10</a></p>
<h2>V1.10.9</h2>
<h2>What's Changed</h2>
<ul>
<li>Add Pydantic classifier by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/5847">pydantic/pydantic#5847</a></li>
<li>📌 Use Cython &lt; v3 by <a href="https://github.com/lig"><code>@​lig</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/5845">pydantic/pydantic#5845</a></li>
<li>[cherry-pick] Fix mypy plugin for 1.4.0 (<a href="https://redirect.github.com/pydantic/pydantic/issues/5927">#5927</a>) by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/5928">pydantic/pydantic#5928</a></li>
<li>Add future and past date hypothesis strategies by <a href="https://github.com/bschoenmaeckers"><code>@​bschoenmaeckers</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/5850">pydantic/pydantic#5850</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.13 (2023-09-27)</h2>
<ul>
<li>Fix: Add max length check to <code>pydantic.validate_email</code>, <a href="https://redirect.github.com/pydantic/pydantic/issues/7673">#7673</a> by <a href="https://github.com/hramezani"><code>@​hramezani</code></a></li>
<li>Docs: Fix pip commands to install v1, <a href="https://redirect.github.com/pydantic/pydantic/issues/6930">#6930</a> by <a href="https://github.com/chbndrhnns"><code>@​chbndrhnns</code></a></li>
</ul>
<h2>v1.10.12 (2023-07-24)</h2>
<ul>
<li>Fixes the <code>maxlen</code> property being dropped on <code>deque</code> validation. Happened only if the deque item has been typed. Changes the <code>_validate_sequence_like</code> func, <a href="https://redirect.github.com/pydantic/pydantic/pull/6581">#6581</a> by <a href="https://github.com/maciekglowka"><code>@​maciekglowka</code></a></li>
</ul>
<h2>v1.10.11 (2023-07-04)</h2>
<ul>
<li>Importing create_model in tools.py through relative path instead of absolute path - so that it doesn't import V2 code when copied over to V2 branch, <a href="https://redirect.github.com/pydantic/pydantic/pull/6361">#6361</a> by <a href="https://github.com/SharathHuddar"><code>@​SharathHuddar</code></a></li>
</ul>
<h2>v1.10.10 (2023-06-30)</h2>
<ul>
<li>Add Pydantic <code>Json</code> field support to settings management, <a href="https://redirect.github.com/pydantic/pydantic/pull/6250">#6250</a> by <a href="https://github.com/hramezani"><code>@​hramezani</code></a></li>
<li>Fixed literal validator errors for unhashable values, <a href="https://redirect.github.com/pydantic/pydantic/pull/6188">#6188</a> by <a href="https://github.com/markus1978"><code>@​markus1978</code></a></li>
<li>Fixed bug with generics receiving forward refs, <a href="https://redirect.github.com/pydantic/pydantic/pull/6130">#6130</a> by <a href="https://github.com/mark-todd"><code>@​mark-todd</code></a></li>
<li>Update install method of FastAPI for internal tests in CI, <a href="https://redirect.github.com/pydantic/pydantic/pull/6117">#6117</a> by <a href="https://github.com/Kludex"><code>@​Kludex</code></a></li>
</ul>
<h2>v1.10.9 (2023-06-07)</h2>
<ul>
<li>Fix trailing zeros not ignored in Decimal validation, <a href="https://redirect.github.com/pydantic/pydantic/pull/5968">#5968</a> by <a href="https://github.com/hramezani"><code>@​hramezani</code></a></li>
<li>Fix mypy plugin for v1.4.0, <a href="https://redirect.github.com/pydantic/pydantic/pull/5928">#5928</a> by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a></li>
<li>Add future and past date hypothesis strategies, <a href="https://redirect.github.com/pydantic/pydantic/pull/5850">#5850</a> by <a href="https://github.com/bschoenmaeckers"><code>@​bschoenmaeckers</code></a></li>
<li>Discourage usage of Cython 3 with Pydantic 1.x, <a href="https://redirect.github.com/pydantic/pydantic/pull/5845">#5845</a> by <a href="https://github.com/lig"><code>@​lig</code></a></li>
</ul>
<h2>v1.10.8 (2023-05-23)</h2>
<ul>
<li>Fix a bug in <code>Literal</code> usage with <code>typing-extension==4.6.0</code>, <a href="https://redirect.github.com/pydantic/pydantic/pull/5826">#5826</a> by <a href="https://github.com/hramezani"><code>@​hramezani</code></a></li>
<li>This solves the (closed) issue <a href="https://redirect.github.com/pydantic/pydantic/pull/3849">#3849</a> where aliased fields that use discriminated union fail to validate when the data contains the non-aliased field name, <a href="https://redirect.github.com/pydantic/pydantic/pull/5736">#5736</a> by <a href="https://github.com/benwah"><code>@​benwah</code></a></li>
<li>Update email-validator dependency to &gt;=2.0.0post2, <a href="https://redirect.github.com/pydantic/pydantic/pull/5627">#5627</a> by <a href="https://github.com/adriangb"><code>@​adriangb</code></a></li>
<li>update <code>AnyClassMethod</code> for changes in <a href="https://redirect.github.com/python/typeshed/issues/9771">python/typeshed#9771</a>, <a href="https://redirect.github.com/pydantic/pydantic/pull/5505">#5505</a> by <a href="https://github.com/ITProKyle"><code>@​ITProKyle</code></a></li>
</ul>
<h2>v1.10.7 (2023-03-22)</h2>
<ul>
<li>Fix creating schema from model using <code>ConstrainedStr</code> with <code>regex</code> as dict key, <a href="https://redirect.github.com/pydantic/pydantic/pull/5223">#5223</a> by <a href="https://github.com/matejetz"><code>@​matejetz</code></a></li>
<li>Address bug in mypy plugin caused by explicit_package_bases=True, <a href="https://redirect.github.com/pydantic/pydantic/pull/5191">#5191</a> by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a></li>
<li>Add implicit defaults in the mypy plugin for Field with no default argument, <a href="https://redirect.github.com/pydantic/pydantic/pull/5190">#5190</a> by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a></li>
<li>Fix schema generated for Enum values used as Literals in discriminated unions, <a href="https://redirect.github.com/pydantic/pydantic/pull/5188">#5188</a> by <a href="https://github.com/javibookline"><code>@​javibookline</code></a></li>
<li>Fix mypy failures caused by the pydantic mypy plugin when users define <code>from_orm</code> in their own classes, <a href="https://redirect.github.com/pydantic/pydantic/pull/5187">#5187</a> by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a></li>
<li>Fix <code>InitVar</code> usage with pydantic dataclasses, mypy version <code>1.1.1</code> and the custom mypy plugin, <a href="https://redirect.github.com/pydantic/pydantic/pull/5162">#5162</a> by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a></li>
</ul>
<h2>v1.10.6 (2023-03-08)</h2>
<ul>
<li>Implement logic to support creating validators from non standard callables by using defaults to identify them and unwrapping <code>functools.partial</code> and <code>functools.partialmethod</code> when checking the signature, <a href="https://redirect.github.com/pydantic/pydantic/pull/5126">#5126</a> by <a href="https://github.com/JensHeinrich"><code>@​JensHeinrich</code></a></li>
<li>Fix mypy plugin for v1.1.1, and fix <code>dataclass_transform</code> decorator for pydantic dataclasses, <a href="https://redirect.github.com/pydantic/pydantic/pull/5111">#5111</a> by <a href="https://github.com/cdce8p"><code>@​cdce8p</code></a></li>
<li>Raise <code>ValidationError</code>, not <code>ConfigError</code>, when a discriminator value is unhashable, <a href="https://redirect.github.com/pydantic/pydantic/pull/4773">#4773</a> by <a href="https://github.com/kurtmckee"><code>@​kurtmckee</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/8822578619bf8d0bb754b1cf7a2a905b50240d01"><code>8822578</code></a> Prepare release 1.10.13 (<a href="https://redirect.github.com/pydantic/pydantic/issues/7674">#7674</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/59d8f38fd6220e3917c53785dbc70317d6f8e631"><code>59d8f38</code></a> [Backport] Add max length check to <code>validate_email</code> (<a href="https://redirect.github.com/pydantic/pydantic/issues/7673">#7673</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/69b92b547f7f268f7914d3346b57c59a0d550e42"><code>69b92b5</code></a> Make the v1 mypy plugin work with both v1 and v2 (<a href="https://redirect.github.com/pydantic/pydantic/issues/6920">#6920</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/87bf41755fe59082abf8352a2cf8c2889ee0849f"><code>87bf417</code></a> Update pip commands to install 1.10 (<a href="https://redirect.github.com/pydantic/pydantic/issues/6930">#6930</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/d9c2af3a701ca982945a590de1a1da98b3fb4003"><code>d9c2af3</code></a> Prepare release 1.10.12 (<a href="https://redirect.github.com/pydantic/pydantic/issues/6825">#6825</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/2aaddf6d692a6a467a401fae5840435c5459aa1b"><code>2aaddf6</code></a> Deque's maxlen property dropped on V1 validation (<a href="https://redirect.github.com/pydantic/pydantic/issues/6586">#6586</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/15c82d978d9e3b3893f00982b9e0c5c8d5c7821d"><code>15c82d9</code></a> Prepare for 1.10.11 (<a href="https://redirect.github.com/pydantic/pydantic/issues/6420">#6420</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/8750c37a553f5107562722605369fcd2cb7cdaa3"><code>8750c37</code></a> no longer tag docs release as latest</li>
<li><a href="https://github.com/pydantic/pydantic/commit/2c0e2a6d8a961ce320915302caadbb31cc565983"><code>2c0e2a6</code></a> Fix import of create_model in tools.py (<a href="https://redirect.github.com/pydantic/pydantic/issues/6364">#6364</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/0e8a387d6752dd859676da53298601ccae6a23a7"><code>0e8a387</code></a> Prepare for 1.10.10 (<a href="https://redirect.github.com/pydantic/pydantic/issues/6308">#6308</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pydantic/pydantic/compare/v1.10.5...v1.10.13">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic&package-manager=pip&previous-version=1.10.5&new-version=1.10.13)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 05:31:47 +0000 UTC
    </div>
</div>

