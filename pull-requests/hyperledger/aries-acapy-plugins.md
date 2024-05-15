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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group across 6 directories with 6 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update in the /firebase_push_notifications directory: [black](https://github.com/psf/black).
Bumps the pip group with 1 update in the /kafka_events/demo/setup directory: [idna](https://github.com/kjd/idna).
Bumps the pip group with 1 update in the /kafka_events/integration directory: [black](https://github.com/psf/black).
Bumps the pip group with 1 update in the /kafka_events/kafka_events/v1_0/deliverer directory: [idna](https://github.com/kjd/idna).
Bumps the pip group with 4 updates in the /oid4vci/integration/afj_runner directory: [idna](https://github.com/kjd/idna), [aiohttp](https://github.com/aio-libs/aiohttp), [pydantic](https://github.com/pydantic/pydantic) and [black](https://github.com/psf/black).
Bumps the pip group with 5 updates in the /redis_events/docker/services directory:

| Package | From | To |
| --- | --- | --- |
| [idna](https://github.com/kjd/idna) | `3.4` | `3.7` |
| [aiohttp](https://github.com/aio-libs/aiohttp) | `3.9.2` | `3.9.4` |
| [pydantic](https://github.com/pydantic/pydantic) | `1.10.13` | `2.7.1` |
| [black](https://github.com/psf/black) | `21.12b0` | `24.3.0` |
| [fastapi](https://github.com/tiangolo/fastapi) | `0.109.1` | `0.111.0` |


Updates `black` from 23.7.0 to 24.3.0
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

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `black` from 21.12b0 to 24.3.0
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

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `aiohttp` from 3.9.2 to 3.9.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.4</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8089">#8089</a>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8104">#8104</a>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8163">#8163</a>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7741">#7741</a>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/master/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.9.4 (2024-04-11)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8089</code>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8104</code>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8163</code>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7741</code>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b3397c7ac44fc80206d28f1dd0d1f3b10c4ec572"><code>b3397c7</code></a> Release v3.9.4 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8201">#8201</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a7e240a9f625a0b9559bdf5f0049c71565352400"><code>a7e240a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8320">#8320</a>/9ba9a4e5 backport][3.9] Fix Python parser to mark responses without...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/28335525d1eac015a7e7584137678cbb6ff19397"><code>2833552</code></a> Escape filenames and paths in HTML when generating index pages (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8317">#8317</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8319">#8319</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ed43040613988fc4666109aca82a5180ff165df5"><code>ed43040</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8309">#8309</a>/c29945a1 backport][3.9] Improve reliability of run_app test (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8315">#8315</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ec2be0500e2674eea019c0966a7a905e9b3d6608"><code>ec2be05</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8299">#8299</a>/28d026eb backport][3.9] Create marker for internal tests (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8307">#8307</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/292d961f4ee2829a1b13fad92444a4fd693fbc87"><code>292d961</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8304">#8304</a>/88c80c14 backport][3.9] Check for backports in CI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8305">#8305</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cebe526b9c34dc3a3da9140409db63014bc4cf19"><code>cebe526</code></a> Fix handling of multipart/form-data (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8280">#8280</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8302">#8302</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/270ae9cf6a9e6159b5e29a950deb6ff7600aebc5"><code>270ae9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8297">#8297</a>/d15f07cf backport][3.9] Upgrade to llhttp 9.2.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8292">#8292</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8298">#8298</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bb231059b14277c34a8a0331e51406d5abe4f424"><code>bb23105</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8283">#8283</a>/54e13b0a backport][3.9] Fix blocking I/O in the event loop while pr...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3f79241bcbc02c9850348fc04c064fcbc980e8f0"><code>3f79241</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8286">#8286</a>/28f1fd88 backport][3.9] docs: remove repetitive word in comment (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8">#8</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.2...v3.9.4">compare view</a></li>
</ul>
</details>
<br />

Updates `pydantic` from 1.10.13 to 1.10.15
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.15</h2>
<h2>What's Changed</h2>
<ul>
<li>Add pydantic.v1 namespace to Pydantic v1 by <a href="https://github.com/exs-dmiketa"><code>@​exs-dmiketa</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9042">pydantic/pydantic#9042</a></li>
<li>Relax version of typing-extensions for V1 by <a href="https://github.com/SonOfLilit"><code>@​SonOfLilit</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8819">pydantic/pydantic#8819</a></li>
<li>patch fix for mypy by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8765">pydantic/pydantic#8765</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.14...v1.10.15">https://github.com/pydantic/pydantic/compare/v1.10.14...v1.10.15</a></p>
<h2>v1.10.14 2024-01-19</h2>
<h2>What's Changed</h2>
<ul>
<li>Update install.md by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7690">pydantic/pydantic#7690</a></li>
<li>Fix ci to only deploy docs on release by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7740">pydantic/pydantic#7740</a></li>
<li>Ubuntu fixes for V1 by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8540">pydantic/pydantic#8540</a> and <a href="https://redirect.github.com/pydantic/pydantic/pull/8587">pydantic/pydantic#8587</a></li>
<li>Fix <code>cached_property</code> handling in dataclasses when copied by <a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8407">pydantic/pydantic#8407</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/8407">pydantic/pydantic#8407</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.14">https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.14</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.15 (2024-04-03)</h2>
<ul>
<li>Add pydantic.v1 namespace to Pydantic v1 by <a href="https://github.com/exs-dmiketa"><code>@​exs-dmiketa</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9042">pydantic/pydantic#9042</a></li>
<li>Relax version of typing-extensions for V1 by <a href="https://github.com/SonOfLilit"><code>@​SonOfLilit</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8819">pydantic/pydantic#8819</a></li>
<li>patch fix for mypy by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8765">pydantic/pydantic#8765</a></li>
</ul>
<h2>v1.10.14 (2024-01-19)</h2>
<ul>
<li>Update install.md by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/7690">#7690</a></li>
<li>Fix ci to only deploy docs on release by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/7740">#7740</a></li>
<li>Ubuntu fixes for V1 by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/8540">#8540</a> and <a href="https://redirect.github.com/pydantic/pydantic/issues/8587">#8587</a></li>
<li>Fix cached_property handling in dataclasses when copied by <a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/8407">#8407</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/5476a758c8ac59887dbfa3aa1c3481d0a0e20837"><code>5476a75</code></a> prep for v1.10.15 release (<a href="https://redirect.github.com/pydantic/pydantic/issues/9157">#9157</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/aa98b58816143d7d265734a56764bf724569bac4"><code>aa98b58</code></a> Add pydantic.v1 namespace to Pydantic v1 (<a href="https://redirect.github.com/pydantic/pydantic/issues/9042">#9042</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/9dac7169e433125c957874b578c211aed789ae8e"><code>9dac716</code></a> Relax version of typing-extensions for V1 (<a href="https://redirect.github.com/pydantic/pydantic/issues/8819">#8819</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/856ea182b85b68632caba132e1faf28aa59ea588"><code>856ea18</code></a> patch fix for mypy (<a href="https://redirect.github.com/pydantic/pydantic/issues/8765">#8765</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/3ddb509786089f9df0658303545ae4b66db2d47c"><code>3ddb509</code></a> Prep for 1.10.14 release (<a href="https://redirect.github.com/pydantic/pydantic/issues/8588">#8588</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/c6fc582ee9fc76acb64cbc0a5a55d0c5c8590205"><code>c6fc582</code></a> Minor tweak to V1 docs url fix (<a href="https://redirect.github.com/pydantic/pydantic/issues/8587">#8587</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/f0766c0e6028f9868e131208387549e3897b02bd"><code>f0766c0</code></a> Fix cached_property handling in dataclasses when copied in V1(<a href="https://redirect.github.com/pydantic/pydantic/issues/8407">#8407</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/4e290ab604cdc0579a447ee1736f1b6763f49812"><code>4e290ab</code></a> Ubuntu fixes for V1 (<a href="https://redirect.github.com/pydantic/pydantic/issues/8540">#8540</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/2e939dc3bfb88f54efb66f8f1a031ff22e4f9865"><code>2e939dc</code></a> Update v1 fixes ci to only deploy docs on release (<a href="https://redirect.github.com/pydantic/pydantic/issues/7740">#7740</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/ae53c9d9b3c083c529b9f6d5b2ea0718545e15d1"><code>ae53c9d</code></a> Update install.md (<a href="https://redirect.github.com/pydantic/pydantic/issues/7690">#7690</a>)</li>
<li>See full diff in <a href="https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.15">compare view</a></li>
</ul>
</details>
<br />

Updates `black` from 23.11.0 to 24.3.0
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

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `aiohttp` from 3.9.2 to 3.9.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.4</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8089">#8089</a>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8104">#8104</a>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8163">#8163</a>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7741">#7741</a>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/master/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.9.4 (2024-04-11)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8089</code>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8104</code>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8163</code>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7741</code>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b3397c7ac44fc80206d28f1dd0d1f3b10c4ec572"><code>b3397c7</code></a> Release v3.9.4 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8201">#8201</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a7e240a9f625a0b9559bdf5f0049c71565352400"><code>a7e240a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8320">#8320</a>/9ba9a4e5 backport][3.9] Fix Python parser to mark responses without...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/28335525d1eac015a7e7584137678cbb6ff19397"><code>2833552</code></a> Escape filenames and paths in HTML when generating index pages (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8317">#8317</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8319">#8319</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ed43040613988fc4666109aca82a5180ff165df5"><code>ed43040</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8309">#8309</a>/c29945a1 backport][3.9] Improve reliability of run_app test (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8315">#8315</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ec2be0500e2674eea019c0966a7a905e9b3d6608"><code>ec2be05</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8299">#8299</a>/28d026eb backport][3.9] Create marker for internal tests (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8307">#8307</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/292d961f4ee2829a1b13fad92444a4fd693fbc87"><code>292d961</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8304">#8304</a>/88c80c14 backport][3.9] Check for backports in CI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8305">#8305</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cebe526b9c34dc3a3da9140409db63014bc4cf19"><code>cebe526</code></a> Fix handling of multipart/form-data (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8280">#8280</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8302">#8302</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/270ae9cf6a9e6159b5e29a950deb6ff7600aebc5"><code>270ae9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8297">#8297</a>/d15f07cf backport][3.9] Upgrade to llhttp 9.2.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8292">#8292</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8298">#8298</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bb231059b14277c34a8a0331e51406d5abe4f424"><code>bb23105</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8283">#8283</a>/54e13b0a backport][3.9] Fix blocking I/O in the event loop while pr...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3f79241bcbc02c9850348fc04c064fcbc980e8f0"><code>3f79241</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8286">#8286</a>/28f1fd88 backport][3.9] docs: remove repetitive word in comment (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8">#8</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.2...v3.9.4">compare view</a></li>
</ul>
</details>
<br />

Updates `pydantic` from 1.10.13 to 2.7.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.15</h2>
<h2>What's Changed</h2>
<ul>
<li>Add pydantic.v1 namespace to Pydantic v1 by <a href="https://github.com/exs-dmiketa"><code>@​exs-dmiketa</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9042">pydantic/pydantic#9042</a></li>
<li>Relax version of typing-extensions for V1 by <a href="https://github.com/SonOfLilit"><code>@​SonOfLilit</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8819">pydantic/pydantic#8819</a></li>
<li>patch fix for mypy by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8765">pydantic/pydantic#8765</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.14...v1.10.15">https://github.com/pydantic/pydantic/compare/v1.10.14...v1.10.15</a></p>
<h2>v1.10.14 2024-01-19</h2>
<h2>What's Changed</h2>
<ul>
<li>Update install.md by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7690">pydantic/pydantic#7690</a></li>
<li>Fix ci to only deploy docs on release by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7740">pydantic/pydantic#7740</a></li>
<li>Ubuntu fixes for V1 by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8540">pydantic/pydantic#8540</a> and <a href="https://redirect.github.com/pydantic/pydantic/pull/8587">pydantic/pydantic#8587</a></li>
<li>Fix <code>cached_property</code> handling in dataclasses when copied by <a href="https://github.com...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 16:10:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group across 7 directories with 7 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update in the /firebase_push_notifications directory: [black](https://github.com/psf/black).
Bumps the pip group with 2 updates in the /kafka_events/demo/setup directory: [certifi](https://github.com/certifi/python-certifi) and [idna](https://github.com/kjd/idna).
Bumps the pip group with 1 update in the /kafka_events/integration directory: [black](https://github.com/psf/black).
Bumps the pip group with 1 update in the /kafka_events/kafka_events/v1_0/deliverer directory: [idna](https://github.com/kjd/idna).
Bumps the pip group with 4 updates in the /oid4vci/integration/afj_runner directory: [aiohttp](https://github.com/aio-libs/aiohttp), [idna](https://github.com/kjd/idna), [pydantic](https://github.com/pydantic/pydantic) and [black](https://github.com/psf/black).
Bumps the pip group with 5 updates in the /redis_events/docker/services directory:

| Package | From | To |
| --- | --- | --- |
| [aiohttp](https://github.com/aio-libs/aiohttp) | `3.9.2` | `3.9.4` |
| [idna](https://github.com/kjd/idna) | `3.4` | `3.7` |
| [pydantic](https://github.com/pydantic/pydantic) | `1.10.13` | `2.7.1` |
| [black](https://github.com/psf/black) | `21.12b0` | `24.3.0` |
| [fastapi](https://github.com/tiangolo/fastapi) | `0.109.1` | `0.111.0` |

Bumps the pip group with 1 update in the /redis_events/integration directory: [fastapi](https://github.com/tiangolo/fastapi).

Updates `black` from 23.7.0 to 24.3.0
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

Updates `certifi` from 2023.5.7 to 2023.7.22
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/8fb96ed81f71e7097ed11bc4d9b19afd7ea5c909"><code>8fb96ed</code></a> 2023.07.22</li>
<li><a href="https://github.com/certifi/python-certifi/commit/afe77220e0eaa722593fc5d294213ff5275d1b40"><code>afe7722</code></a> Bump actions/setup-python from 4.6.1 to 4.7.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/230">#230</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2038739ad56abec7aaddfa90ad2ce6b3ed7f5c7b"><code>2038739</code></a> Bump dessant/lock-threads from 3.0.0 to 4.0.1 (<a href="https://redirect.github.com/certifi/python-certifi/issues/229">#229</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/44df761f4c09d19f32b3cc09208a739043a5e25b"><code>44df761</code></a> Hash pin Actions and enable dependabot (<a href="https://redirect.github.com/certifi/python-certifi/issues/228">#228</a>)</li>
<li>See full diff in <a href="https://github.com/certifi/python-certifi/compare/2023.05.07...2023.07.22">compare view</a></li>
</ul>
</details>
<br />

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `black` from 21.12b0 to 24.3.0
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

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `aiohttp` from 3.9.2 to 3.9.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.4</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8089">#8089</a>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8104">#8104</a>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8163">#8163</a>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7741">#7741</a>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/master/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.9.4 (2024-04-11)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8089</code>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8104</code>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8163</code>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7741</code>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b3397c7ac44fc80206d28f1dd0d1f3b10c4ec572"><code>b3397c7</code></a> Release v3.9.4 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8201">#8201</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a7e240a9f625a0b9559bdf5f0049c71565352400"><code>a7e240a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8320">#8320</a>/9ba9a4e5 backport][3.9] Fix Python parser to mark responses without...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/28335525d1eac015a7e7584137678cbb6ff19397"><code>2833552</code></a> Escape filenames and paths in HTML when generating index pages (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8317">#8317</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8319">#8319</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ed43040613988fc4666109aca82a5180ff165df5"><code>ed43040</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8309">#8309</a>/c29945a1 backport][3.9] Improve reliability of run_app test (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8315">#8315</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ec2be0500e2674eea019c0966a7a905e9b3d6608"><code>ec2be05</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8299">#8299</a>/28d026eb backport][3.9] Create marker for internal tests (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8307">#8307</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/292d961f4ee2829a1b13fad92444a4fd693fbc87"><code>292d961</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8304">#8304</a>/88c80c14 backport][3.9] Check for backports in CI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8305">#8305</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cebe526b9c34dc3a3da9140409db63014bc4cf19"><code>cebe526</code></a> Fix handling of multipart/form-data (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8280">#8280</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8302">#8302</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/270ae9cf6a9e6159b5e29a950deb6ff7600aebc5"><code>270ae9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8297">#8297</a>/d15f07cf backport][3.9] Upgrade to llhttp 9.2.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8292">#8292</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8298">#8298</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bb231059b14277c34a8a0331e51406d5abe4f424"><code>bb23105</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8283">#8283</a>/54e13b0a backport][3.9] Fix blocking I/O in the event loop while pr...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3f79241bcbc02c9850348fc04c064fcbc980e8f0"><code>3f79241</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8286">#8286</a>/28f1fd88 backport][3.9] docs: remove repetitive word in comment (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8">#8</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.2...v3.9.4">compare view</a></li>
</ul>
</details>
<br />

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `pydantic` from 1.10.13 to 1.10.15
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.15</h2>
<h2>What's Changed</h2>
<ul>
<li>Add pydantic.v1 namespace to Pydantic v1 by <a href="https://github.com/exs-dmiketa"><code>@​exs-dmiketa</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9042">pydantic/pydantic#9042</a></li>
<li>Relax version of typing-extensions for V1 by <a href="https://github.com/SonOfLilit"><code>@​SonOfLilit</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8819">pydantic/pydantic#8819</a></li>
<li>patch fix for mypy by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8765">pydantic/pydantic#8765</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.14...v1.10.15">https://github.com/pydantic/pydantic/compare/v1.10.14...v1.10.15</a></p>
<h2>v1.10.14 2024-01-19</h2>
<h2>What's Changed</h2>
<ul>
<li>Update install.md by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7690">pydantic/pydantic#7690</a></li>
<li>Fix ci to only deploy docs on release by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7740">pydantic/pydantic#7740</a></li>
<li>Ubuntu fixes for V1 by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8540">pydantic/pydantic#8540</a> and <a href="https://redirect.github.com/pydantic/pydantic/pull/8587">pydantic/pydantic#8587</a></li>
<li>Fix <code>cached_property</code> handling in dataclasses when copied by <a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8407">pydantic/pydantic#8407</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/8407">pydantic/pydantic#8407</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.14">https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.14</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.15 (2024-04-03)</h2>
<ul>
<li>Add pydantic.v1 namespace to Pydantic v1 by <a href="https://github.com/exs-dmiketa"><code>@​exs-dmiketa</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9042">pydantic/pydantic#9042</a></li>
<li>Relax version of typing-extensions for V1 by <a href="https://github.com/SonOfLilit"><code>@​SonOfLilit</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8819">pydantic/pydantic#8819</a></li>
<li>patch fix for mypy by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8765">pydantic/pydantic#8765</a></li>
</ul>
<h2>v1.10.14 (2024-01-19)</h2>
<ul>
<li>Update install.md by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/7690">#7690</a></li>
<li>Fix ci to only deploy docs on release by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/7740">#7740</a></li>
<li>Ubuntu fixes for V1 by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/8540">#8540</a> and <a href="https://redirect.github.com/pydantic/pydantic/issues/8587">#8587</a></li>
<li>Fix cached_property handling in dataclasses when copied by <a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/8407">#8407</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/5476a758c8ac59887dbfa3aa1c3481d0a0e20837"><code>5476a75</code></a> prep for v1.10.15 release (<a href="https://redirect.github.com/pydantic/pydantic/issues/9157">#9157</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/aa98b58816143d7d265734a56764bf724569bac4"><code>aa98b58</code></a> Add pydantic.v1 namespace to Pydantic v1 (<a href="https://redirect.github.com/pydantic/pydantic/issues/9042">#9042</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/9dac7169e433125c957874b578c211aed789ae8e"><code>9dac716</code></a> Relax version of typing-extensions for V1 (<a href="https://redirect.github.com/pydantic/pydantic/issues/8819">#8819</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/856ea182b85b68632caba132e1faf28aa59ea588"><code>856ea18</code></a> patch fix for mypy (<a href="https://redirect.github.com/pydantic/pydantic/issues/8765">#8765</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/3ddb509786089f9df0658303545ae4b66db2d47c"><code>3ddb509</code></a> Prep for 1.10.14 release (<a href="https://redirect.github.com/pydantic/pydantic/issues/8588">#8588</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/c6fc582ee9fc76acb64cbc0a5a55d0c5c8590205"><code>c6fc582</code></a> Minor tweak to V1 docs url fix (<a href="https://redirect.github.com/pydantic/pydantic/issues/8587">#8587</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/f0766c0e6028f9868e131208387549e3897b02bd"><code>f0766c0</code></a> Fix cached_property handling in dataclasses when copied in V1(<a href="https://redirect.github.com/pydantic/pydantic/issues/8407">#8407</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/4e290ab604cdc0579a447ee1736f1b6763f49812"><code>4e290ab</code></a> Ubuntu fixes for V1 (<a href="https://redirect.github.com/pydantic/pydantic/issues/8540">#8540</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/2e939dc3bfb88f54efb66f8f1a031ff22e4f9865"><code>2e939dc</code></a> Update v1 fixes ci to only deploy docs on release (<a href="https://redirect.github.com/pydantic/pydantic/issues/7740">#7740</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/ae53c9d9b3c083c529b9f6d5b2ea0718545e15d1"><code>ae53c9d</code></a> Update install.md (<a href="https://redirect.github.com/pydantic/pydantic/issues/7690">#7690</a>)</li>
<li>See full diff in <a href="https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.15">compare view</a></li>
</ul>
</details>
<br />

Updates `black` from 23.11.0 to 24.3.0
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

Updates `aiohttp` from 3.9.2 to 3.9.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.4</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8089">#8089</a>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8104">#8104</a>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8163">#8163</a>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7741">#7741</a>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/master/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.9.4 (2024-04-11)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8089</code>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8104</code>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8163</code>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7741</code>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b3397c7ac44fc80206d28f1dd0d1f3b10c4ec572"><code>b3397c7</code></a> Release v3.9.4 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8201">#8201</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a7e240a9f625a0b9559bdf5f0049c71565352400"><code>a7e240a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8320">#8320</a>/9ba9a4e5 backport][3.9] Fix Python parser to mark responses without...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/28335525d1eac015a7e7584137678cbb6ff19397"><code>2833552</code></a> Escape filenames and paths in HTML when generating index pages (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8317">#8317</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8319">#8319</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ed43040613988fc4666109aca82a5180ff165df5"><code>ed43040</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8309">#8309</a>/c29945a1 backport][3.9] Improve reliability of run_app test (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8315">#8315</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ec2be0500e2674eea019c0966a7a905e9b3d6608"><code>ec2be05</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8299">#8299</a>/28d026eb backport][3.9] Create marker for internal tests (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8307">#8307</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/292d961f4ee2829a1b13fad92444a4fd693fbc87"><code>292d961</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8304">#8304</a>/88c80c14 backport][3.9] Check for backports in CI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8305">#8305</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cebe526b9c34dc3a3da9140409db63014bc4cf19"><code>cebe526</code></a> Fix handling of multipart/form-data (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8280">#8280</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8302">#8302</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/270ae9cf6a9e6159b5e29a950deb6ff7600aebc5"><code>270ae9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8297">#8297</a>/d15f07cf backport][3.9] Upgrade to llhttp 9.2.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8292">#8292</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8298">#8298</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bb231059b14277c34a8a0331e51406d5abe4f424"><code>bb23105</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8283">#8283</a>/54e13b0a backport][3.9] Fix blocking I/O in the event loop while pr...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3f79241bcbc02c9850348fc04c064fcbc980e8f0"><code>3f79241</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8286">#8286</a>/28f1fd88 backport][3.9] docs: remove repetitive word in comment (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8">#8</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.2...v3.9.4">compare view</a></li>
</ul>
</details>
<br />

Updates `idna` from 3.4 to 3.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `pydantic` from 1.10.13 to 2.7.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.15</h2>
<h2>What's Changed</h2>
<ul>
<li>Add pydantic.v1 namespace to Pydantic v1 by <a href="https://github.com/exs-dmiketa"><code>@​exs-dmiketa</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/9042">pydantic/pydantic#9042</a></li>
<li>Relax version of typing-extensions for V1 by <a href="https://github.com/SonOfLilit"><code>@​SonOfLilit</code></a> in <a href="https://...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 16:08:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.3.0 in /redis_events in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events with 1 update: [black](https://github.com/psf/black).

Updates `black` from 23.7.0 to 24.3.0
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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 15:53:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/461" class=".btn">#461</a>
            </td>
            <td>
                <b>
                    Release for aries-cloudagent v0.12.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Release v0.12.1
##### The latest supported versions of aries-cloudagent for each plugin are as follows:

| Plugin Name | Supported aries-cloudagent version |
| --- | --- |
|basicmessage_storage | 0.12.1|
|connection_update | 0.12.1|
|firebase_push_notifications | 0.12.1|
|kafka_events | 0.12.1|
|multitenant_provider | 0.12.1|
|oid4vci | 0.12.1|
|redis_events | 0.12.1|
|rpc | 0.12.1|
***
 -  #### Plugins upgraded this release: 
	 -  basicmessage_storage 
	 -  connection_update 
	 -  firebase_push_notifications 
	 -  kafka_events 
	 -  multitenant_provider 
	 -  oid4vci 
	 -  redis_events 
	 -  rpc
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 15:49:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/460" class=".btn">#460</a>
            </td>
            <td>
                <b>
                    OID4VCI plugin - Fix delete  exchange-supported records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quick fix on ./oid4vci/exchange-supported/records delete. There is a typo that duplicates the "credential supported identifier" as a parameter causing deletes to fail.

FYI @dbluhm 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 15:25:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    update release PR workflow token
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I tried using the new PAT token for the PR workflow but it didn't work. I'm thinking it possibly has the permissions required to make the release but not the PR. The normal GITHUB_TOKEN should have the permissions to make the PR so i'm trying that.

![Screenshot from 2024-05-14 08-29-27](https://github.com/hyperledger/aries-acapy-plugins/assets/31809382/4605bbb9-cb29-4a9e-81b8-a55edae41262)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 15:32:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.4 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.4</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/Abdur-rahmaanJ"><code>@​Abdur-rahmaanJ</code></a></li>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/blueraft"><code>@​blueraft</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/carloshbcabral"><code>@​carloshbcabral</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.3</h2>
<h2>Changes</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.4</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>0.4.3</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>refurb</code>] Use function range for <code>reimplemented-operator</code> diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11271">#11271</a>)</li>
<li>[<code>refurb</code>] Ignore methods in <code>reimplemented-operator</code> (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11270">#11270</a>)</li>
<li>[<code>refurb</code>] Implement <code>fstring-number-format</code> (<code>FURB116</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10921">#10921</a>)</li>
<li>[<code>ruff</code>] Implement <code>redirected-noqa</code> (<code>RUF101</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11052">#11052</a>)</li>
<li>[<code>pyflakes</code>] Distinguish between first-party and third-party imports for fix suggestions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11168">#11168</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Ignore non-abstract class attributes when enforcing <code>B024</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11210">#11210</a>)</li>
<li>[<code>flake8-logging</code>] Include inline instantiations when detecting loggers (<a href="https://redirect.github.com/astral-sh/ruff/pull/11154">#11154</a>)</li>
<li>[<code>pylint</code>] Also emit <code>PLR0206</code> for properties with variadic parameters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11200">#11200</a>)</li>
<li>[<code>ruff</code>] Detect duplicate codes as part of <code>unused-noqa</code> (<code>RUF100</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10850">#10850</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Avoid multiline expression if format specifier is present (<a href="https://redirect.github.com/astral-sh/ruff/pull/11123">#11123</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3e8878a1c852399dffedb0236097afcfb4780b81"><code>3e8878a</code></a> Bump version to v0.4.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11352">#11352</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b6b4ad99497b65ebc6b8c21944fe41115c32477a"><code>b6b4ad9</code></a> [red-knot] <a href="https://github.com/override"><code>@​override</code></a> lint rule (<a href="https://redirect.github.com/astral-sh/ruff/issues/11282">#11282</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dd42961dd9d85a3e70baf1acf0bdd60db4393455"><code>dd42961</code></a> [<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (`PLW15...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c80c1712f05b0843976f439124b4678023c14e93"><code>c80c171</code></a> [red-knot] Vendor typeshed's stdlib (<a href="https://redirect.github.com/astral-sh/ruff/issues/11340">#11340</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2fe177c6b4e867d59409c809781a7d6922e778a"><code>e2fe177</code></a> Revert &quot;Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)&quot; (<a href="https://redirect.github.com/astral-sh/ruff/issues/11">#11</a>...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e9d1cddc97572b7bb255f1b6db993e56c0cbdba2"><code>e9d1cdd</code></a> Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dfe4291c0b7249ae892f5f1d513e6f1404436c13"><code>dfe4291</code></a> Improve <code>ruff_python_semantic::all::extract_all_names()</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11335">#11335</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4541337f3d3d0c09fe09910b6324ebe4f61111d9"><code>4541337</code></a> [red-knot] Remove <code>\&lt;Db: SemanticDb&gt;</code> contraints in favor of dynamic dispatch ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8e9ddee392326832016d3a10285b55bf9e2a8319"><code>8e9ddee</code></a> Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/issues/11342">#11342</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/702d2fa1eb93009a662d33f5805fc12ddac69b4f"><code>702d2fa</code></a> Make B024 and B027 documentation more nuanced (<a href="https://redirect.github.com/astral-sh/ruff/issues/11341">#11341</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 05:04:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.4 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.4</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/Abdur-rahmaanJ"><code>@​Abdur-rahmaanJ</code></a></li>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/blueraft"><code>@​blueraft</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/carloshbcabral"><code>@​carloshbcabral</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.3</h2>
<h2>Changes</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.4</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>0.4.3</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>refurb</code>] Use function range for <code>reimplemented-operator</code> diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11271">#11271</a>)</li>
<li>[<code>refurb</code>] Ignore methods in <code>reimplemented-operator</code> (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11270">#11270</a>)</li>
<li>[<code>refurb</code>] Implement <code>fstring-number-format</code> (<code>FURB116</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10921">#10921</a>)</li>
<li>[<code>ruff</code>] Implement <code>redirected-noqa</code> (<code>RUF101</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11052">#11052</a>)</li>
<li>[<code>pyflakes</code>] Distinguish between first-party and third-party imports for fix suggestions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11168">#11168</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Ignore non-abstract class attributes when enforcing <code>B024</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11210">#11210</a>)</li>
<li>[<code>flake8-logging</code>] Include inline instantiations when detecting loggers (<a href="https://redirect.github.com/astral-sh/ruff/pull/11154">#11154</a>)</li>
<li>[<code>pylint</code>] Also emit <code>PLR0206</code> for properties with variadic parameters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11200">#11200</a>)</li>
<li>[<code>ruff</code>] Detect duplicate codes as part of <code>unused-noqa</code> (<code>RUF100</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10850">#10850</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Avoid multiline expression if format specifier is present (<a href="https://redirect.github.com/astral-sh/ruff/pull/11123">#11123</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3e8878a1c852399dffedb0236097afcfb4780b81"><code>3e8878a</code></a> Bump version to v0.4.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11352">#11352</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b6b4ad99497b65ebc6b8c21944fe41115c32477a"><code>b6b4ad9</code></a> [red-knot] <a href="https://github.com/override"><code>@​override</code></a> lint rule (<a href="https://redirect.github.com/astral-sh/ruff/issues/11282">#11282</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dd42961dd9d85a3e70baf1acf0bdd60db4393455"><code>dd42961</code></a> [<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (`PLW15...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c80c1712f05b0843976f439124b4678023c14e93"><code>c80c171</code></a> [red-knot] Vendor typeshed's stdlib (<a href="https://redirect.github.com/astral-sh/ruff/issues/11340">#11340</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2fe177c6b4e867d59409c809781a7d6922e778a"><code>e2fe177</code></a> Revert &quot;Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)&quot; (<a href="https://redirect.github.com/astral-sh/ruff/issues/11">#11</a>...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e9d1cddc97572b7bb255f1b6db993e56c0cbdba2"><code>e9d1cdd</code></a> Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dfe4291c0b7249ae892f5f1d513e6f1404436c13"><code>dfe4291</code></a> Improve <code>ruff_python_semantic::all::extract_all_names()</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11335">#11335</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4541337f3d3d0c09fe09910b6324ebe4f61111d9"><code>4541337</code></a> [red-knot] Remove <code>\&lt;Db: SemanticDb&gt;</code> contraints in favor of dynamic dispatch ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8e9ddee392326832016d3a10285b55bf9e2a8319"><code>8e9ddee</code></a> Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/issues/11342">#11342</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/702d2fa1eb93009a662d33f5805fc12ddac69b4f"><code>702d2fa</code></a> Make B024 and B027 documentation more nuanced (<a href="https://redirect.github.com/astral-sh/ruff/issues/11341">#11341</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 05:02:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.4 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.4</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/Abdur-rahmaanJ"><code>@​Abdur-rahmaanJ</code></a></li>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/blueraft"><code>@​blueraft</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/carloshbcabral"><code>@​carloshbcabral</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.3</h2>
<h2>Changes</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.4</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>0.4.3</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>refurb</code>] Use function range for <code>reimplemented-operator</code> diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11271">#11271</a>)</li>
<li>[<code>refurb</code>] Ignore methods in <code>reimplemented-operator</code> (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11270">#11270</a>)</li>
<li>[<code>refurb</code>] Implement <code>fstring-number-format</code> (<code>FURB116</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10921">#10921</a>)</li>
<li>[<code>ruff</code>] Implement <code>redirected-noqa</code> (<code>RUF101</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11052">#11052</a>)</li>
<li>[<code>pyflakes</code>] Distinguish between first-party and third-party imports for fix suggestions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11168">#11168</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Ignore non-abstract class attributes when enforcing <code>B024</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11210">#11210</a>)</li>
<li>[<code>flake8-logging</code>] Include inline instantiations when detecting loggers (<a href="https://redirect.github.com/astral-sh/ruff/pull/11154">#11154</a>)</li>
<li>[<code>pylint</code>] Also emit <code>PLR0206</code> for properties with variadic parameters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11200">#11200</a>)</li>
<li>[<code>ruff</code>] Detect duplicate codes as part of <code>unused-noqa</code> (<code>RUF100</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10850">#10850</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Avoid multiline expression if format specifier is present (<a href="https://redirect.github.com/astral-sh/ruff/pull/11123">#11123</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3e8878a1c852399dffedb0236097afcfb4780b81"><code>3e8878a</code></a> Bump version to v0.4.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11352">#11352</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b6b4ad99497b65ebc6b8c21944fe41115c32477a"><code>b6b4ad9</code></a> [red-knot] <a href="https://github.com/override"><code>@​override</code></a> lint rule (<a href="https://redirect.github.com/astral-sh/ruff/issues/11282">#11282</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dd42961dd9d85a3e70baf1acf0bdd60db4393455"><code>dd42961</code></a> [<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (`PLW15...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c80c1712f05b0843976f439124b4678023c14e93"><code>c80c171</code></a> [red-knot] Vendor typeshed's stdlib (<a href="https://redirect.github.com/astral-sh/ruff/issues/11340">#11340</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2fe177c6b4e867d59409c809781a7d6922e778a"><code>e2fe177</code></a> Revert &quot;Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)&quot; (<a href="https://redirect.github.com/astral-sh/ruff/issues/11">#11</a>...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e9d1cddc97572b7bb255f1b6db993e56c0cbdba2"><code>e9d1cdd</code></a> Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dfe4291c0b7249ae892f5f1d513e6f1404436c13"><code>dfe4291</code></a> Improve <code>ruff_python_semantic::all::extract_all_names()</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11335">#11335</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4541337f3d3d0c09fe09910b6324ebe4f61111d9"><code>4541337</code></a> [red-knot] Remove <code>\&lt;Db: SemanticDb&gt;</code> contraints in favor of dynamic dispatch ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8e9ddee392326832016d3a10285b55bf9e2a8319"><code>8e9ddee</code></a> Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/issues/11342">#11342</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/702d2fa1eb93009a662d33f5805fc12ddac69b4f"><code>702d2fa</code></a> Make B024 and B027 documentation more nuanced (<a href="https://redirect.github.com/astral-sh/ruff/issues/11341">#11341</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 05:01:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.4 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.4</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/Abdur-rahmaanJ"><code>@​Abdur-rahmaanJ</code></a></li>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/blueraft"><code>@​blueraft</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/carloshbcabral"><code>@​carloshbcabral</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.3</h2>
<h2>Changes</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.4</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>0.4.3</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>refurb</code>] Use function range for <code>reimplemented-operator</code> diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11271">#11271</a>)</li>
<li>[<code>refurb</code>] Ignore methods in <code>reimplemented-operator</code> (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11270">#11270</a>)</li>
<li>[<code>refurb</code>] Implement <code>fstring-number-format</code> (<code>FURB116</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10921">#10921</a>)</li>
<li>[<code>ruff</code>] Implement <code>redirected-noqa</code> (<code>RUF101</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11052">#11052</a>)</li>
<li>[<code>pyflakes</code>] Distinguish between first-party and third-party imports for fix suggestions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11168">#11168</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Ignore non-abstract class attributes when enforcing <code>B024</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11210">#11210</a>)</li>
<li>[<code>flake8-logging</code>] Include inline instantiations when detecting loggers (<a href="https://redirect.github.com/astral-sh/ruff/pull/11154">#11154</a>)</li>
<li>[<code>pylint</code>] Also emit <code>PLR0206</code> for properties with variadic parameters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11200">#11200</a>)</li>
<li>[<code>ruff</code>] Detect duplicate codes as part of <code>unused-noqa</code> (<code>RUF100</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10850">#10850</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Avoid multiline expression if format specifier is present (<a href="https://redirect.github.com/astral-sh/ruff/pull/11123">#11123</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3e8878a1c852399dffedb0236097afcfb4780b81"><code>3e8878a</code></a> Bump version to v0.4.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11352">#11352</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b6b4ad99497b65ebc6b8c21944fe41115c32477a"><code>b6b4ad9</code></a> [red-knot] <a href="https://github.com/override"><code>@​override</code></a> lint rule (<a href="https://redirect.github.com/astral-sh/ruff/issues/11282">#11282</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dd42961dd9d85a3e70baf1acf0bdd60db4393455"><code>dd42961</code></a> [<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (`PLW15...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c80c1712f05b0843976f439124b4678023c14e93"><code>c80c171</code></a> [red-knot] Vendor typeshed's stdlib (<a href="https://redirect.github.com/astral-sh/ruff/issues/11340">#11340</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2fe177c6b4e867d59409c809781a7d6922e778a"><code>e2fe177</code></a> Revert &quot;Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)&quot; (<a href="https://redirect.github.com/astral-sh/ruff/issues/11">#11</a>...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e9d1cddc97572b7bb255f1b6db993e56c0cbdba2"><code>e9d1cdd</code></a> Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dfe4291c0b7249ae892f5f1d513e6f1404436c13"><code>dfe4291</code></a> Improve <code>ruff_python_semantic::all::extract_all_names()</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11335">#11335</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4541337f3d3d0c09fe09910b6324ebe4f61111d9"><code>4541337</code></a> [red-knot] Remove <code>\&lt;Db: SemanticDb&gt;</code> contraints in favor of dynamic dispatch ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8e9ddee392326832016d3a10285b55bf9e2a8319"><code>8e9ddee</code></a> Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/issues/11342">#11342</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/702d2fa1eb93009a662d33f5805fc12ddac69b4f"><code>702d2fa</code></a> Make B024 and B027 documentation more nuanced (<a href="https://redirect.github.com/astral-sh/ruff/issues/11341">#11341</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 04:56:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.4 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.4</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/Abdur-rahmaanJ"><code>@​Abdur-rahmaanJ</code></a></li>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/blueraft"><code>@​blueraft</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/carloshbcabral"><code>@​carloshbcabral</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.3</h2>
<h2>Changes</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.4</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>0.4.3</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>refurb</code>] Use function range for <code>reimplemented-operator</code> diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11271">#11271</a>)</li>
<li>[<code>refurb</code>] Ignore methods in <code>reimplemented-operator</code> (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11270">#11270</a>)</li>
<li>[<code>refurb</code>] Implement <code>fstring-number-format</code> (<code>FURB116</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10921">#10921</a>)</li>
<li>[<code>ruff</code>] Implement <code>redirected-noqa</code> (<code>RUF101</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11052">#11052</a>)</li>
<li>[<code>pyflakes</code>] Distinguish between first-party and third-party imports for fix suggestions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11168">#11168</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Ignore non-abstract class attributes when enforcing <code>B024</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11210">#11210</a>)</li>
<li>[<code>flake8-logging</code>] Include inline instantiations when detecting loggers (<a href="https://redirect.github.com/astral-sh/ruff/pull/11154">#11154</a>)</li>
<li>[<code>pylint</code>] Also emit <code>PLR0206</code> for properties with variadic parameters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11200">#11200</a>)</li>
<li>[<code>ruff</code>] Detect duplicate codes as part of <code>unused-noqa</code> (<code>RUF100</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10850">#10850</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Avoid multiline expression if format specifier is present (<a href="https://redirect.github.com/astral-sh/ruff/pull/11123">#11123</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3e8878a1c852399dffedb0236097afcfb4780b81"><code>3e8878a</code></a> Bump version to v0.4.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11352">#11352</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b6b4ad99497b65ebc6b8c21944fe41115c32477a"><code>b6b4ad9</code></a> [red-knot] <a href="https://github.com/override"><code>@​override</code></a> lint rule (<a href="https://redirect.github.com/astral-sh/ruff/issues/11282">#11282</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dd42961dd9d85a3e70baf1acf0bdd60db4393455"><code>dd42961</code></a> [<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (`PLW15...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c80c1712f05b0843976f439124b4678023c14e93"><code>c80c171</code></a> [red-knot] Vendor typeshed's stdlib (<a href="https://redirect.github.com/astral-sh/ruff/issues/11340">#11340</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2fe177c6b4e867d59409c809781a7d6922e778a"><code>e2fe177</code></a> Revert &quot;Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)&quot; (<a href="https://redirect.github.com/astral-sh/ruff/issues/11">#11</a>...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e9d1cddc97572b7bb255f1b6db993e56c0cbdba2"><code>e9d1cdd</code></a> Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dfe4291c0b7249ae892f5f1d513e6f1404436c13"><code>dfe4291</code></a> Improve <code>ruff_python_semantic::all::extract_all_names()</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11335">#11335</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4541337f3d3d0c09fe09910b6324ebe4f61111d9"><code>4541337</code></a> [red-knot] Remove <code>\&lt;Db: SemanticDb&gt;</code> contraints in favor of dynamic dispatch ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8e9ddee392326832016d3a10285b55bf9e2a8319"><code>8e9ddee</code></a> Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/issues/11342">#11342</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/702d2fa1eb93009a662d33f5805fc12ddac69b4f"><code>702d2fa</code></a> Make B024 and B027 documentation more nuanced (<a href="https://redirect.github.com/astral-sh/ruff/issues/11341">#11341</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 04:53:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/452" class=".btn">#452</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.4 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.4</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/Abdur-rahmaanJ"><code>@​Abdur-rahmaanJ</code></a></li>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/blueraft"><code>@​blueraft</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/carloshbcabral"><code>@​carloshbcabral</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.3</h2>
<h2>Changes</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.4</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11342">#11342</a>)</li>
<li>[<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (<code>PLW1514</code>)  (<a href="https://redirect.github.com/astral-sh/ruff/pull/11288">#11288</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI059</code> (<code>generic-not-last-base-class</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11233">#11233</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI062</code> (<code>duplicate-literal-member</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11269">#11269</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-boolean-trap</code>] Allow passing booleans as positional-only arguments in code such as <code>set(True)</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11287">#11287</a>)</li>
<li>[<code>flake8-bugbear</code>] Ignore enum classes in <code>cached-instance-method</code> (<code>B019</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11312">#11312</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Expand tildes when resolving Ruff server configuration file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11283">#11283</a>)</li>
<li>Fix <code>ruff server</code> hanging after Neovim closes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11291">#11291</a>)</li>
<li>Editor settings are used by default if no file-based configuration exists (<a href="https://redirect.github.com/astral-sh/ruff/pull/11266">#11266</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Consider <code>with</code> statements for <code>too-many-branches</code> (<code>PLR0912</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11321">#11321</a>)</li>
<li>[<code>flake8-blind-except</code>, <code>tryceratops</code>] Respect logged and re-raised expressions in nested statements (<code>BLE001</code>, <code>TRY201</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11301">#11301</a>)</li>
<li>Recognise assignments such as <code>__all__ = builtins.list([&quot;foo&quot;, &quot;bar&quot;])</code> as valid <code>__all__</code> definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11335">#11335</a>)</li>
</ul>
<h2>0.4.3</h2>
<h3>Enhancements</h3>
<ul>
<li>Add support for PEP 696 syntax (<a href="https://redirect.github.com/astral-sh/ruff/pull/11120">#11120</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>refurb</code>] Use function range for <code>reimplemented-operator</code> diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11271">#11271</a>)</li>
<li>[<code>refurb</code>] Ignore methods in <code>reimplemented-operator</code> (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11270">#11270</a>)</li>
<li>[<code>refurb</code>] Implement <code>fstring-number-format</code> (<code>FURB116</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10921">#10921</a>)</li>
<li>[<code>ruff</code>] Implement <code>redirected-noqa</code> (<code>RUF101</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11052">#11052</a>)</li>
<li>[<code>pyflakes</code>] Distinguish between first-party and third-party imports for fix suggestions (<a href="https://redirect.github.com/astral-sh/ruff/pull/11168">#11168</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Ignore non-abstract class attributes when enforcing <code>B024</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11210">#11210</a>)</li>
<li>[<code>flake8-logging</code>] Include inline instantiations when detecting loggers (<a href="https://redirect.github.com/astral-sh/ruff/pull/11154">#11154</a>)</li>
<li>[<code>pylint</code>] Also emit <code>PLR0206</code> for properties with variadic parameters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11200">#11200</a>)</li>
<li>[<code>ruff</code>] Detect duplicate codes as part of <code>unused-noqa</code> (<code>RUF100</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10850">#10850</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Avoid multiline expression if format specifier is present (<a href="https://redirect.github.com/astral-sh/ruff/pull/11123">#11123</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3e8878a1c852399dffedb0236097afcfb4780b81"><code>3e8878a</code></a> Bump version to v0.4.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11352">#11352</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b6b4ad99497b65ebc6b8c21944fe41115c32477a"><code>b6b4ad9</code></a> [red-knot] <a href="https://github.com/override"><code>@​override</code></a> lint rule (<a href="https://redirect.github.com/astral-sh/ruff/issues/11282">#11282</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dd42961dd9d85a3e70baf1acf0bdd60db4393455"><code>dd42961</code></a> [<code>pylint</code>] Detect <code>pathlib.Path.open</code> calls in <code>unspecified-encoding</code> (`PLW15...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c80c1712f05b0843976f439124b4678023c14e93"><code>c80c171</code></a> [red-knot] Vendor typeshed's stdlib (<a href="https://redirect.github.com/astral-sh/ruff/issues/11340">#11340</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2fe177c6b4e867d59409c809781a7d6922e778a"><code>e2fe177</code></a> Revert &quot;Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)&quot; (<a href="https://redirect.github.com/astral-sh/ruff/issues/11">#11</a>...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e9d1cddc97572b7bb255f1b6db993e56c0cbdba2"><code>e9d1cdd</code></a> Simplify arithmetic operation in logical lines checker (<a href="https://redirect.github.com/astral-sh/ruff/issues/11346">#11346</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dfe4291c0b7249ae892f5f1d513e6f1404436c13"><code>dfe4291</code></a> Improve <code>ruff_python_semantic::all::extract_all_names()</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11335">#11335</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4541337f3d3d0c09fe09910b6324ebe4f61111d9"><code>4541337</code></a> [red-knot] Remove <code>\&lt;Db: SemanticDb&gt;</code> contraints in favor of dynamic dispatch ...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8e9ddee392326832016d3a10285b55bf9e2a8319"><code>8e9ddee</code></a> Ignore end-of-line comments when determining blank line rules (<a href="https://redirect.github.com/astral-sh/ruff/issues/11342">#11342</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/702d2fa1eb93009a662d33f5805fc12ddac69b4f"><code>702d2fa</code></a> Make B024 and B027 documentation more nuanced (<a href="https://redirect.github.com/astral-sh/ruff/issues/11341">#11341</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 04:30:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/450" class=".btn">#450</a>
            </td>
            <td>
                <b>
                    :arrow_up: Bulk upgrade common dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follows up from #449 

Uses find-replace-all to upgrade the following dependencies across pyptoject.toml files:
- aiohttp
- bcrypt
- black
- pydantic
- pytest
- pytest-asyncio
- pytest-cov
- pytest-mock
- pytest-ruff
- rope
- ruff

Also specific to redis-events plugin:
- fastapi
- redis
- uvicorn

Please review commit logs to verify this.

Does not include upgrades to older sub-projects, which are pinned to older python versions:
- kafka_events/kafka_events/v1_0/deliverer/pyproject.toml
- kafka_events/kafka_events/v1_0/http_kafka_relay/pyproject.toml

Note: I added a bash script that helps with applying poetry lock to every relevant directory. May be helpful for future use.

Tada! :tada: This should clear up a bunch of open dependabot PRs, and should hopefully make maintaing this multi-project repo a bit easier

___ 

Side-note: the following:
- oid4vci/integration/afj_runner/pyproject.toml

complains about:
```sh
The dependency name for controller does not match the actual package's name: acapy-controller
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 11:05:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/449" class=".btn">#449</a>
            </td>
            <td>
                <b>
                    :heavy_minus_sign: remove `asynctest` dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaces `asynctest` with `unittest` in all modules

Includes formatting changes from #448. Marking as draft until that one's merged
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 10:03:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    :art: Apply formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We're maintaining a fork of this repo, and to avoid merge conflicts in the future, it'd be helpful if formatting were applied to the codebase.

This just applies `black` formatting and `isort` for import organisation. No other changes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 09:40:06 +0000 UTC
    </div>
</div>

