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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2872" class=".btn">#2872</a>
            </td>
            <td>
                <b>
                    Emit the OOB done event even for multi-use invites
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue #2859

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 19:43:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2870" class=".btn">#2870</a>
            </td>
            <td>
                <b>
                    refactor: logging configs setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Looking for some feedback on this. Trying to clean up the logging config
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 16:32:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2869" class=".btn">#2869</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump pillow from 10.2.0 to 10.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pillow](https://github.com/python-pillow/Pillow) from 10.2.0 to 10.3.0.
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


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pillow&package-manager=pip&previous-version=10.2.0&new-version=10.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 16:04:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2867" class=".btn">#2867</a>
            </td>
            <td>
                <b>
                    Add missing VC-DI/LD-Proof verification method option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I replaced the custom `IssuanceOptionsSchema` schema on the vc/issue endpoint with the previous `LDProofOptionsSchema`. The idea will be to revisit the idea of having custom options field for different endpoints in a post 1.0 version. The verificationMethod option is necessary when issuing using unconventional did methods, such as did:web where the wallet can't correlate a verificationMethod with a specific did
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 22:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2866" class=".btn">#2866</a>
            </td>
            <td>
                <b>
                    Fix run_tests script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix a change that I think @dbluhm did awhile back, which is now causing issues when trying to run tests locally.

@dbluhm  what was the reason for the fix?  This PR removes your change but maybe there is an alternative that addresses your reasons without breaking local tests ...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 18:04:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2862" class=".btn">#2862</a>
            </td>
            <td>
                <b>
                    refactor: introduce use_did and use_did_method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements #2857. With one modification: rather than having a single parameter `use_did`, I found that the processing became significantly simpler by having a `use_did` and `use_did_method` parameter. Hopefully that's an acceptable trade off.

WIP: Currently, just the updates to the did exchange routes have been made. Working through the OOB route updates now. Wanted to open early for feedback.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 19:55:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    feat: Integrate AnonCreds with W3C VCDI Format Support in ACA-Py
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Summary
Pull request introduces comprehensive support for AnonCreds within the W3C VCDI formats. The changes include the addition of new models, methods, and protocols that enable the Aries Cloud Agent Python to issue, hold, and verify credentials in alignment with W3C's VCDI standards.

### Changes Overview

- AnonCreds Integration: Updated the anoncreds module to handle VCDI-compliant credential offers, requests, and credentials.
- Indy Models: Adapted indy/models to map onto VCDI credential.
- Issue Credential Protocol v2.0: Incorporated VCDI support into the existing issue_credential protocol
- VCDI Credential Format Handling: Introduced a new vc_di module within formats to handle the specificities of the VCDI credential format.
- Updated alice/faber demo: Introduced handling of multiple cred demo with cred-type argument

### Detailed Changes

- Added handler.py in protocols/issue_credential/v2_0/formats/vc_di to manage VCDI credential operations.
- Created test_handler.py in the same directory to ensure robustness and reliability through comprehensive testing.
- Introduced vc_di.py within models/detail for detailed VCDI model definitions.
- Updated test_routes.py to test the integration of VCDI routes within the agent's service layer.
- Revised routes.py to handle API endpoints related to VCDI credential operations.
- Updated faber.py
- Update alice.py
- Updated agent_container.py
- Updated performance.py


### Additional Notes
Link to the detailed documentation and specifications: [W3C VCDI Integration](https://hackmd.io/@swcurran/ryZDzTbta)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-31 14:10:33 +0000 UTC
    </div>
</div>

