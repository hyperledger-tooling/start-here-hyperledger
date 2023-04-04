---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/524" class=".btn">#524</a>
            </td>
            <td>
                <b>
                    Bump redis from 3.4.1 to 4.4.4 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [redis](https://github.com/redis/redis-py) from 3.4.1 to 4.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/releases">redis's releases</a>.</em></p>
<blockquote>
<h2>4.4.4</h2>
<h1>Changes</h1>
<p>Upgrade urgency: SECURITY, contains fixes to security issues.</p>
<ul>
<li>(CVE-2023-28859) - Cancelling an async future does not, properly trigger, leading to a potential data leak in specific cases.</li>
<li>(CVE-2023-28858) - Cancelling an async future does not, properly trigger, leading to a potential data leak in specific cases.</li>
</ul>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fixing cancelled async futures (<a href="https://redirect.github.com/redis/redis-py/issues/2671">#2671</a> )</li>
</ul>
<h2>4.4.3</h2>
<h1>Changes</h1>
<p>Update urgency: HIGH: There is a critical bug that may affect a subset of users. Upgrade!</p>
<h2>🐛 Bug Fixes</h2>
<ul>
<li><a href="https://cwe.mitre.org/data/definitions/404.html">CWE-404</a> AsyncIO Race Condition Fix (<a href="https://redirect.github.com/redis/redis-py/issues/2624">#2624</a>, <a href="https://redirect.github.com/redis/redis-py/issues/2579">#2579</a>)</li>
</ul>
<h2>4.4.2</h2>
<h1>Changes</h1>
<p>Note: this release include <a href="https://redirect.github.com/redis/redis-py/issues/2548">#2548</a> and it is suggested that users upgrade immediately.</p>
<h2>🧪 Experimental Features</h2>
<ul>
<li>Add support for BF.CARD (<a href="https://redirect.github.com/redis/redis-py/issues/2545">#2545</a>)</li>
</ul>
<h2>🚀 New Features</h2>
<ul>
<li>Add support for custom connection pool class in NodesManager (<a href="https://redirect.github.com/redis/redis-py/issues/2547">#2547</a>)</li>
</ul>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Allow replica to master promotion in nodes_cache (<a href="https://redirect.github.com/redis/redis-py/issues/2549">#2549</a>)</li>
<li>Security Fix: Updating graph parser for potential injection cases (<a href="https://redirect.github.com/redis/redis-py/issues/2548">#2548</a>)</li>
</ul>
<h2>Contributors</h2>
<p>We'd like to thank all the contributors who worked on this release!</p>
<p><a href="https://github.com/Threated"><code>@​Threated</code></a>, <a href="https://github.com/dvora-h"><code>@​dvora-h</code></a>, <a href="https://github.com/shacharPash"><code>@​shacharPash</code></a> and <a href="https://github.com/zakaf"><code>@​zakaf</code></a></p>
<h2>4.4.1</h2>
<h1>Changes</h1>
<h2>🚀 New Features</h2>
<ul>
<li>Add dialect to <code>FT.AGGREGATE</code> (<a href="https://redirect.github.com/redis/redis-py/issues/2537">#2537</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/blob/master/CHANGES">redis's changelog</a>.</em></p>
<blockquote>
<pre><code>* Allow data to drain from async PythonParser when reading during a disconnect()
* Use asyncio.timeout() instead of async_timeout.timeout() for python &gt;= 3.11 ([#2602](https://github.com/redis/redis-py/issues/2602))
* Add test and fix async HiredisParser when reading during a disconnect() ([#2349](https://github.com/redis/redis-py/issues/2349))
* Use hiredis-py pack_command if available.
* Support `.unlink()` in ClusterPipeline
* Simplify synchronous SocketBuffer state management
* Fix string cleanse in Redis Graph
* Make PythonParser resumable in case of error ([#2510](https://github.com/redis/redis-py/issues/2510))
* Add `timeout=None` in `SentinelConnectionManager.read_response`
* Documentation fix: password protected socket connection ([#2374](https://github.com/redis/redis-py/issues/2374))
* Allow `timeout=None` in `PubSub.get_message()` to wait forever
* add `nowait` flag to `asyncio.Connection.disconnect()`
* Update README.md links
* Fix timezone handling for datetime to unixtime conversions
* Fix start_id type for XAUTOCLAIM
* Remove verbose logging from cluster.py
* Add retry mechanism to async version of Connection
* Compare commands case-insensitively in the asyncio command parser
* Allow negative `retries` for `Retry` class to retry forever
* Add `items` parameter to `hset` signature
* Create codeql-analysis.yml ([#1988](https://github.com/redis/redis-py/issues/1988)). Thanks @chayim
* Add limited support for Lua scripting with RedisCluster
* Implement `.lock()` method on RedisCluster
* Fix cursor returned by SCAN for RedisCluster &amp; change default target to PRIMARIES
* Fix scan_iter for RedisCluster
* Remove verbose logging when initializing ClusterPubSub, ClusterPipeline or RedisCluster
* Fix broken connection writer lock-up for asyncio ([#2065](https://github.com/redis/redis-py/issues/2065))
* Fix auth bug when provided with no username ([#2086](https://github.com/redis/redis-py/issues/2086))
* Fix missing ClusterPipeline._lock ([#2189](https://github.com/redis/redis-py/issues/2189))
* Added dynaminc_startup_nodes configuration to RedisCluster
* Fix reusing the old nodes' connections when cluster topology refresh is being done
* Fix RedisCluster to immediately raise AuthenticationError without a retry
* ClusterPipeline Doesn't Handle ConnectionError for Dead Hosts ([#2225](https://github.com/redis/redis-py/issues/2225))
* Remove compatibility code for old versions of Hiredis, drop Packaging dependency
* The `deprecated` library is no longer a dependency
* Failover handling improvements for RedisCluster and Async RedisCluster ([#2377](https://github.com/redis/redis-py/issues/2377))
* Fixed &quot;cannot pickle '_thread.lock' object&quot; bug ([#2354](https://github.com/redis/redis-py/issues/2354), [#2297](https://github.com/redis/redis-py/issues/2297))
* Added CredentialsProvider class to support password rotation
* Enable Lock for asyncio cluster mode
* Fix Sentinel.execute_command doesn't execute across the entire sentinel cluster bug ([#2458](https://github.com/redis/redis-py/issues/2458))
* Added a replacement for the default cluster node in the event of failure ([#2463](https://github.com/redis/redis-py/issues/2463))
* Fix for Unhandled exception related to self.host with unix socket ([#2496](https://github.com/redis/redis-py/issues/2496))
</code></pre>
<ul>
<li>4.1.3 (Feb 8, 2022)
<ul>
<li>Fix flushdb and flushall (<a href="https://redirect.github.com/redis/redis-py/issues/1926">#1926</a>)</li>
<li>Add redis5 and redis4 dockers (<a href="https://redirect.github.com/redis/redis-py/issues/1871">#1871</a>)</li>
<li>Change json.clear test multi to be up to date with redisjson (<a href="https://redirect.github.com/redis/redis-py/issues/1922">#1922</a>)</li>
<li>Fixing volume for unstable_cluster docker (<a href="https://redirect.github.com/redis/redis-py/issues/1914">#1914</a>)</li>
<li>Update changes file with changes since 4.0.0-beta2 (<a href="https://redirect.github.com/redis/redis-py/issues/1915">#1915</a>)</li>
</ul>
</li>
<li>4.1.2 (Jan 27, 2022)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/redis/redis-py/commit/49d9cb751c7c30546fc86d11f8168d7aa007edae"><code>49d9cb7</code></a> Version 4.4.4 (<a href="https://redirect.github.com/redis/redis-py/issues/2671">#2671</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/b3c89acd0ffe8303649ad8207bc911b1d6a033eb"><code>b3c89ac</code></a> AsyncIO Race Condition Fix (<a href="https://redirect.github.com/redis/redis-py/issues/2640">#2640</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/8592cacf9e5069f8f6d392a2bc02aeade87c9d69"><code>8592cac</code></a> version 4.4.2 (<a href="https://redirect.github.com/redis/redis-py/issues/2550">#2550</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/be84b930266932bc81fd5390e6963621ef0b97da"><code>be84b93</code></a> Add support to BF.CARD (<a href="https://redirect.github.com/redis/redis-py/issues/2545">#2545</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/7dd73a306add608807c372a98d833b7cb3394681"><code>7dd73a3</code></a> add support for custom connection pool class in NodesManager (<a href="https://redirect.github.com/redis/redis-py/issues/2547">#2547</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/bae6385c1b0097a1d85c7825604170477d193481"><code>bae6385</code></a> allow replica to master promotion in nodes_cache (<a href="https://redirect.github.com/redis/redis-py/issues/2549">#2549</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/4a825bc76b668951923c57aaff1020c3892f8de2"><code>4a825bc</code></a> String cleanse (<a href="https://redirect.github.com/redis/redis-py/issues/2548">#2548</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/f46d7f3ef7ce64f90acd4a3dcc14375ab9ae9c9d"><code>f46d7f3</code></a> Version 4.4.1 (<a href="https://redirect.github.com/redis/redis-py/issues/2544">#2544</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/c7600b4c7e558d3c05485f76cfcdd3e807c6b13e"><code>c7600b4</code></a> add type checking for graph <strong>eq</strong> (<a href="https://redirect.github.com/redis/redis-py/issues/2531">#2531</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/decd1f6ae5434b111c5b125263549d8743275e51"><code>decd1f6</code></a> ValueError must be AttributeError in <strong>init</strong>.py (<a href="https://redirect.github.com/redis/redis-py/issues/2542">#2542</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/redis/redis-py/compare/3.4.1...v4.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=redis&package-manager=pip&previous-version=3.4.1&new-version=4.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 14:51:33 +0000 UTC
    </div>
</div>

