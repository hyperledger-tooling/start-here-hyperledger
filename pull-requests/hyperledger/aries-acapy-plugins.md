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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group in /kafka_events with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events with 4 updates: [black](https://github.com/psf/black), [idna](https://github.com/kjd/idna), [jwcrypto](https://github.com/latchset/jwcrypto) and [pillow](https://github.com/python-pillow/Pillow).

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

Updates `idna` from 3.6 to 3.7
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
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `jwcrypto` from 1.5.4 to 1.5.6
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

Updates `pillow` from 10.2.0 to 10.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.3.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>CVE-2024-28219: Use strncpy to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Use <code>functools.lru_cache</code> for <code>hopper()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7912">#7912</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Raise ValueError if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improve speed of loading QOI images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7925">#7925</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added RGB to I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Add --report argument to <strong>main</strong>.py to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Added RGB to I;16, I;16L and I;16B conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a> [<a href="https://github.com/Yay295"><code>@​Yay295</code></a>]</li>
<li>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a> [<a href="https://github.com/scaramallion"><code>@​scaramallion</code></a>]</li>
<li>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed joined corners for ImageDraw rounded_rectangle() non-integer dimensions <a href="https://redirect.github.com/python-pillow/Pillow/issues/7881">#7881</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed Python and NumPy pinning on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7880">#7880</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Update UnidentifiedImageError and <strong>version</strong> imports <a href="https://redirect.github.com/python-pillow/Pillow/issues/7644">#7644</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Stop reading EPS image at EOF marker <a href="https://redirect.github.com/python-pillow/Pillow/issues/7753">#7753</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>PSD layer co-ordinates may be negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7706">#7706</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use subprocess with CREATE_NO_WINDOW flag in ImageShow WindowsViewer <a href="https://redirect.github.com/python-pillow/Pillow/issues/7791">#7791</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>When saving GIF frame that restores to background color, do not fill identical pixels <a href="https://redirect.github.com/python-pillow/Pillow/issues/7788">#7788</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed reading PNG iCCP compression method <a href="https://redirect.github.com/python-pillow/Pillow/issues/7823">#7823</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Allow writing IFDRational to UNDEFINED tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7840">#7840</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix logged tag name when loading Exif data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7842">#7842</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use maximum frame size in IHDR chunk when saving APNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7821">#7821</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Prevent opening P TGA images without a palette <a href="https://redirect.github.com/python-pillow/Pillow/issues/7797">#7797</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use palette when loading ICO images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7798">#7798</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use consistent arguments for load_read and load_seek <a href="https://redirect.github.com/python-pillow/Pillow/issues/7713">#7713</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Turn off nullability warnings for macOS SDK <a href="https://redirect.github.com/python-pillow/Pillow/issues/7827">#7827</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix shift-sign issue in Convert.c <a href="https://redirect.github.com/python-pillow/Pillow/issues/7838">#7838</a> [<a href="https://github.com/r-barnes"><code>@​r-barnes</code></a>]</li>
<li>winbuild: Refactor dependency versions into constants <a href="https://redirect.github.com/python-pillow/Pillow/issues/7843">#7843</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Build macOS arm64 wheels natively <a href="https://redirect.github.com/python-pillow/Pillow/issues/7852">#7852</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed typo <a href="https://redirect.github.com/python-pillow/Pillow/issues/7855">#7855</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Open 16-bit grayscale PNGs as I;16 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7849">#7849</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Handle truncated chunks at the end of PNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7709">#7709</a> [<a href="https://github.com/lajiyuan"><code>@​lajiyuan</code></a>]</li>
<li>Match mask size to pasted image size in GifImagePlugin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7779">#7779</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Changed SupportsGetMesh protocol to be public <a href="https://redirect.github.com/python-pillow/Pillow/issues/7841">#7841</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Release GIL while calling <code>WebPAnimDecoderGetNext</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7782">#7782</a> [<a href="https://github.com/evanmiller"><code>@​evanmiller</code></a>]</li>
<li>Fixed reading FLI/FLC images with a prefix chunk <a href="https://redirect.github.com/python-pillow/Pillow/issues/7804">#7804</a> [<a href="https://github.com/twolife"><code>@​twolife</code></a>]</li>
<li>Updated package name for Tidelift <a href="https://redirect.github.com/python-pillow/Pillow/issues/7810">#7810</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7744">#7744</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.3.0 (2024-04-01)</h2>
<ul>
<li>
<p>CVE-2024-28219: Use <code>strncpy</code> to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Deprecate <code>eval()</code>, replacing it with <code>lambda_eval()</code> and <code>unsafe_eval()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Raise <code>ValueError</code> if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a>
[radarhere]</p>
</li>
<li>
<p>Add <code>--report</code> argument to <code>__main__.py</code> to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a>
[nulano, radarhere, hugovk]</p>
</li>
<li>
<p>Added RGB to I;16, I;16L, I;16B and I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a>, <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a>
[radarhere]</p>
</li>
<li>
<p>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a>
[nulano, radarhere]</p>
</li>
<li>
<p>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a>
[Yay295, hugovk, radarhere]</p>
</li>
<li>
<p>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a>
[radarhere]</p>
</li>
<li>
<p>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a>
[radarhere]</p>
</li>
<li>
<p>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a>
[radarhere]</p>
</li>
<li>
<p>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a>
[scaramallion, radarhere]</p>
</li>
<li>
<p>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a>
[radarhere]</p>
</li>
<li>
<p>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a>
[radarhere]</p>
</li>
<li>
<p>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a>
[radarhere]</p>
</li>
<li>
<p>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a>
[radarhere]</p>
</li>
<li>
<p>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a>
[radarhere]</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-pillow/Pillow/commit/5c89d88eee199ba53f64581ea39b6a1bc52feb1a"><code>5c89d88</code></a> 10.3.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/63cbfcfdea2d163ec93bae8d283fcfe4b73b5dc7"><code>63cbfcf</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2776126aa9af322b416eaca247f4f8ebefd08128"><code>2776126</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> from python-pillow/lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/aeb51cbb169eb3285818ba1390ddf2771d897e6e"><code>aeb51cb</code></a> Merge branch 'main' into lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/5beb0b66648db8b542bb5260eed79b25e33d643b"><code>5beb0b6</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/cac6ffa7b399ea79b6239984d1307056a0b19af2"><code>cac6ffa</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a> from python-pillow/imagemath</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/f5eeeacf7539eaa0d93a677d7666bc7c142c8d1c"><code>f5eeeac</code></a> Name as 'options' in lambda_eval and unsafe_eval, but '_dict' in deprecated eval</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/facf3af93dabcbdd8cdbda8c3b50eefafa3bb04c"><code>facf3af</code></a> Added release notes</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2a93aba5cfcf6e241ab4f9392c13e3b74032c061"><code>2a93aba</code></a> Use strncpy to avoid buffer overflow</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/a670597bc30e9d489656fc9d807170b8f3d7ca57"><code>a670597</code></a> Update CHANGES.rst [ci skip]</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/10.2.0...10.3.0">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 19:09:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group in /multitenant_provider with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /multitenant_provider with 4 updates: [black](https://github.com/psf/black), [idna](https://github.com/kjd/idna), [jwcrypto](https://github.com/latchset/jwcrypto) and [pillow](https://github.com/python-pillow/Pillow).

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

Updates `idna` from 3.6 to 3.7
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
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `jwcrypto` from 1.5.4 to 1.5.6
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

Updates `pillow` from 10.2.0 to 10.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.3.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>CVE-2024-28219: Use strncpy to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Use <code>functools.lru_cache</code> for <code>hopper()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7912">#7912</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Raise ValueError if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improve speed of loading QOI images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7925">#7925</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added RGB to I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Add --report argument to <strong>main</strong>.py to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Added RGB to I;16, I;16L and I;16B conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a> [<a href="https://github.com/Yay295"><code>@​Yay295</code></a>]</li>
<li>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a> [<a href="https://github.com/scaramallion"><code>@​scaramallion</code></a>]</li>
<li>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed joined corners for ImageDraw rounded_rectangle() non-integer dimensions <a href="https://redirect.github.com/python-pillow/Pillow/issues/7881">#7881</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed Python and NumPy pinning on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7880">#7880</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Update UnidentifiedImageError and <strong>version</strong> imports <a href="https://redirect.github.com/python-pillow/Pillow/issues/7644">#7644</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Stop reading EPS image at EOF marker <a href="https://redirect.github.com/python-pillow/Pillow/issues/7753">#7753</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>PSD layer co-ordinates may be negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7706">#7706</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use subprocess with CREATE_NO_WINDOW flag in ImageShow WindowsViewer <a href="https://redirect.github.com/python-pillow/Pillow/issues/7791">#7791</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>When saving GIF frame that restores to background color, do not fill identical pixels <a href="https://redirect.github.com/python-pillow/Pillow/issues/7788">#7788</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed reading PNG iCCP compression method <a href="https://redirect.github.com/python-pillow/Pillow/issues/7823">#7823</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Allow writing IFDRational to UNDEFINED tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7840">#7840</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix logged tag name when loading Exif data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7842">#7842</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use maximum frame size in IHDR chunk when saving APNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7821">#7821</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Prevent opening P TGA images without a palette <a href="https://redirect.github.com/python-pillow/Pillow/issues/7797">#7797</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use palette when loading ICO images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7798">#7798</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use consistent arguments for load_read and load_seek <a href="https://redirect.github.com/python-pillow/Pillow/issues/7713">#7713</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Turn off nullability warnings for macOS SDK <a href="https://redirect.github.com/python-pillow/Pillow/issues/7827">#7827</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix shift-sign issue in Convert.c <a href="https://redirect.github.com/python-pillow/Pillow/issues/7838">#7838</a> [<a href="https://github.com/r-barnes"><code>@​r-barnes</code></a>]</li>
<li>winbuild: Refactor dependency versions into constants <a href="https://redirect.github.com/python-pillow/Pillow/issues/7843">#7843</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Build macOS arm64 wheels natively <a href="https://redirect.github.com/python-pillow/Pillow/issues/7852">#7852</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed typo <a href="https://redirect.github.com/python-pillow/Pillow/issues/7855">#7855</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Open 16-bit grayscale PNGs as I;16 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7849">#7849</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Handle truncated chunks at the end of PNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7709">#7709</a> [<a href="https://github.com/lajiyuan"><code>@​lajiyuan</code></a>]</li>
<li>Match mask size to pasted image size in GifImagePlugin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7779">#7779</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Changed SupportsGetMesh protocol to be public <a href="https://redirect.github.com/python-pillow/Pillow/issues/7841">#7841</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Release GIL while calling <code>WebPAnimDecoderGetNext</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7782">#7782</a> [<a href="https://github.com/evanmiller"><code>@​evanmiller</code></a>]</li>
<li>Fixed reading FLI/FLC images with a prefix chunk <a href="https://redirect.github.com/python-pillow/Pillow/issues/7804">#7804</a> [<a href="https://github.com/twolife"><code>@​twolife</code></a>]</li>
<li>Updated package name for Tidelift <a href="https://redirect.github.com/python-pillow/Pillow/issues/7810">#7810</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7744">#7744</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.3.0 (2024-04-01)</h2>
<ul>
<li>
<p>CVE-2024-28219: Use <code>strncpy</code> to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Deprecate <code>eval()</code>, replacing it with <code>lambda_eval()</code> and <code>unsafe_eval()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Raise <code>ValueError</code> if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a>
[radarhere]</p>
</li>
<li>
<p>Add <code>--report</code> argument to <code>__main__.py</code> to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a>
[nulano, radarhere, hugovk]</p>
</li>
<li>
<p>Added RGB to I;16, I;16L, I;16B and I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a>, <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a>
[radarhere]</p>
</li>
<li>
<p>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a>
[nulano, radarhere]</p>
</li>
<li>
<p>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a>
[Yay295, hugovk, radarhere]</p>
</li>
<li>
<p>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a>
[radarhere]</p>
</li>
<li>
<p>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a>
[radarhere]</p>
</li>
<li>
<p>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a>
[radarhere]</p>
</li>
<li>
<p>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a>
[scaramallion, radarhere]</p>
</li>
<li>
<p>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a>
[radarhere]</p>
</li>
<li>
<p>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a>
[radarhere]</p>
</li>
<li>
<p>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a>
[radarhere]</p>
</li>
<li>
<p>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a>
[radarhere]</p>
</li>
<li>
<p>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a>
[radarhere]</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-pillow/Pillow/commit/5c89d88eee199ba53f64581ea39b6a1bc52feb1a"><code>5c89d88</code></a> 10.3.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/63cbfcfdea2d163ec93bae8d283fcfe4b73b5dc7"><code>63cbfcf</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2776126aa9af322b416eaca247f4f8ebefd08128"><code>2776126</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> from python-pillow/lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/aeb51cbb169eb3285818ba1390ddf2771d897e6e"><code>aeb51cb</code></a> Merge branch 'main' into lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/5beb0b66648db8b542bb5260eed79b25e33d643b"><code>5beb0b6</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/cac6ffa7b399ea79b6239984d1307056a0b19af2"><code>cac6ffa</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a> from python-pillow/imagemath</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/f5eeeacf7539eaa0d93a677d7666bc7c142c8d1c"><code>f5eeeac</code></a> Name as 'options' in lambda_eval and unsafe_eval, but '_dict' in deprecated eval</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/facf3af93dabcbdd8cdbda8c3b50eefafa3bb04c"><code>facf3af</code></a> Added release notes</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2a93aba5cfcf6e241ab4f9392c13e3b74032c061"><code>2a93aba</code></a> Use strncpy to avoid buffer overflow</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/a670597bc30e9d489656fc9d807170b8f3d7ca57"><code>a670597</code></a> Update CHANGES.rst [ci skip]</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/10.2.0...10.3.0">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 19:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group in /rpc with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /rpc with 4 updates: [black](https://github.com/psf/black), [idna](https://github.com/kjd/idna), [jwcrypto](https://github.com/latchset/jwcrypto) and [pillow](https://github.com/python-pillow/Pillow).

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

Updates `idna` from 3.6 to 3.7
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
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `jwcrypto` from 1.5.4 to 1.5.6
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

Updates `pillow` from 10.2.0 to 10.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.3.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>CVE-2024-28219: Use strncpy to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Use <code>functools.lru_cache</code> for <code>hopper()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7912">#7912</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Raise ValueError if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improve speed of loading QOI images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7925">#7925</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added RGB to I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Add --report argument to <strong>main</strong>.py to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Added RGB to I;16, I;16L and I;16B conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a> [<a href="https://github.com/Yay295"><code>@​Yay295</code></a>]</li>
<li>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a> [<a href="https://github.com/scaramallion"><code>@​scaramallion</code></a>]</li>
<li>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed joined corners for ImageDraw rounded_rectangle() non-integer dimensions <a href="https://redirect.github.com/python-pillow/Pillow/issues/7881">#7881</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed Python and NumPy pinning on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7880">#7880</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Update UnidentifiedImageError and <strong>version</strong> imports <a href="https://redirect.github.com/python-pillow/Pillow/issues/7644">#7644</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Stop reading EPS image at EOF marker <a href="https://redirect.github.com/python-pillow/Pillow/issues/7753">#7753</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>PSD layer co-ordinates may be negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7706">#7706</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use subprocess with CREATE_NO_WINDOW flag in ImageShow WindowsViewer <a href="https://redirect.github.com/python-pillow/Pillow/issues/7791">#7791</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>When saving GIF frame that restores to background color, do not fill identical pixels <a href="https://redirect.github.com/python-pillow/Pillow/issues/7788">#7788</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed reading PNG iCCP compression method <a href="https://redirect.github.com/python-pillow/Pillow/issues/7823">#7823</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Allow writing IFDRational to UNDEFINED tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7840">#7840</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix logged tag name when loading Exif data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7842">#7842</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use maximum frame size in IHDR chunk when saving APNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7821">#7821</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Prevent opening P TGA images without a palette <a href="https://redirect.github.com/python-pillow/Pillow/issues/7797">#7797</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use palette when loading ICO images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7798">#7798</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use consistent arguments for load_read and load_seek <a href="https://redirect.github.com/python-pillow/Pillow/issues/7713">#7713</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Turn off nullability warnings for macOS SDK <a href="https://redirect.github.com/python-pillow/Pillow/issues/7827">#7827</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix shift-sign issue in Convert.c <a href="https://redirect.github.com/python-pillow/Pillow/issues/7838">#7838</a> [<a href="https://github.com/r-barnes"><code>@​r-barnes</code></a>]</li>
<li>winbuild: Refactor dependency versions into constants <a href="https://redirect.github.com/python-pillow/Pillow/issues/7843">#7843</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Build macOS arm64 wheels natively <a href="https://redirect.github.com/python-pillow/Pillow/issues/7852">#7852</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed typo <a href="https://redirect.github.com/python-pillow/Pillow/issues/7855">#7855</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Open 16-bit grayscale PNGs as I;16 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7849">#7849</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Handle truncated chunks at the end of PNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7709">#7709</a> [<a href="https://github.com/lajiyuan"><code>@​lajiyuan</code></a>]</li>
<li>Match mask size to pasted image size in GifImagePlugin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7779">#7779</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Changed SupportsGetMesh protocol to be public <a href="https://redirect.github.com/python-pillow/Pillow/issues/7841">#7841</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Release GIL while calling <code>WebPAnimDecoderGetNext</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7782">#7782</a> [<a href="https://github.com/evanmiller"><code>@​evanmiller</code></a>]</li>
<li>Fixed reading FLI/FLC images with a prefix chunk <a href="https://redirect.github.com/python-pillow/Pillow/issues/7804">#7804</a> [<a href="https://github.com/twolife"><code>@​twolife</code></a>]</li>
<li>Updated package name for Tidelift <a href="https://redirect.github.com/python-pillow/Pillow/issues/7810">#7810</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7744">#7744</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.3.0 (2024-04-01)</h2>
<ul>
<li>
<p>CVE-2024-28219: Use <code>strncpy</code> to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Deprecate <code>eval()</code>, replacing it with <code>lambda_eval()</code> and <code>unsafe_eval()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Raise <code>ValueError</code> if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a>
[radarhere]</p>
</li>
<li>
<p>Add <code>--report</code> argument to <code>__main__.py</code> to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a>
[nulano, radarhere, hugovk]</p>
</li>
<li>
<p>Added RGB to I;16, I;16L, I;16B and I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a>, <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a>
[radarhere]</p>
</li>
<li>
<p>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a>
[nulano, radarhere]</p>
</li>
<li>
<p>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a>
[Yay295, hugovk, radarhere]</p>
</li>
<li>
<p>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a>
[radarhere]</p>
</li>
<li>
<p>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a>
[radarhere]</p>
</li>
<li>
<p>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a>
[radarhere]</p>
</li>
<li>
<p>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a>
[scaramallion, radarhere]</p>
</li>
<li>
<p>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a>
[radarhere]</p>
</li>
<li>
<p>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a>
[radarhere]</p>
</li>
<li>
<p>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a>
[radarhere]</p>
</li>
<li>
<p>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a>
[radarhere]</p>
</li>
<li>
<p>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a>
[radarhere]</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-pillow/Pillow/commit/5c89d88eee199ba53f64581ea39b6a1bc52feb1a"><code>5c89d88</code></a> 10.3.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/63cbfcfdea2d163ec93bae8d283fcfe4b73b5dc7"><code>63cbfcf</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2776126aa9af322b416eaca247f4f8ebefd08128"><code>2776126</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> from python-pillow/lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/aeb51cbb169eb3285818ba1390ddf2771d897e6e"><code>aeb51cb</code></a> Merge branch 'main' into lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/5beb0b66648db8b542bb5260eed79b25e33d643b"><code>5beb0b6</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/cac6ffa7b399ea79b6239984d1307056a0b19af2"><code>cac6ffa</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a> from python-pillow/imagemath</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/f5eeeacf7539eaa0d93a677d7666bc7c142c8d1c"><code>f5eeeac</code></a> Name as 'options' in lambda_eval and unsafe_eval, but '_dict' in deprecated eval</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/facf3af93dabcbdd8cdbda8c3b50eefafa3bb04c"><code>facf3af</code></a> Added release notes</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2a93aba5cfcf6e241ab4f9392c13e3b74032c061"><code>2a93aba</code></a> Use strncpy to avoid buffer overflow</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/a670597bc30e9d489656fc9d807170b8f3d7ca57"><code>a670597</code></a> Update CHANGES.rst [ci skip]</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/10.2.0...10.3.0">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 19:08:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group in /oid4vci with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /oid4vci with 3 updates: [idna](https://github.com/kjd/idna), [jwcrypto](https://github.com/latchset/jwcrypto) and [pillow](https://github.com/python-pillow/Pillow).

Updates `idna` from 3.6 to 3.7
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
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `jwcrypto` from 1.5.1 to 1.5.6
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

Updates `pillow` from 10.2.0 to 10.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.3.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>CVE-2024-28219: Use strncpy to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Use <code>functools.lru_cache</code> for <code>hopper()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7912">#7912</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Raise ValueError if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improve speed of loading QOI images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7925">#7925</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added RGB to I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Add --report argument to <strong>main</strong>.py to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Added RGB to I;16, I;16L and I;16B conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a> [<a href="https://github.com/Yay295"><code>@​Yay295</code></a>]</li>
<li>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a> [<a href="https://github.com/scaramallion"><code>@​scaramallion</code></a>]</li>
<li>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed joined corners for ImageDraw rounded_rectangle() non-integer dimensions <a href="https://redirect.github.com/python-pillow/Pillow/issues/7881">#7881</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed Python and NumPy pinning on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7880">#7880</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Update UnidentifiedImageError and <strong>version</strong> imports <a href="https://redirect.github.com/python-pillow/Pillow/issues/7644">#7644</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Stop reading EPS image at EOF marker <a href="https://redirect.github.com/python-pillow/Pillow/issues/7753">#7753</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>PSD layer co-ordinates may be negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7706">#7706</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use subprocess with CREATE_NO_WINDOW flag in ImageShow WindowsViewer <a href="https://redirect.github.com/python-pillow/Pillow/issues/7791">#7791</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>When saving GIF frame that restores to background color, do not fill identical pixels <a href="https://redirect.github.com/python-pillow/Pillow/issues/7788">#7788</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed reading PNG iCCP compression method <a href="https://redirect.github.com/python-pillow/Pillow/issues/7823">#7823</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Allow writing IFDRational to UNDEFINED tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7840">#7840</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix logged tag name when loading Exif data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7842">#7842</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use maximum frame size in IHDR chunk when saving APNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7821">#7821</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Prevent opening P TGA images without a palette <a href="https://redirect.github.com/python-pillow/Pillow/issues/7797">#7797</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use palette when loading ICO images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7798">#7798</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use consistent arguments for load_read and load_seek <a href="https://redirect.github.com/python-pillow/Pillow/issues/7713">#7713</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Turn off nullability warnings for macOS SDK <a href="https://redirect.github.com/python-pillow/Pillow/issues/7827">#7827</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix shift-sign issue in Convert.c <a href="https://redirect.github.com/python-pillow/Pillow/issues/7838">#7838</a> [<a href="https://github.com/r-barnes"><code>@​r-barnes</code></a>]</li>
<li>winbuild: Refactor dependency versions into constants <a href="https://redirect.github.com/python-pillow/Pillow/issues/7843">#7843</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Build macOS arm64 wheels natively <a href="https://redirect.github.com/python-pillow/Pillow/issues/7852">#7852</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed typo <a href="https://redirect.github.com/python-pillow/Pillow/issues/7855">#7855</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Open 16-bit grayscale PNGs as I;16 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7849">#7849</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Handle truncated chunks at the end of PNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7709">#7709</a> [<a href="https://github.com/lajiyuan"><code>@​lajiyuan</code></a>]</li>
<li>Match mask size to pasted image size in GifImagePlugin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7779">#7779</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Changed SupportsGetMesh protocol to be public <a href="https://redirect.github.com/python-pillow/Pillow/issues/7841">#7841</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Release GIL while calling <code>WebPAnimDecoderGetNext</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7782">#7782</a> [<a href="https://github.com/evanmiller"><code>@​evanmiller</code></a>]</li>
<li>Fixed reading FLI/FLC images with a prefix chunk <a href="https://redirect.github.com/python-pillow/Pillow/issues/7804">#7804</a> [<a href="https://github.com/twolife"><code>@​twolife</code></a>]</li>
<li>Updated package name for Tidelift <a href="https://redirect.github.com/python-pillow/Pillow/issues/7810">#7810</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7744">#7744</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.3.0 (2024-04-01)</h2>
<ul>
<li>
<p>CVE-2024-28219: Use <code>strncpy</code> to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Deprecate <code>eval()</code>, replacing it with <code>lambda_eval()</code> and <code>unsafe_eval()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Raise <code>ValueError</code> if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a>
[radarhere]</p>
</li>
<li>
<p>Add <code>--report</code> argument to <code>__main__.py</code> to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a>
[nulano, radarhere, hugovk]</p>
</li>
<li>
<p>Added RGB to I;16, I;16L, I;16B and I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a>, <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a>
[radarhere]</p>
</li>
<li>
<p>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a>
[nulano, radarhere]</p>
</li>
<li>
<p>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a>
[Yay295, hugovk, radarhere]</p>
</li>
<li>
<p>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a>
[radarhere]</p>
</li>
<li>
<p>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a>
[radarhere]</p>
</li>
<li>
<p>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a>
[radarhere]</p>
</li>
<li>
<p>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a>
[scaramallion, radarhere]</p>
</li>
<li>
<p>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a>
[radarhere]</p>
</li>
<li>
<p>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a>
[radarhere]</p>
</li>
<li>
<p>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a>
[radarhere]</p>
</li>
<li>
<p>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a>
[radarhere]</p>
</li>
<li>
<p>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a>
[radarhere]</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-pillow/Pillow/commit/5c89d88eee199ba53f64581ea39b6a1bc52feb1a"><code>5c89d88</code></a> 10.3.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/63cbfcfdea2d163ec93bae8d283fcfe4b73b5dc7"><code>63cbfcf</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2776126aa9af322b416eaca247f4f8ebefd08128"><code>2776126</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> from python-pillow/lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/aeb51cbb169eb3285818ba1390ddf2771d897e6e"><code>aeb51cb</code></a> Merge branch 'main' into lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/5beb0b66648db8b542bb5260eed79b25e33d643b"><code>5beb0b6</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/cac6ffa7b399ea79b6239984d1307056a0b19af2"><code>cac6ffa</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a> from python-pillow/imagemath</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/f5eeeacf7539eaa0d93a677d7666bc7c142c8d1c"><code>f5eeeac</code></a> Name as 'options' in lambda_eval and unsafe_eval, but '_dict' in deprecated eval</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/facf3af93dabcbdd8cdbda8c3b50eefafa3bb04c"><code>facf3af</code></a> Added release notes</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2a93aba5cfcf6e241ab4f9392c13e3b74032c061"><code>2a93aba</code></a> Use strncpy to avoid buffer overflow</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/a670597bc30e9d489656fc9d807170b8f3d7ca57"><code>a670597</code></a> Update CHANGES.rst [ci skip]</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/10.2.0...10.3.0">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 19:08:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/427" class=".btn">#427</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group in /connection_update with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /connection_update with 4 updates: [black](https://github.com/psf/black), [idna](https://github.com/kjd/idna), [jwcrypto](https://github.com/latchset/jwcrypto) and [pillow](https://github.com/python-pillow/Pillow).

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

Updates `idna` from 3.6 to 3.7
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
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `jwcrypto` from 1.5.4 to 1.5.6
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

Updates `pillow` from 10.2.0 to 10.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.3.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>CVE-2024-28219: Use strncpy to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Use <code>functools.lru_cache</code> for <code>hopper()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7912">#7912</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Raise ValueError if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improve speed of loading QOI images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7925">#7925</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added RGB to I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Add --report argument to <strong>main</strong>.py to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Added RGB to I;16, I;16L and I;16B conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a> [<a href="https://github.com/Yay295"><code>@​Yay295</code></a>]</li>
<li>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a> [<a href="https://github.com/scaramallion"><code>@​scaramallion</code></a>]</li>
<li>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed joined corners for ImageDraw rounded_rectangle() non-integer dimensions <a href="https://redirect.github.com/python-pillow/Pillow/issues/7881">#7881</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed Python and NumPy pinning on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7880">#7880</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Update UnidentifiedImageError and <strong>version</strong> imports <a href="https://redirect.github.com/python-pillow/Pillow/issues/7644">#7644</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Stop reading EPS image at EOF marker <a href="https://redirect.github.com/python-pillow/Pillow/issues/7753">#7753</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>PSD layer co-ordinates may be negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7706">#7706</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use subprocess with CREATE_NO_WINDOW flag in ImageShow WindowsViewer <a href="https://redirect.github.com/python-pillow/Pillow/issues/7791">#7791</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>When saving GIF frame that restores to background color, do not fill identical pixels <a href="https://redirect.github.com/python-pillow/Pillow/issues/7788">#7788</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed reading PNG iCCP compression method <a href="https://redirect.github.com/python-pillow/Pillow/issues/7823">#7823</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Allow writing IFDRational to UNDEFINED tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7840">#7840</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix logged tag name when loading Exif data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7842">#7842</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use maximum frame size in IHDR chunk when saving APNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7821">#7821</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Prevent opening P TGA images without a palette <a href="https://redirect.github.com/python-pillow/Pillow/issues/7797">#7797</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use palette when loading ICO images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7798">#7798</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use consistent arguments for load_read and load_seek <a href="https://redirect.github.com/python-pillow/Pillow/issues/7713">#7713</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Turn off nullability warnings for macOS SDK <a href="https://redirect.github.com/python-pillow/Pillow/issues/7827">#7827</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix shift-sign issue in Convert.c <a href="https://redirect.github.com/python-pillow/Pillow/issues/7838">#7838</a> [<a href="https://github.com/r-barnes"><code>@​r-barnes</code></a>]</li>
<li>winbuild: Refactor dependency versions into constants <a href="https://redirect.github.com/python-pillow/Pillow/issues/7843">#7843</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Build macOS arm64 wheels natively <a href="https://redirect.github.com/python-pillow/Pillow/issues/7852">#7852</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed typo <a href="https://redirect.github.com/python-pillow/Pillow/issues/7855">#7855</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Open 16-bit grayscale PNGs as I;16 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7849">#7849</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Handle truncated chunks at the end of PNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7709">#7709</a> [<a href="https://github.com/lajiyuan"><code>@​lajiyuan</code></a>]</li>
<li>Match mask size to pasted image size in GifImagePlugin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7779">#7779</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Changed SupportsGetMesh protocol to be public <a href="https://redirect.github.com/python-pillow/Pillow/issues/7841">#7841</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Release GIL while calling <code>WebPAnimDecoderGetNext</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7782">#7782</a> [<a href="https://github.com/evanmiller"><code>@​evanmiller</code></a>]</li>
<li>Fixed reading FLI/FLC images with a prefix chunk <a href="https://redirect.github.com/python-pillow/Pillow/issues/7804">#7804</a> [<a href="https://github.com/twolife"><code>@​twolife</code></a>]</li>
<li>Updated package name for Tidelift <a href="https://redirect.github.com/python-pillow/Pillow/issues/7810">#7810</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7744">#7744</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.3.0 (2024-04-01)</h2>
<ul>
<li>
<p>CVE-2024-28219: Use <code>strncpy</code> to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Deprecate <code>eval()</code>, replacing it with <code>lambda_eval()</code> and <code>unsafe_eval()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Raise <code>ValueError</code> if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a>
[radarhere]</p>
</li>
<li>
<p>Add <code>--report</code> argument to <code>__main__.py</code> to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a>
[nulano, radarhere, hugovk]</p>
</li>
<li>
<p>Added RGB to I;16, I;16L, I;16B and I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a>, <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a>
[radarhere]</p>
</li>
<li>
<p>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a>
[nulano, radarhere]</p>
</li>
<li>
<p>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a>
[Yay295, hugovk, radarhere]</p>
</li>
<li>
<p>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a>
[radarhere]</p>
</li>
<li>
<p>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a>
[radarhere]</p>
</li>
<li>
<p>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a>
[radarhere]</p>
</li>
<li>
<p>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a>
[scaramallion, radarhere]</p>
</li>
<li>
<p>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a>
[radarhere]</p>
</li>
<li>
<p>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a>
[radarhere]</p>
</li>
<li>
<p>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a>
[radarhere]</p>
</li>
<li>
<p>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a>
[radarhere]</p>
</li>
<li>
<p>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a>
[radarhere]</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-pillow/Pillow/commit/5c89d88eee199ba53f64581ea39b6a1bc52feb1a"><code>5c89d88</code></a> 10.3.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/63cbfcfdea2d163ec93bae8d283fcfe4b73b5dc7"><code>63cbfcf</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2776126aa9af322b416eaca247f4f8ebefd08128"><code>2776126</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> from python-pillow/lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/aeb51cbb169eb3285818ba1390ddf2771d897e6e"><code>aeb51cb</code></a> Merge branch 'main' into lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/5beb0b66648db8b542bb5260eed79b25e33d643b"><code>5beb0b6</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/cac6ffa7b399ea79b6239984d1307056a0b19af2"><code>cac6ffa</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a> from python-pillow/imagemath</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/f5eeeacf7539eaa0d93a677d7666bc7c142c8d1c"><code>f5eeeac</code></a> Name as 'options' in lambda_eval and unsafe_eval, but '_dict' in deprecated eval</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/facf3af93dabcbdd8cdbda8c3b50eefafa3bb04c"><code>facf3af</code></a> Added release notes</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2a93aba5cfcf6e241ab4f9392c13e3b74032c061"><code>2a93aba</code></a> Use strncpy to avoid buffer overflow</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/a670597bc30e9d489656fc9d807170b8f3d7ca57"><code>a670597</code></a> Update CHANGES.rst [ci skip]</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/10.2.0...10.3.0">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 19:08:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/426" class=".btn">#426</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group in /basicmessage_storage with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /basicmessage_storage with 4 updates: [black](https://github.com/psf/black), [idna](https://github.com/kjd/idna), [jwcrypto](https://github.com/latchset/jwcrypto) and [pillow](https://github.com/python-pillow/Pillow).

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

Updates `idna` from 3.6 to 3.7
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
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">compare view</a></li>
</ul>
</details>
<br />

Updates `jwcrypto` from 1.5.4 to 1.5.6
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

Updates `pillow` from 10.2.0 to 10.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.3.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.3.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>CVE-2024-28219: Use strncpy to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Use <code>functools.lru_cache</code> for <code>hopper()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7912">#7912</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Raise ValueError if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improve speed of loading QOI images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7925">#7925</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added RGB to I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Add --report argument to <strong>main</strong>.py to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Added RGB to I;16, I;16L and I;16B conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a> [<a href="https://github.com/Yay295"><code>@​Yay295</code></a>]</li>
<li>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a> [<a href="https://github.com/scaramallion"><code>@​scaramallion</code></a>]</li>
<li>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed joined corners for ImageDraw rounded_rectangle() non-integer dimensions <a href="https://redirect.github.com/python-pillow/Pillow/issues/7881">#7881</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed Python and NumPy pinning on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7880">#7880</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Update UnidentifiedImageError and <strong>version</strong> imports <a href="https://redirect.github.com/python-pillow/Pillow/issues/7644">#7644</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Stop reading EPS image at EOF marker <a href="https://redirect.github.com/python-pillow/Pillow/issues/7753">#7753</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>PSD layer co-ordinates may be negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7706">#7706</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use subprocess with CREATE_NO_WINDOW flag in ImageShow WindowsViewer <a href="https://redirect.github.com/python-pillow/Pillow/issues/7791">#7791</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>When saving GIF frame that restores to background color, do not fill identical pixels <a href="https://redirect.github.com/python-pillow/Pillow/issues/7788">#7788</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed reading PNG iCCP compression method <a href="https://redirect.github.com/python-pillow/Pillow/issues/7823">#7823</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Allow writing IFDRational to UNDEFINED tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7840">#7840</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix logged tag name when loading Exif data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7842">#7842</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use maximum frame size in IHDR chunk when saving APNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7821">#7821</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Prevent opening P TGA images without a palette <a href="https://redirect.github.com/python-pillow/Pillow/issues/7797">#7797</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use palette when loading ICO images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7798">#7798</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use consistent arguments for load_read and load_seek <a href="https://redirect.github.com/python-pillow/Pillow/issues/7713">#7713</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Turn off nullability warnings for macOS SDK <a href="https://redirect.github.com/python-pillow/Pillow/issues/7827">#7827</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix shift-sign issue in Convert.c <a href="https://redirect.github.com/python-pillow/Pillow/issues/7838">#7838</a> [<a href="https://github.com/r-barnes"><code>@​r-barnes</code></a>]</li>
<li>winbuild: Refactor dependency versions into constants <a href="https://redirect.github.com/python-pillow/Pillow/issues/7843">#7843</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Build macOS arm64 wheels natively <a href="https://redirect.github.com/python-pillow/Pillow/issues/7852">#7852</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed typo <a href="https://redirect.github.com/python-pillow/Pillow/issues/7855">#7855</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Open 16-bit grayscale PNGs as I;16 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7849">#7849</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Handle truncated chunks at the end of PNG images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7709">#7709</a> [<a href="https://github.com/lajiyuan"><code>@​lajiyuan</code></a>]</li>
<li>Match mask size to pasted image size in GifImagePlugin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7779">#7779</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Changed SupportsGetMesh protocol to be public <a href="https://redirect.github.com/python-pillow/Pillow/issues/7841">#7841</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Release GIL while calling <code>WebPAnimDecoderGetNext</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7782">#7782</a> [<a href="https://github.com/evanmiller"><code>@​evanmiller</code></a>]</li>
<li>Fixed reading FLI/FLC images with a prefix chunk <a href="https://redirect.github.com/python-pillow/Pillow/issues/7804">#7804</a> [<a href="https://github.com/twolife"><code>@​twolife</code></a>]</li>
<li>Updated package name for Tidelift <a href="https://redirect.github.com/python-pillow/Pillow/issues/7810">#7810</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7744">#7744</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.3.0 (2024-04-01)</h2>
<ul>
<li>
<p>CVE-2024-28219: Use <code>strncpy</code> to avoid buffer overflow <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Deprecate <code>eval()</code>, replacing it with <code>lambda_eval()</code> and <code>unsafe_eval()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Raise <code>ValueError</code> if seeking to greater than offset-sized integer in TIFF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7883">#7883</a>
[radarhere]</p>
</li>
<li>
<p>Add <code>--report</code> argument to <code>__main__.py</code> to omit supported formats <a href="https://redirect.github.com/python-pillow/Pillow/issues/7818">#7818</a>
[nulano, radarhere, hugovk]</p>
</li>
<li>
<p>Added RGB to I;16, I;16L, I;16B and I;16N conversion <a href="https://redirect.github.com/python-pillow/Pillow/issues/7918">#7918</a>, <a href="https://redirect.github.com/python-pillow/Pillow/issues/7920">#7920</a>
[radarhere]</p>
</li>
<li>
<p>Fix editable installation with custom build backend and configuration options <a href="https://redirect.github.com/python-pillow/Pillow/issues/7658">#7658</a>
[nulano, radarhere]</p>
</li>
<li>
<p>Fix putdata() for I;16N on big-endian <a href="https://redirect.github.com/python-pillow/Pillow/issues/7209">#7209</a>
[Yay295, hugovk, radarhere]</p>
</li>
<li>
<p>Determine MPO size from markers, not EXIF data <a href="https://redirect.github.com/python-pillow/Pillow/issues/7884">#7884</a>
[radarhere]</p>
</li>
<li>
<p>Improved conversion from RGB to RGBa, LA and La <a href="https://redirect.github.com/python-pillow/Pillow/issues/7888">#7888</a>
[radarhere]</p>
</li>
<li>
<p>Support FITS images with GZIP_1 compression <a href="https://redirect.github.com/python-pillow/Pillow/issues/7894">#7894</a>
[radarhere]</p>
</li>
<li>
<p>Use I;16 mode for 9-bit JPEG 2000 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7900">#7900</a>
[scaramallion, radarhere]</p>
</li>
<li>
<p>Raise ValueError if kmeans is negative <a href="https://redirect.github.com/python-pillow/Pillow/issues/7891">#7891</a>
[radarhere]</p>
</li>
<li>
<p>Remove TIFF tag OSUBFILETYPE when saving using libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7893">#7893</a>
[radarhere]</p>
</li>
<li>
<p>Raise ValueError for negative values when loading P1-P3 PPM images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7882">#7882</a>
[radarhere]</p>
</li>
<li>
<p>Added reading of JPEG2000 palettes <a href="https://redirect.github.com/python-pillow/Pillow/issues/7870">#7870</a>
[radarhere]</p>
</li>
<li>
<p>Added alpha_quality argument when saving WebP images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7872">#7872</a>
[radarhere]</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-pillow/Pillow/commit/5c89d88eee199ba53f64581ea39b6a1bc52feb1a"><code>5c89d88</code></a> 10.3.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/63cbfcfdea2d163ec93bae8d283fcfe4b73b5dc7"><code>63cbfcf</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2776126aa9af322b416eaca247f4f8ebefd08128"><code>2776126</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7928">#7928</a> from python-pillow/lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/aeb51cbb169eb3285818ba1390ddf2771d897e6e"><code>aeb51cb</code></a> Merge branch 'main' into lcms</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/5beb0b66648db8b542bb5260eed79b25e33d643b"><code>5beb0b6</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/cac6ffa7b399ea79b6239984d1307056a0b19af2"><code>cac6ffa</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7927">#7927</a> from python-pillow/imagemath</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/f5eeeacf7539eaa0d93a677d7666bc7c142c8d1c"><code>f5eeeac</code></a> Name as 'options' in lambda_eval and unsafe_eval, but '_dict' in deprecated eval</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/facf3af93dabcbdd8cdbda8c3b50eefafa3bb04c"><code>facf3af</code></a> Added release notes</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/2a93aba5cfcf6e241ab4f9392c13e3b74032c061"><code>2a93aba</code></a> Use strncpy to avoid buffer overflow</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/a670597bc30e9d489656fc9d807170b8f3d7ca57"><code>a670597</code></a> Update CHANGES.rst [ci skip]</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/10.2.0...10.3.0">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 19:07:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/425" class=".btn">#425</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.2 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-03 05:13:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/424" class=".btn">#424</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update pytest-ruff requirement from ^0.1.1 to ^0.3.2 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pytest-ruff](https://github.com/businho/pytest-ruff) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-03 05:09:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/423" class=".btn">#423</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.2 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-03 04:43:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.2 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-03 04:42:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.2 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-03 04:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.2 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-03 04:34:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.2 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-03 04:20:35 +0000 UTC
    </div>
</div>

