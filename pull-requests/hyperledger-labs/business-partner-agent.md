---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/867" class=".btn">#867</a>
            </td>
            <td>
                <b>
                    Bump dot-object and vue-cli-plugin-i18n in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [dot-object](https://github.com/rhalff/dot-object) to 2.1.4 and updates ancestor dependency [vue-cli-plugin-i18n](https://github.com/intlify/vue-cli-plugin-i18n). These dependencies need to be updated together.

Updates `dot-object` from 1.9.0 to 2.1.4
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rhalff/dot-object/blob/master/CHANGELOG.md">dot-object's changelog</a>.</em></p>
<blockquote>
<h2>2020-09-10 Version 2.1.4</h2>
<ul>
<li>[<a href="https://github.com/rhalff/dot-object/commit/94b9eb8a2d"><code>94b9eb8a2d</code></a>] - Fix parsing of array paths for non standard separators (Fixed by boidolr <a href="https://redirect.github.com/rhalff/dot-object/issues/58">#58</a>)</li>
</ul>
<h2>2020-02-16 Version 2.1.3</h2>
<ul>
<li>fix possible pollution of prototype for paths containing <strong>proto</strong></li>
</ul>
<h2>2019-11-02 Version 2.1.1</h2>
<ul>
<li>fix undefined key with root level array.</li>
</ul>
<h2>2019-11-02 Version 2.1.1</h2>
<ul>
<li>Wrong array conversion when brackets are used (Reported by vladshcherbin <a href="https://redirect.github.com/rhalff/dot-object/issues/27">#27</a>)</li>
</ul>
<h2>2019-11-02 Version 2.1.0</h2>
<ul>
<li>fix delete function not being wrapped. (Reported by murphyke <a href="https://redirect.github.com/rhalff/dot-object/issues/40">#40</a>)</li>
</ul>
<h2>2019-11-02 Version 2.0.0</h2>
<ul>
<li>[<a href="https://github.com/rhalff/dot-object/commit/2cb41bbd1b"><code>2cb41bbd1b</code></a>] - Add useBrackets option for the .dot() method (by z1m1n <a href="https://redirect.github.com/rhalff/dot-object/issues/42">#42</a>)</li>
<li>dot() now writes brackets by default (possibly breaking change).
Use Dot.useBrackets = false to keep the old behavior</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rhalff/dot-object/commit/87fd0d9d6d5596b3369ee1918e3f75041d4b334c"><code>87fd0d9</code></a> Release v2.1.4.</li>
<li><a href="https://github.com/rhalff/dot-object/commit/437c54bcb6bbf4807d65d0cd532f85d95f468870"><code>437c54b</code></a> prepare release</li>
<li><a href="https://github.com/rhalff/dot-object/commit/2f78b82bbbbd6978386b083d02faef77f9d436d9"><code>2f78b82</code></a> Merge pull request <a href="https://redirect.github.com/rhalff/dot-object/issues/58">#58</a> from boidolr/master</li>
<li><a href="https://github.com/rhalff/dot-object/commit/94b9eb8a2dc2f46f59c8a861bc826fb3c7a3a320"><code>94b9eb8</code></a> Fix parsing of array paths for non standard separators</li>
<li><a href="https://github.com/rhalff/dot-object/commit/3dcb2defecd643b64a1f24e838468a1128e904bd"><code>3dcb2de</code></a> Merge pull request <a href="https://redirect.github.com/rhalff/dot-object/issues/52">#52</a> from murilobd/add-keepArray-to-doc</li>
<li><a href="https://github.com/rhalff/dot-object/commit/2262089a7022d98dd3624d90be83e44d03ba14fa"><code>2262089</code></a> Update README.md</li>
<li><a href="https://github.com/rhalff/dot-object/commit/67142e73c0f9fdc0c57f561d3f8d7cfb0cdcf256"><code>67142e7</code></a> Merge branch 'release/v2.1.3'</li>
<li><a href="https://github.com/rhalff/dot-object/commit/c4a4dd5682b266192369f1a09c3426bb3586144b"><code>c4a4dd5</code></a> prepare v2.1.3</li>
<li><a href="https://github.com/rhalff/dot-object/commit/f76cff5fe6d01d30ce110d8f454db2e5bd28a7de"><code>f76cff5</code></a> guard for possible prototype polution</li>
<li><a href="https://github.com/rhalff/dot-object/commit/ee628c20e7de0c1d84d67ab9cf81c9e5fa5fa1b7"><code>ee628c2</code></a> Merge tag 'v2.1.2' into develop</li>
<li>Additional commits viewable in <a href="https://github.com/rhalff/dot-object/compare/v1.9.0...v2.1.4">compare view</a></li>
</ul>
</details>
<br />

Updates `vue-cli-plugin-i18n` from 2.3.1 to 2.3.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/intlify/vue-cli-plugin-i18n/releases">vue-cli-plugin-i18n's releases</a>.</em></p>
<blockquote>
<h2>v2.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>build(deps): bump url-parse from 1.5.1 to 1.5.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/248">intlify/vue-cli-plugin-i18n#248</a></li>
<li>fix a typo by <a href="https://github.com/bildeneins"><code>@​bildeneins</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/250">intlify/vue-cli-plugin-i18n#250</a></li>
<li>Fixing typos by <a href="https://github.com/deining"><code>@​deining</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/253">intlify/vue-cli-plugin-i18n#253</a></li>
<li>build(deps): bump ajv from 6.12.2 to 6.12.6 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/256">intlify/vue-cli-plugin-i18n#256</a></li>
<li>build(deps): bump follow-redirects from 1.13.0 to 1.14.7 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/255">intlify/vue-cli-plugin-i18n#255</a></li>
<li>build(deps): bump ajv from 6.12.2 to 6.12.6 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/257">intlify/vue-cli-plugin-i18n#257</a></li>
<li>build(deps): bump node-fetch from 2.6.1 to 2.6.7 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/258">intlify/vue-cli-plugin-i18n#258</a></li>
<li>build(deps): bump trim-off-newlines from 1.0.1 to 1.0.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/259">intlify/vue-cli-plugin-i18n#259</a></li>
<li>build(deps): bump node-fetch from 2.6.1 to 2.6.7 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/260">intlify/vue-cli-plugin-i18n#260</a></li>
<li>build(deps): bump ws from 5.2.2 to 5.2.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/261">intlify/vue-cli-plugin-i18n#261</a></li>
<li>build(deps): bump follow-redirects from 1.14.7 to 1.14.8 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/263">intlify/vue-cli-plugin-i18n#263</a></li>
<li>build(deps): bump url-parse from 1.5.3 to 1.5.7 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/265">intlify/vue-cli-plugin-i18n#265</a></li>
<li>build(deps): bump prismjs from 1.25.0 to 1.27.0 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/266">intlify/vue-cli-plugin-i18n#266</a></li>
<li>build(deps): bump prismjs from 1.25.0 to 1.27.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/267">intlify/vue-cli-plugin-i18n#267</a></li>
<li>build(deps): bump url-parse from 1.5.3 to 1.5.10 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/268">intlify/vue-cli-plugin-i18n#268</a></li>
<li>build(deps): bump url-parse from 1.5.3 to 1.5.10 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/269">intlify/vue-cli-plugin-i18n#269</a></li>
<li>build(deps): bump minimist from 1.2.5 to 1.2.6 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/270">intlify/vue-cli-plugin-i18n#270</a></li>
<li>build(deps): bump minimist from 1.2.5 to 1.2.6 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/271">intlify/vue-cli-plugin-i18n#271</a></li>
<li>build(deps): bump async from 2.6.3 to 2.6.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/272">intlify/vue-cli-plugin-i18n#272</a></li>
<li>build(deps): bump async from 2.6.3 to 2.6.4 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/273">intlify/vue-cli-plugin-i18n#273</a></li>
<li>build(deps): bump eventsource from 1.0.7 to 1.1.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/274">intlify/vue-cli-plugin-i18n#274</a></li>
<li>build(deps): bump eventsource from 1.0.7 to 1.1.1 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/275">intlify/vue-cli-plugin-i18n#275</a></li>
<li>build(deps): bump shell-quote from 1.7.2 to 1.7.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/276">intlify/vue-cli-plugin-i18n#276</a></li>
<li>build(deps): bump shell-quote from 1.7.2 to 1.7.3 in /client-addon by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/277">intlify/vue-cli-plugin-i18n#277</a></li>
<li>build(deps): bump jsdom from 16.4.0 to 16.7.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/278">intlify/vue-cli-plugin-i18n#278</a></li>
<li>Bump vue-i18n-extract to version 1.2.3 by <a href="https://github.com/mateuscruz"><code>@​mateuscruz</code></a> in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/279">intlify/vue-cli-plugin-i18n#279</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/bildeneins"><code>@​bildeneins</code></a> made their first contribution in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/250">intlify/vue-cli-plugin-i18n#250</a></li>
<li><a href="https://github.com/deining"><code>@​deining</code></a> made their first contribution in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/253">intlify/vue-cli-plugin-i18n#253</a></li>
<li><a href="https://github.com/mateuscruz"><code>@​mateuscruz</code></a> made their first contribution in <a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/pull/279">intlify/vue-cli-plugin-i18n#279</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/intlify/vue-cli-plugin-i18n/compare/v2.3.1...v2.3.2">https://github.com/intlify/vue-cli-plugin-i18n/compare/v2.3.1...v2.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/37915e178e34b670bbce48c53b3eeda9ded08756"><code>37915e1</code></a> release: v2.3.2</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/4ef7b1a4538dad156ef64c4b739811e402a9ba7c"><code>4ef7b1a</code></a> Bump vue-i18n-extract to version &quot;1.2.3 (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/279">#279</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/e3bb0e9ea2934682e438bf91c81a7f8682dbf2e0"><code>e3bb0e9</code></a> build(deps): bump jsdom from 16.4.0 to 16.7.0 (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/278">#278</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/0f238cd6f59900055324f9fd9abd14cb4c3c6f62"><code>0f238cd</code></a> build(deps): bump shell-quote from 1.7.2 to 1.7.3 in /client-addon (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/277">#277</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/238ef063d9bd629cb12e22e5159da02fe40f2066"><code>238ef06</code></a> build(deps): bump shell-quote from 1.7.2 to 1.7.3 (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/276">#276</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/9d372648839f7b83cd40cf332e14d977c198c764"><code>9d37264</code></a> build(deps): bump eventsource from 1.0.7 to 1.1.1 in /client-addon (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/275">#275</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/f7caf1689552b06641614fecc0a858baef0e1145"><code>f7caf16</code></a> build(deps): bump eventsource from 1.0.7 to 1.1.1 (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/274">#274</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/b3433e1b3bc2b2d58e7cd187d4d1a924ed863e35"><code>b3433e1</code></a> build(deps): bump async from 2.6.3 to 2.6.4 in /client-addon (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/273">#273</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/7ffd1772865d9cef68fc714654b246463e5a3838"><code>7ffd177</code></a> build(deps): bump async from 2.6.3 to 2.6.4 (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/272">#272</a>)</li>
<li><a href="https://github.com/intlify/vue-cli-plugin-i18n/commit/2f96e52392ec10c381394d653d820ccbf558a240"><code>2f96e52</code></a> build(deps): bump minimist from 1.2.5 to 1.2.6 (<a href="https://redirect.github.com/intlify/vue-cli-plugin-i18n/issues/271">#271</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/intlify/vue-cli-plugin-i18n/compare/v2.3.1...v2.3.2">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 15:40:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/866" class=".btn">#866</a>
            </td>
            <td>
                <b>
                    Remove GitPod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger-labs/business-partner-agent/issues/865
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 15:01:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    Bump beatlabs/delete-old-branches-action from 0.0.9 to 0.0.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [beatlabs/delete-old-branches-action](https://github.com/beatlabs/delete-old-branches-action) from 0.0.9 to 0.0.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/beatlabs/delete-old-branches-action/releases">beatlabs/delete-old-branches-action's releases</a>.</em></p>
<blockquote>
<h2>v0.0.10</h2>
<h2>What's Changed</h2>
<ul>
<li>use latest checkout action with safe.dir fix by <a href="https://github.com/ravinaik1312"><code>@​ravinaik1312</code></a> in <a href="https://redirect.github.com/beatlabs/delete-old-branches-action/pull/22">beatlabs/delete-old-branches-action#22</a></li>
<li>docs: update example version to current by <a href="https://github.com/mdelapenya"><code>@​mdelapenya</code></a> in <a href="https://redirect.github.com/beatlabs/delete-old-branches-action/pull/23">beatlabs/delete-old-branches-action#23</a></li>
<li>Fixes a typo by <a href="https://github.com/iamnotaturtle"><code>@​iamnotaturtle</code></a> in <a href="https://redirect.github.com/beatlabs/delete-old-branches-action/pull/27">beatlabs/delete-old-branches-action#27</a></li>
<li>Updated output due to it will be deprecated by <a href="https://github.com/juanjimenezcasas"><code>@​juanjimenezcasas</code></a> in <a href="https://redirect.github.com/beatlabs/delete-old-branches-action/pull/30">beatlabs/delete-old-branches-action#30</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/iamnotaturtle"><code>@​iamnotaturtle</code></a> made their first contribution in <a href="https://redirect.github.com/beatlabs/delete-old-branches-action/pull/27">beatlabs/delete-old-branches-action#27</a></li>
<li><a href="https://github.com/juanjimenezcasas"><code>@​juanjimenezcasas</code></a> made their first contribution in <a href="https://redirect.github.com/beatlabs/delete-old-branches-action/pull/30">beatlabs/delete-old-branches-action#30</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/beatlabs/delete-old-branches-action/compare/v0.0.9...v0.0.10">https://github.com/beatlabs/delete-old-branches-action/compare/v0.0.9...v0.0.10</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/beatlabs/delete-old-branches-action/commit/6e94df089372a619c01ae2c2f666bf474f890911"><code>6e94df0</code></a> Updated output due to it will be deprecated (<a href="https://redirect.github.com/beatlabs/delete-old-branches-action/issues/30">#30</a>)</li>
<li><a href="https://github.com/beatlabs/delete-old-branches-action/commit/333a962b128190aca5f17b76bdc708daf72ee6f6"><code>333a962</code></a> fix typo (<a href="https://redirect.github.com/beatlabs/delete-old-branches-action/issues/27">#27</a>)</li>
<li><a href="https://github.com/beatlabs/delete-old-branches-action/commit/a91affd63ec6edd643dc901207350855152f204a"><code>a91affd</code></a> docs: update example version to current (<a href="https://redirect.github.com/beatlabs/delete-old-branches-action/issues/23">#23</a>)</li>
<li><a href="https://github.com/beatlabs/delete-old-branches-action/commit/c0b06a6afe86141fd9e0c2540a5f32c3bd218997"><code>c0b06a6</code></a> use latest checkout action with safe.dir fix (<a href="https://redirect.github.com/beatlabs/delete-old-branches-action/issues/22">#22</a>)</li>
<li>See full diff in <a href="https://github.com/beatlabs/delete-old-branches-action/compare/v0.0.9...v0.0.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=beatlabs/delete-old-branches-action&package-manager=github_actions&previous-version=0.0.9&new-version=0.0.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 14:23:03 +0000 UTC
    </div>
</div>

