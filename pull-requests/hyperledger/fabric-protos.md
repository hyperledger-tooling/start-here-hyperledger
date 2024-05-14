---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Bump the bundler group across 1 directory with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps the bundler group with 2 updates in the /docs directory: [activesupport](https://github.com/rails/rails) and [nokogiri](https://github.com/sparklemotion/nokogiri).

Updates `activesupport` from 6.0.4.7 to 6.0.6.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rails/rails/releases">activesupport's releases</a>.</em></p>
<blockquote>
<h2>v6.0.6.1</h2>
<h2>Active Support</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Active Model</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Active Record</h2>
<ul>
<li>
<p>Make <code>sanitize_as_sql_comment</code> more strict</p>
<p>Though this method was likely never meant to take user input, it was
attempting sanitization. That sanitization could be bypassed with
carefully crafted input.</p>
<p>This commit makes the sanitization more robust by replacing any
occurrances of &quot;/<em>&quot; or &quot;</em>/&quot; with &quot;/ <em>&quot; or &quot;</em> /&quot;. It also performs a
first pass to remove one surrounding comment to avoid compatibility
issues for users relying on the existing removal.</p>
<p>This also clarifies in the documentation of annotate that it should not
be provided user input.</p>
<p>[CVE-2023-22794]</p>
</li>
</ul>
<h2>Action View</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Action Pack</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Active Job</h2>
<ul>
<li>No changes.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rails/rails/commit/28bb76d3efc39b2ef663dfe2346f7c2621343cd6"><code>28bb76d</code></a> Version 6.0.6.1</li>
<li><a href="https://github.com/rails/rails/commit/91cf62e7b43c33ae6263adf3d7563da9b68ff21d"><code>91cf62e</code></a> Version 6.0.6</li>
<li><a href="https://github.com/rails/rails/commit/c7d64e91b65d3633146e37c65ad5211352d60a69"><code>c7d64e9</code></a> Preparing for 6.0.5.1 release</li>
<li><a href="https://github.com/rails/rails/commit/c177e45858ebecbdb0782b6f25e538054794277b"><code>c177e45</code></a> updating version and changelog</li>
<li><a href="https://github.com/rails/rails/commit/433115554d3ea0b4dab9df99548c47707cadb20d"><code>4331155</code></a> Preparing for 6.0.5 release</li>
<li><a href="https://github.com/rails/rails/commit/1b5df893d82a27da907e9b8b75deff13179d1df3"><code>1b5df89</code></a> Merge pull request <a href="https://redirect.github.com/rails/rails/issues/45027">#45027</a> from rails/fix-tag-helper-regression</li>
<li><a href="https://github.com/rails/rails/commit/23f8485dced9be73877ae98a6554c7d34156866b"><code>23f8485</code></a> Merge branch '6-0-sec' into 6-0-stable</li>
<li><a href="https://github.com/rails/rails/commit/27a5ec76eed1e5d0bc5649b0e92097267c0b4338"><code>27a5ec7</code></a> Preparing for 6.0.4.8 release</li>
<li><a href="https://github.com/rails/rails/commit/636ee650d4a4edfca8ab6f2e982b543951976a59"><code>636ee65</code></a> updating changelog for release</li>
<li><a href="https://github.com/rails/rails/commit/36a6dad07d572a0098c29d6d96a226638a7caa38"><code>36a6dad</code></a> Fix and add protections for XSS in names.</li>
<li>Additional commits viewable in <a href="https://github.com/rails/rails/compare/v6.0.4.7...v6.0.6.1">compare view</a></li>
</ul>
</details>
<br />

Updates `nokogiri` from 1.16.2 to 1.16.5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/releases">nokogiri's releases</a>.</em></p>
<blockquote>
<h2>v1.16.5 / 2024-05-13</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address CVE-2024-34459. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-r95h-9x8f-r3f7">GHSA-r95h-9x8f-r3f7</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.12.7">v2.12.7</a> from v2.12.6. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre><code>af0f44fa3e664dfb2aa10de8b551447d720c1e8d1f0aa3f35783dcc43e40a874  nokogiri-1.16.5-aarch64-linux.gem
23dc2357b26409a5c33b7e32a82902f0e9995305420f16d1a03ab3ea1a482fec  nokogiri-1.16.5-arm-linux.gem
950d037530edb49f75ad35de0b8038b970a7dda57e2b6326895b0e49fadf6214  nokogiri-1.16.5-arm64-darwin.gem
b7aefc94370c62476b8528e8d8abb6160203abd84a1f4eceda8f1aa8974d9989  nokogiri-1.16.5-java.gem
ec2167160df8fec3137bf95d574ed80ebc1d002bb3b281546b60b4aa9002466e  nokogiri-1.16.5-x64-mingw-ucrt.gem
6984200491fac69974005ecfa2de129d61843d345eafa5d6f58e8b908d1cf107  nokogiri-1.16.5-x64-mingw32.gem
abdc389ab1ec6604492da16bd9d06ad746fdb6bd6a1bd274c400d61ffcadb3c4  nokogiri-1.16.5-x86-linux.gem
63d24981345856f2baf7f4089870a62d3042fb8d3021b280fb04fc052532e3c4  nokogiri-1.16.5-x86-mingw32.gem
71b5f54e378c433d13df67c3b71acc4716129da62402d8181f310c4216a63279  nokogiri-1.16.5-x86_64-darwin.gem
0ca238da870066bed2f7837af6f35791bb9b76c4c5638999c46aac44818a6a97  nokogiri-1.16.5-x86_64-linux.gem
ec36162c68984fa0a90a5c4ae7ab7759460639e716cc1ce75f34c3cb54158ad2  nokogiri-1.16.5.gem
</code></pre>
<h2>v1.16.4 / 2024-04-10</h2>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored zlib in the precompiled native gems is updated to <a href="https://zlib.net/ChangeLog.txt">v1.3.1</a> from v1.3. Nokogiri is not affected by the minizip CVE patched in this version, but this update may satisfy some security scanners. Related, see <a href="https://github.com/sparklemotion/nokogiri/discussions/3168">this discussion</a> about removing the compression libraries altogether in a future version of Nokogiri.</li>
</ul>
<hr />
<p>sha256 checksums:</p>
<pre><code>bdb1dc4378ebcf3ade8f440c7df68f6d76946a1a96c4823a2b4c53c01a320cd5  nokogiri-1.16.4-aarch64-linux.gem
0c994b9996d5576eddcc3201a94ef2bff6fc3627c4ae4d2708b0ec9b9743ec6a  nokogiri-1.16.4-arm-linux.gem
8e86abb64c93c06d3c588042a0e757279e8f1dc88b5210a00be892a9a7a27196  nokogiri-1.16.4-arm64-darwin.gem
bf84fa28be4943692bd64772186e0832fb1061f80714ccb93e111e9d72b1cadc  nokogiri-1.16.4-java.gem
a46808467c1f63a2031e1ca0715cd5336bb4ec759e9c0e2f4c951c1cc30994ae  nokogiri-1.16.4-x64-mingw-ucrt.gem
4cdf64bc5e9443ec3e0b595347ecc8affe21968d9ae934c0825d26630ef96468  nokogiri-1.16.4-x64-mingw32.gem
d86d21bae47dd9f6f5223055e45d33fae08b0b89aad94cbc0ece4f4274fa7af5  nokogiri-1.16.4-x86-linux.gem
d488b872884844686780fda7cf5da44ee884d32faa713a55aeb4736d76718168  nokogiri-1.16.4-x86-mingw32.gem
a896e52a56951ffb0e6a9279afbf485d683e357a053d27f4cfcb2a73b0824628  nokogiri-1.16.4-x86_64-darwin.gem
92ff4f09910255fec84b3bc4c4b182e94cada3ed12b9f7a6ea058e0af186fb31  nokogiri-1.16.4-x86_64-linux.gem
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sparklemotion/nokogiri/blob/main/CHANGELOG.md">nokogiri's changelog</a>.</em></p>
<blockquote>
<h2>v1.16.5</h2>
<h3>Security</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to address CVE-2024-34459. See <a href="https://github.com/sparklemotion/nokogiri/security/advisories/GHSA-r95h-9x8f-r3f7">GHSA-r95h-9x8f-r3f7</a> for more information.</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.12.7">v2.12.7</a> from v2.12.6. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
</ul>
<h2>v1.16.4 / 2024-04-10</h2>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored zlib in the precompiled native gems is updated to <a href="https://zlib.net/ChangeLog.txt">v1.3.1</a> from v1.3. Nokogiri is not affected by the minizip CVE patched in this version, but this update may satisfy some security scanners. Related, see <a href="https://github.com/sparklemotion/nokogiri/discussions/3168">this discussion</a> about removing the compression libraries altogether in a future version of Nokogiri.</li>
</ul>
<h2>v1.16.3 / 2024-03-15</h2>
<h3>Dependencies</h3>
<ul>
<li>[CRuby] Vendored libxml2 is updated to <a href="https://gitlab.gnome.org/GNOME/libxml2/-/releases/v2.12.6">v2.12.6</a> from v2.12.5. (<a href="https://github.com/flavorjones"><code>@​flavorjones</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>[CRuby] <code>XML::Reader</code> sets the <code>@encoding</code> instance variable during reading if it is not passed into the initializer. Previously, it would remain <code>nil</code>. The behavior of <code>Reader#encoding</code> has not changed. This works around changes to how libxml2 reports the encoding used in v2.12.6.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/cd70bd3dc9e0dc15b04b42d67b639eb5804e77d5"><code>cd70bd3</code></a> version bump to v1.16.5</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/afc36de553085b6b397b23a0c09a2449655a3a47"><code>afc36de</code></a> dep: update vendored libxml2 to v2.12.7 (<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3191">#3191</a>)</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/41b4f0846d2c264b48ef93ecd034dd230ab8125a"><code>41b4f08</code></a> ci: add arm64-darwin coverage using macos-14</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/67b9e863a67164ae6ffbe5ed4cc482267db7c436"><code>67b9e86</code></a> dep: update libxml2 to v2.12.7</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/17c0362082341208bf9aadb61939e4de74005b44"><code>17c0362</code></a> version bump to v1.16.4</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/1c329e9c09148155624b52ffe630cc1b01d6787f"><code>1c329e9</code></a> dep: update to zlib 1.3.1 (v1.16.x) (<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3175">#3175</a>)</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/edeac07bb21b3f00c2a6aaf27806ce9d0871a08d"><code>edeac07</code></a> dep: update to zlib 1.3.1</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/80fb6085c069e053457ed6f6325ac032f2b029fe"><code>80fb608</code></a> version bump to v1.16.3</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/710bd96d70f39baadd0405cf0f3c0c42805019af"><code>710bd96</code></a> dep: update libxml 2.12.6 (branch v1.16.x) (<a href="https://redirect.github.com/sparklemotion/nokogiri/issues/3151">#3151</a>)</li>
<li><a href="https://github.com/sparklemotion/nokogiri/commit/461a96ea163b144ea2898d088efe65fce311d5be"><code>461a96e</code></a> fix: Reader#read sets <a href="https://github.com/encoding"><code>@​encoding</code></a> if it is unset</li>
<li>Additional commits viewable in <a href="https://github.com/sparklemotion/nokogiri/compare/v1.16.2...v1.16.5">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 23:42:29 +0000 UTC
    </div>
</div>

