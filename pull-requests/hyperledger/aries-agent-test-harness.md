---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/809" class=".btn">#809</a>
            </td>
            <td>
                <b>
                    Bump the cargo group across 1 directory with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps the cargo group with 2 updates in the /aries-backchannels/aries-vcx directory: [openssl](https://github.com/sfackler/rust-openssl) and [whoami](https://github.com/ardaku/whoami).

Updates `openssl` from 0.10.48 to 0.10.64
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.64</h2>
<h2>What's Changed</h2>
<ul>
<li>Make _STACK opaque for LibreSSL &gt;= 3.9.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2153">sfackler/rust-openssl#2153</a></li>
<li>enable x509 verify and groups list for boringssl by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2155">sfackler/rust-openssl#2155</a></li>
<li>Cleanup some not-required Path::new invocations by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2158">sfackler/rust-openssl#2158</a></li>
<li>fixed a clippy (nightly) warning by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2161">sfackler/rust-openssl#2161</a></li>
<li>Bump actions versions by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2162">sfackler/rust-openssl#2162</a></li>
<li>Add support for setting the nonce type and digest on a PKEY_CTX by <a href="https://github.com/facutuesca"><code>@​facutuesca</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2144">sfackler/rust-openssl#2144</a></li>
<li>rebuild openssl-sys if the underlying openssl has changed by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2157">sfackler/rust-openssl#2157</a></li>
<li>Added binding for EVP_default_properties_enable_fips by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2168">sfackler/rust-openssl#2168</a></li>
<li>LibreSSL 3.9: fix CRYPTO_malloc/free signatures by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2170">sfackler/rust-openssl#2170</a></li>
<li>Expose alias on X509 structs by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2167">sfackler/rust-openssl#2167</a></li>
<li>bump openssl and openssl-sys + changelogs by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2175">sfackler/rust-openssl#2175</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.63...openssl-v0.10.64">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.63...openssl-v0.10.64</a></p>
<h2>openssl-v0.10.63</h2>
<h2>What's Changed</h2>
<ul>
<li>Allow passing a passphrase callback when loading a public key by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2135">sfackler/rust-openssl#2135</a></li>
<li>Expose several additional ciphers for symmetry with symm by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2140">sfackler/rust-openssl#2140</a></li>
<li>brew: add openssl@3.0 (for 3.0.x LTS releases) by <a href="https://github.com/chenrui333"><code>@​chenrui333</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2141">sfackler/rust-openssl#2141</a></li>
<li>Add PKey::from_dhx by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2142">sfackler/rust-openssl#2142</a></li>
<li>Make X509_PURPOSE opaque for LibreSSL &gt;= 3.9.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2145">sfackler/rust-openssl#2145</a></li>
<li>PEM parsing: check last error instead of first by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2148">sfackler/rust-openssl#2148</a></li>
<li>Expose brainpool NIDs on libressl by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2150">sfackler/rust-openssl#2150</a></li>
<li>Add two methods to the PKCS7 API by <a href="https://github.com/facutuesca"><code>@​facutuesca</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2111">sfackler/rust-openssl#2111</a></li>
<li>add more boringssl methods by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2138">sfackler/rust-openssl#2138</a></li>
<li>Release openssl v0.10.63 and openssl-sys v0.9.99 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2152">sfackler/rust-openssl#2152</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.62...openssl-v0.10.63">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.62...openssl-v0.10.63</a></p>
<h2>openssl-v0.10.62</h2>
<h2>What's Changed</h2>
<ul>
<li>fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2119">#2119</a> -- use ErrorStack abstraction in X.509 error handling by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2120">sfackler/rust-openssl#2120</a></li>
<li>Fix building with latest BoringSSL by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2121">sfackler/rust-openssl#2121</a></li>
<li>Fix tests on macOS by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2123">sfackler/rust-openssl#2123</a></li>
<li>Upcoming API changes in LibreSSL 3.9 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2124">sfackler/rust-openssl#2124</a></li>
<li>Add <code>rand_priv_bytes</code> by <a href="https://github.com/overvenus"><code>@​overvenus</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2126">sfackler/rust-openssl#2126</a></li>
<li>Add nid constant for curve brainpoolP320r1 by <a href="https://github.com/nicklaswj"><code>@​nicklaswj</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2129">sfackler/rust-openssl#2129</a></li>
<li>Release openssl v0.10.62 and openssl-sys v0.9.98 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2133">sfackler/rust-openssl#2133</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/overvenus"><code>@​overvenus</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2126">sfackler/rust-openssl#2126</a></li>
<li><a href="https://github.com/nicklaswj"><code>@​nicklaswj</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2129">sfackler/rust-openssl#2129</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.61...openssl-v0.10.62">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.61...openssl-v0.10.62</a></p>
<h2>openssl v0.10.61</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4a19cd48259e0755d9a9067f4c1a51ee63844c66"><code>4a19cd4</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2175">#2175</a> from reaperhulk/changelog</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4e0e05a6293043cf7b9392c0e286c8397ce75996"><code>4e0e05a</code></a> bump openssl and openssl-sys + changelogs</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/c2b124aa2c36b5fc792239391e614df7f6f1fb24"><code>c2b124a</code></a> Be explicit that aliases are not part of X.509 certificates</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/1abf4a5b792228f6e9d8676015623d6315def4c1"><code>1abf4a5</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2167">#2167</a> from alex/expose-alias</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a644ec2542473c854a02b7fe642621e813517979"><code>a644ec2</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2170">#2170</a> from botovq/crypto-free</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/83940d14e30ed4e7c885dd44e3002c1955d5d5ed"><code>83940d1</code></a> LibreSSL 3.9: fix CRYPTO_malloc/free signatures</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/51fc5694821d66983d8639d3b0b4a58024f92a1f"><code>51fc569</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2168">#2168</a> from sfackler/alex-patch-1</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/3c53dee153d4ab801cde3e10d914a16789464a6b"><code>3c53dee</code></a> Added binding for EVP_default_properties_enable_fips</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a12abe1b92c526f6995632ba43f6bfc433b5997d"><code>a12abe1</code></a> Expose alias on X509 structs</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/3acf2eff0baf7db1a5722c14def50cf5b068538e"><code>3acf2ef</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2157">#2157</a> from reaperhulk/rebuild-if-changed</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.48...openssl-v0.10.64">compare view</a></li>
</ul>
</details>
<br />

Updates `whoami` from 1.3.0 to 1.5.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ardaku/whoami/blob/v1/CHANGELOG.md">whoami's changelog</a>.</em></p>
<blockquote>
<h2>[1.5.1] - 2024-03-09</h2>
<h3>Fixed</h3>
<ul>
<li>Broken link in docs</li>
</ul>
<h2>[1.5.0] - 2024-03-03</h2>
<h3>Added</h3>
<ul>
<li>WASI support</li>
<li>Redox support</li>
<li>Fallible functions
<ul>
<li><code>whoami::fallible::devicename()</code></li>
<li><code>whoami::fallible::devicename_os()</code></li>
<li><code>whoami::fallible::distro()</code></li>
<li><code>whoami::fallible::hostname()</code> - notably doesn't normalize to lowercase</li>
<li><code>whoami::fallible::realname()</code></li>
<li><code>whoami::fallible::realname_os()</code></li>
<li><code>whoami::fallible::username()</code></li>
<li><code>whoami::fallible::username_os()</code></li>
</ul>
</li>
<li><code>whoami::Language</code></li>
<li><code>whoami::Country</code></li>
<li><code>whoami::langs()</code></li>
<li><code>whoami::fallible::account()</code></li>
<li><code>whoami::fallible::account_os()</code></li>
<li><code>whoami::DesktopEnv::is_gtk()</code></li>
<li><code>whoami::DesktopEnv::is_kde()</code></li>
</ul>
<h3>Removed</h3>
<ul>
<li>Generated device names that infer casing based on the hostname when the
device name is not available - now returns the hostname unchanged</li>
<li>Partial (potentially unsound) support for Android, iOS, watchOS, tvOS,
Fuchsia, Haiku, Solaris, and a few others.  These targets now use the &quot;fake&quot;
implementation.</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Deprecated <code>whoami::distro_os()</code></li>
<li>Deprecated <code>whoami::hostname()</code></li>
<li>Deprecated <code>whoami::hostname_os()</code></li>
<li>Deprecated <code>whoami::lang()</code></li>
<li>illumos and Redox are no longer untested targets</li>
<li>Documented that illumos and Redox have a higher MSRV (Rust 1.65) than other
targets</li>
<li>Display implementation on <code>Platform::Illumos</code> now displays in lowercase:
illumos</li>
</ul>
<h3>Fixed</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ardaku/whoami/commit/74a0c3b8b834d8f100dad20b266178fef40e0760"><code>74a0c3b</code></a> Prepare to release whoami 1.5.1 (<a href="https://redirect.github.com/ardaku/whoami/issues/109">#109</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/7789b3f9dd1bb869b50893c5fea798c00b4a1f9a"><code>7789b3f</code></a> Backport v2 -&gt; v1: Test docs in CI (<a href="https://redirect.github.com/ardaku/whoami/issues/108">#108</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/4bbaf5201b29d8d5f9f9917524020ad15ed88983"><code>4bbaf52</code></a> Prevent future potential UB in unix wrapper for <code>getpwuid()</code> (<a href="https://redirect.github.com/ardaku/whoami/issues/104">#104</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/358dc0ef16960beafdf14f89198616b0f378b884"><code>358dc0e</code></a> WhoAmI 1.5.0 Release (<a href="https://redirect.github.com/ardaku/whoami/issues/94">#94</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/d6ee13ed9e818aa51b8d86d95e8009a376289a40"><code>d6ee13e</code></a> Fix Instances of Memory Corruption on Illumos (<a href="https://redirect.github.com/ardaku/whoami/issues/93">#93</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/953e702c0b24789a359a4027818af53bcb979db6"><code>953e702</code></a> Support Redox (<a href="https://redirect.github.com/ardaku/whoami/issues/92">#92</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/5bc73e4e6375a22e6b71300e0befc9cf4c97c278"><code>5bc73e4</code></a> Preserve OS case for hostnames (<a href="https://redirect.github.com/ardaku/whoami/issues/86">#86</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/29d5f2210339aa487073a3372876c0a498e46379"><code>29d5f22</code></a> Support WASI (<a href="https://redirect.github.com/ardaku/whoami/issues/84">#84</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/d7885e7c75d9a59ab3d2f5dceb82d46399c7dd7b"><code>d7885e7</code></a> Add <code>Target</code> trait for implementing new targets (<a href="https://redirect.github.com/ardaku/whoami/issues/80">#80</a>)</li>
<li><a href="https://github.com/ardaku/whoami/commit/e3da4c56f9df876f01baea5e8fde6d1a0ac60ae9"><code>e3da4c5</code></a> Add <code>langs()</code> function, deprecate <code>lang()</code> (<a href="https://redirect.github.com/ardaku/whoami/issues/78">#78</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ardaku/whoami/compare/v1.3.0...v1.5.1">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-agent-test-harness/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 14:19:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/808" class=".btn">#808</a>
            </td>
            <td>
                <b>
                    Bump azure/docker-login from 1 to 2 in the all-actions group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps the all-actions group with 1 update: [azure/docker-login](https://github.com/azure/docker-login).

Updates `azure/docker-login` from 1 to 2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/azure/docker-login/releases">azure/docker-login's releases</a>.</em></p>
<blockquote>
<h2>Version 2.0</h2>
<ul>
<li>update of Node20</li>
<li>update dependencies</li>
</ul>
<h2>Update the action to run with Node 16</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Azure/docker-login/commit/15c4aadf093404726ab2ff205b2cdd33fa6d054c"><code>15c4aad</code></a> Merge pull request <a href="https://redirect.github.com/azure/docker-login/issues/69">#69</a> from lgmorand/master</li>
<li><a href="https://github.com/Azure/docker-login/commit/8fa230a0b042fe9799760d6e4003b97bf2d14b7e"><code>8fa230a</code></a> add node_modules</li>
<li><a href="https://github.com/Azure/docker-login/commit/cf6728443801c69f3197bdbe0b79ccdfff5a13b3"><code>cf67284</code></a> action/core =&gt; last version</li>
<li><a href="https://github.com/Azure/docker-login/commit/7aabc0a4ea87221374cc69552b18b5f2f17daf8c"><code>7aabc0a</code></a> rebuild lock</li>
<li><a href="https://github.com/Azure/docker-login/commit/af42a18d08d5f58777b2c416716f245799157c46"><code>af42a18</code></a> fix some npm packages after upgrade to node20</li>
<li><a href="https://github.com/Azure/docker-login/commit/3fe855c6fd503e1769e1e729eca791e38419b426"><code>3fe855c</code></a> Update README.md to use v2</li>
<li><a href="https://github.com/Azure/docker-login/commit/f3bf641aefa4add3a0667e94dbbcb96374bba2fa"><code>f3bf641</code></a> Merge pull request <a href="https://redirect.github.com/azure/docker-login/issues/64">#64</a> from eikooc/master</li>
<li><a href="https://github.com/Azure/docker-login/commit/b35be4d2f7ea3d7b24ff5f34263783a3bda5e9c2"><code>b35be4d</code></a> Update to nodejs v20</li>
<li><a href="https://github.com/Azure/docker-login/commit/51016b52ce67b2e4faf5e4fb04521f9410d5b57f"><code>51016b5</code></a> Merge pull request <a href="https://redirect.github.com/azure/docker-login/issues/61">#61</a> from Azure/stephenmichaelf/remove-integration-tests</li>
<li><a href="https://github.com/Azure/docker-login/commit/6a8199f7d6d6f17a423d09703eca0b39e526c18a"><code>6a8199f</code></a> Remove Integration tests.</li>
<li>Additional commits viewable in <a href="https://github.com/azure/docker-login/compare/v1...v2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=azure/docker-login&package-manager=github_actions&previous-version=1&new-version=2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 14:09:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/807" class=".btn">#807</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 02:30:27 +0000 UTC
    </div>
</div>

