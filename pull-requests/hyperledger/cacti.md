---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3304" class=".btn">#3304</a>
            </td>
            <td>
                <b>
                    build(deps): bump the npm_and_yarn group across 12 directories with 14 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 13 updates in the / directory:

| Package | From | To |
| --- | --- | --- |
| [@grpc/grpc-js](https://github.com/grpc/grpc-node) | `1.10.3` | `1.10.9` |
| [axios](https://github.com/axios/axios) | `1.5.1` | `1.6.0` |
| [bl](https://github.com/rvagg/bl) | `5.0.0` | `5.1.0` |
| [undici](https://github.com/nodejs/undici) | `6.11.1` | `6.12.0` |
| [qs](https://github.com/ljharb/qs) | `6.7.3` | `6.8.3` |
| [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite) | `5.0.13` | `5.1.7` |
| [pkg](https://github.com/vercel/pkg) | `4.5.1` | `5.8.1` |
| [@adobe/css-tools](https://github.com/adobe/css-tools) | `4.2.0` | `4.4.0` |
| [apollo-server-core](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core) | `3.12.0` | `3.13.0` |
| [browserify-sign](https://github.com/crypto-browserify/browserify-sign) | `4.2.1` | `4.2.3` |
| [es5-ext](https://github.com/medikoo/es5-ext) | `0.10.53` | `0.10.64` |
| [react-devtools-core](https://github.com/facebook/react/tree/HEAD/packages/react-devtools-core) | `4.27.8` | `4.28.5` |
| [word-wrap](https://github.com/jonschlinkert/word-wrap) | `1.2.3` | `1.2.5` |

Bumps the npm_and_yarn group with 1 update in the /examples/cactus-example-tcs-huawei directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken).
Bumps the npm_and_yarn group with 1 update in the /examples/test-run-transaction directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-cmd-api-server directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node) and [axios](https://github.com/axios/axios).
Bumps the npm_and_yarn group with 1 update in the /packages/cactus-common directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-core-api directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node) and [axios](https://github.com/axios/axios).
Bumps the npm_and_yarn group with 1 update in the /packages/cactus-plugin-ledger-connector-tcs-huawei-socketio directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken).
Bumps the npm_and_yarn group with 1 update in the /weaver/common/protos-js directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 1 update in the /weaver/core/drivers/fabric-driver directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 1 update in the /weaver/core/identity-management/iin-agent directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 2 updates in the /weaver/samples/fabric/fabric-cli directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node) and [pkg](https://github.com/vercel/pkg).
Bumps the npm_and_yarn group with 1 update in the /weaver/sdks/fabric/interoperation-node-sdk directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).

Updates `@grpc/grpc-js` from 1.10.3 to 1.10.9
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.10.9</h2>
<ul>
<li>Avoid buffering significantly more than <code>grpc.max_receive_message_size</code> per received message.</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.8</h2>
<ul>
<li>Fix a bug that caused channels with <code>unix:</code> targets to not reconnect after the channel goes idle (<a href="https://redirect.github.com/grpc/grpc-node/issues/2750">#2750</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.7</h2>
<ul>
<li>Improve reporting of HTTP error codes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2723">#2723</a>)</li>
<li>Update dependency on <code>@grpc/proto-loader</code> to the latest version (<a href="https://redirect.github.com/grpc/grpc-node/issues/2732">#2732</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.6</h2>
<ul>
<li>Fix a bug that could cause a server to sometimes send the status early (<a href="https://redirect.github.com/grpc/grpc-node/issues/2708">#2708</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.5</h2>
<ul>
<li>Resolve exception when <code>Error.stackTraceLimit</code> is <code>undefined</code> (<a href="https://redirect.github.com/grpc/grpc-node/issues/2701">#2701</a> contributed by <a href="https://github.com/davidfiala"><code>@​davidfiala</code></a>)</li>
<li>Call configured <code>checkServerIdentity</code> when <code>grpc.ssl_target_name_override</code> is set (<a href="https://redirect.github.com/grpc/grpc-node/issues/2704">#2704</a>)</li>
<li>Add more information to DEADLINE_EXCEEDED error details strings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2692">#2692</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.4</h2>
<ul>
<li>Fix a bug that caused server interceptors to crash when using partially-populated <code>ResponderBuilder</code> and <code>ListenerBuilder</code> objects (<a href="https://redirect.github.com/grpc/grpc-node/issues/2696">#2696</a>)</li>
<li>Avoid sending RST_STREAM from the client when the server has already finished its side of the stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2695">#2695</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/674f4e351a619fd4532f84ae6dff96b8ee4e1ed3"><code>674f4e3</code></a> Merge pull request from GHSA-7v5v-9h63-cj86</li>
<li><a href="https://github.com/grpc/grpc-node/commit/7ecaa2d2dcaaa49467d41143169212caf55a40cd"><code>7ecaa2d</code></a> grpc-js: Bump to 1.10.9</li>
<li><a href="https://github.com/grpc/grpc-node/commit/e64d816d7df6d6cde62314beb67d11f1e0a8c79e"><code>e64d816</code></a> grpc-js: Avoid buffering significantly more than max_receive_message_size per...</li>
<li><a href="https://github.com/grpc/grpc-node/commit/45e5fe5462fea6cb4e3898fa2f07a4836f95916a"><code>45e5fe5</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2750">#2750</a> from murgatroid99/grpc-js_idle_uds_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/87a35414021f627f01591cade9b1f9a7dcaaf5d3"><code>87a3541</code></a> grpc-js: Fix UDS channels not reconnecting after going idle</li>
<li><a href="https://github.com/grpc/grpc-node/commit/3105791fbe8a615a28289da33ad584fb868d2ff6"><code>3105791</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2740">#2740</a> from sergiitk/backport-1.10-psm-interop-common-prod-...</li>
<li><a href="https://github.com/grpc/grpc-node/commit/fec135a9800ce884b8dd414782f4bd0014821a0c"><code>fec135a</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2729">#2729</a> from sergiitk/psm-interop-common-prod-tests</li>
<li><a href="https://github.com/grpc/grpc-node/commit/76fe802309ff39c79887d494760de25633b2beb1"><code>76fe802</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2739">#2739</a> from murgatroid99/backport-1.10-grpc-js_linkify-it_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d5edf49f6c59fd8f6e9ead2836bc30af8284284e"><code>d5edf49</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2735">#2735</a> from murgatroid99/grpc-js_linkify-it_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/23c05fca84cf38b9198e0010ebfe02d3ddae51a7"><code>23c05fc</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2732">#2732</a> from murgatroid99/grpc-js_proto-loader_update</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.10.3...@grpc/grpc-js@1.10.9">compare view</a></li>
</ul>
</details>
<br />

Updates `axios` from 1.5.1 to 1.6.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.6.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/f7adacdbaa569281253c8cfc623ad3f4dc909c60"><code>f7adacd</code></a> chore(release): v1.6.0 (<a href="https://redirect.github.com/axios/axios/issues/6031">#6031</a>)</li>
<li><a href="https://github.com/axios/axios/commit/9917e67cbb6c157382863bad8c741de58e3f3c2b"><code>9917e67</code></a> chore(ci): fix release-it arg; (<a href="https://redirect.github.com/axios/axios/issues/6032">#6032</a>)</li>
<li><a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0"><code>96ee232</code></a> fix(CSRF): fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7d45ab2e2ad6e59f5475e39afd4b286b1f393fc0"><code>7d45ab2</code></a> chore(tests): fixed tests to pass in node v19 and v20 with <code>keep-alive</code> enabl...</li>
<li><a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8"><code>5aaff53</code></a> fix(dns): fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a48a63ad823fc20e5a6a705f05f09842ca49f48c"><code>a48a63a</code></a> chore(docs): added AxiosHeaders docs; (<a href="https://redirect.github.com/axios/axios/issues/5932">#5932</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09"><code>a1c8ad0</code></a> fix(types): fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2ac731d60545ba5c4202c25fd2e732ddd8297d82"><code>2ac731d</code></a> chore(docs): update readme.md (<a href="https://redirect.github.com/axios/axios/issues/5889">#5889</a>)</li>
<li>See full diff in <a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">compare view</a></li>
</ul>
</details>
<br />

Updates `bl` from 5.0.0 to 5.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/releases">bl's releases</a>.</em></p>
<blockquote>
<h2>v5.1.0</h2>
<h2><a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">5.1.0</a> (2022-10-18)</h2>
<h3>Features</h3>
<ul>
<li>added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>) (<a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710">433ff89</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>windows support in tests (<a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c">387dfaf</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>GH Actions, Dependabot, auto-release, remove Travis (<a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f">997f058</a>)</li>
<li><strong>no-release:</strong> bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>) (<a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961">078bfe3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/blob/master/CHANGELOG.md">bl's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">5.1.0</a> (2022-10-18)</h2>
<h3>Features</h3>
<ul>
<li>added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>) (<a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710">433ff89</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>windows support in tests (<a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c">387dfaf</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>GH Actions, Dependabot, auto-release, remove Travis (<a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f">997f058</a>)</li>
<li><strong>no-release:</strong> bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>) (<a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961">078bfe3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rvagg/bl/commit/3af8c54d33433c4683be4a74588a9739270ca4d4"><code>3af8c54</code></a> chore(release): 5.1.0 [skip ci]</li>
<li><a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710"><code>433ff89</code></a> feat: added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>)</li>
<li><a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961"><code>078bfe3</code></a> chore(no-release): bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>)</li>
<li><a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c"><code>387dfaf</code></a> fix: windows support in tests</li>
<li><a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f"><code>997f058</code></a> chore: GH Actions, Dependabot, auto-release, remove Travis</li>
<li>See full diff in <a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">compare view</a></li>
</ul>
</details>
<br />

Updates `undici` from 6.11.1 to 6.12.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v6.12.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: broken test by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3045">nodejs/undici#3045</a></li>
<li>fix: http2 header parsing by <a href="https://github.com/climba03003"><code>@​climba03003</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3047">nodejs/undici#3047</a></li>
<li>types: fix Request.refererPolicy and RequestInit.refererPolicy are incompatible by <a href="https://github.com/zbinlin"><code>@​zbinlin</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3039">nodejs/undici#3039</a></li>
<li>fix(types): onHeaders always takes headers as an array of buffer by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3050">nodejs/undici#3050</a></li>
<li>fix: ProxyAgent causes request.headers.host to be forcibly reset by <a href="https://github.com/1zilc"><code>@​1zilc</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3026">nodejs/undici#3026</a></li>
<li>fallback to Buffer.isUtf8 on platforms without icu by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3006">nodejs/undici#3006</a></li>
<li>build(deps): bump github/codeql-action from 3.24.6 to 3.24.9 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3037">nodejs/undici#3037</a></li>
<li>build(deps): bump actions/dependency-review-action from 4.1.3 to 4.2.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3035">nodejs/undici#3035</a></li>
<li>build(deps): bump node from <code>577f8eb</code> to <code>87524df</code> in /build by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3055">nodejs/undici#3055</a></li>
<li>build(deps): bump node from <code>87524df</code> to <code>9696b26</code> in /build by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3058">nodejs/undici#3058</a></li>
<li>fetch: Block ports 4190 &amp; 6679 by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3059">nodejs/undici#3059</a></li>
<li>test: activate testing for interceptors and cache by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3061">nodejs/undici#3061</a></li>
<li>cache: improve test coverage by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3063">nodejs/undici#3063</a></li>
<li>feat: modernize fuzzing by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3060">nodejs/undici#3060</a></li>
<li>fix: request abort by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3056">nodejs/undici#3056</a></li>
<li>fix: signal handling by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3053">nodejs/undici#3053</a></li>
<li>fix(H2): handle goaway properly by <a href="https://github.com/metcoder95"><code>@​metcoder95</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3057">nodejs/undici#3057</a></li>
<li>test: client, set body to null if bigger than CHUNK_LIMIT by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3064">nodejs/undici#3064</a></li>
<li>mock: improve mock interceptor by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3062">nodejs/undici#3062</a></li>
<li>fix: bad client destroy on servername change by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3066">nodejs/undici#3066</a></li>
<li>perf: improve isBlobLike by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3070">nodejs/undici#3070</a></li>
<li>test: add sanity check for llhttp wasm files by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3068">nodejs/undici#3068</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/zbinlin"><code>@​zbinlin</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/3039">nodejs/undici#3039</a></li>
<li><a href="https://github.com/1zilc"><code>@​1zilc</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/3026">nodejs/undici#3026</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0">https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/7751d9bcd5bbba45b60c90183aeab450b60c0831"><code>7751d9b</code></a> Bumped v6.12.0</li>
<li><a href="https://github.com/nodejs/undici/commit/e9c3b22c97b5bf2113057ea2cf1c6dec8868e9fb"><code>e9c3b22</code></a> Revert &quot;automate releases (<a href="https://redirect.github.com/nodejs/undici/issues/3052">#3052</a>)&quot;</li>
<li><a href="https://github.com/nodejs/undici/commit/f51f226522ec75a0613a07a4efc8f78938030c45"><code>f51f226</code></a> automate releases (<a href="https://redirect.github.com/nodejs/undici/issues/3052">#3052</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/502e13472d4bcebbf4669c2a91a7ef97705a0fd7"><code>502e134</code></a> test: add test for llhttp wasm (<a href="https://redirect.github.com/nodejs/undici/issues/3068">#3068</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/413fd4de5b161c1e9a539089a4d51965abd5018d"><code>413fd4d</code></a> perf: improve isBlobLike (<a href="https://redirect.github.com/nodejs/undici/issues/3070">#3070</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/7ae20e6070fa7de2831a907c92fa44268003c145"><code>7ae20e6</code></a> fix: bad client destroy on servername change (<a href="https://redirect.github.com/nodejs/undici/issues/3066">#3066</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ad3fac577cca737976ed82cd9d55027eb8af654c"><code>ad3fac5</code></a> mock: improve mock interceptor (<a href="https://redirect.github.com/nodejs/undici/issues/3062">#3062</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/d399b3db9e16b25e9ed0f07c0e067fe99fa8c409"><code>d399b3d</code></a> test: client, set body to null if bigger than CHUNK_LIMIT (<a href="https://redirect.github.com/nodejs/undici/issues/3064">#3064</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/bc4b20698f38b4f43f0eb4091dad28c83844f3ef"><code>bc4b206</code></a> fix(H2): handle goaway properly (<a href="https://redirect.github.com/nodejs/undici/issues/3057">#3057</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/b6aa794e2db44f20adc4c9cc99009e72048f4fed"><code>b6aa794</code></a> fix: signal handling (<a href="https://redirect.github.com/nodejs/undici/issues/3053">#3053</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0">compare view</a></li>
</ul>
</details>
<br />

Updates `qs` from 6.7.3 to 6.8.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.8.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://redirect.github.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[actions] backport actions from main</li>
<li>[Dev Deps] backport updates from main</li>
<li>[Refactor] <code>stringify</code>: reduce branching</li>
<li>[meta] do not publish workflow files</li>
</ul>
<h2><strong>6.8.2</strong></h2>
<ul>
<li>[Fix] proper comma parsing of URL-encoded commas (<a href="https://redirect.github.com/ljharb/qs/issues/361">#361</a>)</li>
<li>[Fix] parses comma delimited array while having percent-encoded comma treated as normal text (<a href="https://redirect.github.com/ljharb/qs/issues/336">#336</a>)</li>
</ul>
<h2><strong>6.8.1</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: Fix parsing array from object with <code>comma</code> true (<a href="https://redirect.github.com/ljharb/qs/issues/359">#359</a>)</li>
<li>[Fix] <code>parse</code>: throw a TypeError instead of an Error for bad charset (<a href="https://redirect.github.com/ljharb/qs/issues/349">#349</a>)</li>
<li>[Fix] <code>parse</code>: with comma true, handle field that holds an array of arrays (<a href="https://redirect.github.com/ljharb/qs/issues/335">#335</a>)</li>
<li>[fix] <code>parse</code>: with comma true, do not split non-string values (<a href="https://redirect.github.com/ljharb/qs/issues/334">#334</a>)</li>
<li>[meta] add tidelift marketing copy</li>
<li>[meta] add <code>funding</code> field</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>tape</code>, <code>safe-publish-latest</code>, <code>evalmd</code>, <code>has-symbols</code>, <code>iconv-lite</code>, <code>mkdirp</code>, <code>object-inspect</code></li>
<li>[Tests] <code>parse</code>: add passing <code>arrayFormat</code> tests</li>
<li>[Tests] use shared travis-ci configs</li>
<li>[Tests] <code>Buffer.from</code> in node v5.0-v5.9 and v4.0-v4.4 requires a TypedArray</li>
<li>[actions] add automatic rebasing / merge commit blocking</li>
</ul>
<h2><strong>6.8.0</strong></h2>
<ul>
<li>[New] add <code>depth=false</code> to preserve the original key; [Fix] <code>depth=0</code> should preserve the original key (<a href="https://redirect.github.com/ljharb/qs/issues/326">#326</a>)</li>
<li>[New] [Fix] stringify symbols and bigints</li>
<li>[Fix] ensure node 0.12 can stringify Symbols</li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Refactor] <code>formats</code>: tiny bit of cleanup.</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>browserify</code>, <code>safe-publish-latest</code>, <code>iconv-lite</code>, <code>tape</code></li>
<li>[Tests] add tests for <code>depth=0</code> and <code>depth=false</code> behavior, both current and intuitive/intended (<a href="https://redirect.github.com/ljharb/qs/issues/326">#326</a>)</li>
<li>[Tests] use <code>eclint</code> instead of <code>editorconfig-tools</code></li>
<li>[docs] readme: add security note</li>
<li>[meta] add github sponsorship</li>
<li>[meta] add FUNDING.yml</li>
<li>[meta] Clean up license text so it’s properly detected as BSD-3-Clause</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/0db55386013a5d92503944ad42022fd8c112c983"><code>0db5538</code></a> v6.8.3</li>
<li><a href="https://github.com/ljharb/qs/commit/639a381a66845925dba32531dcb9d21c446e9f1f"><code>639a381</code></a> [meta] do not publish workflow files</li>
<li><a href="https://github.com/ljharb/qs/commit/fc3682776670524a42e19709ec4a8138d0d7afda"><code>fc36827</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/4e312c487def80b879d5359e0d1991ce17685191"><code>4e312c4</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/57918dae411c17b232377759baaa52a642762950"><code>57918da</code></a> [Fix] <code>stringify</code>: avoid encoding arrayformat comma when `encodeValuesOnly = ...</li>
<li><a href="https://github.com/ljharb/qs/commit/48673cae0226de23f6f33cc0e17af893b42f5e37"><code>48673ca</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/554ba810f1a49a25dd27c09a466490cedbee5c65"><code>554ba81</code></a> [Tests] clean up stringify tests slightly</li>
<li><a href="https://github.com/ljharb/qs/commit/dbb54a8f14573e3c7512ea01d99f75f6ce0571f8"><code>dbb54a8</code></a> [Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/6868128ca2bd247ba935fbb63d359d0417f6b283"><code>6868128</code></a> [meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/49bed6934b27c3f0ef50e1fcee8d76298d108d52"><code>49bed69</code></a> [actions] backport actions from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.7.3...v6.8.3">compare view</a></li>
</ul>
</details>
<br />

Updates `vite` from 5.0.13 to 5.1.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/releases">vite's releases</a>.</em></p>
<blockquote>
<h2>create-vite@5.1.0</h2>
<p>Please refer to <a href="https://github.com/vitejs/vite/blob/create-vite@5.1.0/packages/create-vite/CHANGELOG.md">CHANGELOG.md</a> for details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/v5.1.7/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->5.1.7 (2024-03-24)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>) (<a href="https://github.com/vitejs/vite/commit/5a056dd">5a056dd</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16250">#16250</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.6 (2024-03-11)<!-- raw HTML omitted --></h2>
<ul>
<li>chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16131">#16131</a>) (<a href="https://github.com/vitejs/vite/commit/a862ecb">a862ecb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16131">#16131</a></li>
<li>fix: check for publicDir before checking if it is a parent directory (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16046">#16046</a>) (<a href="https://github.com/vitejs/vite/commit/b6fb323">b6fb323</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16046">#16046</a></li>
<li>fix: escape single quote when relative base is used (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16060">#16060</a>) (<a href="https://github.com/vitejs/vite/commit/8f74ce4">8f74ce4</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16060">#16060</a></li>
<li>fix: handle function property extension in namespace import (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16113">#16113</a>) (<a href="https://github.com/vitejs/vite/commit/f699194">f699194</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16113">#16113</a></li>
<li>fix: server middleware mode resolve (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16122">#16122</a>) (<a href="https://github.com/vitejs/vite/commit/8403546">8403546</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16122">#16122</a></li>
<li>fix(esbuild): update tsconfck to fix bug that could cause a deadlock  (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16124">#16124</a>) (<a href="https://github.com/vitejs/vite/commit/fd9de04">fd9de04</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16124">#16124</a></li>
<li>fix(worker): hide &quot;The emitted file overwrites&quot; warning if the content is same (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16094">#16094</a>) (<a href="https://github.com/vitejs/vite/commit/60dfa9e">60dfa9e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16094">#16094</a></li>
<li>fix(worker): throw error when circular worker import is detected and support self referencing worker (<a href="https://github.com/vitejs/vite/commit/eef9da1">eef9da1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16103">#16103</a></li>
<li>style(utils): remove null check (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16112">#16112</a>) (<a href="https://github.com/vitejs/vite/commit/0d2df52">0d2df52</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16112">#16112</a></li>
<li>refactor(runtime): share more code between runtime and main bundle (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16063">#16063</a>) (<a href="https://github.com/vitejs/vite/commit/93be84e">93be84e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16063">#16063</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.5 (2024-03-04)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>__vite__mapDeps</code> code injection (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15732">#15732</a>) (<a href="https://github.com/vitejs/vite/commit/aff54e1">aff54e1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15732">#15732</a></li>
<li>fix: analysing build chunk without dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15469">#15469</a>) (<a href="https://github.com/vitejs/vite/commit/bd52283">bd52283</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15469">#15469</a></li>
<li>fix: import with query with imports field (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16085">#16085</a>) (<a href="https://github.com/vitejs/vite/commit/ab823ab">ab823ab</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16085">#16085</a></li>
<li>fix: normalize literal-only entry pattern (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16010">#16010</a>) (<a href="https://github.com/vitejs/vite/commit/1dccc37">1dccc37</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16010">#16010</a></li>
<li>fix: optimizeDeps.entries with literal-only pattern(s) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15853">#15853</a>) (<a href="https://github.com/vitejs/vite/commit/49300b3">49300b3</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15853">#15853</a></li>
<li>fix: output correct error for empty import specifier (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16055">#16055</a>) (<a href="https://github.com/vitejs/vite/commit/a9112eb">a9112eb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16055">#16055</a></li>
<li>fix: upgrade esbuild to 0.20.x (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16062">#16062</a>) (<a href="https://github.com/vitejs/vite/commit/899d9b1">899d9b1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16062">#16062</a></li>
<li>fix(runtime): runtime HMR affects only imported files (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15898">#15898</a>) (<a href="https://github.com/vitejs/vite/commit/57463fc">57463fc</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15898">#15898</a></li>
<li>fix(scanner): respect  <code>experimentalDecorators: true</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15206">#15206</a>) (<a href="https://github.com/vitejs/vite/commit/4144781">4144781</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15206">#15206</a></li>
<li>revert: &quot;fix: upgrade esbuild to 0.20.x&quot; (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16072">#16072</a>) (<a href="https://github.com/vitejs/vite/commit/11cceea">11cceea</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16072">#16072</a></li>
<li>refactor: share code with vite runtime (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15907">#15907</a>) (<a href="https://github.com/vitejs/vite/commit/b20d542">b20d542</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15907">#15907</a></li>
<li>refactor(runtime): use functions from <code>pathe</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16061">#16061</a>) (<a href="https://github.com/vitejs/vite/commit/aac2ef7">aac2ef7</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16061">#16061</a></li>
<li>chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16028">#16028</a>) (<a href="https://github.com/vitejs/vite/commit/7cfe80d">7cfe80d</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16028">#16028</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.4 (2024-02-21)<!-- raw HTML omitted --></h2>
<ul>
<li>perf: remove unnecessary regex s modifier (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15766">#15766</a>) (<a href="https://github.com/vitejs/vite/commit/8dc1b73">8dc1b73</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15766">#15766</a></li>
<li>fix: fs cached checks disabled by default for yarn pnp (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15920">#15920</a>) (<a href="https://github.com/vitejs/vite/commit/8b11fea">8b11fea</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15920">#15920</a></li>
<li>fix: resolve directory correctly when <code>fs.cachedChecks: true</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15983">#15983</a>) (<a href="https://github.com/vitejs/vite/commit/4fe971f">4fe971f</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15983">#15983</a></li>
<li>fix: srcSet with optional descriptor (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15905">#15905</a>) (<a href="https://github.com/vitejs/vite/commit/81b3bd0">81b3bd0</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15905">#15905</a></li>
<li>fix(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15959">#15959</a>) (<a href="https://github.com/vitejs/vite/commit/571a3fd">571a3fd</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15959">#15959</a></li>
<li>fix(watch): build watch fails when outDir is empty string (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15979">#15979</a>) (<a href="https://github.com/vitejs/vite/commit/1d263d3">1d263d3</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15979">#15979</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/e710c2fc6d45405b5f3431bbe812abbb27946aa0"><code>e710c2f</code></a> release: v5.1.7</li>
<li><a href="https://github.com/vitejs/vite/commit/5a056dd2fc80dbafed033062fe6aaf4717309f48"><code>5a056dd</code></a> fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/6f7466e6211027686f40ad7e4ce6ec8477414546"><code>6f7466e</code></a> release: v5.1.6</li>
<li><a href="https://github.com/vitejs/vite/commit/a862ecb941a432b6e3bab62331012e4b53ddd4e8"><code>a862ecb</code></a> chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16131">#16131</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/840354601a2dbdb6419429999e1f9feff31a641f"><code>8403546</code></a> fix: server middleware mode resolve (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16122">#16122</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/b6fb3235c33b1490eb0d7a33b2b62d6fa7a5496f"><code>b6fb323</code></a> fix: check for publicDir before checking if it is a parent directory (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16046">#16046</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/fd9de0473e075c8d69bb3a8867ab15300506e67b"><code>fd9de04</code></a> fix(esbuild): update tsconfck to fix bug that could cause a deadlock  (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16124">#16124</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/f6991948f59e36bc5d108e2befa5883be99f934f"><code>f699194</code></a> fix: handle function property extension in namespace import (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16113">#16113</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/0d2df527168dec95b2967a3013bbf8c1ec8b0286"><code>0d2df52</code></a> style(utils): remove null check (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16112">#16112</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/eef9da13d0028161eacc0ea699988814f29a56e4"><code>eef9da1</code></a> fix(worker): throw error when circular worker import is detected and support ...</li>
<li>Additional commits viewable in <a href="https://github.com/vitejs/vite/commits/v5.1.7/packages/vite">compare view</a></li>
</ul>
</details>
<br />

Updates `pkg` from 4.5.1 to 5.8.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vercel/pkg/releases">pkg's releases</a>.</em></p>
<blockquote>
<h2>5.8.1</h2>
<h3>Patches</h3>
<ul>
<li>Producer: properly call &quot;prebuild-install&quot; if N-API is used: dd9de59c9fca2751bf5d22b57bd9b03d43e85e80</li>
<li>Chore: clean up obsolete eslint disable comments: <a href="https://redirect.github.com/vercel/pkg/issues/1760">#1760</a></li>
<li>Chore: add prettier check in linting step: <a href="https://redirect.github.com/vercel/pkg/issues/1764">#1764</a></li>
<li>Chore: separate individual test scripts: <a href="https://redirect.github.com/vercel/pkg/issues/1759">#1759</a></li>
<li>Chore: use <code>@types/babel__generator</code> package: <a href="https://redirect.github.com/vercel/pkg/issues/1755">#1755</a></li>
<li>Chore: remove unused entry: <a href="https://redirect.github.com/vercel/pkg/issues/1766">#1766</a></li>
<li>Chore: upgrade actions runners: <a href="https://redirect.github.com/vercel/pkg/issues/1767">#1767</a></li>
<li>Style: fix typo in test-99-<a href="https://redirect.github.com/vercel/pkg/issues/1192">#1192</a>/main.js: <a href="https://redirect.github.com/vercel/pkg/issues/1790">#1790</a></li>
<li>Chore: bump prebuild-install@7.1.1: <a href="https://redirect.github.com/vercel/pkg/issues/1788">#1788</a></li>
<li>Fix: add force flag to codesign to avoid already signed error: <a href="https://redirect.github.com/vercel/pkg/issues/1756">#1756</a></li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/ignatiusmb"><code>@​ignatiusmb</code></a>, <a href="https://github.com/eltociear"><code>@​eltociear</code></a>, <a href="https://github.com/PraveenAnaparthi"><code>@​PraveenAnaparthi</code></a>, and <a href="https://github.com/brianunlam"><code>@​brianunlam</code></a> for helping!</p>
<h2>5.8.0</h2>
<h2>Highlights</h2>
<ul>
<li>Support more language features, including but not limited to <code>classPrivateMethods</code> (<a href="https://redirect.github.com/vercel/pkg/issues/1248">#1248</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1249">#1249</a>)
<ul>
<li>Note: pkg uses Babel to trace dependencies. It does NOT transform your sources. You should make sure that your code can run on the target Node.js version.</li>
</ul>
</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.2 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1693">vercel/pkg#1693</a>
<ul>
<li>Add Node 14.20.0, 16.16.0 and 18.5.0 binaries</li>
<li><a href="https://nodejs.org/en/blog/vulnerability/july-2022-security-releases">https://nodejs.org/en/blog/vulnerability/july-2022-security-releases</a></li>
</ul>
</li>
<li>detector: use Babel AST and default plugins by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1648">vercel/pkg#1648</a></li>
<li>test: rearrange and fix order by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1650">vercel/pkg#1650</a></li>
<li>fix: typo in fabricator.ts by <a href="https://github.com/eltociear"><code>@​eltociear</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/eltociear"><code>@​eltociear</code></a> made their first contribution in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/vercel/pkg/compare/5.7.0...5.8.0">https://github.com/vercel/pkg/compare/5.7.0...5.8.0</a></p>
<h2>5.7.0</h2>
<h2>Highlights</h2>
<ul>
<li>Node 18 is now supported!</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.1 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1616">vercel/pkg#1616</a>
<ul>
<li>No longer take NODE_OPTIONS from the environment of the end-user. Only the users (developers who use pkg to package their project) should have control over the flags via the &quot;bake in&quot; (--options) mechanism (Fixes: <a href="https://redirect.github.com/vercel/pkg/issues/954">vercel/pkg#954</a>, <a href="https://redirect.github.com/vercel/pkg/issues/989">vercel/pkg#989</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1194">vercel/pkg#1194</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1517">vercel/pkg#1517</a>)</li>
<li>Patched Node: bump to 16.15.0, add 18.1.0 and drop 17</li>
</ul>
</li>
<li>fix broken tests on node 12; latest pnpm requires node &gt;= 14.19 by <a href="https://github.com/kldzj"><code>@​kldzj</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1613">vercel/pkg#1613</a></li>
<li>dependencies: bump (minor) by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1615">vercel/pkg#1615</a></li>
<li>fix(bootstrap): prevent to override existing node addon file by <a href="https://github.com/renkei"><code>@​renkei</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1611">vercel/pkg#1611</a></li>
</ul>
<h2>New Contributors</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vercel/pkg/commit/5dc987b90ffd191263eb0202833dc382cea0d47d"><code>5dc987b</code></a> 5.8.1</li>
<li><a href="https://github.com/vercel/pkg/commit/f19285db72f4592110f49335923d9199da49a137"><code>f19285d</code></a> fix: add force flag to codesign to avoid already signed error (<a href="https://redirect.github.com/vercel/pkg/issues/1756">#1756</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/e3ac4902e9cb023f0ac2a596e21ff9166d2e268c"><code>e3ac490</code></a> chore: bump prebuild-install@7.1.1 (<a href="https://redirect.github.com/vercel/pkg/issues/1788">#1788</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/be1123c474b3653abf3bfb89c068378f66b3849b"><code>be1123c</code></a> style: fix typo in test-99-<a href="https://redirect.github.com/vercel/pkg/issues/1192">#1192</a>/main.js (<a href="https://redirect.github.com/vercel/pkg/issues/1790">#1790</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/614c02a06830e0a4a898e6cf4eb35dbbf6110af3"><code>614c02a</code></a> chore: upgrade actions runners (<a href="https://redirect.github.com/vercel/pkg/issues/1767">#1767</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/39e99859fe2fd33fb59c4a75318389b477c1a443"><code>39e9985</code></a> chore: remove unused entry (<a href="https://redirect.github.com/vercel/pkg/issues/1766">#1766</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/b8deba40c0c9dced29e5c15aaefe575285e716d6"><code>b8deba4</code></a> chore: use <code>@types/babel__generator</code> package (<a href="https://redirect.github.com/vercel/pkg/issues/1755">#1755</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/332c7d971a6a8f918f6d24470557f2dcb1de5abf"><code>332c7d9</code></a> chore: separate individual test scripts (<a href="https://redirect.github.com/vercel/pkg/issues/1759">#1759</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/6efa7cfbbac323a019680609c2c78bbf7b9fff0f"><code>6efa7cf</code></a> chore: add prettier check in linting step (<a href="https://redirect.github.com/vercel/pkg/issues/1764">#1764</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/56135b583b901d552e3780e749e79e70e71fd3ea"><code>56135b5</code></a> chore: clean up obsolete eslint disable comments (<a href="https://redirect.github.com/vercel/pkg/issues/1760">#1760</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vercel/pkg/compare/4.5.1...5.8.1">compare view</a></li>
</ul>
</details>
<br />

Updates `@adobe/css-tools` from 4.2.0 to 4.4.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/adobe/css-tools/blob/main/History.md"><code>@​adobe/css-tools</code>'s changelog</a>.</em></p>
<blockquote>
<h1>4.4.0 / 2024-06-05</h1>
<ul>
<li>add support for <a href="https://github.com/starting-style"><code>@​starting-style</code></a> <a href="https://redirect.github.com/adobe/css-tools/issues/319">#319</a></li>
</ul>
<h1>4.3.3 / 2024-01-24</h1>
<ul>
<li>Update export property <a href="https://redirect.github.com/adobe/css-tools/issues/271">#271</a></li>
</ul>
<h1>4.3.2 / 2023-11-28</h1>
<ul>
<li>Fix redos vulnerability with specific crafted css string - CVE-2023-48631</li>
<li>Fix Problem parsing with :is() and nested :nth-child() <a href="https://redirect.github.com/adobe/css-tools/issues/211">#211</a></li>
</ul>
<h1>4.3.1 / 2023-03-14</h1>
<ul>
<li>Fix redos vulnerability with specific crafted css string - CVE-2023-26364</li>
</ul>
<h1>4.3.0 / 2023-03-07</h1>
<ul>
<li>Update build tools</li>
<li>Update exports path and files</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/adobe/css-tools/commits">compare view</a></li>
</ul>
</details>
<br />

Updates `apollo-server-core` from 3.12.0 to 3.13.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apollographql/apollo-server/commit/f93284e853efd6da46d91ae40da47a2dd15b61fe"><code>f93284e</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/4745ebed69775959212bbca7b02cff65c1f0dc64"><code>4745ebe</code></a> Rename option from disableValidation to dangerouslyDisableValidation</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/11f5981067f570c60a0003b51f3d634ebd8fa792"><code>11f5981</code></a> Add disableValidation option to apollo-server-core</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/ea2e2c3e071afc9144af00cae7b51720b9cc8b32"><code>ea2e2c3</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/1dd45b8366a6cee75e4ca321eeb5acf107e6c73e"><code>1dd45b8</code></a> get CI passing</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/d38b43bac88acdef4295759d7dcc3d4c348d9575"><code>d38b43b</code></a> Merge pull request from GHSA-j5g3-5c8r-7qfx</li>
<li>See full diff in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server-core@3.13.0/packages/apollo-server-core">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~apollo-bot">apollo-bot</a>, a new releaser for apollo-server-core since your current version.</p>
</details>
<br />

Updates `browserify-sign` from 4.2.1 to 4.2.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/browserify/browserify-sign/blob/main/CHANGELOG.md">browserify-sign's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/browserify/browserify-sign/compare/v4.2.2...v4.2.3">v4.2.3</a> - 2024-03-05</h2>
<h3>Commits</h3>
<ul>
<li>[patch] widen support to 0.12 <a href="https://github.com/browserify/browserify-sign/commit/9247adfd261ededfec1c036c9d8f36c4e9f87c0e"><code>9247adf</code></a></li>
<li>[patch] drop minimum node support to v1 <a href="https://github.com/browserify/browserify-sign/commit/4d0ee49ae2dc238b877dce9aed7e23fb4cb5088d"><code>4d0ee49</code></a></li>
<li>[Dev Deps] update <code>aud</code>, <code>npmignore</code>, <code>tape</code> <a href="https://github.com/browserify/browserify-sign/commit/87f3a35a587b377da2c1987af8d41c57b5afe0a5"><code>87f3a35</code></a></li>
<li>[actions] remove redundant finisher <a href="https://github.com/browserify/browserify-sign/commit/37a475856843b7d1b2403fdafac0024ba252e579"><code>37a4758</code></a></li>
<li>[Deps] pin <code>hash-base</code> to ~3.0, due to a breaking change <a href="https://github.com/browserify/browserify-sign/commit/9e2bf122b70970cb92f69d53e963f18299f14d66"><code>9e2bf12</code></a></li>
<li>[Deps] update <code>parse-asn1 [</code>f427270`](<a href="https://github.com/browserify/browserify-sign/commit/f427270ac11dc6be29f87d7afb046c16376a5a9c">https://github.com/browserify/browserify-sign/commit/f427270ac11dc6be29f87d7afb046c16376a5a9c</a>)</li>
<li>[Deps] update <code>elliptic</code> <a href="https://github.com/browserify/browserify-sign/commit/fb261cea57f92b3d98bc4d8bc6228c43a5de2e91"><code>fb261ce</code></a></li>
<li>[Deps] pin <code>elliptic</code> due to a breaking change <a href="https://github.com/browserify/browserify-sign/commit/168e16fcb54886a0281b0c983e1482a097042684"><code>168e16f</code></a></li>
</ul>
<h2><a href="https://github.com/browserify/browserify-sign/compare/v4.2.1...v4.2.2">v4.2.2</a> - 2023-10-25</h2>
<h3>Fixed</h3>
<ul>
<li>[Tests] log when openssl doesn't support cipher <a href="https://redirect.github.com/browserify/browserify-sign/issues/37"><code>[#37](https://github.com/crypto-browserify/browserify-sign/issues/37)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>Only apps should have lockfiles <a href="https://github.com/browserify/browserify-sign/commit/09a89959393b3c89fedd4f7f3bafa4fec44371d7"><code>09a8995</code></a></li>
<li>[eslint] switch to eslint <a href="https://github.com/browserify/browserify-sign/commit/83fe46374b819e959d56d2c0b931308f7451a664"><code>83fe463</code></a></li>
<li>[meta] add <code>npmignore</code> and <code>auto-changelog</code> <a href="https://github.com/browserify/browserify-sign/commit/44181838e7dcc4d5d0c568f74312ea28f0bcdfd5"><code>4418183</code></a></li>
<li>[meta] fix package.json indentation <a href="https://github.com/browserify/browserify-sign/commit/9ac5a5eaaac8a11eb70ec2febd13745c8764ae02"><code>9ac5a5e</code></a></li>
<li>[Tests] migrate from travis to github actions <a href="https://github.com/browserify/browserify-sign/commit/d845d855def38e2085d5a21e447a48300f99fa60"><code>d845d85</code></a></li>
<li>[Fix] <code>sign</code>: throw on unsupported padding scheme <a href="https://github.com/browserify/browserify-sign/commit/8767739a4516289568bcce9fed8a3b7e23478de9"><code>8767739</code></a></li>
<li>[Fix] properly check the upper bound for DSA signatures <a href="https://github.com/browserify/browserify-sign/commit/85994cd6348b50f2fd1b73c54e20881416f44a30"><code>85994cd</code></a></li>
<li>[Tests] handle openSSL not supporting a scheme <a href="https://github.com/browserify/browserify-sign/commit/f5f17c27f9824de40b5ce8ebd8502111203fd6af"><code>f5f17c2</code></a></li>
<li>[Deps] update <code>bn.js</code>, <code>browserify-rsa</code>, <code>elliptic</code>, <code>parse-asn1</code>, <code>readable-stream</code>, <code>safe-buffer</code> <a href="https://github.com/browserify/browserify-sign/commit/a67d0eb4ffceabb366b69da69ce9a223e9d5e96b"><code>a67d0eb</code></a></li>
<li>[Dev Deps] update <code>nyc</code>, <code>standard</code>, <code>tape</code> <a href="https://github.com/browserify/browserify-sign/commit/cc5350b96702fcba930e0662cf763844fd2f59bf"><code>cc5350b</code></a></li>
<li>[Tests] always run coverage; downgrade <code>nyc</code> <a href="https://github.com/browserify/browserify-sign/commit/75ce1d5c49a6591dd13422016c07f8f9cae13371"><code>75ce1d5</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/browserify/browserify-sign/commit/dcf49ce85a1a66a6fb31689508d916d7894286a9"><code>dcf49ce</code></a></li>
<li>[Tests] add <code>npm run posttest</code> <a href="https://github.com/browserify/browserify-sign/commit/75dd8fd6ce56eb37b12e30807e5f913867b21733"><code>75dd8fd</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/browserify/browserify-sign/commit/3aec0386dc8dfba8698be756ec770df863867c84"><code>3aec038</code></a></li>
<li>[Tests] skip unsupported schemes <a href="https://github.com/browserify/browserify-sign/commit/703c83ea72db2f45714fe749c6f04b05243ca9a8"><code>703c83e</code></a></li>
<li>[Tests] node &lt; 6 lacks array <code>includes</code> <a href="https://github.com/browserify/browserify-sign/commit/3aa43cfbc1fdde8481bcdd3bff581574159b869a"><code>3aa43cf</code></a></li>
<li>[Dev Deps] fix eslint range <a href="https://github.com/browserify/browserify-sign/commit/98d4e0d7ff18871b0ca07415f758a610ccf8ebbe"><code>98d4e0d</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/browserify/browserify-sign/commit/bf2c3ec8fa046a52420ccd322186cc477d82165c"><code>bf2c3ec</code></a> v4.2.3</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/9247adfd261ededfec1c036c9d8f36c4e9f87c0e"><code>9247adf</code></a> [patch] widen support to 0.12</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/f427270ac11dc6be29f87d7afb046c16376a5a9c"><code>f427270</code></a> [Deps] update `parse-asn1</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/87f3a35a587b377da2c1987af8d41c57b5afe0a5"><code>87f3a35</code></a> [Dev Deps] update <code>aud</code>, <code>npmignore</code>, <code>tape</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/fb261cea57f92b3d98bc4d8bc6228c43a5de2e91"><code>fb261ce</code></a> [Deps] update <code>elliptic</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/4d0ee49ae2dc238b877dce9aed7e23fb4cb5088d"><code>4d0ee49</code></a> [patch] drop minimum node support to v1</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/9e2bf122b70970cb92f69d53e963f18299f14d66"><code>9e2bf12</code></a> [Deps] pin <code>hash-base</code> to ~3.0, due to a breaking change</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/168e16fcb54886a0281b0c983e1482a097042684"><code>168e16f</code></a> [Deps] pin <code>elliptic</code> due to a breaking change</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/37a475856843b7d1b2403fdafac0024ba252e579"><code>37a4758</code></a> [actions] remove redundant finisher</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/4af5a90bf8acd9e76e5671dc0497f6ba71968a2c"><code>4af5a90</code></a> v4.2.2</li>
<li>Additional commits viewable in <a href="https://github.com/crypto-browserify/browserify-sign/compare/v4.2.1...v4.2.3">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for browserify-sign since your current version.</p>
</details>
<br />

Updates `es5-ext` from 0.10.53 to 0.10.64
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/medikoo/es5-ext/releases">es5-ext's releases</a>.</em></p>
<blockquote>
<h2>0.10.64 (2024-02-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Revert update to postinstall script meant to fix Powershell issue, as it's a regression for some Linux terminals (<a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a">c2e2bb9</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.63...v0.10.64">Comparison since last release</a></p>
<h2>0.10.63 (2024-02-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Do not rely on problematic regex (<a href="https://github.com/medikoo/es5-ext/commit/3551cdd7b2db08b1632841f819d008757d28e8e2">3551cdd</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/201">#201</a></li>
<li>Support ES2015+ function definitions in <code>function#toStringTokens()</code> (<a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602">a52e957</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/021">#021</a></li>
<li>Ensure postinstall script does not crash on Windows, fixes <a href="https://redirect.github.com/medikoo/es5-ext/issues/181">#181</a> (<a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f">bf8ed79</a>)</li>
</ul>
<h3>Maintenance Improvements</h3>
<ul>
<li>Simplify the manifest message (<a href="https://github.com/medikoo/es5-ext/commit/7855319f41b9736639cf4555bd2c419f17addf55">7855319</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.63">Comparison since last release</a></p>
<h2>0.10.62 (2022-08-02)</h2>
<h3>Maintenance Improvements</h3>
<ul>
<li><strong>Manifest improvements:</strong>
<ul>
<li>(<a href="https://redirect.github.com/medikoo/es5-ext/issues/190">#190</a>) (<a href="https://github.com/medikoo/es5-ext/commit/b8dc53fa439b98541644c64c1275f25d9f2e2235">b8dc53f</a>)</li>
<li>(<a href="https://github.com/medikoo/es5-ext/commit/c51d552c03967858b8f14a4afa305338ba648cce">c51d552</a>)</li>
</ul>
</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.61...v0.10.62">Comparison since last release</a></p>
<h2>0.10.61 (2022-04-20)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Ensure postinstall script does not error (<a href="https://github.com/medikoo/es5-ext/commit/a0be4fdacdbc3aefd6f2952b7b9215827d362bbb">a0be4fd</a>)</li>
</ul>
<h3>Maintenance Improvements</...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-10 22:26:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3303" class=".btn">#3303</a>
            </td>
            <td>
                <b>
                    ci(github): add workflow for DCO check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-10 17:21:25 +0000 UTC
    </div>
</div>

