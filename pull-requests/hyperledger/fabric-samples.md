---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1136" class=".btn">#1136</a>
            </td>
            <td>
                <b>
                    Fix equal string in bash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 11:45:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1135" class=".btn">#1135</a>
            </td>
            <td>
                <b>
                    Bump github.com/consensys/gnark-crypto from 0.9.1 to 0.12.1 in /token-sdk/owner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/consensys/gnark-crypto](https://github.com/consensys/gnark-crypto) from 0.9.1 to 0.12.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/consensys/gnark-crypto/releases">github.com/consensys/gnark-crypto's releases</a>.</em></p>
<blockquote>
<h2>v0.12.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: GLV exponentiation in GT with large exponents by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/451">Consensys/gnark-crypto#451</a> <a href="https://github.com/Consensys/gnark-crypto/security/advisories/GHSA-pffg-92cg-xf5c">Security Advisory</a></li>
<li>feat: kzg extended transcript by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/452">Consensys/gnark-crypto#452</a></li>
<li>perf(fft): introduce cache efficient bit reverse shuffling by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/446">Consensys/gnark-crypto#446</a></li>
<li>perf: Improve performance of point equality checks by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/450">Consensys/gnark-crypto#450</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/Consensys/gnark-crypto/compare/v0.12.0...v0.12.1">https://github.com/Consensys/gnark-crypto/compare/v0.12.0...v0.12.1</a></p>
<h2>v0.12.0</h2>
<h2>What's Changed</h2>
<ul>
<li>
<p>fix malleability sig by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/449">Consensys/gnark-crypto#449</a> <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-44273">https://nvd.nist.gov/vuln/detail/CVE-2023-44273</a></p>
</li>
<li>
<p>perf: multiexp, avoid direct coordinate access to check for zero points by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/414">Consensys/gnark-crypto#414</a></p>
</li>
<li>
<p>perf: edwards, improve the performance of Add, MixedAdd and IsOnCurve by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/441">Consensys/gnark-crypto#441</a></p>
</li>
<li>
<p>perf: edwards, avoid inversions in Add in extended points by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/442">Consensys/gnark-crypto#442</a></p>
</li>
<li>
<p>ci: update ci workflows by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/447">Consensys/gnark-crypto#447</a></p>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/Consensys/gnark-crypto/compare/v0.11.2...v0.12.0">https://github.com/Consensys/gnark-crypto/compare/v0.11.2...v0.12.0</a></p>
<h2>v0.11.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix some typos by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/394">Consensys/gnark-crypto#394</a></li>
<li>Adding testing for deserialization of G1 and G2 points by <a href="https://github.com/asanso"><code>@​asanso</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/393">Consensys/gnark-crypto#393</a></li>
<li>Fix some implicit memory aliasing in for loops by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/395">Consensys/gnark-crypto#395</a></li>
<li>Do not XOR with zero by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/398">Consensys/gnark-crypto#398</a></li>
<li>Disable check shadowing in govet linter by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/397">Consensys/gnark-crypto#397</a></li>
<li>Add a bunch of &quot;nosec G404&quot; comments in test code by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/399">Consensys/gnark-crypto#399</a></li>
<li>Enable misspell linter &amp; fix findings by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/401">Consensys/gnark-crypto#401</a></li>
<li>Fix <code>RSis.CopyWithFreshBuffer</code> by <a href="https://github.com/AlexandreBelling"><code>@​AlexandreBelling</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/402">Consensys/gnark-crypto#402</a></li>
<li>feat: Marshal [][]fr.Element by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/400">Consensys/gnark-crypto#400</a></li>
<li>Run golangci-lint on generated files by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/396">Consensys/gnark-crypto#396</a></li>
<li>docs: ConsenSys -&gt; Consensys by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/406">Consensys/gnark-crypto#406</a></li>
<li>msm: semaphore to limit CPUs + better split strategy (up to 25% perf boost on 96cores) by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/403">Consensys/gnark-crypto#403</a></li>
<li>Feat/fold pedersen by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/407">Consensys/gnark-crypto#407</a></li>
<li>fix: do not read empty slices as nil by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/410">Consensys/gnark-crypto#410</a></li>
<li>fix: incorrect semaphore init could cause msm deadlock by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/411">Consensys/gnark-crypto#411</a></li>
<li>edwards: optimize point negation by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/413">Consensys/gnark-crypto#413</a></li>
<li>Feat/gkr custom gates by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/419">Consensys/gnark-crypto#419</a></li>
<li>perf: fast path for SIS with logTwoBound: 8, logTwoDegree: 6 by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/416">Consensys/gnark-crypto#416</a></li>
<li>feat: add WriteRawTo, UnsafeReadFrom to kzg.ProvingKey by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/422">Consensys/gnark-crypto#422</a></li>
<li>Fix/gkr eq bug by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/421">Consensys/gnark-crypto#421</a></li>
<li>feat: add AsyncReadFrom to fr.Vector and fft.Domain by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/424">Consensys/gnark-crypto#424</a></li>
<li>fix: ECDSA HashToInt bytes-bits mismatch by <a href="https://github.com/ivokub"><code>@​ivokub</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/428">Consensys/gnark-crypto#428</a></li>
<li>Small optimization over the memory usage of MiMC by <a href="https://github.com/AlexandreBelling"><code>@​AlexandreBelling</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/435">Consensys/gnark-crypto#435</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/Consensys/gnark-crypto/blob/master/CHANGELOG.md">github.com/consensys/gnark-crypto's changelog</a>.</em></p>
<blockquote>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2>[v0.11.1] - 2023-07-11</h2>
<h3>Fix</h3>
<ul>
<li>ECDSA HashToInt bytes-bits mismatch (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/428">#428</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2>[v0.11.0] - 2023-05-02</h2>
<h3>Build</h3>
<ul>
<li>go generate</li>
<li>generify bn254 changes</li>
<li>generify bn254 kzg changes</li>
<li>generify marshal changes</li>
<li>generify bn254 kzg changes</li>
<li>bump go1.20</li>
<li>update ci github action dependencies</li>
</ul>
<h3>Chore</h3>
<ul>
<li>PR feedback</li>
</ul>
<h3>Docs</h3>
<ul>
<li>make comments more godoc friendly</li>
<li>remove comment</li>
<li>remove DO NOT EDIT from non-autogenerated files</li>
</ul>
<h3>Feat</h3>
<ul>
<li>fix v computation in ECDSA signature (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/385">#385</a>)</li>
<li>make <code>mapToCurve</code> public to allow for custom cofactor clearing (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/372">#372</a>)</li>
<li>add Double in affine coordinates</li>
<li>kzg.Vk.WriteRawTo</li>
<li>bn254 encoder to support uint64 slices</li>
<li><strong>pairing:</strong> return 1 after easy part if result is 1</li>
</ul>
<h3>Fix</h3>
<ul>
<li>handle all bitmask in point deserialization</li>
<li>littleEndian -&gt; bigEndian</li>
<li>import utils</li>
<li>don't ignore multiexp error</li>
<li>minor errors</li>
<li>generation mistake</li>
<li>bn254 incorporate evals into kzg batch challenge</li>
<li><strong>kzg:</strong> nb of digests in BatchVerifyMultiPoints should be nonzeo</li>
<li><strong>linter:</strong> ineffassign in Fpk marshal</li>
</ul>
<h3>Perf</h3>
<ul>
<li><strong>kzg:</strong> remove G2 scalar mul in single verification</li>
</ul>
<h3>Refactor</h3>
<ul>
<li>break pedersen key into proving (committing) and verifying</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/da0317fd013308db6ce847bc9c3d506a2a3ae0ff"><code>da0317f</code></a> clean: remove useless snippet in mulWindowed (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/453">#453</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/65cdb1d1c214e51454ae6dad4c466324f3ae510d"><code>65cdb1d</code></a> Feat/kzg extended transcript (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/452">#452</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/95e674b3d69279dd0446e34cd8960e2fc4ed8393"><code>95e674b</code></a> perf(fft): introduce cache efficient bit reverse shuffling (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/446">#446</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ec6be1a037f7c496d595c541a8a8d31c47bcfa3d"><code>ec6be1a</code></a> Merge pull request <a href="https://redirect.github.com/consensys/gnark-crypto/issues/451">#451</a> from Consensys/fix/glv</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/aef1eef48ab992db67631dcbec1c8dc259673e5b"><code>aef1eef</code></a> fix: add GT ExpGLV fix to BLS24 + BW6</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/feaf161b4d1e53abf68b5679780ab497ef4818d4"><code>feaf161</code></a> fix: merge and fix tests for expGLV</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ced3076befee5c056f80ec5301438001ef5e9cdd"><code>ced3076</code></a> fix: use max(size(s1), size(s2)) for ExpGLV</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/4096ad9913f1bfc9c67cdddade36ba981ade72ac"><code>4096ad9</code></a> feat: discared useless files</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ace5318b726c7185249bc9c92e1cadae701c1654"><code>ace5318</code></a> Merge pull request <a href="https://redirect.github.com/consensys/gnark-crypto/issues/450">#450</a> from jsign/jsign-eq-improv</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/dc4e2d4f7799c4c36e213d1278fd3b77c07eb4da"><code>dc4e2d4</code></a> feat: added test for [-s]G=-[s]G</li>
<li>Additional commits viewable in <a href="https://github.com/consensys/gnark-crypto/compare/v0.9.1...v0.12.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/consensys/gnark-crypto&package-manager=go_modules&previous-version=0.9.1&new-version=0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 18:49:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    Bump github.com/consensys/gnark-crypto from 0.9.1 to 0.12.1 in /token-sdk/auditor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/consensys/gnark-crypto](https://github.com/consensys/gnark-crypto) from 0.9.1 to 0.12.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/consensys/gnark-crypto/releases">github.com/consensys/gnark-crypto's releases</a>.</em></p>
<blockquote>
<h2>v0.12.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: GLV exponentiation in GT with large exponents by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/451">Consensys/gnark-crypto#451</a> <a href="https://github.com/Consensys/gnark-crypto/security/advisories/GHSA-pffg-92cg-xf5c">Security Advisory</a></li>
<li>feat: kzg extended transcript by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/452">Consensys/gnark-crypto#452</a></li>
<li>perf(fft): introduce cache efficient bit reverse shuffling by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/446">Consensys/gnark-crypto#446</a></li>
<li>perf: Improve performance of point equality checks by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/450">Consensys/gnark-crypto#450</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/Consensys/gnark-crypto/compare/v0.12.0...v0.12.1">https://github.com/Consensys/gnark-crypto/compare/v0.12.0...v0.12.1</a></p>
<h2>v0.12.0</h2>
<h2>What's Changed</h2>
<ul>
<li>
<p>fix malleability sig by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/449">Consensys/gnark-crypto#449</a> <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-44273">https://nvd.nist.gov/vuln/detail/CVE-2023-44273</a></p>
</li>
<li>
<p>perf: multiexp, avoid direct coordinate access to check for zero points by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/414">Consensys/gnark-crypto#414</a></p>
</li>
<li>
<p>perf: edwards, improve the performance of Add, MixedAdd and IsOnCurve by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/441">Consensys/gnark-crypto#441</a></p>
</li>
<li>
<p>perf: edwards, avoid inversions in Add in extended points by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/442">Consensys/gnark-crypto#442</a></p>
</li>
<li>
<p>ci: update ci workflows by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/447">Consensys/gnark-crypto#447</a></p>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/Consensys/gnark-crypto/compare/v0.11.2...v0.12.0">https://github.com/Consensys/gnark-crypto/compare/v0.11.2...v0.12.0</a></p>
<h2>v0.11.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix some typos by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/394">Consensys/gnark-crypto#394</a></li>
<li>Adding testing for deserialization of G1 and G2 points by <a href="https://github.com/asanso"><code>@​asanso</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/393">Consensys/gnark-crypto#393</a></li>
<li>Fix some implicit memory aliasing in for loops by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/395">Consensys/gnark-crypto#395</a></li>
<li>Do not XOR with zero by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/398">Consensys/gnark-crypto#398</a></li>
<li>Disable check shadowing in govet linter by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/397">Consensys/gnark-crypto#397</a></li>
<li>Add a bunch of &quot;nosec G404&quot; comments in test code by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/399">Consensys/gnark-crypto#399</a></li>
<li>Enable misspell linter &amp; fix findings by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/401">Consensys/gnark-crypto#401</a></li>
<li>Fix <code>RSis.CopyWithFreshBuffer</code> by <a href="https://github.com/AlexandreBelling"><code>@​AlexandreBelling</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/402">Consensys/gnark-crypto#402</a></li>
<li>feat: Marshal [][]fr.Element by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/400">Consensys/gnark-crypto#400</a></li>
<li>Run golangci-lint on generated files by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/396">Consensys/gnark-crypto#396</a></li>
<li>docs: ConsenSys -&gt; Consensys by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/406">Consensys/gnark-crypto#406</a></li>
<li>msm: semaphore to limit CPUs + better split strategy (up to 25% perf boost on 96cores) by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/403">Consensys/gnark-crypto#403</a></li>
<li>Feat/fold pedersen by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/407">Consensys/gnark-crypto#407</a></li>
<li>fix: do not read empty slices as nil by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/410">Consensys/gnark-crypto#410</a></li>
<li>fix: incorrect semaphore init could cause msm deadlock by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/411">Consensys/gnark-crypto#411</a></li>
<li>edwards: optimize point negation by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/413">Consensys/gnark-crypto#413</a></li>
<li>Feat/gkr custom gates by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/419">Consensys/gnark-crypto#419</a></li>
<li>perf: fast path for SIS with logTwoBound: 8, logTwoDegree: 6 by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/416">Consensys/gnark-crypto#416</a></li>
<li>feat: add WriteRawTo, UnsafeReadFrom to kzg.ProvingKey by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/422">Consensys/gnark-crypto#422</a></li>
<li>Fix/gkr eq bug by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/421">Consensys/gnark-crypto#421</a></li>
<li>feat: add AsyncReadFrom to fr.Vector and fft.Domain by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/424">Consensys/gnark-crypto#424</a></li>
<li>fix: ECDSA HashToInt bytes-bits mismatch by <a href="https://github.com/ivokub"><code>@​ivokub</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/428">Consensys/gnark-crypto#428</a></li>
<li>Small optimization over the memory usage of MiMC by <a href="https://github.com/AlexandreBelling"><code>@​AlexandreBelling</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/435">Consensys/gnark-crypto#435</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/Consensys/gnark-crypto/blob/master/CHANGELOG.md">github.com/consensys/gnark-crypto's changelog</a>.</em></p>
<blockquote>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2>[v0.11.1] - 2023-07-11</h2>
<h3>Fix</h3>
<ul>
<li>ECDSA HashToInt bytes-bits mismatch (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/428">#428</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2>[v0.11.0] - 2023-05-02</h2>
<h3>Build</h3>
<ul>
<li>go generate</li>
<li>generify bn254 changes</li>
<li>generify bn254 kzg changes</li>
<li>generify marshal changes</li>
<li>generify bn254 kzg changes</li>
<li>bump go1.20</li>
<li>update ci github action dependencies</li>
</ul>
<h3>Chore</h3>
<ul>
<li>PR feedback</li>
</ul>
<h3>Docs</h3>
<ul>
<li>make comments more godoc friendly</li>
<li>remove comment</li>
<li>remove DO NOT EDIT from non-autogenerated files</li>
</ul>
<h3>Feat</h3>
<ul>
<li>fix v computation in ECDSA signature (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/385">#385</a>)</li>
<li>make <code>mapToCurve</code> public to allow for custom cofactor clearing (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/372">#372</a>)</li>
<li>add Double in affine coordinates</li>
<li>kzg.Vk.WriteRawTo</li>
<li>bn254 encoder to support uint64 slices</li>
<li><strong>pairing:</strong> return 1 after easy part if result is 1</li>
</ul>
<h3>Fix</h3>
<ul>
<li>handle all bitmask in point deserialization</li>
<li>littleEndian -&gt; bigEndian</li>
<li>import utils</li>
<li>don't ignore multiexp error</li>
<li>minor errors</li>
<li>generation mistake</li>
<li>bn254 incorporate evals into kzg batch challenge</li>
<li><strong>kzg:</strong> nb of digests in BatchVerifyMultiPoints should be nonzeo</li>
<li><strong>linter:</strong> ineffassign in Fpk marshal</li>
</ul>
<h3>Perf</h3>
<ul>
<li><strong>kzg:</strong> remove G2 scalar mul in single verification</li>
</ul>
<h3>Refactor</h3>
<ul>
<li>break pedersen key into proving (committing) and verifying</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/da0317fd013308db6ce847bc9c3d506a2a3ae0ff"><code>da0317f</code></a> clean: remove useless snippet in mulWindowed (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/453">#453</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/65cdb1d1c214e51454ae6dad4c466324f3ae510d"><code>65cdb1d</code></a> Feat/kzg extended transcript (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/452">#452</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/95e674b3d69279dd0446e34cd8960e2fc4ed8393"><code>95e674b</code></a> perf(fft): introduce cache efficient bit reverse shuffling (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/446">#446</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ec6be1a037f7c496d595c541a8a8d31c47bcfa3d"><code>ec6be1a</code></a> Merge pull request <a href="https://redirect.github.com/consensys/gnark-crypto/issues/451">#451</a> from Consensys/fix/glv</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/aef1eef48ab992db67631dcbec1c8dc259673e5b"><code>aef1eef</code></a> fix: add GT ExpGLV fix to BLS24 + BW6</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/feaf161b4d1e53abf68b5679780ab497ef4818d4"><code>feaf161</code></a> fix: merge and fix tests for expGLV</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ced3076befee5c056f80ec5301438001ef5e9cdd"><code>ced3076</code></a> fix: use max(size(s1), size(s2)) for ExpGLV</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/4096ad9913f1bfc9c67cdddade36ba981ade72ac"><code>4096ad9</code></a> feat: discared useless files</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ace5318b726c7185249bc9c92e1cadae701c1654"><code>ace5318</code></a> Merge pull request <a href="https://redirect.github.com/consensys/gnark-crypto/issues/450">#450</a> from jsign/jsign-eq-improv</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/dc4e2d4f7799c4c36e213d1278fd3b77c07eb4da"><code>dc4e2d4</code></a> feat: added test for [-s]G=-[s]G</li>
<li>Additional commits viewable in <a href="https://github.com/consensys/gnark-crypto/compare/v0.9.1...v0.12.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/consensys/gnark-crypto&package-manager=go_modules&previous-version=0.9.1&new-version=0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 18:38:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    Bump github.com/consensys/gnark-crypto from 0.9.1 to 0.12.1 in /token-sdk/issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/consensys/gnark-crypto](https://github.com/consensys/gnark-crypto) from 0.9.1 to 0.12.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/consensys/gnark-crypto/releases">github.com/consensys/gnark-crypto's releases</a>.</em></p>
<blockquote>
<h2>v0.12.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: GLV exponentiation in GT with large exponents by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/451">Consensys/gnark-crypto#451</a> <a href="https://github.com/Consensys/gnark-crypto/security/advisories/GHSA-pffg-92cg-xf5c">Security Advisory</a></li>
<li>feat: kzg extended transcript by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/452">Consensys/gnark-crypto#452</a></li>
<li>perf(fft): introduce cache efficient bit reverse shuffling by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/446">Consensys/gnark-crypto#446</a></li>
<li>perf: Improve performance of point equality checks by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/450">Consensys/gnark-crypto#450</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/Consensys/gnark-crypto/compare/v0.12.0...v0.12.1">https://github.com/Consensys/gnark-crypto/compare/v0.12.0...v0.12.1</a></p>
<h2>v0.12.0</h2>
<h2>What's Changed</h2>
<ul>
<li>
<p>fix malleability sig by <a href="https://github.com/ThomasPiellard"><code>@​ThomasPiellard</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/449">Consensys/gnark-crypto#449</a> <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-44273">https://nvd.nist.gov/vuln/detail/CVE-2023-44273</a></p>
</li>
<li>
<p>perf: multiexp, avoid direct coordinate access to check for zero points by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/414">Consensys/gnark-crypto#414</a></p>
</li>
<li>
<p>perf: edwards, improve the performance of Add, MixedAdd and IsOnCurve by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/441">Consensys/gnark-crypto#441</a></p>
</li>
<li>
<p>perf: edwards, avoid inversions in Add in extended points by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/442">Consensys/gnark-crypto#442</a></p>
</li>
<li>
<p>ci: update ci workflows by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/447">Consensys/gnark-crypto#447</a></p>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/Consensys/gnark-crypto/compare/v0.11.2...v0.12.0">https://github.com/Consensys/gnark-crypto/compare/v0.11.2...v0.12.0</a></p>
<h2>v0.11.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix some typos by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/394">Consensys/gnark-crypto#394</a></li>
<li>Adding testing for deserialization of G1 and G2 points by <a href="https://github.com/asanso"><code>@​asanso</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/393">Consensys/gnark-crypto#393</a></li>
<li>Fix some implicit memory aliasing in for loops by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/395">Consensys/gnark-crypto#395</a></li>
<li>Do not XOR with zero by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/398">Consensys/gnark-crypto#398</a></li>
<li>Disable check shadowing in govet linter by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/397">Consensys/gnark-crypto#397</a></li>
<li>Add a bunch of &quot;nosec G404&quot; comments in test code by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/399">Consensys/gnark-crypto#399</a></li>
<li>Enable misspell linter &amp; fix findings by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/401">Consensys/gnark-crypto#401</a></li>
<li>Fix <code>RSis.CopyWithFreshBuffer</code> by <a href="https://github.com/AlexandreBelling"><code>@​AlexandreBelling</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/402">Consensys/gnark-crypto#402</a></li>
<li>feat: Marshal [][]fr.Element by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/400">Consensys/gnark-crypto#400</a></li>
<li>Run golangci-lint on generated files by <a href="https://github.com/jtraglia"><code>@​jtraglia</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/396">Consensys/gnark-crypto#396</a></li>
<li>docs: ConsenSys -&gt; Consensys by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/406">Consensys/gnark-crypto#406</a></li>
<li>msm: semaphore to limit CPUs + better split strategy (up to 25% perf boost on 96cores) by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/403">Consensys/gnark-crypto#403</a></li>
<li>Feat/fold pedersen by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/407">Consensys/gnark-crypto#407</a></li>
<li>fix: do not read empty slices as nil by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/410">Consensys/gnark-crypto#410</a></li>
<li>fix: incorrect semaphore init could cause msm deadlock by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/411">Consensys/gnark-crypto#411</a></li>
<li>edwards: optimize point negation by <a href="https://github.com/jsign"><code>@​jsign</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/413">Consensys/gnark-crypto#413</a></li>
<li>Feat/gkr custom gates by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/419">Consensys/gnark-crypto#419</a></li>
<li>perf: fast path for SIS with logTwoBound: 8, logTwoDegree: 6 by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/416">Consensys/gnark-crypto#416</a></li>
<li>feat: add WriteRawTo, UnsafeReadFrom to kzg.ProvingKey by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/422">Consensys/gnark-crypto#422</a></li>
<li>Fix/gkr eq bug by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/421">Consensys/gnark-crypto#421</a></li>
<li>feat: add AsyncReadFrom to fr.Vector and fft.Domain by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/424">Consensys/gnark-crypto#424</a></li>
<li>fix: ECDSA HashToInt bytes-bits mismatch by <a href="https://github.com/ivokub"><code>@​ivokub</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/428">Consensys/gnark-crypto#428</a></li>
<li>Small optimization over the memory usage of MiMC by <a href="https://github.com/AlexandreBelling"><code>@​AlexandreBelling</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/435">Consensys/gnark-crypto#435</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/Consensys/gnark-crypto/blob/master/CHANGELOG.md">github.com/consensys/gnark-crypto's changelog</a>.</em></p>
<blockquote>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2>[v0.11.1] - 2023-07-11</h2>
<h3>Fix</h3>
<ul>
<li>ECDSA HashToInt bytes-bits mismatch (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/428">#428</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2>[v0.11.0] - 2023-05-02</h2>
<h3>Build</h3>
<ul>
<li>go generate</li>
<li>generify bn254 changes</li>
<li>generify bn254 kzg changes</li>
<li>generify marshal changes</li>
<li>generify bn254 kzg changes</li>
<li>bump go1.20</li>
<li>update ci github action dependencies</li>
</ul>
<h3>Chore</h3>
<ul>
<li>PR feedback</li>
</ul>
<h3>Docs</h3>
<ul>
<li>make comments more godoc friendly</li>
<li>remove comment</li>
<li>remove DO NOT EDIT from non-autogenerated files</li>
</ul>
<h3>Feat</h3>
<ul>
<li>fix v computation in ECDSA signature (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/385">#385</a>)</li>
<li>make <code>mapToCurve</code> public to allow for custom cofactor clearing (<a href="https://redirect.github.com/ConsenSys/gnark-crypto/issues/372">#372</a>)</li>
<li>add Double in affine coordinates</li>
<li>kzg.Vk.WriteRawTo</li>
<li>bn254 encoder to support uint64 slices</li>
<li><strong>pairing:</strong> return 1 after easy part if result is 1</li>
</ul>
<h3>Fix</h3>
<ul>
<li>handle all bitmask in point deserialization</li>
<li>littleEndian -&gt; bigEndian</li>
<li>import utils</li>
<li>don't ignore multiexp error</li>
<li>minor errors</li>
<li>generation mistake</li>
<li>bn254 incorporate evals into kzg batch challenge</li>
<li><strong>kzg:</strong> nb of digests in BatchVerifyMultiPoints should be nonzeo</li>
<li><strong>linter:</strong> ineffassign in Fpk marshal</li>
</ul>
<h3>Perf</h3>
<ul>
<li><strong>kzg:</strong> remove G2 scalar mul in single verification</li>
</ul>
<h3>Refactor</h3>
<ul>
<li>break pedersen key into proving (committing) and verifying</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/da0317fd013308db6ce847bc9c3d506a2a3ae0ff"><code>da0317f</code></a> clean: remove useless snippet in mulWindowed (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/453">#453</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/65cdb1d1c214e51454ae6dad4c466324f3ae510d"><code>65cdb1d</code></a> Feat/kzg extended transcript (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/452">#452</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/95e674b3d69279dd0446e34cd8960e2fc4ed8393"><code>95e674b</code></a> perf(fft): introduce cache efficient bit reverse shuffling (<a href="https://redirect.github.com/consensys/gnark-crypto/issues/446">#446</a>)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ec6be1a037f7c496d595c541a8a8d31c47bcfa3d"><code>ec6be1a</code></a> Merge pull request <a href="https://redirect.github.com/consensys/gnark-crypto/issues/451">#451</a> from Consensys/fix/glv</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/aef1eef48ab992db67631dcbec1c8dc259673e5b"><code>aef1eef</code></a> fix: add GT ExpGLV fix to BLS24 + BW6</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/feaf161b4d1e53abf68b5679780ab497ef4818d4"><code>feaf161</code></a> fix: merge and fix tests for expGLV</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ced3076befee5c056f80ec5301438001ef5e9cdd"><code>ced3076</code></a> fix: use max(size(s1), size(s2)) for ExpGLV</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/4096ad9913f1bfc9c67cdddade36ba981ade72ac"><code>4096ad9</code></a> feat: discared useless files</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/ace5318b726c7185249bc9c92e1cadae701c1654"><code>ace5318</code></a> Merge pull request <a href="https://redirect.github.com/consensys/gnark-crypto/issues/450">#450</a> from jsign/jsign-eq-improv</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/dc4e2d4f7799c4c36e213d1278fd3b77c07eb4da"><code>dc4e2d4</code></a> feat: added test for [-s]G=-[s]G</li>
<li>Additional commits viewable in <a href="https://github.com/consensys/gnark-crypto/compare/v0.9.1...v0.12.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/consensys/gnark-crypto&package-manager=go_modules&previous-version=0.9.1&new-version=0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 18:38:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    Fix test-network chaincode-as-a-service deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves a regression introduced in e73bb717db47185a8ccd1b701503b369cd2a73e1.

Previous change defaulted to "auto" as the sequence number but omitted the call to generate the correct sequence number for the "auto" value. This resulted in "auto" being used as the sequence number, which is an error since an integer is required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 13:14:26 +0000 UTC
    </div>
</div>

