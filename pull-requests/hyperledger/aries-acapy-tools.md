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
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump the pip group with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 3 updates: [pydantic](https://github.com/pydantic/pydantic), [requests](https://github.com/psf/requests) and [urllib3](https://github.com/urllib3/urllib3).

Updates `pydantic` from 1.10.5 to 1.10.13
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

Updates `requests` from 2.31.0 to 2.32.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>v2.32.0</h2>
<h2>2.32.0 (2024-05-20)</h2>
<h2>🐍 PYCON US 2024 EDITION 🐍</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li><a href="https://github.com/psf/requests/commit/d6ebc4a2f1f68b7e355fb7e4dd5ffc0845547f9f"><code>d6ebc4a</code></a> v2.32.0</li>
<li><a href="https://github.com/psf/requests/commit/9a40d1277807f0a4f26c9a37eea8ec90faa8aadc"><code>9a40d12</code></a> Avoid reloading root certificates to improve concurrent performance (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li><a href="https://github.com/psf/requests/commit/0c030f78d24f29a459dbf39b28b4cc765e2153d7"><code>0c030f7</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a> from nateprewitt/no_char_detection</li>
<li><a href="https://github.com/psf/requests/commit/555b870eb19d497ddb67042645420083ec8efb02"><code>555b870</code></a> Allow character detection dependencies to be optional in post-packaging steps</li>
<li><a href="https://github.com/psf/requests/commit/d6dded3f00afcf56a7e866cb0732799045301eb0"><code>d6dded3</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6700">#6700</a> from franekmagiera/update-redirect-to-invalid-uri-test</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.31.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />

Updates `urllib3` from 1.26.18 to 1.26.19
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.19</h2>
<h2>🚀 urllib3 is fundraising for HTTP/2 support</h2>
<p><a href="https://sethmlarson.dev/urllib3-is-fundraising-for-http2-support">urllib3 is raising ~$40,000 USD</a> to release HTTP/2 support and ensure long-term sustainable maintenance of the project after a sharp decline in financial support for 2023. If your company or organization uses Python and would benefit from HTTP/2 support in Requests, pip, cloud SDKs, and thousands of other projects <a href="https://opencollective.com/urllib3">please consider contributing financially</a> to ensure HTTP/2 support is developed sustainably and maintained for the long-haul.</p>
<p>Thank you for your support.</p>
<h2>Changes</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/urllib3/urllib3/compare/1.26.18...1.26.19">https://github.com/urllib3/urllib3/compare/1.26.18...1.26.19</a></p>
<p>Note that due to an issue with our release automation, no <code> multiple.intoto.jsonl</code> file is available for this release.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/1.26.19/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h2>1.26.19 (2024-06-17)</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Fixed handling of OpenSSL 3.2.0 new error message for misconfiguring an HTTP proxy as HTTPS. (<code>[#3405](https://github.com/urllib3/urllib3/issues/3405) &lt;https://github.com/urllib3/urllib3/issues/3405&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/d9d85c88aa644af56d5e129634e750ce76e1a765"><code>d9d85c8</code></a> Release 1.26.19</li>
<li><a href="https://github.com/urllib3/urllib3/commit/8528b63b6fe5cfd7b21942cf988670de68fcd8c0"><code>8528b63</code></a> [1.26] Fix downstream tests (<a href="https://redirect.github.com/urllib3/urllib3/issues/3409">#3409</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/40b6d1605814dd1db0a46e202d6e56f2e4c9a468"><code>40b6d16</code></a> Merge pull request from GHSA-34jh-p97f-mpxf</li>
<li><a href="https://github.com/urllib3/urllib3/commit/29cfd02f66376c61bd20f1725477925106321f68"><code>29cfd02</code></a> Fix handling of OpenSSL 3.2.0 new error message &quot;record layer failure&quot; (<a href="https://redirect.github.com/urllib3/urllib3/issues/3405">#3405</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b60064388302f54a3455259ddab121618650a154"><code>b600643</code></a> [1.26] Bump RECENT_DATE (<a href="https://redirect.github.com/urllib3/urllib3/issues/3404">#3404</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/7e2d3890926d4788e219f63e2e36fbeb8714827f"><code>7e2d389</code></a> [1.26] Fix running CPython 2.7 tests in CI (<a href="https://redirect.github.com/urllib3/urllib3/issues/3137">#3137</a>)</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/1.26.18...1.26.19">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 01:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    build(deps): Bump the all-actions group across 1 directory with 6 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps the all-actions group with 6 updates in the / directory:

| Package | From | To |
| --- | --- | --- |
| [actions/checkout](https://github.com/actions/checkout) | `3` | `4` |
| [actions/cache](https://github.com/actions/cache) | `3` | `4` |
| [docker/setup-buildx-action](https://github.com/docker/setup-buildx-action) | `2` | `3` |
| [docker/login-action](https://github.com/docker/login-action) | `2` | `3` |
| [docker/metadata-action](https://github.com/docker/metadata-action) | `4` | `5` |
| [docker/build-push-action](https://github.com/docker/build-push-action) | `3` | `6` |


Updates `actions/checkout` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/releases">actions/checkout's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li>Support fetching without the --progress option by <a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
<li>Release 4.0.0 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1447">actions/checkout#1447</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li><a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v4.0.0">https://github.com/actions/checkout/compare/v3...v4.0.0</a></p>
<h2>v3.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Mark test scripts with Bash'isms to be run via Bash by <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1377">actions/checkout#1377</a></li>
<li>Add option to fetch tags even if fetch-depth &gt; 0 by <a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li>Release 3.6.0 by <a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li><a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.3...v3.6.0">https://github.com/actions/checkout/compare/v3.5.3...v3.6.0</a></p>
<h2>v3.5.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Checkout Issue in self hosted runner due to faulty submodule check-ins by <a href="https://github.com/megamanics"><code>@​megamanics</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li>Fix typos found by codespell by <a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li>Add support for sparse checkouts by <a href="https://github.com/dscho"><code>@​dscho</code></a> and <a href="https://github.com/dfdez"><code>@​dfdez</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
<li>Release v3.5.3 by <a href="https://github.com/TingluoHuang"><code>@​TingluoHuang</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1376">actions/checkout#1376</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/megamanics"><code>@​megamanics</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li><a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li><a href="https://github.com/dfdez"><code>@​dfdez</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v3.5.3">https://github.com/actions/checkout/compare/v3...v3.5.3</a></p>
<h2>v3.5.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Use correct API url / endpoint in GHES by <a href="https://github.com/fhammerl"><code>@​fhammerl</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1289">actions/checkout#1289</a> based on <a href="https://redirect.github.com/actions/checkout/issues/1286">#1286</a> by <a href="https://github.com/1newsr"><code>@​1newsr</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.1...v3.5.2">https://github.com/actions/checkout/compare/v3.5.1...v3.5.2</a></p>
<h2>v3.5.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Improve checkout performance on Windows runners by upgrading <code>@​actions/github</code> dependency by <a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/blob/main/CHANGELOG.md">actions/checkout's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v4.1.7</h2>
<ul>
<li>Bump the minor-npm-dependencies group across 1 directory with 4 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1739">actions/checkout#1739</a></li>
<li>Bump actions/checkout from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1697">actions/checkout#1697</a></li>
<li>Check out other refs/* by commit by <a href="https://github.com/orhantoy"><code>@​orhantoy</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1774">actions/checkout#1774</a></li>
<li>Pin actions/checkout's own workflows to a known, good, stable version. by <a href="https://github.com/jww3"><code>@​jww3</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1776">actions/checkout#1776</a></li>
</ul>
<h2>v4.1.6</h2>
<ul>
<li>Check platform to set archive extension appropriately by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1732">actions/checkout#1732</a></li>
</ul>
<h2>v4.1.5</h2>
<ul>
<li>Update NPM dependencies by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1703">actions/checkout#1703</a></li>
<li>Bump github/codeql-action from 2 to 3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1694">actions/checkout#1694</a></li>
<li>Bump actions/setup-node from 1 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1696">actions/checkout#1696</a></li>
<li>Bump actions/upload-artifact from 2 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1695">actions/checkout#1695</a></li>
<li>README: Suggest <code>user.email</code> to be <code>41898282+github-actions[bot]@users.noreply.github.com</code> by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1707">actions/checkout#1707</a></li>
</ul>
<h2>v4.1.4</h2>
<ul>
<li>Disable <code>extensions.worktreeConfig</code> when disabling <code>sparse-checkout</code> by <a href="https://github.com/jww3"><code>@​jww3</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1692">actions/checkout#1692</a></li>
<li>Add dependabot config by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1688">actions/checkout#1688</a></li>
<li>Bump the minor-actions-dependencies group with 2 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1693">actions/checkout#1693</a></li>
<li>Bump word-wrap from 1.2.3 to 1.2.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1643">actions/checkout#1643</a></li>
</ul>
<h2>v4.1.3</h2>
<ul>
<li>Check git version before attempting to disable <code>sparse-checkout</code> by <a href="https://github.com/jww3"><code>@​jww3</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1656">actions/checkout#1656</a></li>
<li>Add SSH user parameter by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1685">actions/checkout#1685</a></li>
<li>Update <code>actions/checkout</code> version in <code>update-main-version.yml</code> by <a href="https://github.com/jww3"><code>@​jww3</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1650">actions/checkout#1650</a></li>
</ul>
<h2>v4.1.2</h2>
<ul>
<li>Fix: Disable sparse checkout whenever <code>sparse-checkout</code> option is not present <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1598">actions/checkout#1598</a></li>
</ul>
<h2>v4.1.1</h2>
<ul>
<li>Correct link to GitHub Docs by <a href="https://github.com/peterbe"><code>@​peterbe</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1511">actions/checkout#1511</a></li>
<li>Link to release page from what's new section by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1514">actions/checkout#1514</a></li>
</ul>
<h2>v4.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1396">Add support for partial checkout filters</a></li>
</ul>
<h2>v4.0.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1067">Support fetching without the --progress option</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1436">Update to node20</a></li>
</ul>
<h2>v3.6.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1377">Fix: Mark test scripts with Bash'isms to be run via Bash</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/579">Add option to fetch tags even if fetch-depth &gt; 0</a></li>
</ul>
<h2>v3.5.3</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1196">Fix: Checkout fail in self-hosted runners when faulty submodule are checked-in</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1287">Fix typos found by codespell</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/692973e3d937129bcbf40652eb9f2f61becf3332"><code>692973e</code></a> Prepare 4.1.7 release (<a href="https://redirect.github.com/actions/checkout/issues/1775">#1775</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/6ccd57f4c5d15bdc2fef309bd9fb6cc9db2ef1c6"><code>6ccd57f</code></a> Pin actions/checkout's own workflows to a known, good, stable version. (<a href="https://redirect.github.com/actions/checkout/issues/1776">#1776</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/b17fe1e4d59a9d1d95a7aead5e6fcd13e50939a5"><code>b17fe1e</code></a> Handle hidden refs (<a href="https://redirect.github.com/actions/checkout/issues/1774">#1774</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/b80ff79f1755d06ba70441c368a6fe801f5f3a62"><code>b80ff79</code></a> Bump actions/checkout from 3 to 4 (<a href="https://redirect.github.com/actions/checkout/issues/1697">#1697</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/b1ec3021b8fa02164da82ca1557d017d83b0e179"><code>b1ec302</code></a> Bump the minor-npm-dependencies group across 1 directory with 4 updates (<a href="https://redirect.github.com/actions/checkout/issues/1739">#1739</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/a5ac7e51b41094c92402da3b24376905380afc29"><code>a5ac7e5</code></a> Update for 4.1.6 release (<a href="https://redirect.github.com/actions/checkout/issues/1733">#1733</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/24ed1a352802348c9e4e8d13de9177fb95b537ba"><code>24ed1a3</code></a> Check platform for extension (<a href="https://redirect.github.com/actions/checkout/issues/1732">#1732</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/44c2b7a8a4ea60a981eaca3cf939b5f4305c123b"><code>44c2b7a</code></a> README: Suggest <code>user.email</code> to be `41898282+github-actions[bot]<a href="https://github.com/users"><code>@​users</code></a>.norepl...</li>
<li><a href="https://github.com/actions/checkout/commit/8459bc0c7e3759cdf591f513d9f141a95fef0a8f"><code>8459bc0</code></a> Bump actions/upload-artifact from 2 to 4 (<a href="https://redirect.github.com/actions/checkout/issues/1695">#1695</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/3f603f6d5e9f40714f97b2f017aa0df2a443192a"><code>3f603f6</code></a> Bump actions/setup-node from 1 to 4 (<a href="https://redirect.github.com/actions/checkout/issues/1696">#1696</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/checkout/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/cache` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/releases">actions/cache's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update action to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li>feat: save-always flag by <a href="https://github.com/to-s"><code>@​to-s</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li><a href="https://github.com/to-s"><code>@​to-s</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v4.0.0">https://github.com/actions/cache/compare/v3...v4.0.0</a></p>
<h2>v3.3.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Cache v3.3.3 by <a href="https://github.com/robherley"><code>@​robherley</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/robherley"><code>@​robherley</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.3">https://github.com/actions/cache/compare/v3...v3.3.3</a></p>
<h2>v3.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fixed readme with new segment timeout values by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1133">actions/cache#1133</a></li>
<li>Readme fixes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1134">actions/cache#1134</a></li>
<li>Updated description of the lookup-only input for main action by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1130">actions/cache#1130</a></li>
<li>Change two new actions mention as quoted text by <a href="https://github.com/bishal-pdMSFT"><code>@​bishal-pdMSFT</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1131">actions/cache#1131</a></li>
<li>Update Cross-OS Caching tips by <a href="https://github.com/pdotl"><code>@​pdotl</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1122">actions/cache#1122</a></li>
<li>Bazel example (Take <a href="https://redirect.github.com/actions/cache/issues/2">#2</a>️⃣) by <a href="https://github.com/vorburger"><code>@​vorburger</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li>Remove actions to add new PRs and issues to a project board by <a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li>Consume latest toolkit and fix dangling promise bug by <a href="https://github.com/chkimes"><code>@​chkimes</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li>Bump action version to 3.3.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vorburger"><code>@​vorburger</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li><a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li><a href="https://github.com/chkimes"><code>@​chkimes</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li><a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.2">https://github.com/actions/cache/compare/v3...v3.3.2</a></p>
<h2>v3.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Reduced download segment size to 128 MB and timeout to 10 minutes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1129">actions/cache#1129</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.1">https://github.com/actions/cache/compare/v3...v3.3.1</a></p>
<h2>v3.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bug: Permission is missing in cache delete example by <a href="https://github.com/kotokaze"><code>@​kotokaze</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1123">actions/cache#1123</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/blob/main/RELEASES.md">actions/cache's changelog</a>.</em></p>
<blockquote>
<h1>Releases</h1>
<h3>4.0.2</h3>
<ul>
<li>Fixed restore <code>fail-on-cache-miss</code> not working.</li>
</ul>
<h3>4.0.1</h3>
<ul>
<li>Updated <code>isGhes</code> check</li>
</ul>
<h3>4.0.0</h3>
<ul>
<li>Updated minimum runner version support from node 12 -&gt; node 20</li>
</ul>
<h3>3.3.3</h3>
<ul>
<li>Updates <code>@​actions/cache</code> to v3.2.3 to fix accidental mutated path arguments to <code>getCacheVersion</code> <a href="https://redirect.github.com/actions/toolkit/pull/1378">actions/toolkit#1378</a></li>
<li>Additional audit fixes of npm package(s)</li>
</ul>
<h3>3.3.2</h3>
<ul>
<li>Fixes bug with Azure SDK causing blob downloads to get stuck.</li>
</ul>
<h3>3.3.1</h3>
<ul>
<li>Reduced segment size to 128MB and segment timeout to 10 minutes to fail fast in case the cache download is stuck.</li>
</ul>
<h3>3.3.0</h3>
<ul>
<li>Added option to lookup cache without downloading it.</li>
</ul>
<h3>3.2.6</h3>
<ul>
<li>Fix zstd not being used after zstd version upgrade to 1.5.4 on hosted runners.</li>
</ul>
<h3>3.2.5</h3>
<ul>
<li>Added fix to prevent from setting MYSYS environment variable globally.</li>
</ul>
<h3>3.2.4</h3>
<ul>
<li>Added option to fail job on cache miss.</li>
</ul>
<h3>3.2.3</h3>
<ul>
<li>Support cross os caching on Windows as an opt-in feature.</li>
<li>Fix issue with symlink restoration on Windows for cross-os caches.</li>
</ul>
<h3>3.2.2</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/cache/commit/0c45773b623bea8c8e75f6c82b208c3cf94ea4f9"><code>0c45773</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1327">#1327</a> from cdce8p/fix-fail-on-cache-miss</li>
<li><a href="https://github.com/actions/cache/commit/8a55f839aa4b4578e47bdc8a52828637cbb9a454"><code>8a55f83</code></a> Add test case for process exit</li>
<li><a href="https://github.com/actions/cache/commit/3884cace147bdf9307fcc52a277f421af7b30798"><code>3884cac</code></a> Bump version</li>
<li><a href="https://github.com/actions/cache/commit/e29dad3e36390db18fc19fb666cb1302f4929002"><code>e29dad3</code></a> Fix fail-on-cache-miss not working</li>
<li><a href="https://github.com/actions/cache/commit/ab5e6d0c87105b4c9c2047343972218f562e4319"><code>ab5e6d0</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1341">#1341</a> from bethanyj28/main</li>
<li><a href="https://github.com/actions/cache/commit/89c7d86c71006451e399dfcc588eed8e392e0dcf"><code>89c7d86</code></a> licensed cache</li>
<li><a href="https://github.com/actions/cache/commit/d2c84da363007d814e47d50565ba3794c1a84c56"><code>d2c84da</code></a> update <code>@​actions/cache</code></li>
<li><a href="https://github.com/actions/cache/commit/37e7d4eb166540050942d75a6e40742cbfc92f65"><code>37e7d4e</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1340">#1340</a> from actions/bethanyj28/update-publish-flow</li>
<li><a href="https://github.com/actions/cache/commit/a18323f50430a57f9094db3ce508dc1e3a25d4a2"><code>a18323f</code></a> add release action</li>
<li><a href="https://github.com/actions/cache/commit/a2ed59d39b352305bdd2f628719a53b2cc4f9613"><code>a2ed59d</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1305">#1305</a> from actions/yacaovsnc/update_examples</li>
<li>Additional commits viewable in <a href="https://github.com/actions/cache/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/setup-buildx-action` from 2 to 3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/setup-buildx-action/releases">docker/setup-buildx-action's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/264">docker/setup-buildx-action#264</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/267">docker/setup-buildx-action#267</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.10.0...v3.0.0">https://github.com/docker/setup-buildx-action/compare/v2.10.0...v3.0.0</a></p>
<h2>v2.10.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.7.1 to 0.10.0 by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/258">docker/setup-buildx-action#258</a></li>
<li>Bump word-wrap from 1.2.3 to 1.2.5 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/253">docker/setup-buildx-action#253</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.9.1...v2.10.0">https://github.com/docker/setup-buildx-action/compare/v2.9.1...v2.10.0</a></p>
<h2>v2.9.1</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.7.0 to 0.7.1 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/248">docker/setup-buildx-action#248</a>
<ul>
<li>Fixes an issue where building Buildx does not match the local platform (<a href="https://redirect.github.com/docker/actions-toolkit/pull/135">docker/actions-toolkit#135</a>)</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.9.0...v2.9.1">https://github.com/docker/setup-buildx-action/compare/v2.9.0...v2.9.1</a></p>
<h2>v2.9.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.6.0 to 0.7.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/246">docker/setup-buildx-action#246</a>
<ul>
<li>Adds support to cache Buildx binary to hosted tool cache and GHA cache backend</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.8.0...v2.9.0">https://github.com/docker/setup-buildx-action/compare/v2.8.0...v2.9.0</a></p>
<h2>v2.8.0</h2>
<ul>
<li>Only set specific flags for drivers supporting them by <a href="https://github.com/nicks"><code>@​nicks</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/241">docker/setup-buildx-action#241</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.5.0 to 0.6.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/242">docker/setup-buildx-action#242</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.7.0...v2.8.0">https://github.com/docker/setup-buildx-action/compare/v2.7.0...v2.8.0</a></p>
<h2>v2.7.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/237">docker/setup-buildx-action#237</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/238">docker/setup-buildx-action#238</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.6.0...v2.7.0">https://github.com/docker/setup-buildx-action/compare/v2.6.0...v2.7.0</a></p>
<h2>v2.6.0</h2>
<ul>
<li>Set node name for k8s driver when appending nodes by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/219">docker/setup-buildx-action#219</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.1.0-beta.18 to 0.3.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/220">docker/setup-buildx-action#220</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/229">docker/setup-buildx-action#229</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/231">docker/setup-buildx-action#231</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/236">docker/setup-buildx-action#236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.5.0...v2.6.0">https://github.com/docker/setup-buildx-action/compare/v2.5.0...v2.6.0</a></p>
<h2>v2.5.0</h2>
<ul>
<li><code>cleanup</code> input to remove builder and temp files by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/213">docker/setup-buildx-action#213</a></li>
<li>do not remove builder using the <code>docker</code> driver by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/218">docker/setup-buildx-action#218</a></li>
<li>fix current context as builder name for <code>docker</code> driver by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/209">docker/setup-buildx-action#209</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.4.1...v2.5.0">https://github.com/docker/setup-buildx-action/compare/v2.4.1...v2.5.0</a></p>
<h2>v2.4.1</h2>
<ul>
<li>Get releases from actions toolkit by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/setup-buildx-action/issues/200">#200</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/setup-buildx-action/commit/d70bba72b1f3fd22344832f00baa16ece964efeb"><code>d70bba7</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/307">#307</a> from crazy-max/bump-toolkit</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/7638634cb70c02d327dde3b558f22b0db32054a3"><code>7638634</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c68420fe0b4de2444121eec8f08bc2500c8d9216"><code>c68420f</code></a> bump <code>@​docker/actions-toolkit</code> from 0.19.0 to 0.20.0</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/2b51285047da1547ffb1b2203d8be4c0af6b1f20"><code>2b51285</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/306">#306</a> from docker/dependabot/npm_and_yarn/docker/actions-to...</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/0f00370563710ebfbdf4287b76a0a5d88864e7f9"><code>0f00370</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/11c9683db9ea73b2090280c1cfa7d725bd8a60fa"><code>11c9683</code></a> build(deps): bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/56a16b8f2aa74bcbd3ab9ec13027cd3ac8e3f94f"><code>56a16b8</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/303">#303</a> from crazy-max/fix-inputs</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c23f46eb919af18b86ac6f0f4646a63a7a452b4d"><code>c23f46e</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/f876da6242168c5bb185ad517fb42f0b59fba456"><code>f876da6</code></a> rename and align config inputs</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/b7cf918227e7a90a94eea8534a6b0cc1965a0ccd"><code>b7cf918</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/304">#304</a> from crazy-max/rm-docs-dir</li>
<li>Additional commits viewable in <a href="https://github.com/docker/setup-buildx-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/login-action` from 2 to 3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/login-action/releases">docker/login-action's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/login-action/pull/593">docker/login-action#593</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/login-action/pull/598">docker/login-action#598</a></li>
<li>Bump <code>@​aws-sdk/client-ecr</code> and <code>@​aws-sdk/client-ecr-public</code> to 3.410.0 in <a href="https://redirect.github.com/docker/login-action/pull/555">docker/login-action#555</a> <a href="https://redirect.github.com/docker/login-action/pull/560">docker/login-action#560</a> <a href="https://redirect.github.com/docker/login-action/pull/582">docker/login-action#582</a> <a href="https://redirect.github.com/docker/login-action/pull/599">docker/login-action#599</a></li>
<li>Bump semver from 6.3.0 to 6.3.1 in <a href="https://redirect.github.com/docker/login-action/pull/556">docker/login-action#556</a></li>
<li>Bump https-proxy-agent to 7.0.2 <a href="https://redirect.github.com/docker/login-action/pull/561">docker/login-action#561</a> <a href="https://redirect.github.com/docker/login-action/pull/588">docker/login-action#588</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.2.0...v3.0.0">https://github.com/docker/login-action/compare/v2.2.0...v3.0.0</a></p>
<h2>v2.2.0</h2>
<ul>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/login-action/pull/409">docker/login-action#409</a> <a href="https://redirect.github.com/docker/login-action/pull/470">docker/login-action#470</a> <a href="https://redirect.github.com/docker/login-action/pull/476">docker/login-action#476</a></li>
<li>Bump <code>@​aws-sdk/client-ecr</code> and <code>@​aws-sdk/client-ecr-public</code> to 3.347.1 in <a href="https://redirect.github.com/docker/login-action/pull/524">docker/login-action#524</a> <a href="https://redirect.github.com/docker/login-action/pull/364">docker/login-action#364</a> <a href="https://redirect.github.com/docker/login-action/pull/363">docker/login-action#363</a></li>
<li>Bump minimatch from 3.0.4 to 3.1.2 in <a href="https://redirect.github.com/docker/login-action/pull/354">docker/login-action#354</a></li>
<li>Bump json5 from 2.2.0 to 2.2.3 in <a href="https://redirect.github.com/docker/login-action/pull/378">docker/login-action#378</a></li>
<li>Bump http-proxy-agent from 5.0.0 to 7.0.0 in <a href="https://redirect.github.com/docker/login-action/pull/509">docker/login-action#509</a></li>
<li>Bump https-proxy-agent from 5.0.1 to 7.0.0 in <a href="https://redirect.github.com/docker/login-action/pull/508">docker/login-action#508</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.1.0...v2.2.0">https://github.com/docker/login-action/compare/v2.1.0...v2.2.0</a></p>
<h2>v2.1.0</h2>
<ul>
<li>Ensure AWS temp credentials are redacted in workflow logs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/login-action/issues/275">#275</a>)</li>
<li>Bump <code>@​actions/core</code> from 1.6.0 to 1.10.0 (<a href="https://redirect.github.com/docker/login-action/issues/252">#252</a> <a href="https://redirect.github.com/docker/login-action/issues/292">#292</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr</code> from 3.53.0 to 3.186.0 (<a href="https://redirect.github.com/docker/login-action/issues/298">#298</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr-public</code> from 3.53.0 to 3.186.0 (<a href="https://redirect.github.com/docker/login-action/issues/299">#299</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.0.0...v2.1.0">https://github.com/docker/login-action/compare/v2.0.0...v2.1.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/login-action/commit/0d4c9c5ea7693da7b068278f7b52bda2a190a446"><code>0d4c9c5</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/722">#722</a> from crazy-max/update-readme</li>
<li><a href="https://github.com/docker/login-action/commit/b29e14f6a983abc16efafe71e083f4b1ba2b1e5b"><code>b29e14f</code></a> add contributing section to README</li>
<li><a href="https://github.com/docker/login-action/commit/218a70c516af2f25cb9fc1e5a14a5a3576e7093f"><code>218a70c</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/721">#721</a> from docker/dependabot/npm_and_yarn/docker/actions-to...</li>
<li><a href="https://github.com/docker/login-action/commit/b8200806cfe29e3355c44f34309b26916aae48f6"><code>b820080</code></a> build(deps): bump <code>@​docker/actions-toolkit</code> from 0.23.0 to 0.24.0</li>
<li><a href="https://github.com/docker/login-action/commit/27530a9fbbe988616da1dc41b4a8072f949d8042"><code>27530a9</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/720">#720</a> from docker/dependabot/npm_and_yarn/aws-sdk-dependenc...</li>
<li><a href="https://github.com/docker/login-action/commit/d072a60421ee5ac6ee763e9306c27f92e8ce5a20"><code>d072a60</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/7c627b5124287958ac76b37cc2d94f1c9ef72aaa"><code>7c627b5</code></a> build(deps): bump the aws-sdk-dependencies group across 1 directory with 2 up...</li>
<li><a href="https://github.com/docker/login-action/commit/787cfc66231286ca823ebc099f52001f53aa8f42"><code>787cfc6</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/694">#694</a> from docker/dependabot/npm_and_yarn/undici-5.28.4</li>
<li><a href="https://github.com/docker/login-action/commit/8e66e916f8ed83b241171904f8e1b9e0a83070bc"><code>8e66e91</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/5ba5e97350e175e4c4e222569e6746675408a75c"><code>5ba5e97</code></a> build(deps): bump undici from 5.28.3 to 5.28.4</li>
<li>Additional commits viewable in <a href="https://github.com/docker/login-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/metadata-action` from 4 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/releases">docker/metadata-action's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/328">docker/metadata-action#328</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/metadata-action/pull/333">docker/metadata-action#333</a></li>
<li>Bump csv-parse from 5.4.0 to 5.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/320">docker/metadata-action#320</a></li>
<li>Bump semver from 7.5.1 to 7.5.2 in <a href="https://redirect.github.com/docker/metadata-action/pull/304">docker/metadata-action#304</a></li>
<li>Bump handlebars from 4.7.7 to 4.7.8 in <a href="https://redirect.github.com/docker/metadata-action/pull/315">docker/metadata-action#315</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.6.0...v5.0.0">https://github.com/docker/metadata-action/compare/v4.6.0...v5.0.0</a></p>
<h2>v4.6.0</h2>
<ul>
<li>Dedup and sort labels by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/301">docker/metadata-action#301</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/302">docker/metadata-action#302</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.5.0...v4.6.0">https://github.com/docker/metadata-action/compare/v4.5.0...v4.6.0</a></p>
<h2>v4.5.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.1.0 to 0.3.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/296">docker/metadata-action#296</a></li>
<li>Bump csv-parse from 5.3.8 to 5.4.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/294">docker/metadata-action#294</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.4.0...v4.5.0">https://github.com/docker/metadata-action/compare/v4.4.0...v4.5.0</a></p>
<h2>v4.4.0</h2>
<ul>
<li>Add <code>context</code> input to define the metadata provider by <a href="https://github.com/neilime"><code>@​neilime</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/248">docker/metadata-action#248</a></li>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/266">docker/metadata-action#266</a> <a href="https://redirect.github.com/docker/metadata-action/pull/273">docker/metadata-action#273</a> <a href="https://redirect.github.com/docker/metadata-action/pull/284">docker/metadata-action#284</a></li>
<li>Bump csv-parse from 5.3.3 to 5.3.8 in <a href="https://redirect.github.com/docker/metadata-action/pull/271">docker/metadata-action#271</a> <a href="https://redirect.github.com/docker/metadata-action/pull/286">docker/metadata-action#286</a></li>
<li>Bump moment-timezone from 0.5.40 to 0.5.43 in <a href="https://redirect.github.com/docker/metadata-action/pull/268">docker/metadata-action#268</a> <a href="https://redirect.github.com/docker/metadata-action/pull/278">docker/metadata-action#278</a> <a href="https://redirect.github.com/docker/metadata-action/pull/281">docker/metadata-action#281</a></li>
<li>Bump semver from 7.4.0 to 7.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/285">docker/metadata-action#285</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.3.0...v4.4.0">https://github.com/docker/metadata-action/compare/v4.3.0...v4.4.0</a></p>
<h2>v4.3.0</h2>
<ul>
<li>Provide outputs as env vars by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/257">#257</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.2.0...v4.3.0">https://github.com/docker/metadata-action/compare/v4.2.0...v4.3.0</a></p>
<h2>v4.2.0</h2>
<ul>
<li>Add <code>tz</code> attribute to handlebar date function by <a href="https://github.com/chroju"><code>@​chroju</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/251">#251</a>)</li>
<li>Bump minimatch from 3.0.4 to 3.1.2 (<a href="https://redirect.github.com/docker/metadata-action/issues/242">#242</a>)</li>
<li>Bump csv-parse from 5.3.1 to 5.3.3 (<a href="https://redirect.github.com/docker/metadata-action/issues/245">#245</a>)</li>
<li>Bump json5 from 2.2.0 to 2.2.3 (<a href="https://redirect.github.com/docker/metadata-action/issues/252">#252</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.1.1...v4.2.0">https://github.com/docker/metadata-action/compare/v4.1.1...v4.2.0</a></p>
<h2>v4.1.1</h2>
<ul>
<li>Revert changes to set associated head sha on pull request event by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/239">#239</a>)
<ul>
<li>User can still set associated head sha on PR by setting the env var <code>DOCKER_METADATA_PR_HEAD_SHA=true</code></li>
</ul>
</li>
<li>Bump csv-parse from 5.3.0 to 5.3.1 (<a href="https://redirect.github.com/docker/metadata-action/issues/237">#237</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.1.0...v4.1.1">https://github.com/docker/metadata-action/compare/v4.1.0...v4.1.1</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Upgrade guide</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/blob/master/UPGRADE.md">docker/metadata-action's upgrade guide</a>.</em></p>
<blockquote>
<h1>Upgrade notes</h1>
<h2>v2 to v3</h2>
<ul>
<li>Repository has been moved to docker org. Replace <code>crazy-max/ghaction-docker-meta@v2</code>
with <code>docker/metadata-action@v5</code></li>
<li>The default bake target has been changed: <code>ghaction-docker-meta</code> &gt; <code>docker-metadata-action</code></li>
</ul>
<h2>v1 to v2</h2>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#inputs">inputs</a>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-sha"><code>tag-sha</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-edge--tag-edge-branch"><code>tag-edge</code> / <code>tag-edge-branch</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-semver"><code>tag-semver</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-match--tag-match-group"><code>tag-match</code> / <code>tag-match-group</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-latest"><code>tag-latest</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-schedule"><code>tag-schedule</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-custom--tag-custom-only"><code>tag-custom</code> / <code>tag-custom-only</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#label-custom"><code>label-custom</code></a></li>
</ul>
</li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#basic-workflow">Basic workflow</a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#semver-workflow">Semver workflow</a></li>
</ul>
<h3>inputs</h3>
<table>
<thead>
<tr>
<th>New</th>
<th>Unchanged</th>
<th>Removed</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>tags</code></td>
<td><code>images</code></td>
<td><code>tag-sha</code></td>
</tr>
<tr>
<td><code>flavor</code></td>
<td><code>sep-tags</code></td>
<td><code>tag-edge</code></td>
</tr>
<tr>
<td><code>labels</code></td>
<td><code>sep-labels</code></td>
<td><code>tag-edge-branch</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-semver</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match-group</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-latest</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-schedule</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom-only</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>label-custom</code></td>
</tr>
</tbody>
</table>
<h4><code>tag-sha</code></h4>
<pre lang="yaml"><code>tags: |
  type=sha
</code></pre>
<h4><code>tag-edge</code> / <code>tag-edge-branch</code></h4>
<pre lang="yaml"><code>tags: |
  # default branch
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/metadata-action/commit/8e5442c4ef9f78752691e2d8f8d19755c6f78e81"><code>8e5442c</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/382">#382</a> from crazy-max/dont-set-cwd-prefix</li>
<li><a href="https://github.com/docker/metadata-action/commit/eda41b71bf54521bf493851a7dab9da9624655ac"><code>eda41b7</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/388c08f740dca49f310f648ea63c30046d49a255"><code>388c08f</code></a> don't set cwd:// prefix for local bake files</li>
<li><a href="https://github.com/docker/metadata-action/commit/dbef88086f6cef02e264edb7dbf63250c17cef6c"><code>dbef880</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/374">#374</a> from docker/dependabot/npm_and_yarn/moment-timezone-0...</li>
<li><a href="https://github.com/docker/metadata-action/commit/b73e7a71ace0f6ec603f2c5052d8304f33e5dbff"><code>b73e7a7</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/b9fba690eb63fbb6eee7f71bd710b75d4f0128c8"><code>b9fba69</code></a> chore(deps): Bump moment-timezone from 0.5.43 to 0.5.44</li>
<li><a href="https://github.com/docker/metadata-action/commit/ac82374ba6046fefd36df45f67cec12fa6ebeb75"><code>ac82374</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/373">#373</a> from docker/dependabot/npm_and_yarn/moment-2.30.1</li>
<li><a href="https://github.com/docker/metadata-action/commit/c92519a44ee7b643d904a587e47563f49f24b387"><code>c92519a</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/3b4179d34de6b2ba21a306f387c50672dbbe8612"><code>3b4179d</code></a> chore(deps): Bump moment from 2.29.4 to 2.30.1</li>
<li><a href="https://github.com/docker/metadata-action/commit/0784993ef80dda711a73b98a352e2b73c7feaf32"><code>0784993</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/371">#371</a> from docker/dependabot/npm_and_yarn/docker/actions-to...</li>
<li>Additional commits viewable in <a href="https://github.com/docker/metadata-action/compare/v4...v5">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/build-push-action` from 3 to 6
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v6.0.0</h2>
<ul>
<li>Export build record and generate <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">build summary</a> by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1120">docker/build-push-action#1120</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.24.0 to 0.26.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1132">docker/build-push-action#1132</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1136">docker/build-push-action#1136</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1138">docker/build-push-action#1138</a></li>
<li>Bump braces from 3.0.2 to 3.0.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1137">docker/build-push-action#1137</a></li>
</ul>
<blockquote>
<p>[!NOTE]
This major release adds support for generating <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">Build summary</a> and exporting build record for your build. You can disable this feature by setting <a href="https://docs.docker.com/build/ci/github-actions/build-summary/#disable-job-summary"> <code>DOCKER_BUILD_NO_SUMMARY: true</code> environment variable in your workflow</a>.</p>
</blockquote>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0">https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0</a></p>
<h2>v5.4.0</h2>
<ul>
<li>Show builder information before building by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1128">docker/build-push-action#1128</a></li>
<li>Handle attestations correctly with provenance and sbom inputs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1086">docker/build-push-action#1086</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.19.0 to 0.24.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1088">docker/build-push-action#1088</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1105">docker/build-push-action#1105</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1121">docker/build-push-action#1121</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1127">docker/build-push-action#1127</a></li>
<li>Bump undici from 5.28.3 to 5.28.4 in <a href="https://redirect.github.com/docker/build-push-action/pull/1090">docker/build-push-action#1090</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0">https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0</a></p>
<h2>v5.3.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1080">docker/build-push-action#1080</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0">https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0</a></p>
<h2>v5.2.0</h2>
<ul>
<li>Disable quotes detection for <code>outputs</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1074">docker/build-push-action#1074</a></li>
<li>Warn about ignored inputs by <a href="https://github.com/favonia"><code>@​favonia</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1019">docker/build-push-action#1019</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.14.0 to 0.18.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1070">docker/build-push-action#1070</a></li>
<li>Bump undici from 5.26.3 to 5.28.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1057">docker/build-push-action#1057</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0">https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0</a></p>
<h2>v5.1.0</h2>
<ul>
<li>Add <code>annotations</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/992">docker/build-push-action#992</a></li>
<li>Add <code>secret-envs</code> input by <a href="https://github.com/elias-lundgren"><code>@​elias-lundgren</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/980">docker/build-push-action#980</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.17.3 to 7.23.2 in <a href="https://redirect.github.com/docker/build-push-action/pull/991">docker/build-push-action#991</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.13.0-rc.1 to 0.14.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/990">docker/build-push-action#990</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1006">docker/build-push-action#1006</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0">https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0</a></p>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/954">docker/build-push-action#954</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/959">docker/build-push-action#959</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0">https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0</a></p>
<h2>v4.2.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/c382f710d39a5bb4e430307530a720f50c2d3318"><code>c382f71</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1120">#1120</a> from crazy-max/build-summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/5a5b70d974381b812e448a9ea8efef0c0781e8a7"><code>5a5b70d</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/dc24cf9e252ee3b05f80a1637b2950c11d305b3d"><code>dc24cf9</code></a> don't generate summary for cloud driver</li>
<li><a href="https://github.com/docker/build-push-action/commit/667cb22c52a8762431790112e70ef7f545dbf2d2"><code>667cb22</code></a> DOCKER_BUILD_NO_SUMMARY env to disable summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/d880b1964b626c7ac1763e83768e139202071136"><code>d880b19</code></a> generate build summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/e51051ad0baf1cdf23788f7f0980f675806b580e"><code>e51051a</code></a> export build record and upload artifact</li>
<li><a href="https://github.com/docker/build-push-action/commit/86c2bd00318427a320d2cee5bbc61251df6f647e"><code>86c2bd0</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1137">#1137</a> from docker/dependabot/npm_and_yarn/braces-3.0.3</li>
<li><a href="https://github.com/docker/build-push-action/commit/268d2b16117932ad41015c96fbc27a7641533625"><code>268d2b1</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1138">#1138</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/2b8dc7f52914dfdd416618a1f33d11277b7d64d2"><code>2b8dc7f</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/840c12be1707e3d7115f8d61da2c8b78442cc538"><code>840c12b</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.25.1 to 0.26.0</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v3...v6">compare view</a></li>
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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 12:15:33 +0000 UTC
    </div>
</div>

