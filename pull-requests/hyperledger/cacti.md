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
                PR <a href="https://github.com/hyperledger/cacti/pull/2294" class=".btn">#2294</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.10.0 to 5.19.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.10.0 to 5.19.1.
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
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.10.0...v5.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.10.0&new-version=5.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 21:50:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2293" class=".btn">#2293</a>
            </td>
            <td>
                <b>
                    feat(quorum): private transaction support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #951



Co-authored-by: Travis Payne <travis.payne@accenture.com>
Co-authored-by: johnhomantaring <john.h.o.mantaring@accenture.com>
Co-authored-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
Co-authored-by: aldousalvarez aldousss.alvarez@gmail.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 07:49:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2292" class=".btn">#2292</a>
            </td>
            <td>
                <b>
                    Bump werkzeug from 2.0.1 to 2.2.3 in /packages-python/cactus_validator_socketio_indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [werkzeug](https://github.com/pallets/werkzeug) from 2.0.1 to 2.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/werkzeug/releases">werkzeug's releases</a>.</em></p>
<blockquote>
<h2>2.2.3</h2>
<p>This is a fix release for the 2.2.x release branch.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-3">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/26?closed=1">https://github.com/pallets/werkzeug/milestone/26?closed=1</a></li>
</ul>
<p>This release contains security fixes for:</p>
<ul>
<li><a href="https://github.com/pallets/werkzeug/security/advisories/GHSA-xg9f-g7g7-2323">https://github.com/pallets/werkzeug/security/advisories/GHSA-xg9f-g7g7-2323</a></li>
<li><a href="https://github.com/pallets/werkzeug/security/advisories/GHSA-px8h-6qxv-m22q">https://github.com/pallets/werkzeug/security/advisories/GHSA-px8h-6qxv-m22q</a></li>
</ul>
<h2>2.2.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-2">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/25?closed=1">https://github.com/pallets/werkzeug/milestone/25?closed=1</a></li>
</ul>
<h2>2.2.1</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-1">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/24?closed=1">https://github.com/pallets/werkzeug/milestone/24?closed=1</a></li>
</ul>
<h2>2.2.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated features. The 2.2.x branch is now the supported bugfix branch, the 2.1.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-0">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/20?closed=1">https://github.com/pallets/werkzeug/milestone/20?closed=1</a></li>
</ul>
<h2>2.1.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.1.0">2.1.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-2">https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/22?closed=1">https://github.com/pallets/werkzeug/milestone/22?closed=1</a></li>
</ul>
<h2>2.1.1</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.1.0">2.1.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-1">https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/19?closed=1">https://github.com/pallets/werkzeug/milestone/19?closed=1</a></li>
</ul>
<h2>2.1.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated features. The 2.1.x branch is now the supported bugfix branch, the 2.0.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-0">https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/16?closed=1">https://github.com/pallets/werkzeug/milestone/16?closed=1</a></li>
</ul>
<h2>2.0.3</h2>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.0.x/changes/#version-2-0-3">https://werkzeug.palletsprojects.com/en/2.0.x/changes/#version-2-0-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/18?closed=1">https://github.com/pallets/werkzeug/milestone/18?closed=1</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/werkzeug/blob/main/CHANGES.rst">werkzeug's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.2.3</h2>
<p>Released 2023-02-14</p>
<ul>
<li>Ensure that URL rules using path converters will redirect with strict slashes when
the trailing slash is missing. :issue:<code>2533</code></li>
<li>Type signature for <code>get_json</code> specifies that return type is not optional when
<code>silent=False</code>. :issue:<code>2508</code></li>
<li><code>parse_content_range_header</code> returns <code>None</code> for a value like <code>bytes */-1</code>
where the length is invalid, instead of raising an <code>AssertionError</code>. :issue:<code>2531</code></li>
<li>Address remaining <code>ResourceWarning</code> related to the socket used by <code>run_simple</code>.
Remove <code>prepare_socket</code>, which now happens when creating the server. :issue:<code>2421</code></li>
<li>Update pre-existing headers for <code>multipart/form-data</code> requests with the test
client. :issue:<code>2549</code></li>
<li>Fix handling of header extended parameters such that they are no longer quoted.
:issue:<code>2529</code></li>
<li><code>LimitedStream.read</code> works correctly when wrapping a stream that may not return
the requested size in one <code>read</code> call. :issue:<code>2558</code></li>
<li>A cookie header that starts with <code>=</code> is treated as an empty key and discarded,
rather than stripping the leading <code>==</code>.</li>
<li>Specify a maximum number of multipart parts, default 1000, after which a
<code>RequestEntityTooLarge</code> exception is raised on parsing. This mitigates a DoS
attack where a larger number of form/file parts would result in disproportionate
resource use.</li>
</ul>
<h2>Version 2.2.2</h2>
<p>Released 2022-08-08</p>
<ul>
<li>Fix router to restore the 2.1 <code>strict_slashes == False</code> behaviour
whereby leaf-requests match branch rules and vice
versa. :pr:<code>2489</code></li>
<li>Fix router to identify invalid rules rather than hang parsing them,
and to correctly parse <code>/</code> within converter arguments. :pr:<code>2489</code></li>
<li>Update subpackage imports in :mod:<code>werkzeug.routing</code> to use the
<code>import as</code> syntax for explicitly re-exporting public attributes.
:pr:<code>2493</code></li>
<li>Parsing of some invalid header characters is more robust. :pr:<code>2494</code></li>
<li>When starting the development server, a warning not to use it in a
production deployment is always shown. :issue:<code>2480</code></li>
<li><code>LocalProxy.__wrapped__</code> is always set to the wrapped object when
the proxy is unbound, fixing an issue in doctest that would cause it
to fail. :issue:<code>2485</code></li>
<li>Address one <code>ResourceWarning</code> related to the socket used by
<code>run_simple</code>. :issue:<code>2421</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/werkzeug/commit/22a254fca2ad0130adbbcbd11d3de51bcb04a08b"><code>22a254f</code></a> release version 2.2.3</li>
<li><a href="https://github.com/pallets/werkzeug/commit/517cac5a804e8c4dc4ed038bb20dacd038e7a9f1"><code>517cac5</code></a> Merge pull request from GHSA-xg9f-g7g7-2323</li>
<li><a href="https://github.com/pallets/werkzeug/commit/babc8d9e8c9fa995ef26050698bc9b5a92803664"><code>babc8d9</code></a> rewrite docs about request data limits</li>
<li><a href="https://github.com/pallets/werkzeug/commit/09449ee77934a0c883f5959785864ecae6aaa2c9"><code>09449ee</code></a> clean up docs</li>
<li><a href="https://github.com/pallets/werkzeug/commit/fe899d0cdf767a7289a8bf746b7f72c2907a1b4b"><code>fe899d0</code></a> limit the maximum number of multipart form parts</li>
<li><a href="https://github.com/pallets/werkzeug/commit/cf275f42acad1b5950c50ffe8ef58fe62cdce028"><code>cf275f4</code></a> Merge pull request from GHSA-px8h-6qxv-m22q</li>
<li><a href="https://github.com/pallets/werkzeug/commit/8c2b4b82d0cade0d37e6a88e2cd2413878e8ebd4"><code>8c2b4b8</code></a> don't strip leading = when parsing cookie</li>
<li><a href="https://github.com/pallets/werkzeug/commit/7c7ce5cb73f3f7d3b9c09340e4f322aeb583dbc5"><code>7c7ce5c</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://github-redirect.dependabot.com/pallets/werkzeug/issues/2585">#2585</a>)</li>
<li><a href="https://github.com/pallets/werkzeug/commit/19ae03e6a39b3f63fd08fef4fddae4385cdddf25"><code>19ae03e</code></a> [pre-commit.ci] auto fixes from pre-commit.com hooks</li>
<li><a href="https://github.com/pallets/werkzeug/commit/a83d3b8bf070810874c8e8d03dcce270666e10fe"><code>a83d3b8</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/werkzeug/compare/2.0.1...2.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=werkzeug&package-manager=pip&previous-version=2.0.1&new-version=2.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 04:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2291" class=".btn">#2291</a>
            </td>
            <td>
                <b>
                    Bump werkzeug from 2.0.1 to 2.2.3 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [werkzeug](https://github.com/pallets/werkzeug) from 2.0.1 to 2.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/werkzeug/releases">werkzeug's releases</a>.</em></p>
<blockquote>
<h2>2.2.3</h2>
<p>This is a fix release for the 2.2.x release branch.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-3">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/26?closed=1">https://github.com/pallets/werkzeug/milestone/26?closed=1</a></li>
</ul>
<p>This release contains security fixes for:</p>
<ul>
<li><a href="https://github.com/pallets/werkzeug/security/advisories/GHSA-xg9f-g7g7-2323">https://github.com/pallets/werkzeug/security/advisories/GHSA-xg9f-g7g7-2323</a></li>
<li><a href="https://github.com/pallets/werkzeug/security/advisories/GHSA-px8h-6qxv-m22q">https://github.com/pallets/werkzeug/security/advisories/GHSA-px8h-6qxv-m22q</a></li>
</ul>
<h2>2.2.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-2">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/25?closed=1">https://github.com/pallets/werkzeug/milestone/25?closed=1</a></li>
</ul>
<h2>2.2.1</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-1">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/24?closed=1">https://github.com/pallets/werkzeug/milestone/24?closed=1</a></li>
</ul>
<h2>2.2.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated features. The 2.2.x branch is now the supported bugfix branch, the 2.1.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-0">https://werkzeug.palletsprojects.com/en/2.2.x/changes/#version-2-2-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/20?closed=1">https://github.com/pallets/werkzeug/milestone/20?closed=1</a></li>
</ul>
<h2>2.1.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.1.0">2.1.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-2">https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/22?closed=1">https://github.com/pallets/werkzeug/milestone/22?closed=1</a></li>
</ul>
<h2>2.1.1</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/werkzeug/releases/tag/2.1.0">2.1.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-1">https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/19?closed=1">https://github.com/pallets/werkzeug/milestone/19?closed=1</a></li>
</ul>
<h2>2.1.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated features. The 2.1.x branch is now the supported bugfix branch, the 2.0.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-0">https://werkzeug.palletsprojects.com/en/2.1.x/changes/#version-2-1-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/16?closed=1">https://github.com/pallets/werkzeug/milestone/16?closed=1</a></li>
</ul>
<h2>2.0.3</h2>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.0.x/changes/#version-2-0-3">https://werkzeug.palletsprojects.com/en/2.0.x/changes/#version-2-0-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/18?closed=1">https://github.com/pallets/werkzeug/milestone/18?closed=1</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/werkzeug/blob/main/CHANGES.rst">werkzeug's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.2.3</h2>
<p>Released 2023-02-14</p>
<ul>
<li>Ensure that URL rules using path converters will redirect with strict slashes when
the trailing slash is missing. :issue:<code>2533</code></li>
<li>Type signature for <code>get_json</code> specifies that return type is not optional when
<code>silent=False</code>. :issue:<code>2508</code></li>
<li><code>parse_content_range_header</code> returns <code>None</code> for a value like <code>bytes */-1</code>
where the length is invalid, instead of raising an <code>AssertionError</code>. :issue:<code>2531</code></li>
<li>Address remaining <code>ResourceWarning</code> related to the socket used by <code>run_simple</code>.
Remove <code>prepare_socket</code>, which now happens when creating the server. :issue:<code>2421</code></li>
<li>Update pre-existing headers for <code>multipart/form-data</code> requests with the test
client. :issue:<code>2549</code></li>
<li>Fix handling of header extended parameters such that they are no longer quoted.
:issue:<code>2529</code></li>
<li><code>LimitedStream.read</code> works correctly when wrapping a stream that may not return
the requested size in one <code>read</code> call. :issue:<code>2558</code></li>
<li>A cookie header that starts with <code>=</code> is treated as an empty key and discarded,
rather than stripping the leading <code>==</code>.</li>
<li>Specify a maximum number of multipart parts, default 1000, after which a
<code>RequestEntityTooLarge</code> exception is raised on parsing. This mitigates a DoS
attack where a larger number of form/file parts would result in disproportionate
resource use.</li>
</ul>
<h2>Version 2.2.2</h2>
<p>Released 2022-08-08</p>
<ul>
<li>Fix router to restore the 2.1 <code>strict_slashes == False</code> behaviour
whereby leaf-requests match branch rules and vice
versa. :pr:<code>2489</code></li>
<li>Fix router to identify invalid rules rather than hang parsing them,
and to correctly parse <code>/</code> within converter arguments. :pr:<code>2489</code></li>
<li>Update subpackage imports in :mod:<code>werkzeug.routing</code> to use the
<code>import as</code> syntax for explicitly re-exporting public attributes.
:pr:<code>2493</code></li>
<li>Parsing of some invalid header characters is more robust. :pr:<code>2494</code></li>
<li>When starting the development server, a warning not to use it in a
production deployment is always shown. :issue:<code>2480</code></li>
<li><code>LocalProxy.__wrapped__</code> is always set to the wrapped object when
the proxy is unbound, fixing an issue in doctest that would cause it
to fail. :issue:<code>2485</code></li>
<li>Address one <code>ResourceWarning</code> related to the socket used by
<code>run_simple</code>. :issue:<code>2421</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/werkzeug/commit/22a254fca2ad0130adbbcbd11d3de51bcb04a08b"><code>22a254f</code></a> release version 2.2.3</li>
<li><a href="https://github.com/pallets/werkzeug/commit/517cac5a804e8c4dc4ed038bb20dacd038e7a9f1"><code>517cac5</code></a> Merge pull request from GHSA-xg9f-g7g7-2323</li>
<li><a href="https://github.com/pallets/werkzeug/commit/babc8d9e8c9fa995ef26050698bc9b5a92803664"><code>babc8d9</code></a> rewrite docs about request data limits</li>
<li><a href="https://github.com/pallets/werkzeug/commit/09449ee77934a0c883f5959785864ecae6aaa2c9"><code>09449ee</code></a> clean up docs</li>
<li><a href="https://github.com/pallets/werkzeug/commit/fe899d0cdf767a7289a8bf746b7f72c2907a1b4b"><code>fe899d0</code></a> limit the maximum number of multipart form parts</li>
<li><a href="https://github.com/pallets/werkzeug/commit/cf275f42acad1b5950c50ffe8ef58fe62cdce028"><code>cf275f4</code></a> Merge pull request from GHSA-px8h-6qxv-m22q</li>
<li><a href="https://github.com/pallets/werkzeug/commit/8c2b4b82d0cade0d37e6a88e2cd2413878e8ebd4"><code>8c2b4b8</code></a> don't strip leading = when parsing cookie</li>
<li><a href="https://github.com/pallets/werkzeug/commit/7c7ce5cb73f3f7d3b9c09340e4f322aeb583dbc5"><code>7c7ce5c</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://github-redirect.dependabot.com/pallets/werkzeug/issues/2585">#2585</a>)</li>
<li><a href="https://github.com/pallets/werkzeug/commit/19ae03e6a39b3f63fd08fef4fddae4385cdddf25"><code>19ae03e</code></a> [pre-commit.ci] auto fixes from pre-commit.com hooks</li>
<li><a href="https://github.com/pallets/werkzeug/commit/a83d3b8bf070810874c8e8d03dcce270666e10fe"><code>a83d3b8</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/werkzeug/compare/2.0.1...2.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=werkzeug&package-manager=pip&previous-version=2.0.1&new-version=2.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 04:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2289" class=".btn">#2289</a>
            </td>
            <td>
                <b>
                    New README and illustrations for the Cacti Project
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sketched out a tentative roadmap for the deeper merging of the Cactus and Weaver code bases.

Signed-off-by: VRamakrishna <vramakr2@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 19:44:21 +0000 UTC
    </div>
</div>

