---
layout: default
title: acapy-java-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/acapy-java-client
---

# acapy-java-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/acapy-java-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    fix for ledger roles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 21:40:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    [#33] Cannot register NYM with /ledger/register-nym
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 20:34:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    web socket listener and exception handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 15:49:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    tenant aware event handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 10:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Add support for WebSocket/Webhook topic='settings'
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
        Created At 2022-04-13 09:27:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Bump actions/setup-java from 2 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-java](https://github.com/actions/setup-java) from 2 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-java/releases">actions/setup-java's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<p>In scope of this release we changed version of the runtime Node.js for the setup-java action and updated package-lock.json file to  v2.</p>
<h3>Breaking Changes</h3>
<p>With the update to Node 16 in <a href="https://github-redirect.dependabot.com/actions/setup-java/pull/290">#290</a>, all scripts will now be run with Node 16 rather than Node 12.</p>
<h2>v2.5.0</h2>
<p>In scope of this pull request we add support for Microsoft Build of OpenJDK (<a href="https://github-redirect.dependabot.com/actions/setup-java/pull/252">actions/setup-java#252</a>).</p>
<pre lang="yaml"><code>steps:
  - name: Checkout
    uses: actions/checkout@v2
  - name: Setup-java
    uses: actions/setup-java@v2
    with:
      distribution: microsoft
      java-version: 11
</code></pre>
<h3>Supported distributions</h3>
<p>Currently, the following distributions are supported:</p>
<table>
<thead>
<tr>
<th>Keyword</th>
<th>Distribution</th>
<th>Official site</th>
<th>License</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>temurin</code></td>
<td>Eclipse Temurin</td>
<td><a href="https://adoptium.net/">Link</a></td>
<td><a href="https://adoptium.net/about.html">Link</a></td>
</tr>
<tr>
<td><code>zulu</code></td>
<td>Zulu OpenJDK</td>
<td><a href="https://www.azul.com/downloads/zulu-community/?package=jdk">Link</a></td>
<td><a href="https://www.azul.com/products/zulu-and-zulu-enterprise/zulu-terms-of-use/">Link</a></td>
</tr>
<tr>
<td><code>adopt</code> or <code>adopt-hotspot</code></td>
<td>Adopt OpenJDK Hotspot</td>
<td><a href="https://adoptopenjdk.net/">Link</a></td>
<td><a href="https://adoptopenjdk.net/about.html">Link</a></td>
</tr>
<tr>
<td><code>adopt-openj9</code></td>
<td>Adopt OpenJDK OpenJ9</td>
<td><a href="https://adoptopenjdk.net/">Link</a></td>
<td><a href="https://adoptopenjdk.net/about.html">Link</a></td>
</tr>
<tr>
<td><code>liberica</code></td>
<td>Liberica JDK</td>
<td><a href="https://bell-sw.com/">Link</a></td>
<td><a href="https://bell-sw.com/liberica_eula/">Link</a></td>
</tr>
<tr>
<td><code>microsoft</code></td>
<td>Microsoft Build of OpenJDK</td>
<td><a href="https://www.microsoft.com/openjdk">Link</a></td>
<td><a href="https://docs.microsoft.com/java/openjdk/faq">Link</a></td>
</tr>
</tbody>
</table>
<h2>v2.4.0</h2>
<p>In scope of this pull request we add support for Liberica JDK (<a href="https://github-redirect.dependabot.com/actions/setup-java/pull/225">actions/setup-java#225</a>).</p>
<pre lang="yaml"><code>steps:
  - name: Checkout
    uses: actions/checkout@v2
  - name: Setup-java
    uses: actions/setup-java@v2
    with:
      distribution: liberica
      java-version: 11
</code></pre>
<h3>Supported distributions</h3>
<p>Currently, the following distributions are supported:</p>
<table>
<thead>
<tr>
<th>Keyword</th>
<th>Distribution</th>
<th>Official site</th>
<th>License</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>zulu</code></td>
<td>Zulu OpenJDK</td>
<td><a href="https://www.azul.com/downloads/zulu-community/?package=jdk">Link</a></td>
<td><a href="https://www.azul.com/products/zulu-and-zulu-enterprise/zulu-terms-of-use/">Link</a></td>
</tr>
<tr>
<td><code>adopt</code> or <code>adopt-hotspot</code></td>
<td>Adopt OpenJDK Hotspot</td>
<td><a href="https://adoptopenjdk.net/">Link</a></td>
<td><a href="https://adoptopenjdk.net/about.html">Link</a></td>
</tr>
<tr>
<td><code>adopt-openj9</code></td>
<td>Adopt OpenJDK OpenJ9</td>
<td><a href="https://adoptopenjdk.net/">Link</a></td>
<td><a href="https://adoptopenjdk.net/about.html">Link</a></td>
</tr>
<tr>
<td><code>temurin</code></td>
<td>Eclipse Temurin</td>
<td><a href="https://adoptium.net/">Link</a></td>
<td><a href="https://adoptium.net/about.html">Link</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-java/commit/0aa6f2a84f8634ac1a1bd81dfdf6d5aab98c70f1"><code>0aa6f2a</code></a> Bump minimist from 1.2.5 to 1.2.6 (<a href="https://github-redirect.dependabot.com/actions/setup-java/issues/303">#303</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/dc1a9f27915005c4867178213f98cc27415de97a"><code>dc1a9f2</code></a> Caching on GHES (<a href="https://github-redirect.dependabot.com/actions/setup-java/issues/308">#308</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/e886040dc21d1d2c3f71482e1b6518445ef5e620"><code>e886040</code></a> Update zulu-installer.test.ts (<a href="https://github-redirect.dependabot.com/actions/setup-java/issues/310">#310</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/efbea1411b18823f99d704f247a3090511af93db"><code>efbea14</code></a> Update util.ts</li>
<li><a href="https://github.com/actions/setup-java/commit/c41070eda4f4d598540a89ad4a0e333b2b5bba07"><code>c41070e</code></a> Update util.ts</li>
<li><a href="https://github.com/actions/setup-java/commit/f69f00b5e5324696b07f6b1c92f0470a6df00780"><code>f69f00b</code></a> Update lockfileVersion (<a href="https://github-redirect.dependabot.com/actions/setup-java/issues/293">#293</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/2e1dfa1fb43424fa6465aaeacd047e9ef2f69961"><code>2e1dfa1</code></a> Update Default runtime to node16 (<a href="https://github-redirect.dependabot.com/actions/setup-java/issues/290">#290</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/a12e082d834968c1847f782019214fadd20719f6"><code>a12e082</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-java/issues/224">#224</a> from KengoTODA/remove-husky</li>
<li><a href="https://github.com/actions/setup-java/commit/04d53533c260c5d4b63a5c354d85d12ee217ebd6"><code>04d5353</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-java/issues/215">#215</a> from beatngu13/update-readme-cache-key</li>
<li><a href="https://github.com/actions/setup-java/commit/d8da887cad432a14fdb5025b0f7ebde23972b258"><code>d8da887</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-java/issues/196">#196</a> from oscard0m/add-cache-to-node-workflows</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-java/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-java&package-manager=github_actions&previous-version=2&new-version=3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-08 14:20:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    added test to connect two multi ledger sub wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 08:52:36 +0000 UTC
    </div>
</div>

