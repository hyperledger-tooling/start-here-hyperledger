---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Bump pillow from 8.4.0 to 10.2.0 in /inference-contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [pillow](https://github.com/python-pillow/Pillow) from 8.4.0 to 10.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.2.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.2.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.2.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>Add <code>keep_rgb</code> option when saving JPEG to prevent conversion of RGB colorspace <a href="https://redirect.github.com/python-pillow/Pillow/issues/7553">#7553</a> [<a href="https://github.com/bgilbert"><code>@​bgilbert</code></a>]</li>
<li>Trim negative glyph offsets in ImageFont.getmask() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7672">#7672</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Removed unnecessary &quot;pragma: no cover&quot; <a href="https://redirect.github.com/python-pillow/Pillow/issues/7668">#7668</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Trim glyph size in ImageFont.getmask() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7669">#7669</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix loading IPTC images and update test <a href="https://redirect.github.com/python-pillow/Pillow/issues/7667">#7667</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Allow uncompressed TIFF images to be saved in chunks <a href="https://redirect.github.com/python-pillow/Pillow/issues/7650">#7650</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Concatenate multiple JPEG EXIF markers <a href="https://redirect.github.com/python-pillow/Pillow/issues/7496">#7496</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Changed IPTC tile tuple to match other plugins <a href="https://redirect.github.com/python-pillow/Pillow/issues/7661">#7661</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Do not assign new fp attribute when exiting context manager <a href="https://redirect.github.com/python-pillow/Pillow/issues/7566">#7566</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support arbitrary masks for uncompressed RGB DDS images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7589">#7589</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support setting ROWSPERSTRIP tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7654">#7654</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Apply ImageFont.MAX_STRING_LENGTH to ImageFont.getmask() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7662">#7662</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Optimise <code>ImageColor</code> using <code>functools.lru_cache</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7657">#7657</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Restricted environment keys for ImageMath.eval() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7655">#7655</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Optimise <code>ImageMode.getmode</code> using <code>functools.lru_cache</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7641">#7641</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Added trusted PyPI publishing <a href="https://redirect.github.com/python-pillow/Pillow/issues/7616">#7616</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Compile FriBiDi for Windows ARM64 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7629">#7629</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Fix incorrect color blending for overlapping glyphs <a href="https://redirect.github.com/python-pillow/Pillow/issues/7497">#7497</a> [<a href="https://github.com/ZachNagengast"><code>@​ZachNagengast</code></a>]</li>
<li>Add .git-blame-ignore-revs file <a href="https://redirect.github.com/python-pillow/Pillow/issues/7528">#7528</a> [<a href="https://github.com/akx"><code>@​akx</code></a>]</li>
<li>Attempt memory mapping when tile args is a string <a href="https://redirect.github.com/python-pillow/Pillow/issues/7565">#7565</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fill identical pixels with transparency in subsequent frames when saving GIF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7568">#7568</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unnecessary string length check <a href="https://redirect.github.com/python-pillow/Pillow/issues/7560">#7560</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Determine mask mode in Python instead of C <a href="https://redirect.github.com/python-pillow/Pillow/issues/7548">#7548</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Corrected duration when combining multiple GIF frames into single frame <a href="https://redirect.github.com/python-pillow/Pillow/issues/7521">#7521</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Handle disposing GIF background from outside palette <a href="https://redirect.github.com/python-pillow/Pillow/issues/7515">#7515</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Seek past the data when skipping a PSD layer <a href="https://redirect.github.com/python-pillow/Pillow/issues/7483">#7483</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>ImageMath: Inline <code>isinstance</code> check <a href="https://redirect.github.com/python-pillow/Pillow/issues/7623">#7623</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Update actions/upload-artifact action to v4 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7619">#7619</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Import plugins relative to the module <a href="https://redirect.github.com/python-pillow/Pillow/issues/7576">#7576</a> [<a href="https://github.com/deliangyang"><code>@​deliangyang</code></a>]</li>
<li>Translate encoder error codes to strings; deprecate <code>ImageFile.raise_oserror()</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7609">#7609</a> [<a href="https://github.com/bgilbert"><code>@​bgilbert</code></a>]</li>
<li>Updated readthedocs to latest version of Python <a href="https://redirect.github.com/python-pillow/Pillow/issues/7611">#7611</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Support reading BC4U and DX10 BC1 images <a href="https://redirect.github.com/python-pillow/Pillow/issues/6486">#6486</a> [<a href="https://github.com/REDxEYE"><code>@​REDxEYE</code></a>]</li>
<li>Optimize ImageStat.Stat.extrema <a href="https://redirect.github.com/python-pillow/Pillow/issues/7593">#7593</a> [<a href="https://github.com/florath"><code>@​florath</code></a>]</li>
<li>Handle pathlib.Path in FreeTypeFont <a href="https://redirect.github.com/python-pillow/Pillow/issues/7578">#7578</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use list comprehensions to create transformed lists <a href="https://redirect.github.com/python-pillow/Pillow/issues/7597">#7597</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
<li>Added support for reading DX10 BC4 DDS images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7603">#7603</a> [<a href="https://github.com/sambvfx"><code>@​sambvfx</code></a>]</li>
<li>Optimized ImageStat.Stat.count <a href="https://redirect.github.com/python-pillow/Pillow/issues/7599">#7599</a> [<a href="https://github.com/florath"><code>@​florath</code></a>]</li>
<li>Moved error from truetype() to FreeTypeFont <a href="https://redirect.github.com/python-pillow/Pillow/issues/7587">#7587</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Correct PDF palette size when saving <a href="https://redirect.github.com/python-pillow/Pillow/issues/7555">#7555</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed closing file pointer with olefile 0.47 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7594">#7594</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>ruff: Minor optimizations of list comprehensions, x in set, etc. <a href="https://redirect.github.com/python-pillow/Pillow/issues/7524">#7524</a> [<a href="https://github.com/cclauss"><code>@​cclauss</code></a>]</li>
<li>Build Windows wheels using cibuildwheel <a href="https://redirect.github.com/python-pillow/Pillow/issues/7580">#7580</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Raise ValueError when TrueType font size is zero or less <a href="https://redirect.github.com/python-pillow/Pillow/issues/7584">#7584</a> [<a href="https://github.com/akx"><code>@​akx</code></a>]</li>
<li>Install cibuildwheel from requirements file <a href="https://redirect.github.com/python-pillow/Pillow/issues/7581">#7581</a> [<a href="https://github.com/hugovk"><code>@​hugovk</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.2.0 (2024-01-02)</h2>
<ul>
<li>
<p>Add <code>keep_rgb</code> option when saving JPEG to prevent conversion of RGB colorspace <a href="https://redirect.github.com/python-pillow/Pillow/issues/7553">#7553</a>
[bgilbert, radarhere]</p>
</li>
<li>
<p>Trim glyph size in ImageFont.getmask() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7669">#7669</a>, <a href="https://redirect.github.com/python-pillow/Pillow/issues/7672">#7672</a>
[radarhere, nulano]</p>
</li>
<li>
<p>Deprecate IptcImagePlugin helpers <a href="https://redirect.github.com/python-pillow/Pillow/issues/7664">#7664</a>
[nulano, hugovk, radarhere]</p>
</li>
<li>
<p>Allow uncompressed TIFF images to be saved in chunks <a href="https://redirect.github.com/python-pillow/Pillow/issues/7650">#7650</a>
[radarhere]</p>
</li>
<li>
<p>Concatenate multiple JPEG EXIF markers <a href="https://redirect.github.com/python-pillow/Pillow/issues/7496">#7496</a>
[radarhere]</p>
</li>
<li>
<p>Changed IPTC tile tuple to match other plugins <a href="https://redirect.github.com/python-pillow/Pillow/issues/7661">#7661</a>
[radarhere]</p>
</li>
<li>
<p>Do not assign new fp attribute when exiting context manager <a href="https://redirect.github.com/python-pillow/Pillow/issues/7566">#7566</a>
[radarhere]</p>
</li>
<li>
<p>Support arbitrary masks for uncompressed RGB DDS images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7589">#7589</a>
[radarhere, akx]</p>
</li>
<li>
<p>Support setting ROWSPERSTRIP tag <a href="https://redirect.github.com/python-pillow/Pillow/issues/7654">#7654</a>
[radarhere]</p>
</li>
<li>
<p>Apply ImageFont.MAX_STRING_LENGTH to ImageFont.getmask() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7662">#7662</a>
[radarhere]</p>
</li>
<li>
<p>Optimise <code>ImageColor</code> using <code>functools.lru_cache</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7657">#7657</a>
[hugovk]</p>
</li>
<li>
<p>Restricted environment keys for ImageMath.eval() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7655">#7655</a>
[wiredfool, radarhere]</p>
</li>
<li>
<p>Optimise <code>ImageMode.getmode</code> using <code>functools.lru_cache</code> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7641">#7641</a>
[hugovk, radarhere]</p>
</li>
<li>
<p>Fix incorrect color blending for overlapping glyphs <a href="https://redirect.github.com/python-pillow/Pillow/issues/7497">#7497</a>
[ZachNagengast, nulano, radarhere]</p>
</li>
<li>
<p>Attempt memory mapping when tile args is a string <a href="https://redirect.github.com/python-pillow/Pillow/issues/7565">#7565</a>
[radarhere]</p>
</li>
<li>
<p>Fill identical pixels with transparency in subsequent frames when saving GIF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7568">#7568</a>
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
<li><a href="https://github.com/python-pillow/Pillow/commit/6956d0b2853f5c7ec5f6ec4c60725c5a7ee73aeb"><code>6956d0b</code></a> 10.2.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/31c8dacdc727673e9099f1ac86019714cdccec67"><code>31c8dac</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7675">#7675</a> from python-pillow/pre-commit-ci-update-config</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/40a3f91af2c78870676a13629b5902bab4ab4cf0"><code>40a3f91</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7674">#7674</a> from nulano/url-example</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/cb41b0cc78eeefbd9ed2ce8c10f8d6d4c405a706"><code>cb41b0c</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/de62b25ed318f1604aa4ccd6f942a04c6b2c8b59"><code>de62b25</code></a> fix image url in &quot;Reading from URL&quot; example</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/7c526a6c6bdc7cb947f0aee1d1ee17c266ff6c61"><code>7c526a6</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/d93a5ad70bf94dbb63bdbfb19491a02976574d6d"><code>d93a5ad</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7553">#7553</a> from bgilbert/jpeg-rgb</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/aed764fe8404926472499208a39e5bf90d861b2a"><code>aed764f</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/f8df5303fa9daf40cf8bfe232403cb40389d8f8f"><code>f8df530</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7672">#7672</a> from nulano/imagefont-negative-crop</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/24e9485e6bb733a1a816f228dc75fd0086a93e19"><code>24e9485</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7671">#7671</a> from radarhere/imagetransform</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/8.4.0...10.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pillow&package-manager=pip&previous-version=8.4.0&new-version=10.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pdo-contracts/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 01:02:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Allow for local override of contract families to be built
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                By default, all contract families are built. Tests will be run from all families.

This update supports a local cmake file (Local.cmake) that will allow for local overrides of variables. In particular, this is useful to set the new CMake variable CONTRACT_FAMILIES to just the subset that you want to build.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 00:11:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Updated Jupyter notebooks for exchange family 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Significant update for the Jupyter notebooks in the exchange contract family. Notebooks added for creating and importing orders, for interacting with an issuer as an account holder, and for kick starting the factories there is a new index file.

To make all this work, this update adds an experimental file format for sharing contract information. The file uses the python zip library (distributed with python) to package the PDO files and the context files. 

Updated from earlier draft PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 21:41:41 +0000 UTC
    </div>
</div>

