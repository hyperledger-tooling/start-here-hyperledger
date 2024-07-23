---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/774" class=".btn">#774</a>
            </td>
            <td>
                <b>
                    Allow for `lite` plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow for `lite` plugins to be listed in a text file and these will be skipped by the integration test management script and CI/CD workflows.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 15:54:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/772" class=".btn">#772</a>
            </td>
            <td>
                <b>
                    Modular credential format support for oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR, we've restructured the OID4VCI plugin by extracting the JWT credential issuance logic and moving it to a new JWT_VC_JSON plugin. This adjustment enables the OID4VCI plugin to concentrate exclusively on the protocol, eliminating the need to process individual credential formats. This modular approach simplifies the addition of new credential formats in the future without requiring changes to the OID4VCI plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 22:21:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/771" class=".btn">#771</a>
            </td>
            <td>
                <b>
                    Library upgrades
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Weekly group upgrades for the libraries reported by dependabot.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 19:51:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/770" class=".btn">#770</a>
            </td>
            <td>
                <b>
                    fix: debug value in cred id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a quick fix for a debug value mistakenly committed in #768.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 17:47:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/769" class=".btn">#769</a>
            </td>
            <td>
                <b>
                    Bump the npm_and_yarn group across 1 directory with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 4 updates in the /oid4vci/integration/credo directory: [semver](https://github.com/npm/node-semver), [expo](https://github.com/expo/expo/tree/HEAD/packages/expo), [ws](https://github.com/websockets/ws) and [braces](https://github.com/micromatch/braces).

Updates `semver` from 5.7.2 to 7.6.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.6.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.4...v7.6.0">7.6.0</a> (2024-01-31)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/a7ab13a46201e342d34e84a989632b380f755baf"><code>a7ab13a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/671">#671</a> preserve pre-release and build parts of a version on coerce (<a href="https://redirect.github.com/npm/node-semver/issues/671">#671</a>) (<a href="https://github.com/madtisa"><code>@​madtisa</code></a>, madtisa, <a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
</ul>
<h3>Chores</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/816c7b2cbfcb1986958a290f941eddfd0441139e"><code>816c7b2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/0bd24d943cbd1a7f6a2b8d384590bfa98559e1de"><code>0bd24d9</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> bump <code>@​npmcli/template-oss</code> from 4.21.1 to 4.21.3 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/e521932f115a81030f4e7c34e8631cdd3c6a108b"><code>e521932</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/88739918080debeb239aae840b35c07436148e50"><code>8873991</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> chore: chore: postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/f317dc8689781bcfd98e2c32b46157276acdd47c"><code>f317dc8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> bump <code>@​npmcli/template-oss</code> from 4.19.0 to 4.21.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/7303db1fe54d6905b23ccb0162878e37d73535ef"><code>7303db1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/658">#658</a> add clean() test for build metadata (<a href="https://redirect.github.com/npm/node-semver/issues/658">#658</a>) (<a href="https://github.com/jethrodaniel"><code>@​jethrodaniel</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6240d75a7c620b0a222f05969a91fdc3dc2be0fb"><code>6240d75</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/656">#656</a> add missing quotes in README.md (<a href="https://redirect.github.com/npm/node-semver/issues/656">#656</a>) (<a href="https://github.com/zyxkad"><code>@​zyxkad</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/14d263faa156e408a033b9b12a2f87735c2df42c"><code>14d263f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/7c34e1ac1bcc0bc6579b30745c96075c69bd0332"><code>7c34e1a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> bump <code>@​npmcli/template-oss</code> from 4.18.1 to 4.19.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/123e0b03287e1af295ef82d55f55c16805596f35"><code>123e0b0</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/737d5e1cf10e631bab8a28594aa2d5c9d4090814"><code>737d5e1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> bump <code>@​npmcli/template-oss</code> from 4.18.0 to 4.18.1 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/cce61804ba6f997225a1267135c06676fe0524d2"><code>cce6180</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/b914a3d0d26ca27d2685053d7d390af4e02eedd9"><code>b914a3d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> bump <code>@​npmcli/template-oss</code> from 4.17.0 to 4.18.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
</ul>
<h2>v7.5.4</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.4...v7.6.0">7.6.0</a> (2024-01-31)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/a7ab13a46201e342d34e84a989632b380f755baf"><code>a7ab13a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/671">#671</a> preserve pre-release and build parts of a version on coerce (<a href="https://redirect.github.com/npm/node-semver/issues/671">#671</a>) (<a href="https://github.com/madtisa"><code>@​madtisa</code></a>, madtisa, <a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
</ul>
<h3>Chores</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/816c7b2cbfcb1986958a290f941eddfd0441139e"><code>816c7b2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/0bd24d943cbd1a7f6a2b8d384590bfa98559e1de"><code>0bd24d9</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> bump <code>@​npmcli/template-oss</code> from 4.21.1 to 4.21.3 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/e521932f115a81030f4e7c34e8631cdd3c6a108b"><code>e521932</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/88739918080debeb239aae840b35c07436148e50"><code>8873991</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> chore: chore: postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/f317dc8689781bcfd98e2c32b46157276acdd47c"><code>f317dc8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> bump <code>@​npmcli/template-oss</code> from 4.19.0 to 4.21.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/7303db1fe54d6905b23ccb0162878e37d73535ef"><code>7303db1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/658">#658</a> add clean() test for build metadata (<a href="https://redirect.github.com/npm/node-semver/issues/658">#658</a>) (<a href="https://github.com/jethrodaniel"><code>@​jethrodaniel</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6240d75a7c620b0a222f05969a91fdc3dc2be0fb"><code>6240d75</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/656">#656</a> add missing quotes in README.md (<a href="https://redirect.github.com/npm/node-semver/issues/656">#656</a>) (<a href="https://github.com/zyxkad"><code>@​zyxkad</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/14d263faa156e408a033b9b12a2f87735c2df42c"><code>14d263f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/7c34e1ac1bcc0bc6579b30745c96075c69bd0332"><code>7c34e1a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> bump <code>@​npmcli/template-oss</code> from 4.18.1 to 4.19.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/123e0b03287e1af295ef82d55f55c16805596f35"><code>123e0b0</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/737d5e1cf10e631bab8a28594aa2d5c9d4090814"><code>737d5e1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> bump <code>@​npmcli/template-oss</code> from 4.18.0 to 4.18.1 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/cce61804ba6f997225a1267135c06676fe0524d2"><code>cce6180</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/b914a3d0d26ca27d2685053d7d390af4e02eedd9"><code>b914a3d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> bump <code>@​npmcli/template-oss</code> from 4.17.0 to 4.18.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/377f709718053a477ed717089c4403c4fec332a1"><code>377f709</code></a> chore: release 7.6.0 (<a href="https://redirect.github.com/npm/node-semver/issues/661">#661</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/a7ab13a46201e342d34e84a989632b380f755baf"><code>a7ab13a</code></a> feat: preserve pre-release and build parts of a version on coerce (<a href="https://redirect.github.com/npm/node-semver/issues/671">#671</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/816c7b2cbfcb1986958a290f941eddfd0441139e"><code>816c7b2</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/0bd24d943cbd1a7f6a2b8d384590bfa98559e1de"><code>0bd24d9</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.21.1 to 4.21.3</li>
<li><a href="https://github.com/npm/node-semver/commit/e521932f115a81030f4e7c34e8631cdd3c6a108b"><code>e521932</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/88739918080debeb239aae840b35c07436148e50"><code>8873991</code></a> chore: chore: chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/f317dc8689781bcfd98e2c32b46157276acdd47c"><code>f317dc8</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.19.0 to 4.21.0</li>
<li><a href="https://github.com/npm/node-semver/commit/7303db1fe54d6905b23ccb0162878e37d73535ef"><code>7303db1</code></a> chore: add clean() test for build metadata (<a href="https://redirect.github.com/npm/node-semver/issues/658">#658</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6240d75a7c620b0a222f05969a91fdc3dc2be0fb"><code>6240d75</code></a> chore: add missing quotes in README.md (<a href="https://redirect.github.com/npm/node-semver/issues/656">#656</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/14d263faa156e408a033b9b12a2f87735c2df42c"><code>14d263f</code></a> chore: postinstall for dependabot template-oss PR</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v5.7.2...v7.6.0">compare view</a></li>
</ul>
</details>
<br />

Updates `expo` from 50.0.17 to 51.0.20
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expo/expo/blob/main/CHANGELOG.md">expo's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<p>This is the log of notable changes to the Expo client that are developer-facing.
Package-specific changes not released in any SDK will be added here just before the release. Until then, you can find them in changelogs of the individual packages (see <a href="https://github.com/expo/expo/blob/main/packages">packages</a> directory).</p>
<h2>Unpublished</h2>
<h3>📚 3rd party library updates</h3>
<h3>🛠 Breaking changes</h3>
<h3>🎉 New features</h3>
<h3>🐛 Bug fixes</h3>
<h2>51.0.0 — 2024-05-07</h2>
<h3>🛠 Breaking changes</h3>
<ul>
<li><strong><code>expo-auth-session</code></strong>
<ul>
<li>Drop deprecated <code>expoClientId</code> field from auth proxy. (<a href="https://redirect.github.com/expo/expo/pull/28590">#28590</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-barcode-scanner</code></strong>
<ul>
<li><code>expo-barcode-scanner</code> is now deprecated. Please use <code>expo-camera</code> instead. (<a href="https://redirect.github.com/expo/expo/pull/26025">#26025</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-constants</code></strong>
<ul>
<li>Remove deprecated installationId, isDevice, nativeAppVersion, nativeBuildVersion, platform.platform, platform.systemVersion, platform.userInterfaceIdiom properties. (<a href="https://redirect.github.com/expo/expo/pull/26329">#26329</a> by <a href="https://github.com/aleqsio"><code>@​aleqsio</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-face-detector</code></strong>
<ul>
<li><code>expo-face-detector</code> is now deprecated. We recommed using <a href="https://github.com/mrousavy/react-native-vision-camera">react-native-vision-camera</a> instead. (<a href="https://redirect.github.com/expo/expo/pull/26026">#26026</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-location</code></strong>
<ul>
<li>[Web] <code>getPermissionsAsync</code> no longer prompts the user for permission instead we use the new browser API <code>navigator.permissions.query</code> to check the permission status. (<a href="https://redirect.github.com/expo/expo/pull/26837">#26836</a> by <a href="https://github.com/hems"><code>@​hems</code></a>) (<a href="https://redirect.github.com/expo/expo/pull/26837">#26837</a> by <a href="https://github.com/hems"><code>@​hems</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-local-authentication</code></strong>
<ul>
<li><code>SecurityLevel.BIOMETRIC</code> has been deprecated in favour of <code>SecurityLevel.BIOMETRIC_STRONG</code> and <code>SecurityLevel.BIOMETRIC_WEAK</code>. Using <code>SecurityLevel.BIOMETRIC</code> might lead to unexpected behaviour. (<a href="https://redirect.github.com/expo/expo/pull/26768">#26768</a> by <a href="https://github.com/behenate"><code>@​behenate</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-modules-core</code></strong>
<ul>
<li>Removed <code>ReactNativeHostHandler.onRegisterJSIModules</code> interface. (<a href="https://redirect.github.com/expo/expo/pull/26357">#26357</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
<li>Dropped supports for React Native 0.73 and lower. (<a href="https://redirect.github.com/expo/expo/pull/27601">#27601</a>, <a href="https://redirect.github.com/expo/expo/pull/27689">#27689</a>, <a href="https://redirect.github.com/expo/expo/pull/27629">#27629</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-sms</code></strong>
<ul>
<li>[web] <code>sendSMSAsync</code> now throws error code <code>ERR_UNAVAILABLE</code> instead of <code>E_SMS_UNAVAILABLE</code>. (<a href="https://redirect.github.com/expo/expo/pull/27437">#27437</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-sqlite</code></strong>
<ul>
<li>Refactor <code>expo-sqlite/next</code> API to be more React idiomatic. (<a href="https://redirect.github.com/expo/expo/pull/25657">#25657</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
<li>Moved the previous default export as <code>expo-sqlite/legacy</code> and promoted <code>expo-sqlite/next</code> as the default. <code>expo-sqlite/next</code> import is still as-is for backward compatibility. (<a href="https://redirect.github.com/expo/expo/pull/28278">#28278</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
</ul>
</li>
</ul>
<h3>🎉 New features</h3>
<ul>
<li><strong><code>expo-barcode-scanner</code></strong>
<ul>
<li><code>BarCodeScannerResult</code> now returns an additional <code>raw</code> field corresponding to the barcode value as it was encoded in the barcode without parsing. Will always be undefined on iOS. (<a href="https://redirect.github.com/expo/expo/pull/25391">#25391</a> by <a href="https://github.com/ajacquierbret"><code>@​ajacquierbret</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-blur</code></strong>
<ul>
<li>Added support for Apple tvOS. (<a href="https://redirect.github.com/expo/expo/pull/26965">#26965</a> by <a href="https://github.com/douglowder"><code>@​douglowder</code></a>)</li>
<li>Mark React client components with &quot;use client&quot; directives. (<a href="https://redirect.github.com/expo/expo/pull/27300">#27300</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-asset</code></strong>
<ul>
<li>Added config plugin to allow assets to be linked at build time. (<a href="https://redirect.github.com/expo/expo/pull/27052">#27052</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
<li>Add Apple TV support to the new iOS native module. (<a href="https://redirect.github.com/expo/expo/pull/27823">#27823</a> by <a href="https://github.com/douglowder"><code>@​douglowder</code></a>)</li>
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
<li>See full diff in <a href="https://github.com/expo/expo/commits/HEAD/packages/expo">compare view</a></li>
</ul>
</details>
<br />

Updates `ws` from 6.2.2 to 6.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>6.2.3</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 6.x release line (eeb76d31).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d87f3b6d3a00513af9bbb74f45ba9183af4e5f43"><code>d87f3b6</code></a> [dist] 6.2.3</li>
<li><a href="https://github.com/websockets/ws/commit/eeb76d313e2a00dd5247ca3597bba7877d064a63"><code>eeb76d3</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/6.2.2...6.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `braces` from 3.0.2 to 3.0.3
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/micromatch/braces/commit/74b2db2938fad48a2ea54a9c8bf27a37a62c350d"><code>74b2db2</code></a> 3.0.3</li>
<li><a href="https://github.com/micromatch/braces/commit/88f1429a0f47e1dd3813de35211fc97ffda27f9e"><code>88f1429</code></a> update eslint. lint, fix unit tests.</li>
<li><a href="https://github.com/micromatch/braces/commit/415d660c3002d1ab7e63dbf490c9851da80596ff"><code>415d660</code></a> Snyk js braces 6838727 (<a href="https://redirect.github.com/micromatch/braces/issues/40">#40</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/190510f79db1adf21d92798b0bb6fccc1f72c9d6"><code>190510f</code></a> fix tests, skip 1 test in test/braces.expand</li>
<li><a href="https://github.com/micromatch/braces/commit/716eb9f12d820b145a831ad678618731927e8856"><code>716eb9f</code></a> readme bump</li>
<li><a href="https://github.com/micromatch/braces/commit/a5851e57f45c3431a94d83fc565754bc10f5bbc3"><code>a5851e5</code></a> Merge pull request <a href="https://redirect.github.com/micromatch/braces/issues/37">#37</a> from coderaiser/fix/vulnerability</li>
<li><a href="https://github.com/micromatch/braces/commit/2092bd1fb108d2c59bd62e243b70ad98db961538"><code>2092bd1</code></a> feature: braces: add maxSymbols (<a href="https://github.com/micromatch/braces/issues/">https://github.com/micromatch/braces/issues/</a>...</li>
<li><a href="https://github.com/micromatch/braces/commit/9f5b4cf47329351bcb64287223ffb6ecc9a5e6d3"><code>9f5b4cf</code></a> fix: vulnerability (<a href="https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727">https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/98414f9f1fabe021736e26836d8306d5de747e0d"><code>98414f9</code></a> remove funding file</li>
<li><a href="https://github.com/micromatch/braces/commit/665ab5d561c017a38ba7aafd92cc6655b91d8c14"><code>665ab5d</code></a> update keepEscaping doc (<a href="https://redirect.github.com/micromatch/braces/issues/27">#27</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/micromatch/braces/compare/3.0.2...3.0.3">compare view</a></li>
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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 17:09:02 +0000 UTC
    </div>
</div>

