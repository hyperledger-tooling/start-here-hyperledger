---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    [WIP] fix offset in blockstore
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
        Created At 2023-02-20 11:46:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/499" class=".btn">#499</a>
            </td>
            <td>
                <b>
                    Seek back to write location after read from chunk file
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
        Created At 2023-02-16 09:58:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    Bump github.com/prometheus/client_golang from 1.0.0 to 1.11.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/prometheus/client_golang](https://github.com/prometheus/client_golang) from 1.0.0 to 1.11.1.
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
<h2>v1.11.0 / 2021-06-07</h2>
<ul>
<li>[CHANGE] Add new collectors package. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[CHANGE] <code>prometheus.NewExpvarCollector</code> is deprecated, use <code>collectors.NewExpvarCollector</code> instead. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[CHANGE] <code>prometheus.NewGoCollector</code> is deprecated, use <code>collectors.NewGoCollector</code> instead. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[CHANGE] <code>prometheus.NewBuildInfoCollector</code> is deprecated, use <code>collectors.NewBuildInfoCollector</code> instead. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[FEATURE] Add new collector for database/sql#DBStats. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/866">#866</a></li>
<li>[FEATURE] API client: Add exemplars API support. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/861">#861</a></li>
<li>[ENHANCEMENT] API client: Add newer fields to Rules API. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/855">#855</a></li>
<li>[ENHANCEMENT] API client: Add missing fields to Targets API. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/856">#856</a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/846">prometheus/client_golang#846</a></li>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/849">prometheus/client_golang#849</a></li>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/853">prometheus/client_golang#853</a></li>
<li>Add newer fields to Rules API by <a href="https://github.com/gouthamve"><code>@​gouthamve</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/855">prometheus/client_golang#855</a></li>
<li>Add missing fields to targets API by <a href="https://github.com/yeya24"><code>@​yeya24</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/856">prometheus/client_golang#856</a></li>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/857">prometheus/client_golang#857</a></li>
<li>Add exemplars API support by <a href="https://github.com/yeya24"><code>@​yeya24</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/861">prometheus/client_golang#861</a></li>
<li>Improve description of MaxAge in summary docs by <a href="https://github.com/Dean-Coakley"><code>@​Dean-Coakley</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/864">prometheus/client_golang#864</a></li>
<li>Add new collectors package by <a href="https://github.com/johejo"><code>@​johejo</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/862">prometheus/client_golang#862</a></li>
<li>Add collector for database/sql#DBStats by <a href="https://github.com/johejo"><code>@​johejo</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/866">prometheus/client_golang#866</a></li>
<li>Make dbStatsCollector more DRY by <a href="https://github.com/beorn7"><code>@​beorn7</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/867">prometheus/client_golang#867</a></li>
<li>Change maintainers from <a href="https://github.com/beorn7"><code>@​beorn7</code></a> to @bwplotka/<a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> by <a href="https://github.com/beorn7"><code>@​beorn7</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/873">prometheus/client_golang#873</a></li>
<li>Document implications of negative observations by <a href="https://github.com/beorn7"><code>@​beorn7</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/871">prometheus/client_golang#871</a></li>
<li>Update Go modules by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/875">prometheus/client_golang#875</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/gouthamve"><code>@​gouthamve</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/855">prometheus/client_golang#855</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/prometheus/client_golang/compare/v1.10.0...v1.11.0">https://github.com/prometheus/client_golang/compare/v1.10.0...v1.11.0</a></p>
<h2>1.10.0 / 2021-03-18</h2>
<ul>
<li>[CHANGE] Minimum required Go version is now 1.13.</li>
<li>[CHANGE] API client: Add matchers to <code>LabelNames</code> and <code>LabesValues</code>. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/828">#828</a></li>
<li>[FEATURE] API client: Add buildinfo call. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/841">#841</a></li>
<li>[BUGFIX] Fix build on riscv64. <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/833">#833</a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Add SECURITY.md by <a href="https://github.com/roidelapluie"><code>@​roidelapluie</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/831">prometheus/client_golang#831</a></li>
<li>Bump prometheus/procfs to 0.3.0 to fix building on riscv64 by <a href="https://github.com/zhsj"><code>@​zhsj</code></a> in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/833">prometheus/client_golang#833</a></li>
<li>Fix typo in comments in <a href="https://github-redirect.dependabot.com/prometheus/client_golang/pull/835">prometheus/client_golang#835</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li><a href="https://github.com/prometheus/client_golang/commit/8184d76b3b0bd3b01ed903690431ccb6826bf3e0"><code>8184d76</code></a> Cut v1.11.0 (<a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/877">#877</a>)</li>
<li><a href="https://github.com/prometheus/client_golang/commit/253906201bda760621fa671fa1541a4ac3df29bd"><code>2539062</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/875">#875</a> from prometheus/superq/update_mods</li>
<li><a href="https://github.com/prometheus/client_golang/commit/68cd1e9262e2fe03a79c9a8bab6737f04995e8a5"><code>68cd1e9</code></a> Update Go modules</li>
<li><a href="https://github.com/prometheus/client_golang/commit/f22935db759faadc48285fee37718436d5b9cb67"><code>f22935d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/871">#871</a> from prometheus/beorn7/doc</li>
<li><a href="https://github.com/prometheus/client_golang/commit/11aba26a91c3ea0581eef96f8ec9fc5cdce204f9"><code>11aba26</code></a> Change maintainers from <a href="https://github.com/beorn7"><code>@​beorn7</code></a> to @bwplotka/<a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> (<a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/873">#873</a>)</li>
<li><a href="https://github.com/prometheus/client_golang/commit/f34145a85eaff9d42ff629a2975e8118ab41773c"><code>f34145a</code></a> Document implications of negative observations</li>
<li><a href="https://github.com/prometheus/client_golang/commit/a7515ca7c9c6388a5ab84ea336faef795bbf866f"><code>a7515ca</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/867">#867</a> from prometheus/beorn7/collectors</li>
<li><a href="https://github.com/prometheus/client_golang/commit/81a9556c8b4ffac3dd75f7aedf720b3ae73e1276"><code>81a9556</code></a> Make dbStatsCollector more DRY</li>
<li><a href="https://github.com/prometheus/client_golang/commit/a66da1df4a7e12cb9f84cf5ae3c7adec4539ed27"><code>a66da1d</code></a> Add collector for database/sql#DBStats (<a href="https://github-redirect.dependabot.com/prometheus/client_golang/issues/866">#866</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/prometheus/client_golang/compare/v1.0.0...v1.11.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/prometheus/client_golang&package-manager=go_modules&previous-version=1.0.0&new-version=1.11.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/orion-server/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 02:14:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    Change docker image to Ubuntu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">security</span>
            </td>
            <td>
                Switching to Ubuntu docker image increases the image size from ~30MB to ~140MB.

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 13:40:24 +0000 UTC
    </div>
</div>

