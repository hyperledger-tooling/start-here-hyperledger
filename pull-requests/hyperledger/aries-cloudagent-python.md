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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2750" class=".btn">#2750</a>
            </td>
            <td>
                <b>
                    Fix pytest collection errors when anoncreds package is not installed
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
        Created At 2024-01-30 23:25:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2749" class=".btn">#2749</a>
            </td>
            <td>
                <b>
                    Add cached copy of BBS v1 context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts #2739
Fixes #2738

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 22:40:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2748" class=".btn">#2748</a>
            </td>
            <td>
                <b>
                    fix(credo-interop): various didexchange and did:peer related fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2742 and various other issues discovered while testing ACA-Py against AFJ.

- Send and accept `didexchange/1.1` as handshake protocol in OOB
- Credo did not like the fact that we were including both `jwk` and `kid` in the protected headers of signed attachments. The `kid` was redundant so I removed it.
- Credo does not accept `Multikey` verification method type yet (I opened a PR though: https://github.com/openwallet-foundation/credo-ts/pull/1720 -- tests failing :smile:). So I adjusted our did:peer:4 doc creation to use `Ed25519VerificationKey2020` for now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 21:40:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2747" class=".btn">#2747</a>
            </td>
            <td>
                <b>
                    chore: pin black version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Though relatively infrequent, the result of formatting with black can change from version to version. This PR pins the version of black used in the github action to a specific version. This version should be kept in sync with the version selected in the pyproject.toml to avoid situations where new versions of black cause PR checks to fail because formatting changed between versions.

This PR also bumps the currently selected version of black to 24.1.1, which is the most recent black version that was run in recent PRs. This should provide the best continuity until the next time we choose to update black.

Should correct the issues seen in #2737 and #2746 (black was passing locally).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 00:57:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2746" class=".btn">#2746</a>
            </td>
            <td>
                <b>
                    fix: partial revert of ConnRecord schema change
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR partially reverts some of the changes made in #2661 relating to the `ConnRecordSchema`. The changes in that PR caused the generated openapi to rename the definition to `StoredConnRecord`. We can get the same fix while not causing a change to the name in the openapi; this is preferable because otherwise it impacts downstream consumers of the openapi definition.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 00:50:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2745" class=".btn">#2745</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aiohttp from 3.9.1 to 3.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.9.1 to 3.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.2</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>Fixed server-side websocket connection leak.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7978">#7978</a>.</p>
</li>
<li>
<p>Fixed <code>web.FileResponse</code> doing blocking I/O in the event loop.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8012">#8012</a>.</p>
</li>
<li>
<p>Fixed double compress when compression enabled and compressed file exists in server file responses.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8014">#8014</a>.</p>
</li>
<li>
<p>Added runtime type check for <code>ClientSession</code> <code>timeout</code> parameter.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8021">#8021</a>.</p>
</li>
<li>
<p>Fixed an unhandled exception in the Python HTTP parser on header lines starting with a colon -- by :user:<code>pajod</code>.</p>
<p>Invalid request lines with anything but a dot between the HTTP major and minor version are now rejected.
Invalid header field names containing question mark or slash are now rejected.
Such requests are incompatible with :rfc:<code>9110#section-5.6.2</code> and are not known to be of any legitimate use.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8074">#8074</a>.</p>
</li>
<li>
<p>Improved validation of paths for static resources requests to the server -- by :user:<code>bdraco</code>.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/master/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.9.2 (2024-01-28)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>Fixed server-side websocket connection leak.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7978</code>.</p>
</li>
<li>
<p>Fixed <code>web.FileResponse</code> doing blocking I/O in the event loop.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8012</code>.</p>
</li>
<li>
<p>Fixed double compress when compression enabled and compressed file exists in server file responses.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8014</code>.</p>
</li>
<li>
<p>Added runtime type check for <code>ClientSession</code> <code>timeout</code> parameter.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8021</code>.</p>
</li>
<li>
<p>Fixed an unhandled exception in the Python HTTP parser on header lines starting with a colon -- by :user:<code>pajod</code>.</p>
<p>Invalid request lines with anything but a dot between the HTTP major and minor version are now rejected.
Invalid header field names containing question mark or slash are now rejected.
Such requests are incompatible with :rfc:<code>9110#section-5.6.2</code> and are not known to be of any legitimate use.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8074</code>.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/24a6d64966d99182e95f5d3a29541ef2fec397ad"><code>24a6d64</code></a> Release v3.9.2 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8082">#8082</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/9118a5831e8a65b8c839eb7e4ac983e040ff41df"><code>9118a58</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8079">#8079</a>/1c335944 backport][3.9] Validate static paths (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8080">#8080</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/435ad46e6c26cbf6ed9a38764e9ba8e7441a0e3b"><code>435ad46</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/3955">#3955</a>/8960063e backport][3.9] Replace all tmpdir fixtures with tmp_path (...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/d33bc21414e283c9e6fe7f6caf69e2ed60d66c82"><code>d33bc21</code></a> Improve validation in HTTP parser (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8074">#8074</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8078">#8078</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/0d945d1be08f2ba8475513216a66411f053c3217"><code>0d945d1</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7916">#7916</a>/822fbc74 backport][3.9] Add more information to contributing page (...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3ec4fa1f0e0a0dad218c75dbe5ed09e22d5cc284"><code>3ec4fa1</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8069">#8069</a>/69bbe874 backport][3.9] 📝 Only show changelog draft for non-release...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/419d715c42c46daf1a59e0aff61c1f6d10236982"><code>419d715</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8066">#8066</a>/cba34699 backport][3.9] 💅📝 Restructure the changelog for clarity (#...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a54dab3b36bcf0d815b9244f52ae7bc5da08f387"><code>a54dab3</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8049">#8049</a>/a379e634 backport][3.9] Set cause for ClientPayloadError (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8050">#8050</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/437ac47fe332106a07a2d5335bb89619f1bc23f7"><code>437ac47</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7995">#7995</a>/43a5bc50 backport][3.9] Fix examples of <code>fallback_charset_resolver</code>...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/034e5e34ee11c6138c773d85123490e691e1b708"><code>034e5e3</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8042">#8042</a>/4b91b530 backport][3.9] Tightening the runtime type check for ssl (...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.1...v3.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.9.1&new-version=3.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-01-30 00:26:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2744" class=".btn">#2744</a>
            </td>
            <td>
                <b>
                    Address traceability context bug #2743
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is to address #2743

There is an odd bug that's been ongoing for some time where when trying to expand a did document with the `pyld` library it fails.

Since this happen in a very specific condition, this PR looks to implement a workaround.

When we need to verify a json-ld VC where the issuer/verificationMethod is a `did:web:` scheme, we first manually resolve the did document with the `requests` module, then extract the traceability context form the document if present, then frame the document directly....

Its not pretty, but its the best solution I could come up with that has minimal impact on the existing code. If anyone has a better solution, I'm happy to change it!

@swcurran @dbluhm this is the last critical PR I would like to see in the 0.12 release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 23:54:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2741" class=".btn">#2741</a>
            </td>
            <td>
                <b>
                    Upgrade anoncreds to 0.2.0-dev9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Waiting on integration tests...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 21:39:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2739" class=".btn">#2739</a>
            </td>
            <td>
                <b>
                    Update BBS+ context to bypass redirections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 17:30:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2737" class=".btn">#2737</a>
            </td>
            <td>
                <b>
                    bump pydid to v 0.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses #2677

@dbluhm I ran a `poetry update pydid` after changing the version in the `pyproject.toml` file. Seems like it did the trick.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 21:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2734" class=".btn">#2734</a>
            </td>
            <td>
                <b>
                    Upgrade anoncred-rs to version 0.2.0-dev8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still waiting for integration tests locally.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 16:37:46 +0000 UTC
    </div>
</div>

