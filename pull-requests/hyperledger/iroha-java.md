---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Bump com.github.docker-java:docker-java from 3.3.0 to 3.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [com.github.docker-java:docker-java](https://github.com/docker-java/docker-java) from 3.3.0 to 3.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker-java/docker-java/releases">com.github.docker-java:docker-java's releases</a>.</em></p>
<blockquote>
<h2>3.4.0</h2>
<h2>Changes</h2>
<ul>
<li>Add -parameters option for compilation of project <a href="https://github.com/holgerstolzenberg"><code>@​holgerstolzenberg</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2317">#2317</a>)</li>
</ul>
<h2>📈 Enhancements</h2>
<ul>
<li>Enable protocol configuration of SSLContext <a href="https://github.com/tkrah"><code>@​tkrah</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2337">#2337</a>)</li>
<li>Add Network create attribute <a href="https://github.com/juanmolle"><code>@​juanmolle</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2344">#2344</a>)</li>
</ul>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Consider already existing images as successful pulls. <a href="https://github.com/n-g"><code>@​n-g</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2335">#2335</a>)</li>
</ul>
<h2>🧰 Maintenance</h2>
<ul>
<li>Update images <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2346">#2346</a>)</li>
</ul>
<h2>3.3.6</h2>
<h2>Changes</h2>
<ul>
<li>Test against Java 21 <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2304">#2304</a>)</li>
<li>Update actions/checkout and actions/setup-java version to v4 <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2309">#2309</a>)</li>
</ul>
<h2>📈 Enhancements</h2>
<ul>
<li>Add <code>Runtimes</code> to <code>Info</code> response <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2311">#2311</a>)</li>
</ul>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Remove exclusion and fix httpclient5 compatibility <a href="https://github.com/Sineaggi"><code>@​Sineaggi</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2294">#2294</a>)</li>
<li>If BuildImage fails but logs something about success, don't succeed <a href="https://github.com/niloc132"><code>@​niloc132</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2305">#2305</a>)</li>
</ul>
<h2>3.3.5</h2>
<h2>Changes</h2>
<ul>
<li>Ignore LogSwarmObjectIT#testLogsCmd <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2280">#2280</a>)</li>
</ul>
<h2>📈 Enhancements</h2>
<ul>
<li>Add missing states in ServiceUpdateState <a href="https://github.com/Nowheresly"><code>@​Nowheresly</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2292">#2292</a>)</li>
<li>Add StartInterval to health check since it will be supported by the 1.44 docker API <a href="https://github.com/henri-tremblay"><code>@​henri-tremblay</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2244">#2244</a>)</li>
</ul>
<h2>🧰 Maintenance</h2>
<ul>
<li>Enable japicmp in docker-java-api module <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2279">#2279</a>)</li>
</ul>
<h2>3.3.4</h2>
<h2>Changes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker-java/docker-java/commit/a1393bf2e1265ba1e6eca4240af55396852f8a7c"><code>a1393bf</code></a> Enable protocol configuration of SSLContext (<a href="https://redirect.github.com/docker-java/docker-java/issues/2337">#2337</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/f14cff90924f7aa5bf570ab49e6e91532ba8a362"><code>f14cff9</code></a> Add -parameters option for compilation of project (<a href="https://redirect.github.com/docker-java/docker-java/issues/2317">#2317</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/242c76ae01aea5c965ee5f1037ba84bafb84015c"><code>242c76a</code></a> Add Network create attribute (<a href="https://redirect.github.com/docker-java/docker-java/issues/2344">#2344</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/b28b0dc267bc3ab9feb5645957311e5fa42ce94e"><code>b28b0dc</code></a> Consider already existing images as successful pull (<a href="https://redirect.github.com/docker-java/docker-java/issues/2335">#2335</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/f146f9696db7b4d4180d95677a879f8597d34ed8"><code>f146f96</code></a> Update images (<a href="https://redirect.github.com/docker-java/docker-java/issues/2346">#2346</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/b29527510d9f7c16b30b138ae4a2f6703d88bb01"><code>b295275</code></a> Add <code>Runtimes</code> to <code>Info</code> response (<a href="https://redirect.github.com/docker-java/docker-java/issues/2311">#2311</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/4f6c5937983ff4ae7cc82bead44afe3afee4d0ed"><code>4f6c593</code></a> Test against Java 21 (<a href="https://redirect.github.com/docker-java/docker-java/issues/2304">#2304</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/3514b3ba9c6d938e2a0435ad8d84905cb1cdfed1"><code>3514b3b</code></a> Remove exclusion and fix httpclient5 compatibility (<a href="https://redirect.github.com/docker-java/docker-java/issues/2294">#2294</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/4d8c436d6cbe312be22b157c3ebdb6eb973140ae"><code>4d8c436</code></a> If BuildImage fails but logs something about success, don't succeed (<a href="https://redirect.github.com/docker-java/docker-java/issues/2305">#2305</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/129f7868a0463bad09f74dcfb26391b224be6784"><code>129f786</code></a> Update actions/checkout and actions/setup-java version to v4 (<a href="https://redirect.github.com/docker-java/docker-java/issues/2309">#2309</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/docker-java/docker-java/compare/3.3.0...3.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.github.docker-java:docker-java&package-manager=gradle&previous-version=3.3.0&new-version=3.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 05:40:14 +0000 UTC
    </div>
</div>

