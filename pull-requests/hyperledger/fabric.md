---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4473" class=".btn">#4473</a>
            </td>
            <td>
                <b>
                    remove an unused parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

This commit removes an unused parameter named "namespace" from a function that computes the expiring block number for a private key stored in a collection with a "block to live" policy.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 12:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4472" class=".btn">#4472</a>
            </td>
            <td>
                <b>
                    Add inspect option into checkcommitreadiness command to output discre…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds `inspect` option into checkcommitreadiness command to output discrepancy details.

#### Type of change

- New feature

#### Description
I have proposed an extension to lifecycle chaincode checkcommitreadiness to provide details of the discrepancies as shown in  https://github.com/hyperledger/fabric/issues/4428.

As a sub-task stemming from issue #4428, this patch adds `inspect` option into checkcommitreadiness command to output discrepancy details.

After this patch is merged, I will submit some patches for the integration tests and documentation.

#### Additional details

The example of output when executing checkcommitreadiness with inspect flag in the implementation:

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect
Chaincode definition for chaincode 'basic', version '2.0', sequence '2' on channel 'mychannel' approval status by org:
Org1MSP: false (mismatch: [EndorsementInfo, ValidationInfo, Collections])
Org2MSP: false (mismatch: [ChaincodeParameters])
```

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect --output json
{
        "approvals": {
                "Org1MSP": false,
                "Org2MSP": false
        },
        "mismatches": {
                "Org1MSP": {
                        "items": [
                                "EndorsementInfo (Check the Version, InitRequired, EndorsementPlugin)",
                                "ValidationInfo (Check the ValidationParameter, ValidationPlugin)",
                                "Collections (Check the Collections)"
                        ]
                },
                "Org2MSP": {
                        "items": [
                                "ChaincodeParameters (Check the Sequence, ChaincodeName)"
                        ]
                }
        }
}
```

#### Related issues

- https://github.com/hyperledger/fabric/issues/4428

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 00:17:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4470" class=".btn">#4470</a>
            </td>
            <td>
                <b>
                    Use the errors.Is to check error type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset uses errors.Is to check error type.

Change-Id: Ieae0eaa2527d05fa67aa31afdda42d150fff0980

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

errors.Is is recommened since Go 1.13 to check error type. The error may be wrapped.

More details: https://github.com/golang/go/wiki/ErrorValueFAQ.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 22:10:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4469" class=".btn">#4469</a>
            </td>
            <td>
                <b>
                    Fix comment prefix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The comment prefix should match method name.

Change-Id: I817951e2c94db1705293709fc49f2fc67cf71373

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Fix comment prefix that is not matched with the method name.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 21:15:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4467" class=".btn">#4467</a>
            </td>
            <td>
                <b>
                    Remove usage of fmt.Errorf
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset uses the errors pkg to follow the guideline at

https://hyperledger-fabric.readthedocs.io/en/latest/error-handling.html

Change-Id: I36eaac1b429c69195e4af1bb5bb25fc1a2578168

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Remove the usage of fmt.Errorf. Follow the official guideline to change
to the errors package.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 21:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4466" class=".btn">#4466</a>
            </td>
            <td>
                <b>
                    Update add_orderer.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Documentation update

#### Description

Update add_orderer.md to reflect the correct way to add a new orderer to an existing channel.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 13:21:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4465" class=".btn">#4465</a>
            </td>
            <td>
                <b>
                    Bft bp block verifier peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change
- New feature

#### Description

Peer using an updatable block verifier


#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 12:19:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4464" class=".btn">#4464</a>
            </td>
            <td>
                <b>
                    Bump github.com/consensys/gnark-crypto from 0.6.0 to 0.12.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/consensys/gnark-crypto](https://github.com/consensys/gnark-crypto) from 0.6.0 to 0.12.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/consensys/gnark-crypto/releases">github.com/consensys/gnark-crypto's releases</a>.</em></p>
<blockquote>
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
<li>perf: improve fft domain  memory footprint by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/437">Consensys/gnark-crypto#437</a></li>
<li>Refactor/gkr test vectors by <a href="https://github.com/Tabaie"><code>@​Tabaie</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/425">Consensys/gnark-crypto#425</a></li>
<li>v0.11.2 by <a href="https://github.com/gbotrel"><code>@​gbotrel</code></a> in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/438">Consensys/gnark-crypto#438</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/asanso"><code>@​asanso</code></a> made their first contribution in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/393">Consensys/gnark-crypto#393</a></li>
<li><a href="https://github.com/jsign"><code>@​jsign</code></a> made their first contribution in <a href="https://redirect.github.com/Consensys/gnark-crypto/pull/413">Consensys/gnark-crypto#413</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/Consensys/gnark-crypto/compare/v0.11.1...v0.11.2">https://github.com/Consensys/gnark-crypto/compare/v0.11.1...v0.11.2</a></p>
<h2>v0.11.1</h2>
<h2>Security</h2>
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
<li><a href="https://github.com/Consensys/gnark-crypto/commit/81ffe9cbd19c7fa6899c97a5ac7b3ec14b30ac06"><code>81ffe9c</code></a> Merge pull request <a href="https://redirect.github.com/consensys/gnark-crypto/issues/449">#449</a> from Consensys/fix/malleability_sig</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/4719f0a857ca4eca193e89603ab6b6061ed12bea"><code>4719f0a</code></a> chore: generate</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/015c708b012b1a2448d5dc230b5228b62369cc11"><code>015c708</code></a> test: ensure the test path is taken</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/64de55ee719de25b7f4142f25462c5c309eb308e"><code>64de55e</code></a> chore: generate</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/4c8d1aa3d05082eb407cb3b00cf6e10f6acede32"><code>4c8d1aa</code></a> refactor: make marshal errors private</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/666b963da3399074c7e9e80cfa0f37aebdb4fdbe"><code>666b963</code></a> chore: generate</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/f6e00f83e40cc0351764791bf498cdcea118c9e6"><code>f6e00f8</code></a> chore: use *big.Int (convention)</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/045e2564545cbcf6694f690cd5565985d17321f3"><code>045e256</code></a> chore: generate</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/14d20d56850054cfa9985889cb0ae5e1c3f8e59d"><code>14d20d5</code></a> fix: remove test that signature value R.X == 0</li>
<li><a href="https://github.com/Consensys/gnark-crypto/commit/44c64cd951a395c6e006b8e25596d8acce7b1bf8"><code>44c64cd</code></a> fix: check EdDSA signature values not zero</li>
<li>Additional commits viewable in <a href="https://github.com/consensys/gnark-crypto/compare/v0.6.0...v0.12.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/consensys/gnark-crypto&package-manager=go_modules&previous-version=0.6.0&new-version=0.12.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 11:38:42 +0000 UTC
    </div>
</div>

