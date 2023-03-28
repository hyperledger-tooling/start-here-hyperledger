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
                PR <a href="https://github.com/hyperledger/cello/pull/523" class=".btn">#523</a>
            </td>
            <td>
                <b>
                    Bump redis from 3.4.1 to 4.5.3 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [redis](https://github.com/redis/redis-py) from 3.4.1 to 4.5.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/releases">redis's releases</a>.</em></p>
<blockquote>
<h2>4.5.3</h2>
<h1>Changes</h1>
<p>Update urgency: HIGH: There is a critical bug that may affect a subset of users. Upgrade!</p>
<h2>🐛 Bug Fixes</h2>
<ul>
<li><a href="https://cwe.mitre.org/data/definitions/404.html">CWE-404</a> AsyncIO Race Condition Fix (<a href="https://redirect.github.com/redis/redis-py/issues/2624">#2624</a>, <a href="https://redirect.github.com/redis/redis-py/issues/2579">#2579</a>)</li>
</ul>
<h2>4.5.2</h2>
<h1>Changes</h1>
<h2>🚀 New Features</h2>
<ul>
<li>Introduce AbstractConnection so that UnixDomainSocketConnection can call super().<strong>init</strong> (<a href="https://redirect.github.com/redis/redis-py/issues/2588">#2588</a>)</li>
<li>Added queue_class to REDIS_ALLOWED_KEYS (<a href="https://redirect.github.com/redis/redis-py/issues/2577">#2577</a>)</li>
<li>Made search document subscriptable (<a href="https://redirect.github.com/redis/redis-py/issues/2615">#2615</a>)</li>
<li>Sped up the protocol parsing (<a href="https://redirect.github.com/redis/redis-py/issues/2596">#2596</a>)</li>
</ul>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fix behaviour of async PythonParser to match RedisParser as for issue <a href="https://redirect.github.com/redis/redis-py/issues/2349">#2349</a> (<a href="https://redirect.github.com/redis/redis-py/issues/2582">#2582</a>)</li>
<li>Replace async_timeout by asyncio.timeout (<a href="https://redirect.github.com/redis/redis-py/issues/2602">#2602</a>)</li>
<li>Update json().arrindex() default values (<a href="https://redirect.github.com/redis/redis-py/issues/2611">#2611</a>)</li>
</ul>
<h2>🧰 Maintenance</h2>
<ul>
<li>Coverage for pypy-3.9 (<a href="https://redirect.github.com/redis/redis-py/issues/2608">#2608</a>)</li>
<li>Developer Experience: Adding redis version compatibility details to the README (<a href="https://redirect.github.com/redis/redis-py/issues/2621">#2621</a>)</li>
<li>Remove redundant assignment to RedisCluster.nodes_manager. (<a href="https://redirect.github.com/redis/redis-py/issues/2620">#2620</a>)</li>
<li>Developer Experience: [types] update return type of smismember to list[int] (<a href="https://redirect.github.com/redis/redis-py/issues/2617">#2617</a>)</li>
<li>Developer Experience: [docs] ConnectionPool SSL example (<a href="https://redirect.github.com/redis/redis-py/issues/2605">#2605</a>)</li>
<li>Developer Experience: Fixed CredentialsProvider examples (<a href="https://redirect.github.com/redis/redis-py/issues/2587">#2587</a>)</li>
<li>Developer Experience: Update README to make pip install copy-pastable on zsh (<a href="https://redirect.github.com/redis/redis-py/issues/2584">#2584</a>)</li>
<li>Developer Experience: Fix for <code>lpop</code> and <code>rpop</code> return typing (<a href="https://redirect.github.com/redis/redis-py/issues/2590">#2590</a>)</li>
</ul>
<h2>Contributors</h2>
<p>We'd like to thank all the contributors who worked on this release!</p>
<p><a href="https://github.com/CrimsonGlory"><code>@​CrimsonGlory</code></a>, <a href="https://github.com/Galtozzy"><code>@​Galtozzy</code></a>, <a href="https://github.com/aksinha334"><code>@​aksinha334</code></a>, <a href="https://github.com/barshaul"><code>@​barshaul</code></a>, <a href="https://github.com/chayim"><code>@​chayim</code></a>, <a href="https://github.com/davemcphee"><code>@​davemcphee</code></a>, <a href="https://github.com/dvora-h"><code>@​dvora-h</code></a>, <a href="https://github.com/kristjanvalur"><code>@​kristjanvalur</code></a>, <a href="https://github.com/ryin1"><code>@​ryin1</code></a>, <a href="https://github.com/sileht"><code>@​sileht</code></a>, <a href="https://github.com/thebarbershop"><code>@​thebarbershop</code></a>, <a href="https://github.com/uglide"><code>@​uglide</code></a>, <a href="https://github.com/woutdenolf"><code>@​woutdenolf</code></a> and <a href="https://github.com/zakaf"><code>@​zakaf</code></a></p>
<h2>4.5.1</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fix <a href="https://redirect.github.com/redis/redis-py/issues/2581">#2581</a> <code>UnixDomainSocketConnection</code> object has no attribute <code>_command_packer</code> (<a href="https://redirect.github.com/redis/redis-py/issues/2583">#2583</a>)</li>
</ul>
<h2>Contributors</h2>
<p>We'd like to thank all the contributors who worked on this release!</p>
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
<li><a href="https://github.com/redis/redis-py/commit/66a4d6b2a493dd3a20cc299ab5fef3c14baad965"><code>66a4d6b</code></a> AsyncIO Race Condition Fix (<a href="https://redirect.github.com/redis/redis-py/issues/2641">#2641</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/318b114f4da9846a2a7c150e1fb702e9bebd9fdf"><code>318b114</code></a> Version 4.5.2 (<a href="https://redirect.github.com/redis/redis-py/issues/2627">#2627</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/1b2f408259405d412d7530291902f9e0c8bd34b3"><code>1b2f408</code></a> Fix behaviour of async PythonParser to match RedisParser as for issue <a href="https://redirect.github.com/redis/redis-py/issues/2349">#2349</a> (...</li>
<li><a href="https://github.com/redis/redis-py/commit/7d474f90453c7b90bd06c94e0250b618120a599d"><code>7d474f9</code></a> introduce AbstractConnection so that UnixDomainSocketConnection can call supe...</li>
<li><a href="https://github.com/redis/redis-py/commit/c87172347584301f453c601c483126e4800257b7"><code>c871723</code></a> pypy-3.9 CI (<a href="https://redirect.github.com/redis/redis-py/issues/2608">#2608</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/d63313bf6080acaf18d61e072c78303adc0d4166"><code>d63313b</code></a> add queue_class to REDIS_ALLOWED_KEYS (<a href="https://redirect.github.com/redis/redis-py/issues/2577">#2577</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/c61eeb2e3b5dff1f01eb1e665f424c7e75354f56"><code>c61eeb2</code></a> Adding supported redis/library details (<a href="https://redirect.github.com/redis/redis-py/issues/2621">#2621</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/25e85e51e57b7aae9eb8fc77cfb0a45a07a501a7"><code>25e85e5</code></a> fix: replace async_timeout by asyncio.timeout (<a href="https://redirect.github.com/redis/redis-py/issues/2602">#2602</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/91ab12a0f1bdf0e433131e1a51578e9fa2f89718"><code>91ab12a</code></a> Remove redundant assignment. (<a href="https://redirect.github.com/redis/redis-py/issues/2620">#2620</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/8bfd492240fd33489a86cd3d353e3ece1fc94c10"><code>8bfd492</code></a> Making search document subscriptable (<a href="https://redirect.github.com/redis/redis-py/issues/2615">#2615</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/redis/redis-py/compare/3.4.1...v4.5.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=redis&package-manager=pip&previous-version=3.4.1&new-version=4.5.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-03-27 21:56:49 +0000 UTC
    </div>
</div>

