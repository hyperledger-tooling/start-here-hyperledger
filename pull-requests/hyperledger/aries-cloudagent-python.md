---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2533" class=".btn">#2533</a>
            </td>
            <td>
                <b>
                    refactor: make ldp_vc logic reusable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a refactor of LDP VC handling within ICv2 and PPv2 to make it usable outside of those protocol's handlers. I believe this results in a cleaner implementation, separating the concerns of preparing a credential from the ICv2 protocol and its messages and handlers for those messages.

This refactor enables the other major addition in this PR, adding a couple of new endpoints for LDP VC issue and verify, `POST /vc/ldp/issue` and `POST /vc/ldp/verify`. These endpoints are similar to the `/jsonld/sign` and `/jsonld/verify` endpoints. However, the big difference is that the `/jsonld` endpoints did not use the same LDP signing methods used in ICv2 or PPv2. This has caused the two implementations to diverge more and more over time. With this PR, these endpoints are still available but are marked as deprecated. One other significant difference, the inputs for endpoints have changed to be more specific to signing and verifying LDP VCs and not just arbitrary JSON-LD documents.

Fixes #2468.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 18:59:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2529" class=".btn">#2529</a>
            </td>
            <td>
                <b>
                    Feat: Support subwallet upgradation using the Upgrade command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2507 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 16:31:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2527" class=".btn">#2527</a>
            </td>
            <td>
                <b>
                    chore: update pydid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This update includes changes recently committed to the 0.10.X releases, correcting an issue that prevented mediators from handling `didcomm:transport/queue` as a service endpoint.

A small but notable difference between this and the 0.10.X releases: in changes queued for the "next" release, we added `peerdid`. `peerdid` also depends on pydid. I had to backport fixes to the pydid 0.3.x line to workaround conflicts caused by using 0.4.0 of pydid with peerdid. I'm working with the SICPA team to resolve this. In the meantime, 0.3.9 will work exactly as we need anyways.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 17:42:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2525" class=".btn">#2525</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.0.5 to 2.0.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 2.0.5 to 2.0.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.0.6</h2>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (GHSA-v845-jxx5-vc9f)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.0.6 (2023-10-02)</h1>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/262e3e332209ee93ff70e2b13502c8f20c105ac8"><code>262e3e3</code></a> Release 2.0.6</li>
<li><a href="https://github.com/urllib3/urllib3/commit/644124ecd0b6e417c527191f866daa05a5a2056d"><code>644124e</code></a> Merge pull request from GHSA-v845-jxx5-vc9f</li>
<li><a href="https://github.com/urllib3/urllib3/commit/740380c59ca2a7c2dceca19e5dba99f6b7060e62"><code>740380c</code></a> Bump cryptography from 41.0.3 to 41.0.4 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3131">#3131</a>)</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/v2.0.5...2.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.0.5&new-version=2.0.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 00:22:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2524" class=".btn">#2524</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.0.2 to 2.0.6 in /demo/playground/scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 2.0.2 to 2.0.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.0.6</h2>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (GHSA-v845-jxx5-vc9f)</li>
</ul>
<h2>2.0.5</h2>
<ul>
<li>Allowed pyOpenSSL third-party module without any deprecation warning. <a href="https://redirect.github.com/urllib3/urllib3/issues/3126">#3126</a></li>
<li>Fixed default <code>blocksize</code> of <code>HTTPConnection</code> classes to match high-level classes. Previously was 8KiB, now 16KiB. <a href="https://redirect.github.com/urllib3/urllib3/issues/3066%3E">#3066</a></li>
</ul>
<h2>2.0.4</h2>
<ul>
<li>Added support for union operators to <code>HTTPHeaderDict</code> (<a href="https://redirect.github.com/urllib3/urllib3/issues/2254">#2254</a>)</li>
<li>Added <code>BaseHTTPResponse</code> to <code>urllib3.__all__</code> (<a href="https://redirect.github.com/urllib3/urllib3/issues/3078">#3078</a>)</li>
<li>Fixed <code>urllib3.connection.HTTPConnection</code> to raise the <code>http.client.connect</code> audit event to have the same behavior as the standard library HTTP client (<a href="https://redirect.github.com/urllib3/urllib3/issues/2757">#2757</a>)</li>
<li>Relied on the standard library for checking hostnames in supported PyPy releases (<a href="https://redirect.github.com/urllib3/urllib3/issues/3087">#3087</a>)</li>
</ul>
<h2>2.0.3</h2>
<ul>
<li>Allowed alternative SSL libraries such as LibreSSL, while still issuing a warning as we cannot help users facing issues with implementations other than OpenSSL. <a href="https://redirect.github.com/urllib3/urllib3/issues/3020">#3020</a></li>
<li>Deprecated URLs which don't have an explicit scheme <a href="https://redirect.github.com/urllib3/urllib3/pull/2950">#2950</a></li>
<li>Fixed response decoding with Zstandard when compressed data is made of several frames. <a href="https://redirect.github.com/urllib3/urllib3/issues/3008">#3008</a></li>
<li>Fixed <code>assert_hostname=False</code> to correctly skip hostname check. <a href="https://redirect.github.com/urllib3/urllib3/issues/3051">#3051</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.0.6 (2023-10-02)</h1>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
</ul>
<h1>2.0.5 (2023-09-20)</h1>
<ul>
<li>Allowed pyOpenSSL third-party module without any deprecation warning. (<code>[#3126](https://github.com/urllib3/urllib3/issues/3126) &lt;https://github.com/urllib3/urllib3/issues/3126&gt;</code>__)</li>
<li>Fixed default <code>blocksize</code> of <code>HTTPConnection</code> classes to match high-level classes. Previously was 8KiB, now 16KiB. (<code>[#3066](https://github.com/urllib3/urllib3/issues/3066) &lt;https://github.com/urllib3/urllib3/issues/3066&gt;</code>__)</li>
</ul>
<h1>2.0.4 (2023-07-19)</h1>
<ul>
<li>Added support for union operators to <code>HTTPHeaderDict</code> (<code>[#2254](https://github.com/urllib3/urllib3/issues/2254) &lt;https://github.com/urllib3/urllib3/issues/2254&gt;</code>__)</li>
<li>Added <code>BaseHTTPResponse</code> to <code>urllib3.__all__</code> (<code>[#3078](https://github.com/urllib3/urllib3/issues/3078) &lt;https://github.com/urllib3/urllib3/issues/3078&gt;</code>__)</li>
<li>Fixed <code>urllib3.connection.HTTPConnection</code> to raise the <code>http.client.connect</code> audit event to have the same behavior as the standard library HTTP client (<code>[#2757](https://github.com/urllib3/urllib3/issues/2757) &lt;https://github.com/urllib3/urllib3/issues/2757&gt;</code>__)</li>
<li>Relied on the standard library for checking hostnames in supported PyPy releases (<code>[#3087](https://github.com/urllib3/urllib3/issues/3087) &lt;https://github.com/urllib3/urllib3/issues/3087&gt;</code>__)</li>
</ul>
<h1>2.0.3 (2023-06-07)</h1>
<ul>
<li>Allowed alternative SSL libraries such as LibreSSL, while still issuing a warning as we cannot help users facing issues with implementations other than OpenSSL. (<code>[#3020](https://github.com/urllib3/urllib3/issues/3020) &lt;https://github.com/urllib3/urllib3/issues/3020&gt;</code>__)</li>
<li>Deprecated URLs which don't have an explicit scheme (<code>[#2950](https://github.com/urllib3/urllib3/issues/2950) &lt;https://github.com/urllib3/urllib3/pull/2950&gt;</code>_)</li>
<li>Fixed response decoding with Zstandard when compressed data is made of several frames. (<code>[#3008](https://github.com/urllib3/urllib3/issues/3008) &lt;https://github.com/urllib3/urllib3/issues/3008&gt;</code>__)</li>
<li>Fixed <code>assert_hostname=False</code> to correctly skip hostname check. (<code>[#3051](https://github.com/urllib3/urllib3/issues/3051) &lt;https://github.com/urllib3/urllib3/issues/3051&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/262e3e332209ee93ff70e2b13502c8f20c105ac8"><code>262e3e3</code></a> Release 2.0.6</li>
<li><a href="https://github.com/urllib3/urllib3/commit/644124ecd0b6e417c527191f866daa05a5a2056d"><code>644124e</code></a> Merge pull request from GHSA-v845-jxx5-vc9f</li>
<li><a href="https://github.com/urllib3/urllib3/commit/740380c59ca2a7c2dceca19e5dba99f6b7060e62"><code>740380c</code></a> Bump cryptography from 41.0.3 to 41.0.4 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3131">#3131</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d9f85a749488188c286cd50606d159874db94d5f"><code>d9f85a7</code></a> Release 2.0.5</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d41f4122966f7f4f5f92001ad518e5d9dafcc886"><code>d41f412</code></a> Undeprecate pyOpenSSL module (<a href="https://redirect.github.com/urllib3/urllib3/issues/3127">#3127</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b6c04cb3e62ef5a0e4947d037c12fb3ca79e024a"><code>b6c04cb</code></a> Fix a link to &quot;absolute URI&quot; definition (<a href="https://redirect.github.com/urllib3/urllib3/issues/3128">#3128</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/af7c78fa30f5a4e265911371d0c59b6baeddca0f"><code>af7c78f</code></a> refactor: change double conditional to one (<a href="https://redirect.github.com/urllib3/urllib3/issues/3118">#3118</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/34c13c8e68df6f89890ba08b9fc4fbf87ed21669"><code>34c13c8</code></a> Refer to current internet standards in docs on proxies (<a href="https://redirect.github.com/urllib3/urllib3/issues/3124">#3124</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/a3e94f218cd8297db73302eadae235f0c832a809"><code>a3e94f2</code></a> Fix a name of an attribute in docs (<a href="https://redirect.github.com/urllib3/urllib3/issues/3125">#3125</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/da69d4f4f95bc7ef9307fc8e0499c2121f1e4791"><code>da69d4f</code></a> Fix docs build (<a href="https://redirect.github.com/urllib3/urllib3/issues/3123">#3123</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/2.0.2...2.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.0.2&new-version=2.0.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 23:30:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2523" class=".btn">#2523</a>
            </td>
            <td>
                <b>
                    Add /rotate to revocation api.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added in `handle_full_registry` but seems to be some issues with how the counts work.
Cannot set the `next_index` to start at 0 because the credential data is invalid.
And because we don't track the index and current revocation id externally, we can't trigger the `handle_full_registry` until after a credential is created. So for every list/index we lose 1 slot. The only way I could successfully have registries rollover AND create the credentials successfully was triggering 1 slot before the max. cred. num.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 23:19:00 +0000 UTC
    </div>
</div>

