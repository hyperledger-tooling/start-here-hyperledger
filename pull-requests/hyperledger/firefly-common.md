---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    CRUD utility for building microservices on the DB layer, and BigInt query fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There's a lot of boilerplate still needed when building a microservice on top of `firefly-common` DB utilities.

This hasn't been addressed in FireFly Core, because so few of the collection are completely "standard", they need all kinds of special tweaks on a per collection basis. So the code is justified.

But in microservices like EVMConnect trying to pick up the framework, it would be great to just define the metadata of the collection and get the basic set of functions for free.

... so here's what's needed after this change (for SQL based DBs at least) - much better I hope:
https://github.com/hyperledger/firefly-common/blob/0d471d9d062ec110bd6426472a524e4ab2b8d440/pkg/dbsql/crud_test.go#L62-L96

I also found there was no `BigIntField` definition in the query support of `ffapi` - which seemed like a bad omission, particularly las we store the DB data in hex. A follow-on change would be needed in FF Core to pick that up for all `FFBigInt` fields

> In draft as I have a little remaining test coverage to close out on
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 17:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Make common version library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've got this copied and pasted around. Felt like it should be a common utility.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 09:08:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Add text/plain content type support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Useful for APIs that relies on envelope based authentication, for instance in many decentralized identity frameworks, which may become part of FireFly in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 16:15:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    improvements for metrics 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Here is the list of improvements:
- Added go and cpu metrics as default
- added more documentation on how the terms used in function names are used in a real metrics string
- added a way to add a component label for all metrics so that we can separate the same metrics (e.g. HTTP requests) of different components
- allowed more chars to be used in the name string
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 14:09:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    adding common cache utility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a common cache manager to manage different cache instances used in a component.

Also resolves #54 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 10:53:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Bump github.com/prometheus/client_golang from 1.11.0 to 1.11.1
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
<li>[SECURITY FIX] promhttp: Check validity of method and code label values <a href="https://redirect.github.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a> (Addressed <a href="https://github.com/prometheus/client_golang/security/advisories/GHSA-cg3q-j54f-5p7p"><code>CVE-2022-21698</code></a>)</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>promhttp: Check validity of method and code label values by <a href="https://github.com/bwplotka"><code>@​bwplotka</code></a> and <a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> in  <a href="https://redirect.github.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a></li>
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
<li>[FEATURE] Add Support for Native Histograms. <a href="https://redirect.github.com/prometheus/client_golang/issues/1150">#1150</a></li>
<li>[CHANGE] Extend <code>prometheus.Registry</code> to implement <code>prometheus.Collector</code> interface. <a href="https://redirect.github.com/prometheus/client_golang/issues/1103">#1103</a></li>
</ul>
<h2>1.13.1 / 2022-11-01</h2>
<ul>
<li>[BUGFIX] Fix race condition with Exemplar in Counter. <a href="https://redirect.github.com/prometheus/client_golang/issues/1146">#1146</a></li>
<li>[BUGFIX] Fix <code>CumulativeCount</code> value of <code>+Inf</code> bucket created from exemplar. <a href="https://redirect.github.com/prometheus/client_golang/issues/1148">#1148</a></li>
<li>[BUGFIX] Fix double-counting bug in <code>promhttp.InstrumentRoundTripperCounter</code>. <a href="https://redirect.github.com/prometheus/client_golang/issues/1118">#1118</a></li>
</ul>
<h2>1.13.0 / 2022-08-05</h2>
<ul>
<li>[CHANGE] Minimum required Go version is now 1.17 (we also test client_golang against new 1.19 version).</li>
<li>[ENHANCEMENT] Added <code>prometheus.TransactionalGatherer</code> interface for <code>promhttp.Handler</code> use which allows using low allocation update techniques for custom collectors. <a href="https://redirect.github.com/prometheus/client_golang/issues/989">#989</a></li>
<li>[ENHANCEMENT] Added exemplar support to <code>prometheus.NewConstHistogram</code>. See <a href="https://github.com/prometheus/client_golang/blob/main/prometheus/examples_test.go#L602"><code>ExampleNewConstHistogram_WithExemplar</code></a> example on how to use it. <a href="https://redirect.github.com/prometheus/client_golang/issues/986">#986</a></li>
<li>[ENHANCEMENT] <code>prometheus/push.Pusher</code> has now context aware methods that pass context to HTTP request. <a href="https://redirect.github.com/prometheus/client_golang/issues/1028">#1028</a></li>
<li>[ENHANCEMENT] <code>prometheus/push.Pusher</code> has now <code>Error</code> method that retrieve last error. <a href="https://redirect.github.com/prometheus/client_golang/issues/1075">#1075</a></li>
<li>[ENHANCEMENT] <code>testutil.GatherAndCompare</code> provides now readable diff on failed comparisons. <a href="https://redirect.github.com/prometheus/client_golang/issues/998">#998</a></li>
<li>[ENHANCEMENT] Query API now supports timeouts. <a href="https://redirect.github.com/prometheus/client_golang/issues/1014">#1014</a></li>
<li>[ENHANCEMENT] New <code>MetricVec</code> method <code>DeletePartialMatch(labels Labels)</code> for deleting all metrics that match provided labels. <a href="https://redirect.github.com/prometheus/client_golang/issues/1013">#1013</a></li>
<li>[ENHANCEMENT] <code>api.Config</code> now accepts passing custom <code>*http.Client</code>. <a href="https://redirect.github.com/prometheus/client_golang/issues/1025">#1025</a></li>
<li>[BUGFIX] Raise exemplar labels limit from 64 to 128 bytes as specified in OpenMetrics spec. <a href="https://redirect.github.com/prometheus/client_golang/issues/1091">#1091</a></li>
<li>[BUGFIX] Allow adding exemplar to +Inf bucket to const histograms. <a href="https://redirect.github.com/prometheus/client_golang/issues/1094">#1094</a></li>
<li>[ENHANCEMENT] Most <code>promhttp.Instrument*</code> middlewares now supports adding exemplars to metrics. This allows hooking those to your tracing middleware that retrieves trace ID and put it in exemplar if present. <a href="https://redirect.github.com/prometheus/client_golang/issues/1055">#1055</a></li>
<li>[ENHANCEMENT] Added <code>testutil.ScrapeAndCompare</code> method. <a href="https://redirect.github.com/prometheus/client_golang/issues/1043">#1043</a></li>
<li>[BUGFIX] Fixed <code>GopherJS</code> build support. <a href="https://redirect.github.com/prometheus/client_golang/issues/897">#897</a></li>
<li>[ENHANCEMENT] :warning: Added way to specify what <code>runtime/metrics</code>  <code>collectors.NewGoCollector</code> should use. See <a href="https://github.com/prometheus/client_golang/blob/main/prometheus/collectors/go_collector_latest_test.go#L263"><code>ExampleGoCollector_WithAdvancedGoMetrics</code></a>. <a href="https://redirect.github.com/prometheus/client_golang/issues/1102">#1102</a></li>
</ul>
<h2>1.12.2 / 2022-05-13</h2>
<ul>
<li>[CHANGE] Added <code>collectors.WithGoCollections</code> that allows to choose what collection of Go runtime metrics user wants: Equivalent of <a href="https://pkg.go.dev/runtime#MemStats"><code>MemStats</code> structure</a> configured using <code>GoRuntimeMemStatsCollection</code>, new based on dedicated <a href="https://pkg.go.dev/runtime/metrics">runtime/metrics</a> metrics represented by <code>GoRuntimeMetricsCollection</code> option, or both by specifying <code>GoRuntimeMemStatsCollection | GoRuntimeMetricsCollection</code> flag. <a href="https://redirect.github.com/prometheus/client_golang/issues/1031">#1031</a></li>
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
<li>[BUGFIX] Make the Go 1.17 collector concurrency-safe <a href="https://redirect.github.com/prometheus/client_golang/issues/969">#969</a>
<ul>
<li>Use simpler locking in the Go 1.17 collector <a href="https://redirect.github.com/prometheus/client_golang/issues/975">#975</a></li>
</ul>
</li>
<li>[BUGFIX] Reduce granularity of histogram buckets for Go 1.17 collector <a href="https://redirect.github.com/prometheus/client_golang/issues/974">#974</a></li>
<li>[ENHANCEMENT] API client: make HTTP reads more efficient <a href="https://redirect.github.com/prometheus/client_golang/issues/976">#976</a></li>
</ul>
<h2>1.12.0 / 2022-01-19</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prometheus/client_golang/commit/989baa30fe956631907493ccee1f8e7708660d96"><code>989baa3</code></a> promhttp: Check validity of method and code label values (<a href="https://redirect.github.com/prometheus/client_golang/issues/962">#962</a>) (<a href="https://redirect.github.com/prometheus/client_golang/issues/987">#987</a>)</li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-common/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 09:56:34 +0000 UTC
    </div>
</div>

