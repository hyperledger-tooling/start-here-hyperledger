---
layout: default
title: aries-framework-go-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go-ext
---

# aries-framework-go-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump github.com/containerd/containerd from 1.5.5 to 1.5.18 in /test/bdd/vdr/orb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.5.5 to 1.5.18.
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
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.5.5...v1.5.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.5.5&new-version=1.5.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 14:40:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump github.com/prometheus/client_golang from 1.11.0 to 1.11.1 in /component/vdr/orb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/prometheus/client_golang](https://github.com/prometheus/client_golang) from 1.11.0 to 1.11.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prometheus/client_golang/releases">github.com/prometheus/client_golang's releases</a>.</em></p>
<blockquote>
<h2>1.11.1 / 2022-02-15</h2>
<ul>
<li>[SECURITY FIX] promhttp: Check validity of method and code label values <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a> (Addressed <a href="https://github.com/prometheus/client_golang/security/advisories/GHSA-cg3q-j54f-5p7p"><code>CVE-2022-21698</code></a>)</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>promhttp: Check validity of method and code label values by <a href="https://github.com/bwplotka"><code>@​bwplotka</code></a> and <a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> in  <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1">https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prometheus/client_golang/blob/main/CHANGELOG.md">github.com/prometheus/client_golang's changelog</a>.</em></p>
<blockquote>
<h2>Unreleased</h2>
<h2>1.14.0 / 2022-11-08</h2>
<ul>
<li>[FEATURE] Add Support for Native Histograms. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1150">#1150</a></li>
<li>[CHANGE] Extend <code>prometheus.Registry</code> to implement <code>prometheus.Collector</code> interface. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1103">#1103</a></li>
</ul>
<h2>1.13.1 / 2022-11-01</h2>
<ul>
<li>[BUGFIX] Fix race condition with Exemplar in Counter. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1146">#1146</a></li>
<li>[BUGFIX] Fix <code>CumulativeCount</code> value of <code>+Inf</code> bucket created from exemplar. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1148">#1148</a></li>
<li>[BUGFIX] Fix double-counting bug in <code>promhttp.InstrumentRoundTripperCounter</code>. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1118">#1118</a></li>
</ul>
<h2>1.13.0 / 2022-08-05</h2>
<ul>
<li>[CHANGE] Minimum required Go version is now 1.17 (we also test client_golang against new 1.19 version).</li>
<li>[ENHANCEMENT] Added <code>prometheus.TransactionalGatherer</code> interface for <code>promhttp.Handler</code> use which allows using low allocation update techniques for custom collectors. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/989">#989</a></li>
<li>[ENHANCEMENT] Added exemplar support to <code>prometheus.NewConstHistogram</code>. See <a href="https://github.com/prometheus/client_golang/blob/main/prometheus/examples_test.go#L602"><code>ExampleNewConstHistogram_WithExemplar</code></a> example on how to use it. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/986">#986</a></li>
<li>[ENHANCEMENT] <code>prometheus/push.Pusher</code> has now context aware methods that pass context to HTTP request. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1028">#1028</a></li>
<li>[ENHANCEMENT] <code>prometheus/push.Pusher</code> has now <code>Error</code> method that retrieve last error. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1075">#1075</a></li>
<li>[ENHANCEMENT] <code>testutil.GatherAndCompare</code> provides now readable diff on failed comparisons. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/998">#998</a></li>
<li>[ENHANCEMENT] Query API now supports timeouts. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1014">#1014</a></li>
<li>[ENHANCEMENT] New <code>MetricVec</code> method <code>DeletePartialMatch(labels Labels)</code> for deleting all metrics that match provided labels. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1013">#1013</a></li>
<li>[ENHANCEMENT] <code>api.Config</code> now accepts passing custom <code>*http.Client</code>. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1025">#1025</a></li>
<li>[BUGFIX] Raise exemplar labels limit from 64 to 128 bytes as specified in OpenMetrics spec. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1091">#1091</a></li>
<li>[BUGFIX] Allow adding exemplar to +Inf bucket to const histograms. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1094">#1094</a></li>
<li>[ENHANCEMENT] Most <code>promhttp.Instrument*</code> middlewares now supports adding exemplars to metrics. This allows hooking those to your tracing middleware that retrieves trace ID and put it in exemplar if present. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1055">#1055</a></li>
<li>[ENHANCEMENT] Added <code>testutil.ScrapeAndCompare</code> method. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1043">#1043</a></li>
<li>[BUGFIX] Fixed <code>GopherJS</code> build support. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/897">#897</a></li>
<li>[ENHANCEMENT] :warning: Added way to specify what <code>runtime/metrics</code>  <code>collectors.NewGoCollector</code> should use. See <a href="https://github.com/prometheus/client_golang/blob/main/prometheus/collectors/go_collector_latest_test.go#L263"><code>ExampleGoCollector_WithAdvancedGoMetrics</code></a>. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1102">#1102</a></li>
</ul>
<h2>1.12.2 / 2022-05-13</h2>
<ul>
<li>[CHANGE] Added <code>collectors.WithGoCollections</code> that allows to choose what collection of Go runtime metrics user wants: Equivalent of <a href="https://pkg.go.dev/runtime#MemStats"><code>MemStats</code> structure</a> configured using <code>GoRuntimeMemStatsCollection</code>, new based on dedicated <a href="https://pkg.go.dev/runtime/metrics">runtime/metrics</a> metrics represented by <code>GoRuntimeMetricsCollection</code> option, or both by specifying <code>GoRuntimeMemStatsCollection | GoRuntimeMetricsCollection</code> flag. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1031">#1031</a></li>
<li>[CHANGE] :warning: Change in <code>collectors.NewGoCollector</code> metrics: Reverting addition of new ~80 runtime metrics by default. You can enable this back with <code>GoRuntimeMetricsCollection</code> option or <code>GoRuntimeMemStatsCollection | GoRuntimeMetricsCollection</code> for smooth transition.</li>
<li>[BUGFIX] Fixed the bug that causes generated histogram metric names to end with <code>_total</code>. ⚠️ This changes 3 metric names in the new Go collector that was reverted from default in this release.
<ul>
<li><code>go_gc_heap_allocs_by_size_bytes_total</code> -&gt; <code>go_gc_heap_allocs_by_size_bytes</code>,</li>
<li><code>go_gc_heap_frees_by_size_bytes_total</code> -&gt; <code>go_gc_heap_allocs_by_size_bytes</code></li>
<li><code>go_gc_pauses_seconds_total</code> -&gt; <code>go_gc_pauses_seconds</code>.</li>
</ul>
</li>
<li>[CHANCE] Removed <code>-Inf</code> buckets from new Go Collector histograms.</li>
</ul>
<h2>1.12.1 / 2022-01-29</h2>
<ul>
<li>[BUGFIX] Make the Go 1.17 collector concurrency-safe <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/969">#969</a>
<ul>
<li>Use simpler locking in the Go 1.17 collector <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/975">#975</a></li>
</ul>
</li>
<li>[BUGFIX] Reduce granularity of histogram buckets for Go 1.17 collector <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/974">#974</a></li>
<li>[ENHANCEMENT] API client: make HTTP reads more efficient <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/976">#976</a></li>
</ul>
<h2>1.12.0 / 2022-01-19</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prometheus/client_golang/commit/989baa30fe956631907493ccee1f8e7708660d96"><code>989baa3</code></a> promhttp: Check validity of method and code label values (<a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/962">#962</a>) (<a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/987">#987</a>)</li>
<li>See full diff in <a href="https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/prometheus/client_golang&package-manager=go_modules&previous-version=1.11.0&new-version=1.11.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 03:11:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump github.com/prometheus/client_golang from 1.11.0 to 1.11.1 in /test/bdd/vdr/orb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/prometheus/client_golang](https://github.com/prometheus/client_golang) from 1.11.0 to 1.11.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prometheus/client_golang/releases">github.com/prometheus/client_golang's releases</a>.</em></p>
<blockquote>
<h2>1.11.1 / 2022-02-15</h2>
<ul>
<li>[SECURITY FIX] promhttp: Check validity of method and code label values <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a> (Addressed <a href="https://github.com/prometheus/client_golang/security/advisories/GHSA-cg3q-j54f-5p7p"><code>CVE-2022-21698</code></a>)</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>promhttp: Check validity of method and code label values by <a href="https://github.com/bwplotka"><code>@​bwplotka</code></a> and <a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> in  <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1">https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prometheus/client_golang/blob/main/CHANGELOG.md">github.com/prometheus/client_golang's changelog</a>.</em></p>
<blockquote>
<h2>Unreleased</h2>
<h2>1.14.0 / 2022-11-08</h2>
<ul>
<li>[FEATURE] Add Support for Native Histograms. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1150">#1150</a></li>
<li>[CHANGE] Extend <code>prometheus.Registry</code> to implement <code>prometheus.Collector</code> interface. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1103">#1103</a></li>
</ul>
<h2>1.13.1 / 2022-11-01</h2>
<ul>
<li>[BUGFIX] Fix race condition with Exemplar in Counter. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1146">#1146</a></li>
<li>[BUGFIX] Fix <code>CumulativeCount</code> value of <code>+Inf</code> bucket created from exemplar. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1148">#1148</a></li>
<li>[BUGFIX] Fix double-counting bug in <code>promhttp.InstrumentRoundTripperCounter</code>. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1118">#1118</a></li>
</ul>
<h2>1.13.0 / 2022-08-05</h2>
<ul>
<li>[CHANGE] Minimum required Go version is now 1.17 (we also test client_golang against new 1.19 version).</li>
<li>[ENHANCEMENT] Added <code>prometheus.TransactionalGatherer</code> interface for <code>promhttp.Handler</code> use which allows using low allocation update techniques for custom collectors. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/989">#989</a></li>
<li>[ENHANCEMENT] Added exemplar support to <code>prometheus.NewConstHistogram</code>. See <a href="https://github.com/prometheus/client_golang/blob/main/prometheus/examples_test.go#L602"><code>ExampleNewConstHistogram_WithExemplar</code></a> example on how to use it. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/986">#986</a></li>
<li>[ENHANCEMENT] <code>prometheus/push.Pusher</code> has now context aware methods that pass context to HTTP request. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1028">#1028</a></li>
<li>[ENHANCEMENT] <code>prometheus/push.Pusher</code> has now <code>Error</code> method that retrieve last error. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1075">#1075</a></li>
<li>[ENHANCEMENT] <code>testutil.GatherAndCompare</code> provides now readable diff on failed comparisons. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/998">#998</a></li>
<li>[ENHANCEMENT] Query API now supports timeouts. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1014">#1014</a></li>
<li>[ENHANCEMENT] New <code>MetricVec</code> method <code>DeletePartialMatch(labels Labels)</code> for deleting all metrics that match provided labels. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1013">#1013</a></li>
<li>[ENHANCEMENT] <code>api.Config</code> now accepts passing custom <code>*http.Client</code>. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1025">#1025</a></li>
<li>[BUGFIX] Raise exemplar labels limit from 64 to 128 bytes as specified in OpenMetrics spec. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1091">#1091</a></li>
<li>[BUGFIX] Allow adding exemplar to +Inf bucket to const histograms. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1094">#1094</a></li>
<li>[ENHANCEMENT] Most <code>promhttp.Instrument*</code> middlewares now supports adding exemplars to metrics. This allows hooking those to your tracing middleware that retrieves trace ID and put it in exemplar if present. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1055">#1055</a></li>
<li>[ENHANCEMENT] Added <code>testutil.ScrapeAndCompare</code> method. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1043">#1043</a></li>
<li>[BUGFIX] Fixed <code>GopherJS</code> build support. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/897">#897</a></li>
<li>[ENHANCEMENT] :warning: Added way to specify what <code>runtime/metrics</code>  <code>collectors.NewGoCollector</code> should use. See <a href="https://github.com/prometheus/client_golang/blob/main/prometheus/collectors/go_collector_latest_test.go#L263"><code>ExampleGoCollector_WithAdvancedGoMetrics</code></a>. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1102">#1102</a></li>
</ul>
<h2>1.12.2 / 2022-05-13</h2>
<ul>
<li>[CHANGE] Added <code>collectors.WithGoCollections</code> that allows to choose what collection of Go runtime metrics user wants: Equivalent of <a href="https://pkg.go.dev/runtime#MemStats"><code>MemStats</code> structure</a> configured using <code>GoRuntimeMemStatsCollection</code>, new based on dedicated <a href="https://pkg.go.dev/runtime/metrics">runtime/metrics</a> metrics represented by <code>GoRuntimeMetricsCollection</code> option, or both by specifying <code>GoRuntimeMemStatsCollection | GoRuntimeMetricsCollection</code> flag. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/1031">#1031</a></li>
<li>[CHANGE] :warning: Change in <code>collectors.NewGoCollector</code> metrics: Reverting addition of new ~80 runtime metrics by default. You can enable this back with <code>GoRuntimeMetricsCollection</code> option or <code>GoRuntimeMemStatsCollection | GoRuntimeMetricsCollection</code> for smooth transition.</li>
<li>[BUGFIX] Fixed the bug that causes generated histogram metric names to end with <code>_total</code>. ⚠️ This changes 3 metric names in the new Go collector that was reverted from default in this release.
<ul>
<li><code>go_gc_heap_allocs_by_size_bytes_total</code> -&gt; <code>go_gc_heap_allocs_by_size_bytes</code>,</li>
<li><code>go_gc_heap_frees_by_size_bytes_total</code> -&gt; <code>go_gc_heap_allocs_by_size_bytes</code></li>
<li><code>go_gc_pauses_seconds_total</code> -&gt; <code>go_gc_pauses_seconds</code>.</li>
</ul>
</li>
<li>[CHANCE] Removed <code>-Inf</code> buckets from new Go Collector histograms.</li>
</ul>
<h2>1.12.1 / 2022-01-29</h2>
<ul>
<li>[BUGFIX] Make the Go 1.17 collector concurrency-safe <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/969">#969</a>
<ul>
<li>Use simpler locking in the Go 1.17 collector <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/975">#975</a></li>
</ul>
</li>
<li>[BUGFIX] Reduce granularity of histogram buckets for Go 1.17 collector <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/974">#974</a></li>
<li>[ENHANCEMENT] API client: make HTTP reads more efficient <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/976">#976</a></li>
</ul>
<h2>1.12.0 / 2022-01-19</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prometheus/client_golang/commit/989baa30fe956631907493ccee1f8e7708660d96"><code>989baa3</code></a> promhttp: Check validity of method and code label values (<a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/962">#962</a>) (<a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/987">#987</a>)</li>
<li>See full diff in <a href="https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/prometheus/client_golang&package-manager=go_modules&previous-version=1.11.0&new-version=1.11.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 03:09:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump github.com/opencontainers/runc from 1.0.0-rc9 to 1.1.2 in /component/storage/mongodb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.0.0-rc9 to 1.1.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/releases">github.com/opencontainers/runc's releases</a>.</em></p>
<blockquote>
<h2>runc 1.1 -- &quot;A plan depends as much upon execution as it does upon concept.&quot;</h2>
<p>This release only contains very minor changes from v1.1.0-rc.1 and is
the first release of the 1.1.y release series of runc. We do not plan to make
any new releases of the 1.0.y release series of runc, so users are strongly
encouraged to update to 1.1.0.</p>
<p>Changed:</p>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
</ul>
<h3>Static Linking Notices</h3>
<p>The <code>runc</code> binary distributed with this release are <em>statically linked</em> with
the following <a href="https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html">GNU LGPL-2.1</a> licensed libraries, with <code>runc</code> acting
as a &quot;work that uses the Library&quot;:</p>
<ul>
<li><a href="https://github.com/seccomp/libseccomp">libseccomp</a></li>
</ul>
<p>The versions of these libraries were not modified from their upstream versions,
but in order to comply with the LGPL-2.1 (§6(a)), we have attached the
complete source code for those libraries which (when combined with the attached
runc source code) may be used to exercise your rights under the LGPL-2.1.</p>
<p>However we strongly suggest that you make use of your distribution's packages
or download them from the authoritative upstream sources, especially since
these libraries are related to the security of your containers.</p>
<!-- raw HTML omitted -->
<p>Thanks to the following people who made this release possible:</p>
<ul>
<li>Akihiro Suda <a href="mailto:akihiro.suda.cz@hco.ntt.co.jp">akihiro.suda.cz@hco.ntt.co.jp</a></li>
<li>Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></li>
<li>Kir Kolyshkin <a href="mailto:kolyshkin@gmail.com">kolyshkin@gmail.com</a></li>
</ul>
<p>Signed-off-by: Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></p>
<h2>runc 1.1-rc1 -- &quot;He who controls the spice controls the universe.&quot;</h2>
<p>This release is the first release candidate for the next minor release
following runc 1.0. It contains all of the bugfixes included in runc 1.0
patch releases (up to and including 1.0.3).</p>
<p>A fair few new features have been added, and several features have been
deprecated (with plans for removal in runc 1.2). At the moment we only
plan to do a single release candidate for runc 1.1, and once 1.1.0 is
released we will not continue updating the 1.0.z runc branch.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/blob/main/CHANGELOG.md">github.com/opencontainers/runc's changelog</a>.</em></p>
<blockquote>
<h2>[1.1.2] - 2022-05-11</h2>
<blockquote>
<p>I should think I'm going to be a perpetual student.</p>
</blockquote>
<h3>Security</h3>
<ul>
<li>A bug was found in runc where runc exec --cap executed processes with
non-empty inheritable Linux process capabilities, creating an atypical Linux
environment. For more information, see <a href="https://github.com/opencontainers/runc/security/advisories/GHSA-f3fp-gc8g-vw66">GHSA-f3fp-gc8g-vw66</a> and
CVE-2022-29162.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>runc spec</code> no longer sets any inheritable capabilities in the created
example OCI spec (<code>config.json</code>) file.</li>
</ul>
<h2>[1.1.1] - 2022-03-28</h2>
<blockquote>
<p>Violence is the last refuge of the incompetent.</p>
</blockquote>
<h3>Added</h3>
<ul>
<li>CI is now also run on centos-stream-9. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li><code>runc run/start</code> can now run a container with read-only <code>/dev</code> in OCI spec,
rather than error out. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3355">#3355</a>)</li>
<li><code>runc exec</code> now ensures that <code>--cgroup</code> argument is a sub-cgroup. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3403">#3403</a>)</li>
<li>libcontainer systemd v2 manager no longer errors out if one of the files
listed in <code>/sys/kernel/cgroup/delegate</code> do not exist in container's cgroup.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3387">#3387</a>, <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3404">#3404</a>)</li>
<li>Loose OCI spec validation to avoid bogus &quot;Intel RDT is not supported&quot; error.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3406">#3406</a>)</li>
<li>libcontainer/cgroups no longer panics in cgroup v1 managers if <code>stat</code>
of <code>/sys/fs/cgroup/unified</code> returns an error other than ENOENT. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3435">#3435</a>)</li>
</ul>
<h2>[1.1.0] - 2022-01-14</h2>
<blockquote>
<p>A plan depends as much upon execution as it does upon concept.</p>
</blockquote>
<h3>Changed</h3>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
</ul>
<h2>[1.1.0-rc.1] - 2021-12-14</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/runc/commit/a916309fff0f838eb94e928713dbc3c0d0ac7aa4"><code>a916309</code></a> VERSION: release 1.1.2</li>
<li><a href="https://github.com/opencontainers/runc/commit/364ec0f1b4fa188ad96049c590ecb42fa70ea165"><code>364ec0f</code></a> runc: do not set inheritable capabilities</li>
<li><a href="https://github.com/opencontainers/runc/commit/58546650ce11cdc2e2690bcb1de4a468e691de6d"><code>5854665</code></a> merge branch 'pr-3439' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/8959e372549a81ac6a7cc25281f6b8a423d847ca"><code>8959e37</code></a> VERSION: back to development</li>
<li><a href="https://github.com/opencontainers/runc/commit/52de29d7e0f8c0899bd7efb8810dd07f0073fa87"><code>52de29d</code></a> VERSION: release 1.1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/2636e1cb3643c87f98b7b8a950c88087656e7645"><code>2636e1c</code></a> CHANGELOG.md: add 1.1.1 release notes</li>
<li><a href="https://github.com/opencontainers/runc/commit/ae28db14244c87ab1e26db09a8ad6e5b2882ccc7"><code>ae28db1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a> from kolyshkin/1.1-add-centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/036cc348994b7fa573380401644a6faac9e102e7"><code>036cc34</code></a> CI/cirrus: add centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/c65363285b3eee6e2e3a7b356f8967ae17263d41"><code>c653632</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3438">#3438</a> from kolyshkin/1.1-fix-badges</li>
<li><a href="https://github.com/opencontainers/runc/commit/db953158e14658c62ad6cda9ac087bdb1b1e3e8c"><code>db95315</code></a> README.md: add cirrus-ci badge</li>
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.0.0-rc9...v1.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.0.0-rc9&new-version=1.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 23:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump github.com/opencontainers/runc from 1.0.0-rc9 to 1.1.2 in /component/storage/couchdb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.0.0-rc9 to 1.1.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/releases">github.com/opencontainers/runc's releases</a>.</em></p>
<blockquote>
<h2>runc 1.1 -- &quot;A plan depends as much upon execution as it does upon concept.&quot;</h2>
<p>This release only contains very minor changes from v1.1.0-rc.1 and is
the first release of the 1.1.y release series of runc. We do not plan to make
any new releases of the 1.0.y release series of runc, so users are strongly
encouraged to update to 1.1.0.</p>
<p>Changed:</p>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
</ul>
<h3>Static Linking Notices</h3>
<p>The <code>runc</code> binary distributed with this release are <em>statically linked</em> with
the following <a href="https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html">GNU LGPL-2.1</a> licensed libraries, with <code>runc</code> acting
as a &quot;work that uses the Library&quot;:</p>
<ul>
<li><a href="https://github.com/seccomp/libseccomp">libseccomp</a></li>
</ul>
<p>The versions of these libraries were not modified from their upstream versions,
but in order to comply with the LGPL-2.1 (§6(a)), we have attached the
complete source code for those libraries which (when combined with the attached
runc source code) may be used to exercise your rights under the LGPL-2.1.</p>
<p>However we strongly suggest that you make use of your distribution's packages
or download them from the authoritative upstream sources, especially since
these libraries are related to the security of your containers.</p>
<!-- raw HTML omitted -->
<p>Thanks to the following people who made this release possible:</p>
<ul>
<li>Akihiro Suda <a href="mailto:akihiro.suda.cz@hco.ntt.co.jp">akihiro.suda.cz@hco.ntt.co.jp</a></li>
<li>Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></li>
<li>Kir Kolyshkin <a href="mailto:kolyshkin@gmail.com">kolyshkin@gmail.com</a></li>
</ul>
<p>Signed-off-by: Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></p>
<h2>runc 1.1-rc1 -- &quot;He who controls the spice controls the universe.&quot;</h2>
<p>This release is the first release candidate for the next minor release
following runc 1.0. It contains all of the bugfixes included in runc 1.0
patch releases (up to and including 1.0.3).</p>
<p>A fair few new features have been added, and several features have been
deprecated (with plans for removal in runc 1.2). At the moment we only
plan to do a single release candidate for runc 1.1, and once 1.1.0 is
released we will not continue updating the 1.0.z runc branch.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/blob/main/CHANGELOG.md">github.com/opencontainers/runc's changelog</a>.</em></p>
<blockquote>
<h2>[1.1.2] - 2022-05-11</h2>
<blockquote>
<p>I should think I'm going to be a perpetual student.</p>
</blockquote>
<h3>Security</h3>
<ul>
<li>A bug was found in runc where runc exec --cap executed processes with
non-empty inheritable Linux process capabilities, creating an atypical Linux
environment. For more information, see <a href="https://github.com/opencontainers/runc/security/advisories/GHSA-f3fp-gc8g-vw66">GHSA-f3fp-gc8g-vw66</a> and
CVE-2022-29162.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>runc spec</code> no longer sets any inheritable capabilities in the created
example OCI spec (<code>config.json</code>) file.</li>
</ul>
<h2>[1.1.1] - 2022-03-28</h2>
<blockquote>
<p>Violence is the last refuge of the incompetent.</p>
</blockquote>
<h3>Added</h3>
<ul>
<li>CI is now also run on centos-stream-9. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li><code>runc run/start</code> can now run a container with read-only <code>/dev</code> in OCI spec,
rather than error out. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3355">#3355</a>)</li>
<li><code>runc exec</code> now ensures that <code>--cgroup</code> argument is a sub-cgroup. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3403">#3403</a>)</li>
<li>libcontainer systemd v2 manager no longer errors out if one of the files
listed in <code>/sys/kernel/cgroup/delegate</code> do not exist in container's cgroup.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3387">#3387</a>, <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3404">#3404</a>)</li>
<li>Loose OCI spec validation to avoid bogus &quot;Intel RDT is not supported&quot; error.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3406">#3406</a>)</li>
<li>libcontainer/cgroups no longer panics in cgroup v1 managers if <code>stat</code>
of <code>/sys/fs/cgroup/unified</code> returns an error other than ENOENT. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3435">#3435</a>)</li>
</ul>
<h2>[1.1.0] - 2022-01-14</h2>
<blockquote>
<p>A plan depends as much upon execution as it does upon concept.</p>
</blockquote>
<h3>Changed</h3>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
</ul>
<h2>[1.1.0-rc.1] - 2021-12-14</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/runc/commit/a916309fff0f838eb94e928713dbc3c0d0ac7aa4"><code>a916309</code></a> VERSION: release 1.1.2</li>
<li><a href="https://github.com/opencontainers/runc/commit/364ec0f1b4fa188ad96049c590ecb42fa70ea165"><code>364ec0f</code></a> runc: do not set inheritable capabilities</li>
<li><a href="https://github.com/opencontainers/runc/commit/58546650ce11cdc2e2690bcb1de4a468e691de6d"><code>5854665</code></a> merge branch 'pr-3439' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/8959e372549a81ac6a7cc25281f6b8a423d847ca"><code>8959e37</code></a> VERSION: back to development</li>
<li><a href="https://github.com/opencontainers/runc/commit/52de29d7e0f8c0899bd7efb8810dd07f0073fa87"><code>52de29d</code></a> VERSION: release 1.1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/2636e1cb3643c87f98b7b8a950c88087656e7645"><code>2636e1c</code></a> CHANGELOG.md: add 1.1.1 release notes</li>
<li><a href="https://github.com/opencontainers/runc/commit/ae28db14244c87ab1e26db09a8ad6e5b2882ccc7"><code>ae28db1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a> from kolyshkin/1.1-add-centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/036cc348994b7fa573380401644a6faac9e102e7"><code>036cc34</code></a> CI/cirrus: add centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/c65363285b3eee6e2e3a7b356f8967ae17263d41"><code>c653632</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3438">#3438</a> from kolyshkin/1.1-fix-badges</li>
<li><a href="https://github.com/opencontainers/runc/commit/db953158e14658c62ad6cda9ac087bdb1b1e3e8c"><code>db95315</code></a> README.md: add cirrus-ci badge</li>
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.0.0-rc9...v1.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.0.0-rc9&new-version=1.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 23:57:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump github.com/opencontainers/runc from 1.0.0-rc9 to 1.1.2 in /component/storage/mysql
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.0.0-rc9 to 1.1.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/releases">github.com/opencontainers/runc's releases</a>.</em></p>
<blockquote>
<h2>runc 1.1 -- &quot;A plan depends as much upon execution as it does upon concept.&quot;</h2>
<p>This release only contains very minor changes from v1.1.0-rc.1 and is
the first release of the 1.1.y release series of runc. We do not plan to make
any new releases of the 1.0.y release series of runc, so users are strongly
encouraged to update to 1.1.0.</p>
<p>Changed:</p>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
</ul>
<h3>Static Linking Notices</h3>
<p>The <code>runc</code> binary distributed with this release are <em>statically linked</em> with
the following <a href="https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html">GNU LGPL-2.1</a> licensed libraries, with <code>runc</code> acting
as a &quot;work that uses the Library&quot;:</p>
<ul>
<li><a href="https://github.com/seccomp/libseccomp">libseccomp</a></li>
</ul>
<p>The versions of these libraries were not modified from their upstream versions,
but in order to comply with the LGPL-2.1 (§6(a)), we have attached the
complete source code for those libraries which (when combined with the attached
runc source code) may be used to exercise your rights under the LGPL-2.1.</p>
<p>However we strongly suggest that you make use of your distribution's packages
or download them from the authoritative upstream sources, especially since
these libraries are related to the security of your containers.</p>
<!-- raw HTML omitted -->
<p>Thanks to the following people who made this release possible:</p>
<ul>
<li>Akihiro Suda <a href="mailto:akihiro.suda.cz@hco.ntt.co.jp">akihiro.suda.cz@hco.ntt.co.jp</a></li>
<li>Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></li>
<li>Kir Kolyshkin <a href="mailto:kolyshkin@gmail.com">kolyshkin@gmail.com</a></li>
</ul>
<p>Signed-off-by: Aleksa Sarai <a href="mailto:cyphar@cyphar.com">cyphar@cyphar.com</a></p>
<h2>runc 1.1-rc1 -- &quot;He who controls the spice controls the universe.&quot;</h2>
<p>This release is the first release candidate for the next minor release
following runc 1.0. It contains all of the bugfixes included in runc 1.0
patch releases (up to and including 1.0.3).</p>
<p>A fair few new features have been added, and several features have been
deprecated (with plans for removal in runc 1.2). At the moment we only
plan to do a single release candidate for runc 1.1, and once 1.1.0 is
released we will not continue updating the 1.0.z runc branch.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/blob/main/CHANGELOG.md">github.com/opencontainers/runc's changelog</a>.</em></p>
<blockquote>
<h2>[1.1.2] - 2022-05-11</h2>
<blockquote>
<p>I should think I'm going to be a perpetual student.</p>
</blockquote>
<h3>Security</h3>
<ul>
<li>A bug was found in runc where runc exec --cap executed processes with
non-empty inheritable Linux process capabilities, creating an atypical Linux
environment. For more information, see <a href="https://github.com/opencontainers/runc/security/advisories/GHSA-f3fp-gc8g-vw66">GHSA-f3fp-gc8g-vw66</a> and
CVE-2022-29162.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>runc spec</code> no longer sets any inheritable capabilities in the created
example OCI spec (<code>config.json</code>) file.</li>
</ul>
<h2>[1.1.1] - 2022-03-28</h2>
<blockquote>
<p>Violence is the last refuge of the incompetent.</p>
</blockquote>
<h3>Added</h3>
<ul>
<li>CI is now also run on centos-stream-9. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li><code>runc run/start</code> can now run a container with read-only <code>/dev</code> in OCI spec,
rather than error out. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3355">#3355</a>)</li>
<li><code>runc exec</code> now ensures that <code>--cgroup</code> argument is a sub-cgroup. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3403">#3403</a>)</li>
<li>libcontainer systemd v2 manager no longer errors out if one of the files
listed in <code>/sys/kernel/cgroup/delegate</code> do not exist in container's cgroup.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3387">#3387</a>, <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3404">#3404</a>)</li>
<li>Loose OCI spec validation to avoid bogus &quot;Intel RDT is not supported&quot; error.
(<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3406">#3406</a>)</li>
<li>libcontainer/cgroups no longer panics in cgroup v1 managers if <code>stat</code>
of <code>/sys/fs/cgroup/unified</code> returns an error other than ENOENT. (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3435">#3435</a>)</li>
</ul>
<h2>[1.1.0] - 2022-01-14</h2>
<blockquote>
<p>A plan depends as much upon execution as it does upon concept.</p>
</blockquote>
<h3>Changed</h3>
<ul>
<li>libcontainer will now refuse to build without the nsenter package being
correctly compiled (specifically this requires CGO to be enabled). This
should avoid folks accidentally creating broken runc binaries (and
incorrectly importing our internal libraries into their projects). (<a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3331">#3331</a>)</li>
</ul>
<h2>[1.1.0-rc.1] - 2021-12-14</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/runc/commit/a916309fff0f838eb94e928713dbc3c0d0ac7aa4"><code>a916309</code></a> VERSION: release 1.1.2</li>
<li><a href="https://github.com/opencontainers/runc/commit/364ec0f1b4fa188ad96049c590ecb42fa70ea165"><code>364ec0f</code></a> runc: do not set inheritable capabilities</li>
<li><a href="https://github.com/opencontainers/runc/commit/58546650ce11cdc2e2690bcb1de4a468e691de6d"><code>5854665</code></a> merge branch 'pr-3439' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/8959e372549a81ac6a7cc25281f6b8a423d847ca"><code>8959e37</code></a> VERSION: back to development</li>
<li><a href="https://github.com/opencontainers/runc/commit/52de29d7e0f8c0899bd7efb8810dd07f0073fa87"><code>52de29d</code></a> VERSION: release 1.1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/2636e1cb3643c87f98b7b8a950c88087656e7645"><code>2636e1c</code></a> CHANGELOG.md: add 1.1.1 release notes</li>
<li><a href="https://github.com/opencontainers/runc/commit/ae28db14244c87ab1e26db09a8ad6e5b2882ccc7"><code>ae28db1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3436">#3436</a> from kolyshkin/1.1-add-centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/036cc348994b7fa573380401644a6faac9e102e7"><code>036cc34</code></a> CI/cirrus: add centos-stream-9</li>
<li><a href="https://github.com/opencontainers/runc/commit/c65363285b3eee6e2e3a7b356f8967ae17263d41"><code>c653632</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/opencontainers/runc/issues/3438">#3438</a> from kolyshkin/1.1-fix-badges</li>
<li><a href="https://github.com/opencontainers/runc/commit/db953158e14658c62ad6cda9ac087bdb1b1e3e8c"><code>db95315</code></a> README.md: add cirrus-ci badge</li>
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.0.0-rc9...v1.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.0.0-rc9&new-version=1.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 23:57:48 +0000 UTC
    </div>
</div>

