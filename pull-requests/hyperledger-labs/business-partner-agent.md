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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/860" class=".btn">#860</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.9.1 to 5.19.1 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.9.1 to 5.19.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.19.1</h2>
<h2>⚠️ Security Release ⚠️</h2>
<ul>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-r6ch-mqf9-qc9w">Regular Expression Denial of Service in Headers</a> with CVE-2023-24807</li>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-5r9g-qh6m-jxff">CRLF Injection in Nodejs ‘undici’ via host</a> with CVE-2023-23936</li>
</ul>
<p>This release is part of the Node.js security release train: <a href="https://nodejs.org/en/blog/vulnerability/february-2023-security-releases/">https://nodejs.org/en/blog/vulnerability/february-2023-security-releases/</a></p>
<h2>v5.19.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(fetch): raise AbortSignal max event listeners by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1910">nodejs/undici#1910</a></li>
<li>fix: content-disposition header parsing by <a href="https://github.com/climba03003"><code>@​climba03003</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1911">nodejs/undici#1911</a></li>
<li>fix: remove test by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1916">nodejs/undici#1916</a></li>
<li>feat: add Headers.prototype.getSetCookie by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1915">nodejs/undici#1915</a></li>
<li>fix(headers): clone getSetCookie list &amp; add getSetCookie type by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1917">nodejs/undici#1917</a></li>
<li>doc(mock): update out-of-date reply documentation by <a href="https://github.com/p9f"><code>@​p9f</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1913">nodejs/undici#1913</a></li>
<li>fix(types): add missing keepAlive params by <a href="https://github.com/SkeLLLa"><code>@​SkeLLLa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1918">nodejs/undici#1918</a></li>
<li>Make the fetch() abort test pass locally, on Linux and Mac, Node 18/19. by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1927">nodejs/undici#1927</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/climba03003"><code>@​climba03003</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1911">nodejs/undici#1911</a></li>
<li><a href="https://github.com/p9f"><code>@​p9f</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1913">nodejs/undici#1913</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.18.0...v5.19.0">https://github.com/nodejs/undici/compare/v5.18.0...v5.19.0</a></p>
<h2>v5.18.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Add ability to set TCP keepalive by <a href="https://github.com/xconverge"><code>@​xconverge</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1904">nodejs/undici#1904</a></li>
<li>use faster timers by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1908">nodejs/undici#1908</a></li>
<li>fix: ensure header value is a string by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1899">nodejs/undici#1899</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.17.1...v5.18.0">https://github.com/nodejs/undici/compare/v5.17.1...v5.18.0</a></p>
<h2>v5.17.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: bad buffer slice (<a href="https://github.com/nodejs/undici/commit/d2be675575512794dcd41b9683b209fc15368154">https://github.com/nodejs/undici/commit/d2be675575512794dcd41b9683b209fc15368154</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.17.0...v5.17.1">https://github.com/nodejs/undici/compare/v5.17.0...v5.17.1</a></p>
<h2>v5.17.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(wpts): Blob is a global getter in &gt;=v19.x.x by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1880">nodejs/undici#1880</a></li>
<li>doc: fix anchor links dispatcher.stream by <a href="https://github.com/RafaelGSS"><code>@​RafaelGSS</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1881">nodejs/undici#1881</a></li>
<li>wpt: make runner more resilient by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1884">nodejs/undici#1884</a></li>
<li>Make test pass in v19.x by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1879">nodejs/undici#1879</a></li>
<li>Correct the type of DispatchOptions[&quot;headers&quot;] by <a href="https://github.com/pan93412"><code>@​pan93412</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1896">nodejs/undici#1896</a></li>
<li>perf(content-type parser): faster string collector by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1894">nodejs/undici#1894</a></li>
<li>feat: expose content-type parser by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1895">nodejs/undici#1895</a></li>
<li>fix(types): Update DispatchOptions type for missing &quot;blocking&quot; by <a href="https://github.com/xconverge"><code>@​xconverge</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1889">nodejs/undici#1889</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/984d53bad97c98529424a7f3bef6be1d0e76d039"><code>984d53b</code></a> Bumped v5.19.1</li>
<li><a href="https://github.com/nodejs/undici/commit/6c32c0fd5b874328e5e1f635e2cc431aa21cddab"><code>6c32c0f</code></a> lint fixes</li>
<li><a href="https://github.com/nodejs/undici/commit/f2324e549943f0b0937b09fb1c0c16cc7c93abdf"><code>f2324e5</code></a> Merge pull request from GHSA-r6ch-mqf9-qc9w</li>
<li><a href="https://github.com/nodejs/undici/commit/a2eff05401358f6595138df963837c24348f2034"><code>a2eff05</code></a> Merge pull request from GHSA-5r9g-qh6m-jxff</li>
<li><a href="https://github.com/nodejs/undici/commit/f5c89e5c87c7d702996b152c4ad86302b60c4181"><code>f5c89e5</code></a> Bumped v5.19.0</li>
<li><a href="https://github.com/nodejs/undici/commit/f7c6c6a4a2aef7ee3b8207c4eeab700cb0cfc7dc"><code>f7c6c6a</code></a> Make the fetch() abort test pass locally, on Linux and Mac, Node 18 and 19 (#...</li>
<li><a href="https://github.com/nodejs/undici/commit/aebb232d22e9adafce015b985093114a95b560f0"><code>aebb232</code></a> fix(types): add missing keepAlive params (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1918">#1918</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/e155c6db5cec9bc577d548fa7c7378013631c79c"><code>e155c6d</code></a> doc(mock): update out-of-date reply documentation (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1913">#1913</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/87fa73498d6014a33989179cfaa4347dcb29600f"><code>87fa734</code></a> fix(headers): clone getSetCookie list &amp; add getSetCookie type (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1917">#1917</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ba5ef44b71eff5a86a8473850a326ff7392664d3"><code>ba5ef44</code></a> feat: add Headers.prototype.getSetCookie (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1915">#1915</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.9.1...v5.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.9.1&new-version=5.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-02-17 00:09:36 +0000 UTC
    </div>
</div>

