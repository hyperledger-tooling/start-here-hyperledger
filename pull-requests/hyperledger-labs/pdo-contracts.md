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
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Reformat documents for 80 character limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No content changes. Just reformats.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-13 23:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Bump pillow from 8.4.0 to 10.0.1 in /inference-contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [pillow](https://github.com/python-pillow/Pillow) from 8.4.0 to 10.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/releases">pillow's releases</a>.</em></p>
<blockquote>
<h2>10.0.1</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.0.1.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.0.1.html</a></p>
<h2>Changes</h2>
<ul>
<li>Updated libwebp to 1.3.2 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7395">#7395</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Updated zlib to 1.3 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7344">#7344</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<h2>10.0.0</h2>
<p><a href="https://pillow.readthedocs.io/en/stable/releasenotes/10.0.0.html">https://pillow.readthedocs.io/en/stable/releasenotes/10.0.0.html</a></p>
<h2>Changes</h2>
<ul>
<li>Fixed deallocating mask images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7246">#7246</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added ImageFont.MAX_STRING_LENGTH <a href="https://redirect.github.com/python-pillow/Pillow/issues/7244">#7244</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fix Windows build with pyproject.toml <a href="https://redirect.github.com/python-pillow/Pillow/issues/7230">#7230</a> [<a href="https://github.com/nulano"><code>@​nulano</code></a>]</li>
<li>Do not close provided file handles with libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7199">#7199</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Convert to HSV if mode is HSV in getcolor() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7226">#7226</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added alpha_only argument to getbbox() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7123">#7123</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Prioritise speed in <em>repr_png</em> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7242">#7242</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Limit size even if one dimension is zero in decompression bomb check <a href="https://redirect.github.com/python-pillow/Pillow/issues/7235">#7235</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Restored 32-bit support <a href="https://redirect.github.com/python-pillow/Pillow/issues/7234">#7234</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed deleted file from codecov.yml and increased coverage threshold <a href="https://redirect.github.com/python-pillow/Pillow/issues/7232">#7232</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed support for 32-bit <a href="https://redirect.github.com/python-pillow/Pillow/issues/7228">#7228</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use --config-settings instead of deprecated --global-option <a href="https://redirect.github.com/python-pillow/Pillow/issues/7171">#7171</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Better C integer definitions <a href="https://redirect.github.com/python-pillow/Pillow/issues/6645">#6645</a> [<a href="https://github.com/Yay295"><code>@​Yay295</code></a>]</li>
<li>Fixed finding dependencies on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7175">#7175</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Improved checks in font_render <a href="https://redirect.github.com/python-pillow/Pillow/issues/7218">#7218</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Change <code>grabclipboard()</code> to use PNG compression on macOS <a href="https://redirect.github.com/python-pillow/Pillow/issues/7219">#7219</a> [<a href="https://github.com/abey79"><code>@​abey79</code></a>]</li>
<li>Added PyPy 3.10 and removed PyPy 3.8 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7216">#7216</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Added in_place argument to ImageOps.exif_transpose() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7092">#7092</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Corrected error code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7177">#7177</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Use &quot;not in&quot; <a href="https://redirect.github.com/python-pillow/Pillow/issues/7174">#7174</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Only call text_layout once in getmask2 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7206">#7206</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed calling putpalette() on L and LA images before load() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7187">#7187</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused INT64 definition <a href="https://redirect.github.com/python-pillow/Pillow/issues/7180">#7180</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Updated xz to 5.4.3 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7136">#7136</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed saving TIFF multiframe images with LONG8 tag types <a href="https://redirect.github.com/python-pillow/Pillow/issues/7078">#7078</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Do not set size unnecessarily if image fails to open <a href="https://redirect.github.com/python-pillow/Pillow/issues/7056">#7056</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused code <a href="https://redirect.github.com/python-pillow/Pillow/issues/7210">#7210</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed unused variables <a href="https://redirect.github.com/python-pillow/Pillow/issues/7205">#7205</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed signedness comparison warning <a href="https://redirect.github.com/python-pillow/Pillow/issues/7203">#7203</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed combining single duration across duplicate APNG frames <a href="https://redirect.github.com/python-pillow/Pillow/issues/7146">#7146</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Remove temporary file when error is raised <a href="https://redirect.github.com/python-pillow/Pillow/issues/7148">#7148</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Do not use temporary file when grabbing clipboard on Linux <a href="https://redirect.github.com/python-pillow/Pillow/issues/7200">#7200</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>If the clipboard fails to open on Windows, wait and try again <a href="https://redirect.github.com/python-pillow/Pillow/issues/7141">#7141</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Fixed saving multiple 1 mode frames to GIF <a href="https://redirect.github.com/python-pillow/Pillow/issues/7181">#7181</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Replaced absolute PIL import with relative import <a href="https://redirect.github.com/python-pillow/Pillow/issues/7173">#7173</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
<li>Removed files and types override <a href="https://redirect.github.com/python-pillow/Pillow/issues/7194">#7194</a> [<a href="https://github.com/radarhere"><code>@​radarhere</code></a>]</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst">pillow's changelog</a>.</em></p>
<blockquote>
<h2>10.0.1 (2023-09-15)</h2>
<ul>
<li>
<p>Updated libwebp to 1.3.2 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7395">#7395</a>
[radarhere]</p>
</li>
<li>
<p>Updated zlib to 1.3 <a href="https://redirect.github.com/python-pillow/Pillow/issues/7344">#7344</a>
[radarhere]</p>
</li>
</ul>
<h2>10.0.0 (2023-07-01)</h2>
<ul>
<li>
<p>Fixed deallocating mask images <a href="https://redirect.github.com/python-pillow/Pillow/issues/7246">#7246</a>
[radarhere]</p>
</li>
<li>
<p>Added ImageFont.MAX_STRING_LENGTH <a href="https://redirect.github.com/python-pillow/Pillow/issues/7244">#7244</a>
[radarhere, hugovk]</p>
</li>
<li>
<p>Fix Windows build with pyproject.toml <a href="https://redirect.github.com/python-pillow/Pillow/issues/7230">#7230</a>
[hugovk, nulano, radarhere]</p>
</li>
<li>
<p>Do not close provided file handles with libtiff <a href="https://redirect.github.com/python-pillow/Pillow/issues/7199">#7199</a>
[radarhere]</p>
</li>
<li>
<p>Convert to HSV if mode is HSV in getcolor() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7226">#7226</a>
[radarhere]</p>
</li>
<li>
<p>Added alpha_only argument to getbbox() <a href="https://redirect.github.com/python-pillow/Pillow/issues/7123">#7123</a>
[radarhere. hugovk]</p>
</li>
<li>
<p>Prioritise speed in <em>repr_png</em> <a href="https://redirect.github.com/python-pillow/Pillow/issues/7242">#7242</a>
[radarhere]</p>
</li>
<li>
<p>Do not use CFFI access by default on PyPy <a href="https://redirect.github.com/python-pillow/Pillow/issues/7236">#7236</a>
[radarhere]</p>
</li>
<li>
<p>Limit size even if one dimension is zero in decompression bomb check <a href="https://redirect.github.com/python-pillow/Pillow/issues/7235">#7235</a>
[radarhere]</p>
</li>
<li>
<p>Use --config-settings instead of deprecated --global-option <a href="https://redirect.github.com/python-pillow/Pillow/issues/7171">#7171</a>
[radarhere]</p>
</li>
<li>
<p>Better C integer definitions <a href="https://redirect.github.com/python-pillow/Pillow/issues/6645">#6645</a>
[Yay295, hugovk]</p>
</li>
<li>
<p>Fixed finding dependencies on Cygwin <a href="https://redirect.github.com/python-pillow/Pillow/issues/7175">#7175</a>
[radarhere]</p>
</li>
<li>
<p>Changed grabclipboard() to use PNG instead of JPG compression on macOS <a href="https://redirect.github.com/python-pillow/Pillow/issues/7219">#7219</a>
[abey79, radarhere]</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-pillow/Pillow/commit/e34d346f10c0b1c814661e662a3e0c1ef084cf1c"><code>e34d346</code></a> Updated order</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/a62f2402a6bcf11a0a1670542216725a3f9190e0"><code>a62f240</code></a> 10.0.1 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/d50250d9eab741ae3ddd592d8910cfd7973b9d35"><code>d50250d</code></a> Added release notes for 10.0.1</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/b4c7d4b8b2710b7af6cc944a804902eb75fd9056"><code>b4c7d4b</code></a> Update CHANGES.rst [ci skip]</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/730f74600e8215ab510f71bb1fbb49d906c4356b"><code>730f746</code></a> Updated libwebp to 1.3.2</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/b0e28048d692effadfe7a4268a03e1d20e0198bb"><code>b0e2804</code></a> Updated zlib to 1.3</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/6e28ed1f36d0eb74053af54e1eddc9c29db698cd"><code>6e28ed1</code></a> 10.0.0 version bump</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/c827f3b30f50bf04fd65daeeba6bbfd56fc7b50e"><code>c827f3b</code></a> Merge pull request <a href="https://redirect.github.com/python-pillow/Pillow/issues/7246">#7246</a> from radarhere/deallocate</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/39a3b1d83edcf826c3864e26bedff5b4e4dd331b"><code>39a3b1d</code></a> Fixed deallocating mask images</li>
<li><a href="https://github.com/python-pillow/Pillow/commit/8c1dc819fd91471825da01976ac0e0bc8789590f"><code>8c1dc81</code></a> Update CHANGES.rst [ci skip]</li>
<li>Additional commits viewable in <a href="https://github.com/python-pillow/Pillow/compare/8.4.0...10.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pillow&package-manager=pip&previous-version=8.4.0&new-version=10.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-01-13 22:40:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    New sample PDO contracts for managing policy-based access to OpenVINO ML models
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR introduces new sample PDO contracts for managing policy-based access to OpenVINO ML models. Files are located under inference-contract/. Please see inference-contract/README.md for overview of the new capabilities, as well instructions for testing the new samples.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 00:39:18 +0000 UTC
    </div>
</div>

