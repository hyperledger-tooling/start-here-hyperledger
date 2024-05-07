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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2933" class=".btn">#2933</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump ecdsa from 0.16.1 to 0.19.0 in the pip group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update in the / directory: [ecdsa](https://github.com/tlsfuzzer/python-ecdsa).

Updates `ecdsa` from 0.16.1 to 0.19.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tlsfuzzer/python-ecdsa/releases">ecdsa's releases</a>.</em></p>
<blockquote>
<h2>ecdsa 0.19.0</h2>
<h2>New API:</h2>
<ul>
<li><code>to_ssh</code> in <code>VerifyingKey</code> and <code>SigningKey</code>, supports Ed25519 keys only
(Pablo Mazzini)</li>
</ul>
<h2>New features:</h2>
<ul>
<li>Support for twisted Brainpool curves</li>
</ul>
<h2>Doc fix:</h2>
<ul>
<li>Fix curve equation in glossary</li>
<li>Documentation for signature encoding and signature decoding functions</li>
</ul>
<h2>Maintenance:</h2>
<ul>
<li>Dropped official support for 3.3 and 3.4 (because of problems running them
in CI, not because it's actually incompatible; support for 2.6 and 2.7 is
unaffected)</li>
<li>Fixes around hypothesis parameters</li>
<li>Officially support Python 3.11 and 3.12</li>
<li>Small updates to test suite to make it work with 3.11 and 3.12 and new
releases of test dependencies</li>
<li>Dropped the internal <code>_rwlock</code> module as it's unused</li>
<li>Added mutation testing to CI, lots of speed-ups to the test suite
to make it happen</li>
<li>Removal of unnecessary <code>six.b</code> literals (Alexandre Detiste)</li>
</ul>
<p>Deprecations:</p>
<ul>
<li><code>int_to_string</code>, <code>string_to_int</code>, and <code>digest_integer</code> from <code>ecdsa.ecdsa</code>
module are now considered deprecated, they will be removed in a future
release</li>
</ul>
<h2>ecdsa 0.18.0</h2>
<h1>New features:</h1>
<ul>
<li>Support for EdDSA (Ed25519, Ed448) signature creation and verification.</li>
<li>Support for Ed25519 and Ed448 in PKCS#8 and public key files.</li>
<li>Support for point precomputation for EdDSA.</li>
</ul>
<h1>New API:</h1>
<ul>
<li>CurveEdTw class to represent the Twisted Edwards curve parameters.</li>
<li>PointEdwards class to represent points on Twisted Edwards curve and
provide point arithmetic on it.</li>
<li><code>curve_by_name</code> in <code>curves</code> module to get a <code>Curve</code> object by providing curve
name.</li>
</ul>
<p>Bug fix:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tlsfuzzer/python-ecdsa/blob/master/NEWS">ecdsa's changelog</a>.</em></p>
<blockquote>
<ul>
<li>Release 0.19.0 (08 Apr 2024)</li>
</ul>
<p>New API:</p>
<ul>
<li><code>to_ssh</code> in <code>VerifyingKey</code> and <code>SigningKey</code>, supports Ed25519 keys only
(Pablo Mazzini)</li>
</ul>
<p>New features:</p>
<ul>
<li>Support for twisted Brainpool curves</li>
</ul>
<p>Doc fix:</p>
<ul>
<li>Fix curve equation in glossary</li>
<li>Documentation for signature encoding and signature decoding functions</li>
</ul>
<p>Maintenance:</p>
<ul>
<li>Dropped official support for 3.3 and 3.4 (because of problems running them
in CI, not because it's actually incompatible; support for 2.6 and 2.7 is
unaffected)</li>
<li>Fixes aroung hypothesis parameters</li>
<li>Officially support Python 3.11 and 3.12</li>
<li>Small updates to test suite to make it work with 3.11 and 3.12 and new
releases of test dependencies</li>
<li>Dropped the internal <code>_rwlock</code> module as it's unused</li>
<li>Added mutation testing to CI, lots of speed-ups to the test suite
to make it happen</li>
<li>Removal of unnecessary <code>six.b</code> literals (Alexandre Detiste)</li>
</ul>
<p>Deprecations:</p>
<ul>
<li>
<p><code>int_to_string</code>, <code>string_to_int</code>, and <code>digest_integer</code> from <code>ecdsa.ecdsa</code>
module are now considered deprecated, they will be removed in a future
release</p>
</li>
<li>
<p>Release 0.18.0 (09 Jul 2022)</p>
</li>
</ul>
<p>New API:</p>
<ul>
<li><code>curve_by_name</code> in <code>curves</code> module to get a <code>Curve</code> object by providing curve
name.</li>
</ul>
<p>Bug fix:</p>
<ul>
<li>Make the <code>VerifyingKey</code> encoded with explicit parameters use the same
kind of point encoding for public key and curve generator.</li>
<li>Better handling of malformed curve parameters (as in CVE-2022-0778);
make python-ecdsa raise <code>MalformedPointError</code> instead of <code>AssertionError</code>.</li>
</ul>
<p>Doc fix:</p>
<ul>
<li>Publish the documentation on <a href="https://ecdsa.readthedocs.io/">https://ecdsa.readthedocs.io/</a>,
include explanation of basics of handling of ECC data formats and how to use
the library for elliptic curve arithmetic.</li>
<li>Make object names more consistent, make them into hyperlinks on the
readthedocs documentation.</li>
<li>Make security note more explicit (Ian Rodney)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/be70016f8911f79e891a65dcfcb602e5ba866ed3"><code>be70016</code></a> Merge pull request <a href="https://redirect.github.com/tlsfuzzer/python-ecdsa/issues/337">#337</a> from tlsfuzzer/release-0.19</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/217735bb28dd30c12619564da8b0ec7022ec0a95"><code>217735b</code></a> allow early exit from worker processes when running mutation testing</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/6e7adff153ad877747f56771c842a94bca65ede9"><code>6e7adff</code></a> don't check rate if no tests executed</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/c56030efe0044c6deb8a5f815eabb590e574fc41"><code>c56030e</code></a> make coveralls submission work with py2.6 again</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/66d0d74a331af339715e1e70274a45f775817f7f"><code>66d0d74</code></a> add release notes for 0.19.0 release</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/0d5a38ca8ada5f2fec67904236f563f562b402d4"><code>0d5a38c</code></a> Merge pull request <a href="https://redirect.github.com/tlsfuzzer/python-ecdsa/issues/156">#156</a> from tomato42/cosmic-ray</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/02c83503ffcd06a0ac15535a3afac88ad5725710"><code>02c8350</code></a> be more permissive for the PR mutation test coverage</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/4845e8fa64c1b1463e400ac1a0d5c4e87615bcde"><code>4845e8f</code></a> better is_prime()</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/09f0d106d13d05089078c95a947ad4f3a2602a5f"><code>09f0d10</code></a> add hard timeout for test mutation test suite</li>
<li><a href="https://github.com/tlsfuzzer/python-ecdsa/commit/e16173b25dfc9ea4b1cc323874369c1d38fb3664"><code>e16173b</code></a> two digit precision for the mutation score badge</li>
<li>Additional commits viewable in <a href="https://github.com/tlsfuzzer/python-ecdsa/compare/python-ecdsa-0.16.1...python-ecdsa-0.19.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ecdsa&package-manager=pip&previous-version=0.16.1&new-version=0.19.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 20:43:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2927" class=".btn">#2927</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed all relative paths to absolute paths for PyPI project description compatibility
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 19:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2926" class=".btn">#2926</a>
            </td>
            <td>
                <b>
                    0.12.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 17:01:58 +0000 UTC
    </div>
</div>

