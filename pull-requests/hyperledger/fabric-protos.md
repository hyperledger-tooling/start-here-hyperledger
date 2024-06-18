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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    Bump Go dependencies (0.2.x)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-12 15:11:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Bump Go dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 15:10:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    Bump the bundler group across 1 directory with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps the bundler group with 3 updates in the /docs directory: [activesupport](https://github.com/rails/rails), [nokogiri](https://github.com/sparklemotion/nokogiri) and [rexml](https://github.com/ruby/rexml).

Updates `activesupport` from 6.0.4.7 to 7.1.3.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rails/rails/releases">activesupport's releases</a>.</em></p>
<blockquote>
<h2>7.1.3.4</h2>
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
<li>No changes.</li>
</ul>
<h2>Action View</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Action Pack</h2>
<ul>
<li>Include the HTTP Permissions-Policy on non-HTML Content-Types
[CVE-2024-28103]</li>
</ul>
<h2>Active Job</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Action Mailer</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Action Cable</h2>
<ul>
<li>No changes.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rails/rails/blob/v7.1.3.4/activesupport/CHANGELOG.md">activesupport's changelog</a>.</em></p>
<blockquote>
<h2>Rails 7.1.3.4 (June 04, 2024)</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Rails 7.1.3.3 (May 16, 2024)</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Rails 7.1.3.2 (February 21, 2024)</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Rails 7.1.3.1 (February 21, 2024)</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Rails 7.1.3 (January 16, 2024)</h2>
<ul>
<li>
<p>Handle nil <code>backtrace_locations</code> in <code>ActiveSupport::SyntaxErrorProxy</code>.</p>
<p><em>Eugene Kenny</em></p>
</li>
<li>
<p>Fix <code>ActiveSupport::JSON.encode</code> to prevent duplicate keys.</p>
<p>If the same key exist in both String and Symbol form it could
lead to the same key being emitted twice.</p>
<p><em>Manish Sharma</em></p>
</li>
<li>
<p>Fix <code>ActiveSupport::Cache::Store#read_multi</code> when using a cache namespace
and local cache strategy.</p>
<p><em>Mark Oleson</em></p>
</li>
<li>
<p>Fix <code>Time.now/DateTime.now/Date.today</code> to return results in a system timezone after <code>#travel_to</code>.</p>
<p>There is a bug in the current implementation of #travel_to:
it remembers a timezone of its argument, and all stubbed methods start
returning results in that remembered timezone. However, the expected
behaviour is to return results in a system timezone.</p>
<p><em>Aleksei Chernenkov</em></p>
</li>
<li>
<p>Fix <code>:unless_exist</code> option for <code>MemoryStore#write</code> (et al) when using a
cache namespace.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rails/rails/commit/19eebf6d33dd15a0172e3ed2481bec57a89a2404"><code>19eebf6</code></a> Preparing for 7.1.3.4 release</li>
<li><a href="https://github.com/rails/rails/commit/bd7c28a498fde00fdb04f95bca874437b8c94606"><code>bd7c28a</code></a> update changelog</li>
<li><a href="https://github.com/rails/rails/commit/747a03ba7722b6f0a7ce42e86cea83cf07a2e6ef"><code>747a03b</code></a> Preparing for 7.1.3.3 release</li>
<li><a href="https://github.com/rails/rails/commit/6f0d1ad14b92b9f5906e44740fce8b4f1c7075dc"><code>6f0d1ad</code></a> Preparing for 7.1.3.2 release</li>
<li><a href="https://github.com/rails/rails/commit/c25f0fcaa221ff836c958b8938bd06358f8aedae"><code>c25f0fc</code></a> Respect raise_on_missing_ in controller</li>
<li><a href="https://github.com/rails/rails/commit/d73ed958dc91d6b8cbb0bef7b4cdcfc013bd876f"><code>d73ed95</code></a> Preparing for 7.1.3.1 release</li>
<li><a href="https://github.com/rails/rails/commit/43037d8f94a245d2084c0aac24a73bd73a0db328"><code>43037d8</code></a> update changelog</li>
<li><a href="https://github.com/rails/rails/commit/36c1591bcb5e0ee3084759c7f42a706fe5bb7ca7"><code>36c1591</code></a> Preparing for 7.1.3 release</li>
<li><a href="https://github.com/rails/rails/commit/a84622f1a86e2bf06c173c41c733a568db64c7b5"><code>a84622f</code></a> Sync changelog</li>
<li><a href="https://github.com/rails/rails/commit/894f9330a7255780cdf269755cf11f307f4920f6"><code>894f933</code></a> Merge pull request <a href="https://redirect.github.com/rails/rails/issues/50764">#50764</a> from eugeneius/syntax_error_proxy_nil_backtrace_loc...</li>
<li>Additional commits viewable in <a href="https://github.com/rails/rails/compare/v6.0.4.7...v7.1.3.4">compare view</a></li>
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

Updates `rexml` from 3.2.5 to 3.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ruby/rexml/releases">rexml's releases</a>.</em></p>
<blockquote>
<h2>REXML 3.3.0 - 2024-06-11</h2>
<h3>Improvements</h3>
<ul>
<li>Added support for strscan 0.7.0 installed with Ruby 2.6.
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/142">GH-142</a></li>
<li>Reported by Fernando Trigoso.</li>
</ul>
</li>
</ul>
<h3>Thanks</h3>
<ul>
<li>Fernando Trigoso</li>
</ul>
<h2>REXML 3.2.9 - 2024-06-09</h2>
<h3>Improvements</h3>
<ul>
<li>
<p>Added support for old strscan.</p>
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/132">GH-132</a></li>
<li>Reported by Adam</li>
</ul>
</li>
<li>
<p>Improved attribute value parse performance.</p>
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/135">GH-135</a></li>
<li>Patch by NAITOH Jun.</li>
</ul>
</li>
<li>
<p>Improved <code>REXML::Node#each_recursive</code> performance.</p>
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/134">GH-134</a></li>
<li><a href="https://redirect.github.com/ruby/rexml/issues/139">GH-139</a></li>
<li>Patch by Hiroya Fujinami.</li>
</ul>
</li>
<li>
<p>Improved text parse performance.</p>
<ul>
<li>Reported by mprogrammer.</li>
</ul>
</li>
</ul>
<h3>Thanks</h3>
<ul>
<li>Adam</li>
<li>NAITOH Jun</li>
<li>Hiroya Fujinami</li>
<li>mprogrammer</li>
</ul>
<h2>REXML 3.2.8 - 2024-05-16</h2>
<h3>Fixes</h3>
<ul>
<li>Suppressed a warning</li>
</ul>
<h2>REXML 3.2.7 - 2024-05-16</h2>
<h3>Improvements</h3>
<ul>
<li>Improve parse performance by using <code>StringScanner</code>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ruby/rexml/blob/master/NEWS.md">rexml's changelog</a>.</em></p>
<blockquote>
<h2>3.3.0 - 2024-06-11 {#version-3-3-0}</h2>
<h3>Improvements</h3>
<ul>
<li>Added support for strscan 0.7.0 installed with Ruby 2.6.
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/142">GH-142</a></li>
<li>Reported by Fernando Trigoso.</li>
</ul>
</li>
</ul>
<h3>Thanks</h3>
<ul>
<li>Fernando Trigoso</li>
</ul>
<h2>3.2.9 - 2024-06-09 {#version-3-2-9}</h2>
<h3>Improvements</h3>
<ul>
<li>
<p>Added support for old strscan.</p>
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/132">GH-132</a></li>
<li>Reported by Adam.</li>
</ul>
</li>
<li>
<p>Improved attribute value parse performance.</p>
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/135">GH-135</a></li>
<li>Patch by NAITOH Jun.</li>
</ul>
</li>
<li>
<p>Improved <code>REXML::Node#each_recursive</code> performance.</p>
<ul>
<li><a href="https://redirect.github.com/ruby/rexml/issues/134">GH-134</a></li>
<li><a href="https://redirect.github.com/ruby/rexml/issues/139">GH-139</a></li>
<li>Patch by Hiroya Fujinami.</li>
</ul>
</li>
<li>
<p>Improved text parse performance.</p>
<ul>
<li>Reported by mprogrammer.</li>
</ul>
</li>
</ul>
<h3>Thanks</h3>
<ul>
<li>Adam</li>
<li>NAITOH Jun</li>
<li>Hiroya Fujinami</li>
<li>mprogrammer</li>
</ul>
<h2>3.2.8 - 2024-05-16 {#version-3-2-8}</h2>
<h3>Fixes</h3>
<ul>
<li>Suppressed a warning</li>
</ul>
<h2>3.2.7 - 2024-05-16 {#version-3-2-7}</h2>
<h3>Improvements</h3>
<ul>
<li>Improve parse performance by using <code>StringScanner</code>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ruby/rexml/commit/8247bdc55c85073e953fd27687f42e427b6f071b"><code>8247bdc</code></a> Add 3.3.0 entry</li>
<li><a href="https://github.com/ruby/rexml/commit/0d9b98c7f6bd221c362644329c4cee8a2338ddc4"><code>0d9b98c</code></a> ci: don't use Ruby 2.5 for gem test</li>
<li><a href="https://github.com/ruby/rexml/commit/31738ccfc3324f4b32769fa1695c78c06a88c277"><code>31738cc</code></a> Add support for strscan 0.7.0 installed with Ruby 2.6</li>
<li><a href="https://github.com/ruby/rexml/commit/a7d66f2d3b9142a5afbfceb921a1b51546aee7ee"><code>a7d66f2</code></a> ci document: use the latest Ruby</li>
<li><a href="https://github.com/ruby/rexml/commit/5078c86573002e4dfd8543dba5b313f234f08e95"><code>5078c86</code></a> news: fix a typo</li>
<li><a href="https://github.com/ruby/rexml/commit/7ca7ccdfc65f5bb1d61797163ef213774a99cbbb"><code>7ca7ccd</code></a> Bump version</li>
<li><a href="https://github.com/ruby/rexml/commit/964c9dc7896e9a0b8ba012702fb06d6538b6acf1"><code>964c9dc</code></a> Add 3.2.9 entry</li>
<li><a href="https://github.com/ruby/rexml/commit/e06b3fb2660c682423e10d59b92d192c42e9825d"><code>e06b3fb</code></a> Improve text parse performance</li>
<li><a href="https://github.com/ruby/rexml/commit/dab80658b684a093f4ef8b2c0b154df58aa710c9"><code>dab8065</code></a> Improve <code>Node#each_recursive</code> performance (<a href="https://redirect.github.com/ruby/rexml/issues/139">#139</a>)</li>
<li><a href="https://github.com/ruby/rexml/commit/da67561afb2a5f6910c69d5e0e73bea8d457f303"><code>da67561</code></a> test: reduce the number of rehearsal executions</li>
<li>Additional commits viewable in <a href="https://github.com/ruby/rexml/compare/v3.2.5...v3.3.0">compare view</a></li>
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
        Created At 2024-06-11 14:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Bump braces from 3.0.2 to 3.0.3 in /bindings/node in the npm_and_yarn group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 1 update in the /bindings/node directory: [braces](https://github.com/micromatch/braces).

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


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=braces&package-manager=npm_and_yarn&previous-version=3.0.2&new-version=3.0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-11 14:39:04 +0000 UTC
    </div>
</div>

