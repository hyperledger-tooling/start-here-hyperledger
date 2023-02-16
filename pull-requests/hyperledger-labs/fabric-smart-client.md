---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.5.16 to 1.5.18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.5.16 to 1.5.18.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/releases">github.com/containerd/containerd's releases</a>.</em></p>
<blockquote>
<h2>containerd 1.5.18</h2>
<p>Welcome to the v1.5.18 release of containerd!</p>
<p>The eighteenth patch release for containerd 1.5 includes fixes for CVE-2023-25153 and CVE-2023-25173
along with a security update for Go.</p>
<h3>Notable Updates</h3>
<ul>
<li><strong>Fix supplementary groups not being set up properly</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-hmfx-3pcx-653p">GHSA-hmfx-3pcx-653p</a>)</li>
<li><strong>Fix OCI image importer memory exhaustion</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-259w-8hf6-59c2">GHSA-259w-8hf6-59c2</a>)</li>
<li><strong>Update Go to 1.19.6</strong> (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8112">#8112</a>)</li>
</ul>
<p>See the changelog for complete list of changes</p>
<p>Please try out the release binaries and report any issues at
<a href="https://github.com/containerd/containerd/issues">https://github.com/containerd/containerd/issues</a>.</p>
<h3>Contributors</h3>
<ul>
<li>Akihiro Suda</li>
<li>Derek McGowan</li>
<li>Ye Sijun</li>
<li>Samuel Karp</li>
<li>Phil Estes</li>
<li>Swagat Bora</li>
<li>Wei Fu</li>
</ul>
<h3>Changes</h3>
<!-- raw HTML omitted -->
<ul>
<li>[release/1.5] Prepare release notes for v1.5.18 (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8117">#8117</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/ddf9de6cbb30f9edf1b04d304eac67d1383e406b"><code>ddf9de6cb</code></a> Prepare release notes for v1.5.18</li>
</ul>
</li>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-hmfx-3pcx-653p">GHSA-hmfx-3pcx-653p</a>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/a62c38bf2173faa813018939710fc8491e4f7dba"><code>a62c38bf2</code></a> oci: fix additional GIDs</li>
<li><a href="https://github.com/containerd/containerd/commit/3b89da580b76471d6c03cb1fc6c14db6aa23d3db"><code>3b89da580</code></a> oci: fix loop iterator aliasing</li>
<li><a href="https://github.com/containerd/containerd/commit/b07ec6b251bd51f06bc72ef408f31e3f6e6e87f9"><code>b07ec6b25</code></a> oci: skip checking gid for WithAppendAdditionalGroups</li>
<li><a href="https://github.com/containerd/containerd/commit/356672cb56fd5a0eed11e5089ac824c7ab09ffac"><code>356672cb5</code></a> refactor: reduce duplicate code</li>
<li><a href="https://github.com/containerd/containerd/commit/6a7b7617cfbd90009a2e05e0e5eff4ef92028d7b"><code>6a7b7617c</code></a> add WithAdditionalGIDs test</li>
<li><a href="https://github.com/containerd/containerd/commit/832bcf300b1ec29c9b08326aab2d4eafee58dd85"><code>832bcf300</code></a> add WithAppendAdditionalGroups helper</li>
</ul>
</li>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-259w-8hf6-59c2">GHSA-259w-8hf6-59c2</a>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/19a347e456f3ab66909edca5351aa6f4ed1be177"><code>19a347e45</code></a> importer: stream oci-layout and manifest.json</li>
</ul>
</li>
<li>[release/1.5] Go 1.19.6 (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8112">#8112</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc243</code></a> Go 1.19.6</li>
</ul>
</li>
<li>[release/1.5] Fix retry logic within devmapper device deactivation (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8089">#8089</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d045d</code></a> Fix retry logic within devmapper device deactivation</li>
</ul>
</li>
<li>[release/1.5] CI: skip some jobs when <code>repo != containerd/containerd</code> (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8084">#8084</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/34451bc66453aad2f911aa8bffa6817061e4a72b"><code>34451bc66</code></a> CI: skip some jobs when <code>repo != containerd/containerd</code></li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/39bb06f98f17c7a226b10269d325c861585b2389"><code>39bb06f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8117">#8117</a> from dmcgowan/prepare-v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/ddf9de6cbb30f9edf1b04d304eac67d1383e406b"><code>ddf9de6</code></a> Prepare release notes for v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/28e461805038a431c0bd1c04f31a438470c24450"><code>28e4618</code></a> Merge pull request from GHSA-hmfx-3pcx-653p</li>
<li><a href="https://github.com/containerd/containerd/commit/959e1cf9602f3b7a71bdca7b6344b40e00504730"><code>959e1cf</code></a> Merge pull request from GHSA-259w-8hf6-59c2</li>
<li><a href="https://github.com/containerd/containerd/commit/b4538c253204b169366b7f3d3f990b47eae7ade0"><code>b4538c2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8112">#8112</a> from AkihiroSuda/cherrypick-8109-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc2</code></a> Go 1.19.6</li>
<li><a href="https://github.com/containerd/containerd/commit/7c3b24362756e11c841ec7fa4a8aecb8f94e6894"><code>7c3b243</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8089">#8089</a> from swagatbora90/backport-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d04</code></a> Fix retry logic within devmapper device deactivation</li>
<li><a href="https://github.com/containerd/containerd/commit/9e9f4c8ea77d016387bee13eeb773f4a79d6c054"><code>9e9f4c8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8084">#8084</a> from AkihiroSuda/ci-skip-on-fork-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/a62c38bf2173faa813018939710fc8491e4f7dba"><code>a62c38b</code></a> oci: fix additional GIDs</li>
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.5.16...v1.5.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.5.16&new-version=1.5.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-smart-client/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 14:38:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    Bump github.com/ipld/go-ipld-prime from 0.9.0 to 0.19.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/ipld/go-ipld-prime](https://github.com/ipld/go-ipld-prime) from 0.9.0 to 0.19.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ipld/go-ipld-prime/releases">github.com/ipld/go-ipld-prime's releases</a>.</em></p>
<blockquote>
<h2>v0.19.0</h2>
<p>go-ipld-prime's release policy says that:</p>
<blockquote>
<p>even numbers should be easy upgrades; odd numbers may change things</p>
</blockquote>
<p>The only major, potentially disruptive change in this release is a bump to Go 1.18.</p>
<h4>🛠 Breaking Changes</h4>
<p>Update go.mod to Go 1.18.</p>
<h4>🔦 Highlights</h4>
<ul>
<li><strong>Codecs</strong>: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/472">Correct JSON codec Bytes handling</a>. This change does not impact DAG-JSON, which is the generally recommended codec for JSON output as the JSON codec cannot properly handle Bytes or Links.</li>
<li><strong>Dependencies</strong>:
<ul>
<li>Update to go-multihash@v0.2.1: <a href="https://github.com/multiformats/go-multihash/releases/tag/v0.2.1">https://github.com/multiformats/go-multihash/releases/tag/v0.2.1</a></li>
<li>Update to go-multicodec@v0.6.0: <a href="https://github.com/multiformats/go-multicodec/releases/tag/v0.6.0">https://github.com/multiformats/go-multicodec/releases/tag/v0.6.0</a></li>
<li>Update to go-cid@v0.3.2: <a href="https://github.com/ipfs/go-cid/compare/v0.2.0...v0.3.2">https://github.com/ipfs/go-cid/compare/v0.2.0...v0.3.2</a></li>
</ul>
</li>
</ul>
<h2>v0.18.0</h2>
<p>go-ipld-prime's release policy says that:</p>
<blockquote>
<p>even numbers should be easy upgrades; odd numbers may change things</p>
</blockquote>
<p>So, as an even number, this v0.18.0 release should be a smooth ride for upgraders from v0.17.0. We have 3 major feature additions, all focused on <a href="https://pkg.go.dev/github.com/ipld/go-ipld-prime/node/bindnode">Bindnode</a>.</p>
<h4>🔦 Highlights</h4>
<ul>
<li><strong>Bindnode</strong>: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/414">Custom Go type converters</a> - Bindnode performs bidirectional mapping of Go types to the IPLD Data Model, and in doing so, it assumes a straightforward mapping of values to their encoded forms. But there are common cases where a Go type doesn't have a straightforward path to serialization, either because the encoded form needs a custom layout, or because bindnode doesn't have enough information to infer a serialization pattern. Custom Go type converters for bindnode allow a user to supply a pair of converter functions for a Go type that dictate how to map that type to an IPLD Data Model kind. See the <strong><a href="https://pkg.go.dev/github.com/ipld/go-ipld-prime/node/bindnode">bindnode documentation</a></strong> for more information.</li>
<li><strong>Bindnode</strong>: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/437">Type registry</a> - Setting up Go type mappings with Bindnode involves some boilerplate. A basic type registry is now available that takes some of this boilerplate away; giving you a single place to register, and perform conversions to and from Go types, Data Model (<code>Node</code>) forms or directly through serialization. See the <strong><a href="https://pkg.go.dev/github.com/ipld/go-ipld-prime/node/bindnode/registry">bindnode/registry documentation</a></strong> for more information.</li>
<li><strong>Bindnode</strong>: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/414/commits/87211682cb963ef1c98fa63909f67a8b02d1108c">Full <code>uint64</code> support</a> - the <code>uint64</code> support introduced in go-ipld-prime@v0.17.0 has been wired into Bindnode. The Data Model (<code>Node</code>) forms expose integers as <code>int64</code> values, which is lossy for unsigned 64-bit integers. Bindnode Go types using <code>uint64</code> values are now lossless in round-trips through serialization to codecs that support the full range (DAG-CBOR most notably).</li>
</ul>
<p>You can see all of these new features in action using Filecoin Go types, allowing a mapping between Go types, Data Model (<code>Node</code>) forms, and their DAG-CBOR serialized forms with <a href="https://github-redirect.dependabot.com/filecoin-project/go-fil-markets/pull/713">data-transfer vouchers</a>. These features also allow us to interact with the original Go types, without modification, including <code>big.Int</code> serialization to <code>Bytes</code>, Filecoin <code>Signature</code> serialization to a byte-prefix discriminated <code>Bytes</code> and more. Since the Go types are unchanged, they can also simultaneously support <a href="https://github.com/whyrusleeping/cbor-gen">cbor-gen</a> serialization, allowing an easier migration path.</p>
<h2>v0.17.0</h2>
<p><strong>go-ipld-prime</strong>'s release policy says that:</p>
<blockquote>
<p>even numbers should be easy upgrades; odd numbers may change things</p>
</blockquote>
<p>In that spirit, this v0.17.0 release includes some potentially breaking changes. Although minor, they are marked below and they may lead to behavioral changes in your use of this library.</p>
<h4>🛠 Breaking Changes</h4>
<ul>
<li><strong>Codecs</strong>:
<ul>
<li>DAG-CBOR, DAG-JSON: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/433">Error on <code>cid.Undef</code> links in dag{json,cbor} encoding</a> - previously, encoding Link nodes that were empty CIDs (uninitialized zero-value or explicitly <code>cid.Undef</code>) would have passed through the DAG-CBOR or DAG-JSON codecs, silently producing erroneous output that wouldn't successfully pass back through a decode. (Rod Vagg)</li>
</ul>
</li>
<li><strong>Bindnode</strong>:
<ul>
<li><a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/427">Panic early if API has been passed ptr-to-ptr</a> - previous usage of bindnode using pointers-to-pointers may have deferred (or in some cases avoided) panics until deeper usage of the API, this change makes it earlier to make it clear that pointer-to-pointer is not appropriate usage. (Rod Vagg)</li>
</ul>
</li>
<li><strong>Build</strong>:
<ul>
<li><a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/394">Drop Go 1.16.x testing &amp; begin testing Go 1.18.x</a> (Daniel Martí)</li>
<li>Note also that in this release, the <a href="https://github.com/ipfs/go-cid">github.com/ipfs/<strong>go-cid</strong></a> dependency is upgraded from 0.0.4 to 0.2.0 which includes a breaking change with the removal of the <code>cid.Codecs</code> and <code>cid.CodecToStr</code> maps which may disruptive. See <a href="https://github.com/ipfs/go-cid/releases/tag/v0.2.0">the go-cid@0.2.0 release page for details</a>.</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ipld/go-ipld-prime/blob/master/CHANGELOG.md">github.com/ipld/go-ipld-prime's changelog</a>.</em></p>
<blockquote>
<h3>v0.19.0</h3>
<p><em>2022 October 13</em></p>
<p>go-ipld-prime's release policy says that:</p>
<blockquote>
<p>even numbers should be easy upgrades; odd numbers may change things</p>
</blockquote>
<p>The major change in this release is a bump to Go 1.18.</p>
<h4>🛠 Breaking Changes</h4>
<p>Update go.mod to Go 1.18.</p>
<h4>🔦 Highlights</h4>
<ul>
<li><strong>Codecs</strong>: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/472">Correct JSON codec Bytes handling</a>. This change does not impact DAG-JSON, which is the generally recommended codec for JSON output as the JSON codec cannot properly handle Bytes or Links.</li>
<li><strong>Dependencies</strong>:
<ul>
<li>Update to go-multihash@v0.2.1: <a href="https://github.com/multiformats/go-multihash/releases/tag/v0.2.1">https://github.com/multiformats/go-multihash/releases/tag/v0.2.1</a></li>
<li>Update to go-multicodec@v0.6.0: <a href="https://github.com/multiformats/go-multicodec/releases/tag/v0.6.0">https://github.com/multiformats/go-multicodec/releases/tag/v0.6.0</a></li>
<li>Update to go-cid@v0.3.2: <a href="https://github.com/ipfs/go-cid/compare/v0.2.0...v0.3.2">https://github.com/ipfs/go-cid/compare/v0.2.0...v0.3.2</a></li>
</ul>
</li>
</ul>
<h3>v0.18.0</h3>
<p><em>2022 August 01</em></p>
<p>go-ipld-prime's release policy says that:</p>
<blockquote>
<p>even numbers should be easy upgrades; odd numbers may change things</p>
</blockquote>
<p>So, as an even number, this v0.18.0 release should be a smooth ride for upgraders from v0.17.0. We have 3 major feature additions, all focused on <a href="https://pkg.go.dev/github.com/ipld/go-ipld-prime/node/bindnode">Bindnode</a>.</p>
<h4>🔦 Highlights</h4>
<ul>
<li><strong>Bindnode</strong>: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/414">Custom Go type converters</a> - Bindnode performs bidirectional mapping of Go types to the IPLD Data Model, and in doing so, it assumes a straightforward mapping of values to their encoded forms. But there are common cases where a Go type doesn't have a straightforward path to serialization, either because the encoded form needs a custom layout, or because bindnode doesn't have enough information to infer a serialization pattern. Custom Go type converters for bindnode allow a user to supply a pair of converter functions for a Go type that dictate how to map that type to an IPLD Data Model kind. See the <strong><a href="https://pkg.go.dev/github.com/ipld/go-ipld-prime/node/bindnode">bindnode documentation</a></strong> for more information.</li>
<li><strong>Bindnode</strong>: <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/437">Type registry</a> - Setting up Go type mappings with Bindnode involves some boilerplate. A basic type registry is now available that takes some of this boilerplate away; giving you a single place to register, and perform conversions to and from Go types, Data Model (<code>Node</code>) forms or directly through serialization. See the <strong><a href="https://pkg.go.dev/github.com/ipld/go-ipld-prime/node/bindnode/registry">bindnode/registry documentation</a></strong> for more information.</li>
<li><strong>Bindnode</strong> <a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/pull/414/commits/87211682cb963ef1c98fa63909f67a8b02d1108c">Full <code>uint64</code> support</a> - the <code>uint64</code> support introduced in go-ipld-prime@v0.17.0 has been wired into Bindnode. The Data Model (<code>Node</code>) forms expose integers as <code>int64</code> values, which is lossy for unsigned 64-bit integers. Bindnode Go types using <code>uint64</code> values are now lossless in round-trips through serialization to codecs that support the full range (DAG-CBOR most notably).</li>
</ul>
<p>You can see all of these new features in action using Filecoin Go types, allowing a mapping between Go types, Data Model (<code>Node</code>) forms, and their DAG-CBOR serialized forms with <a href="https://github-redirect.dependabot.com/filecoin-project/go-fil-markets/pull/713">data-transfer vouchers</a>. These features also allow us to interact with the original Go types, without modification, including <code>big.Int</code> serialization to <code>Bytes</code>, Filecoin <code>Signature</code> serialization to a byte-prefix discriminated <code>Bytes</code> and more. Since the Go types are unchanged, they can also simultaneously support <a href="https://github.com/whyrusleeping/cbor-gen">cbor-gen</a> serialization, allowing an easier migration path.</p>
<h3>v0.17.0</h3>
<p><em>2022 Jun 15</em></p>
<p>go-ipld-prime's release policy says that:</p>
<blockquote>
<p>even numbers should be easy upgrades; odd numbers may change things</p>
</blockquote>
<p>In that spirit, this v0.17.0 release includes some potentially breaking changes. Although minor, they are marked below and they may lead to behavioral changes in your use of this library.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/ac99fc3ecbe040a04ff4dcb83a00c9f65e863b15"><code>ac99fc3</code></a> Prepare v0.19.0</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/146d1c8529676fe9ee0604f014656af2395505fc"><code>146d1c8</code></a> fix: correct json codec links &amp; bytes handling</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/7548eb883bda4712355797547a0628a0ad1c00cb"><code>7548eb8</code></a> build(deps): bump github.com/google/go-cmp from 0.5.8 to 0.5.9 (<a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/issues/468">#468</a>)</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/4b84deb80396dd4b66b9072cf0048cccb128f7eb"><code>4b84deb</code></a> build(deps): bump github.com/ipfs/go-cid from 0.3.0 to 0.3.2 (<a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/issues/466">#466</a>)</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/a007538ff21d75c67f6b80ceb140553d17347d65"><code>a007538</code></a> build(deps): bump github.com/ipfs/go-cid in /storage/bsadapter (<a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/issues/465">#465</a>)</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/6c3aeeaf946efb11d54dac446aa9adb56f0f3502"><code>6c3aeea</code></a> build(deps): bump github.com/ipfs/go-cid in /storage/bsrvadapter (<a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/issues/464">#464</a>)</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/8fd3dea583cd0ebd6bb65060fbe5ac570e4440c7"><code>8fd3dea</code></a> test(basicnode): increase test coverage for int and map types (<a href="https://github-redirect.dependabot.com/ipld/go-ipld-prime/issues/454">#454</a>)</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/e57582f782f7edc6c631448bf0933a5022037961"><code>e57582f</code></a> build(deps): bump github.com/ipfs/go-cid in /storage/bsrvadapter</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/8572ef0d8b8bd8781e243f97a3b78739f8fd7ceb"><code>8572ef0</code></a> build(deps): bump github.com/ipfs/go-cid in /storage/bsadapter</li>
<li><a href="https://github.com/ipld/go-ipld-prime/commit/e23acb3d85bcf21dba0459f525c4d33390161ed7"><code>e23acb3</code></a> build(deps): bump github.com/ipfs/go-cid from 0.2.0 to 0.3.0</li>
<li>Additional commits viewable in <a href="https://github.com/ipld/go-ipld-prime/compare/v0.9.0...v0.19.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ipld/go-ipld-prime&package-manager=go_modules&previous-version=0.9.0&new-version=0.19.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-smart-client/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 22:12:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    Fixes in orderer yaml template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Listen address should be set to 0.0.0.0

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 13:15:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    Nwo enhancements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 19:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    various improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                - db service, badger driver: load badger option from FSC configuration
- additional logs

Linked to: https://github.com/hyperledger-labs/fabric-token-sdk/pull/454
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 09:46:45 +0000 UTC
    </div>
</div>

