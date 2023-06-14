---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/707" class=".btn">#707</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.5.2 to 1.5.18 in /integration/go_chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.5.2 to 1.5.18.
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
<li><strong>Update Go to 1.19.6</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/8112">#8112</a>)</li>
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
<li>[release/1.5] Prepare release notes for v1.5.18 (<a href="https://redirect.github.com/containerd/containerd/pull/8117">#8117</a>)
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
<li>[release/1.5] Go 1.19.6 (<a href="https://redirect.github.com/containerd/containerd/pull/8112">#8112</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc243</code></a> Go 1.19.6</li>
</ul>
</li>
<li>[release/1.5] Fix retry logic within devmapper device deactivation (<a href="https://redirect.github.com/containerd/containerd/pull/8089">#8089</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d045d</code></a> Fix retry logic within devmapper device deactivation</li>
</ul>
</li>
<li>[release/1.5] CI: skip some jobs when <code>repo != containerd/containerd</code> (<a href="https://redirect.github.com/containerd/containerd/pull/8084">#8084</a>)
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
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/blob/main/RELEASES.md">github.com/containerd/containerd's changelog</a>.</em></p>
<blockquote>
<h1>Versioning and Release</h1>
<p>This document details the versioning and release plan for containerd. Stability
is a top goal for this project, and we hope that this document and the processes
it entails will help to achieve that. It covers the release process, versioning
numbering, backporting, API stability and support horizons.</p>
<p>If you rely on containerd, it would be good to spend time understanding the
areas of the API that are and are not supported and how they impact your
project in the future.</p>
<p>This document will be considered a living document. Supported timelines,
backport targets and API stability guarantees will be updated here as they
change.</p>
<p>If there is something that you require or this document leaves out, please
reach out by <a href="https://github.com/containerd/containerd/issues">filing an issue</a>.</p>
<h2>Releases</h2>
<p>Releases of containerd will be versioned using dotted triples, similar to
<a href="http://semver.org/">Semantic Version</a>. For the purposes of this document, we
will refer to the respective components of this triple as
<code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>. The version number may have additional information,
such as alpha, beta and release candidate qualifications. Such releases will be
considered &quot;pre-releases&quot;.</p>
<h3>Major and Minor Releases</h3>
<p>Major and minor releases of containerd will be made from main. Releases of
containerd will be marked with GPG signed tags and announced at
<a href="https://github.com/containerd/containerd/releases">https://github.com/containerd/containerd/releases</a>. The tag will be of the
format <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> and should be made with the command <code>git tag -s v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</p>
<p>After a minor release, a branch will be created, with the format
<code>release/&lt;major&gt;.&lt;minor&gt;</code> from the minor tag. All further patch releases will
be done from that branch. For example, once we release <code>v1.0.0</code>, a branch
<code>release/1.0</code> will be created from that tag. All future patch releases will be
done against that branch.</p>
<h3>Pre-releases</h3>
<p>Pre-releases, such as alphas, betas and release candidates will be conducted
from their source branch. For major and minor releases, these releases will be
done from main. For patch releases, these pre-releases should be done within
the corresponding release branch.</p>
<p>While pre-releases are done to assist in the stabilization process, no
guarantees are provided.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/39bb06f98f17c7a226b10269d325c861585b2389"><code>39bb06f</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8117">#8117</a> from dmcgowan/prepare-v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/ddf9de6cbb30f9edf1b04d304eac67d1383e406b"><code>ddf9de6</code></a> Prepare release notes for v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/28e461805038a431c0bd1c04f31a438470c24450"><code>28e4618</code></a> Merge pull request from GHSA-hmfx-3pcx-653p</li>
<li><a href="https://github.com/containerd/containerd/commit/959e1cf9602f3b7a71bdca7b6344b40e00504730"><code>959e1cf</code></a> Merge pull request from GHSA-259w-8hf6-59c2</li>
<li><a href="https://github.com/containerd/containerd/commit/b4538c253204b169366b7f3d3f990b47eae7ade0"><code>b4538c2</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8112">#8112</a> from AkihiroSuda/cherrypick-8109-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc2</code></a> Go 1.19.6</li>
<li><a href="https://github.com/containerd/containerd/commit/7c3b24362756e11c841ec7fa4a8aecb8f94e6894"><code>7c3b243</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8089">#8089</a> from swagatbora90/backport-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d04</code></a> Fix retry logic within devmapper device deactivation</li>
<li><a href="https://github.com/containerd/containerd/commit/9e9f4c8ea77d016387bee13eeb773f4a79d6c054"><code>9e9f4c8</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8084">#8084</a> from AkihiroSuda/ci-skip-on-fork-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/a62c38bf2173faa813018939710fc8491e4f7dba"><code>a62c38b</code></a> oci: fix additional GIDs</li>
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.5.2...v1.5.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.5.2&new-version=1.5.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-private-chaincode/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 00:00:09 +0000 UTC
    </div>
</div>

