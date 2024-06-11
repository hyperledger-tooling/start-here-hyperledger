---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump @grpc/grpc-js, fabric-common, fabric-network and fabric-protos in /common/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) to 1.9.15 and updates ancestor dependencies [@grpc/grpc-js](https://github.com/grpc/grpc-node), [fabric-common](https://github.com/hyperledger/fabric-sdk-node), [fabric-network](https://github.com/hyperledger/fabric-sdk-node) and [fabric-protos](https://github.com/hyperledger/fabric-sdk-node). These dependencies need to be updated together.

Updates `@grpc/grpc-js` from 1.7.3 to 1.9.15
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.9.15</h2>
<ul>
<li>Avoid buffering significantly more than <code>grpc.max_receive_message_size</code> per received message.</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.14</h2>
<ul>
<li>Fix a bug that could rarely cause connection leaks (<a href="https://redirect.github.com/grpc/grpc-node/issues/2644">#2644</a>)</li>
<li>Fix a bug that could cause clients to go IDLE incorrectly some time after calling <code>waitForReady</code> (<a href="https://redirect.github.com/grpc/grpc-node/issues/2643">#2643</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.13</h2>
<ul>
<li>Fix a bug that could cause the Node process to close early when establishing a connection while a request is pending (<a href="https://redirect.github.com/grpc/grpc-node/issues/2626">#2626</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.12</h2>
<ul>
<li>Fix a bug that could cause connectivity state information to become stale in some circumstances (<a href="https://redirect.github.com/grpc/grpc-node/issues/2623">#2623</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.11</h2>
<ul>
<li>Fix a busy loop when recovering from a failure to establish a connection to a unix domain socket address target (<a href="https://redirect.github.com/grpc/grpc-node/issues/2618">#2618</a>)</li>
<li>Fix a bug that caused clients to stop trying to connect to a fixed IP address target after a working connection drops (<a href="https://redirect.github.com/grpc/grpc-node/issues/2619">#2619</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.10</h2>
<ul>
<li>Provide the correct port to the proxy when connecting to a target without an explicitly specified port (<a href="https://redirect.github.com/grpc/grpc-node/issues/2608">#2608</a> contributed by <a href="https://github.com/segevfiner"><code>@​segevfiner</code></a>)</li>
<li>Properly handle goaway events with no additional data attached (<a href="https://redirect.github.com/grpc/grpc-node/issues/2611">#2611</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.9</h2>
<ul>
<li>Fix a busy loop when recovering from a failure to establish a connection to a fixed IP address target (<a href="https://redirect.github.com/grpc/grpc-node/issues/2609">#2609</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.8</h2>
<ul>
<li>Fix a memory leak caused by creating and closing multiple clients (<a href="https://redirect.github.com/grpc/grpc-node/issues/2606">#2606</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.7</h2>
<ul>
<li>Fix a bug that could cause a client to not update name resolution after multiple failed connection attempts (<a href="https://redirect.github.com/grpc/grpc-node/issues/2602">#2602</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.6</h2>
<ul>
<li>Include more information in most &quot;No connection established&quot; errors (<a href="https://redirect.github.com/grpc/grpc-node/issues/2598">#2598</a>)</li>
<li>Remove the <code>index</code> tracer, and add more information to other trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2599">#2599</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.5</h2>
<ul>
<li>Fix a type inconsistency in <code>server-call.ts</code> (<a href="https://redirect.github.com/grpc/grpc-node/issues/2589">#2589</a> contributed by <a href="https://github.com/rsnullptr"><code>@​rsnullptr</code></a>)</li>
<li>Close ports if the server is shut down while the bind operation is ongoing (<a href="https://redirect.github.com/grpc/grpc-node/issues/2590">#2590</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.4</h2>
<ul>
<li>Fix a bug that could cause a client to sometimes incorrectly hold the process open when no longer in use (<a href="https://redirect.github.com/grpc/grpc-node/issues/2586">#2586</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.3</h2>
<ul>
<li>Make a few improvements to DNS resolving timing (<a href="https://redirect.github.com/grpc/grpc-node/issues/2571">#2571</a>)</li>
</ul>
<p>Experimental changes:</p>
<ul>
<li>Added <code>grpc.experimental.BackoffTimeout#getEndTime</code></li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.9.2</h2>
<ul>
<li>Handle error when sending keepalive pings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2563">#2563</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/08b0422dae56467ecae1007e899efe66a8c4a650"><code>08b0422</code></a> Merge pull request from GHSA-7v5v-9h63-cj86</li>
<li><a href="https://github.com/grpc/grpc-node/commit/c75e04894829ff5c0eac83a3eea96724ec7cd118"><code>c75e048</code></a> grpc-js: Bump to 1.9.15</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d5d62b4d94acf05d4335122efa9e36b07955eb2d"><code>d5d62b4</code></a> grpc-js: Avoid buffering significantly more than max_receive_message_size per...</li>
<li><a href="https://github.com/grpc/grpc-node/commit/02d034489a923f7f9cb15d4720cc2c865b11ef12"><code>02d0344</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2741">#2741</a> from sergiitk/backport-1.9-psm-interop-common-prod-t...</li>
<li><a href="https://github.com/grpc/grpc-node/commit/cf14020643472af7ec56c3591c73f91d74c4aa73"><code>cf14020</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2729">#2729</a> from sergiitk/psm-interop-common-prod-tests</li>
<li><a href="https://github.com/grpc/grpc-node/commit/da44229934a18519126f6993b6feed00c60ded0a"><code>da44229</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2738">#2738</a> from murgatroid99/backport-1.9-grpc-js_linkify-it_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/5ae7c8c84518fa49ec639cd36051d65e50db5a6c"><code>5ae7c8c</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2735">#2735</a> from murgatroid99/grpc-js_linkify-it_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/eed21ba0bba8e8b1d8bc01001cfd0faf61bb9a75"><code>eed21ba</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2714">#2714</a> from sergiitk/backport-1.9-psm-interop-pkg-dev</li>
<li><a href="https://github.com/grpc/grpc-node/commit/63763a40003b17e5e8f3f9c8d7f4aeb6592569f6"><code>63763a4</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2712">#2712</a> from sergiitk/psm-interop-pkg-dev</li>
<li><a href="https://github.com/grpc/grpc-node/commit/5be83dd878c5a2b857c38b113aabb3fad9bd376d"><code>5be83dd</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2643">#2643</a> from murgatroid99/grpc-js_idle_timer_fix</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.7.3...@grpc/grpc-js@1.9.15">compare view</a></li>
</ul>
</details>
<br />

Updates `fabric-common` from 2.2.18 to 2.2.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/fabric-sdk-node/releases">fabric-common's releases</a>.</em></p>
<blockquote>
<h2>v2.2.20</h2>
<h2>What's Changed</h2>
<ul>
<li>Update dependencies to address CVE-2023-45857 by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/689">hyperledger/fabric-sdk-node#689</a></li>
</ul>
<h2>Supported Node versions</h2>
<p>The updated dependency to address CVE-2023-45857 is used only by the CouchDB wallet implementation, and requires Node 14 or later. Therefore Node 10 and 12 are no longer supported by the <strong>fabric-network</strong> package. If you need to continue running on one of these unsupported Node versions, you should continue to use <strong>fabric-network@2.2.19</strong>.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20</a></p>
<h2>v2.2.19</h2>
<h2>What's Changed</h2>
<ul>
<li>Explicitly import <a href="https://www.npmjs.com/package/long">long</a> to address changes to typing in dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/682">hyperledger/fabric-sdk-node#682</a></li>
<li>Use require to import <a href="https://www.npmjs.com/package/long">long</a> to improve compatibility with client application TypeScript configuration by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/683">hyperledger/fabric-sdk-node#683</a></li>
<li>Regenerate fabric-protos using current <a href="https://www.npmjs.com/package/protobufjs">protobufjs</a> to address typing issues introduced by new versions of dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/684">hyperledger/fabric-sdk-node#684</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/ea65b92719f6024168b55cd01631711634752d4b"><code>ea65b92</code></a> Release v2.2.20 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/690">#690</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/cd20a8443882509844a4ed656b8dbe1f076302fb"><code>cd20a84</code></a> Update dependencies to address CVE-2023-45857 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/689">#689</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/53b41aea00f15ef8afd69eedb3264380c8298d22"><code>53b41ae</code></a> Update version following v2.2.19 release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/686">#686</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/7d6752ec4d19c4c06150fadc25e8753e60fa6d61"><code>7d6752e</code></a> Release v2.2.19 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/685">#685</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/80573efebb1883bd5bec86e268a6c6cd37ea1011"><code>80573ef</code></a> Regenerate fabric-protos using current protobufjs (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/684">#684</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/83729649113304a08cd1e7519613ab0bf7b3897d"><code>8372964</code></a> Use require to import long (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/683">#683</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/8743c2e75151f1ce9249039804f0127ebeb014fd"><code>8743c2e</code></a> Fixes required by changes to typing in dependencies (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/682">#682</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/9bf4de090e02cf0f3a5595ae3b98c6dd45b92808"><code>9bf4de0</code></a> Update versions following release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/677">#677</a>)</li>
<li>See full diff in <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.20">compare view</a></li>
</ul>
</details>
<br />

Updates `fabric-network` from 2.2.18 to 2.2.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/fabric-sdk-node/releases">fabric-network's releases</a>.</em></p>
<blockquote>
<h2>v2.2.20</h2>
<h2>What's Changed</h2>
<ul>
<li>Update dependencies to address CVE-2023-45857 by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/689">hyperledger/fabric-sdk-node#689</a></li>
</ul>
<h2>Supported Node versions</h2>
<p>The updated dependency to address CVE-2023-45857 is used only by the CouchDB wallet implementation, and requires Node 14 or later. Therefore Node 10 and 12 are no longer supported by the <strong>fabric-network</strong> package. If you need to continue running on one of these unsupported Node versions, you should continue to use <strong>fabric-network@2.2.19</strong>.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20</a></p>
<h2>v2.2.19</h2>
<h2>What's Changed</h2>
<ul>
<li>Explicitly import <a href="https://www.npmjs.com/package/long">long</a> to address changes to typing in dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/682">hyperledger/fabric-sdk-node#682</a></li>
<li>Use require to import <a href="https://www.npmjs.com/package/long">long</a> to improve compatibility with client application TypeScript configuration by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/683">hyperledger/fabric-sdk-node#683</a></li>
<li>Regenerate fabric-protos using current <a href="https://www.npmjs.com/package/protobufjs">protobufjs</a> to address typing issues introduced by new versions of dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/684">hyperledger/fabric-sdk-node#684</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/ea65b92719f6024168b55cd01631711634752d4b"><code>ea65b92</code></a> Release v2.2.20 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/690">#690</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/cd20a8443882509844a4ed656b8dbe1f076302fb"><code>cd20a84</code></a> Update dependencies to address CVE-2023-45857 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/689">#689</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/53b41aea00f15ef8afd69eedb3264380c8298d22"><code>53b41ae</code></a> Update version following v2.2.19 release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/686">#686</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/7d6752ec4d19c4c06150fadc25e8753e60fa6d61"><code>7d6752e</code></a> Release v2.2.19 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/685">#685</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/80573efebb1883bd5bec86e268a6c6cd37ea1011"><code>80573ef</code></a> Regenerate fabric-protos using current protobufjs (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/684">#684</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/83729649113304a08cd1e7519613ab0bf7b3897d"><code>8372964</code></a> Use require to import long (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/683">#683</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/8743c2e75151f1ce9249039804f0127ebeb014fd"><code>8743c2e</code></a> Fixes required by changes to typing in dependencies (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/682">#682</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/9bf4de090e02cf0f3a5595ae3b98c6dd45b92808"><code>9bf4de0</code></a> Update versions following release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/677">#677</a>)</li>
<li>See full diff in <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.20">compare view</a></li>
</ul>
</details>
<br />

Updates `fabric-protos` from 2.2.18 to 2.2.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/fabric-sdk-node/releases">fabric-protos's releases</a>.</em></p>
<blockquote>
<h2>v2.2.20</h2>
<h2>What's Changed</h2>
<ul>
<li>Update dependencies to address CVE-2023-45857 by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/689">hyperledger/fabric-sdk-node#689</a></li>
</ul>
<h2>Supported Node versions</h2>
<p>The updated dependency to address CVE-2023-45857 is used only by the CouchDB wallet implementation, and requires Node 14 or later. Therefore Node 10 and 12 are no longer supported by the <strong>fabric-network</strong> package. If you need to continue running on one of these unsupported Node versions, you should continue to use <strong>fabric-network@2.2.19</strong>.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20</a></p>
<h2>v2.2.19</h2>
<h2>What's Changed</h2>
<ul>
<li>Explicitly import <a href="https://www.npmjs.com/package/long">long</a> to address changes to typing in dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/682">hyperledger/fabric-sdk-node#682</a></li>
<li>Use require to import <a href="https://www.npmjs.com/package/long">long</a> to improve compatibility with client application TypeScript configuration by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/683">hyperledger/fabric-sdk-node#683</a></li>
<li>Regenerate fabric-protos using current <a href="https://www.npmjs.com/package/protobufjs">protobufjs</a> to address typing issues introduced by new versions of dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/684">hyperledger/fabric-sdk-node#684</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/ea65b92719f6024168b55cd01631711634752d4b"><code>ea65b92</code></a> Release v2.2.20 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/690">#690</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/cd20a8443882509844a4ed656b8dbe1f076302fb"><code>cd20a84</code></a> Update dependencies to address CVE-2023-45857 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/689">#689</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/53b41aea00f15ef8afd69eedb3264380c8298d22"><code>53b41ae</code></a> Update version following v2.2.19 release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/686">#686</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/7d6752ec4d19c4c06150fadc25e8753e60fa6d61"><code>7d6752e</code></a> Release v2.2.19 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/685">#685</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/80573efebb1883bd5bec86e268a6c6cd37ea1011"><code>80573ef</code></a> Regenerate fabric-protos using current protobufjs (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/684">#684</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/83729649113304a08cd1e7519613ab0bf7b3897d"><code>8372964</code></a> Use require to import long (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/683">#683</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/8743c2e75151f1ce9249039804f0127ebeb014fd"><code>8743c2e</code></a> Fixes required by changes to typing in dependencies (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/682">#682</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/9bf4de090e02cf0f3a5595ae3b98c6dd45b92808"><code>9bf4de0</code></a> Update versions following release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/677">#677</a>)</li>
<li>See full diff in <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.20">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 01:01:55 +0000 UTC
    </div>
</div>

