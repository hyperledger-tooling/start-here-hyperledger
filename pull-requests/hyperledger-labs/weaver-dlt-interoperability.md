---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/440" class=".btn">#440</a>
            </td>
            <td>
                <b>
                    build(deps): Bump h2 from 0.3.17 to 0.3.26 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.17 to 0.3.26.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/releases">h2's releases</a>.</em></p>
<blockquote>
<h2>v0.3.26</h2>
<h2>What's Changed</h2>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<p>See <a href="https://seanmonstar.com/blog/hyper-http2-continuation-flood/">https://seanmonstar.com/blog/hyper-http2-continuation-flood/</a> for more info.</p>
<h2>v0.3.25</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: optimize header list size calculations by <a href="https://github.com/Noah-Kennedy"><code>@​Noah-Kennedy</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/750">hyperium/h2#750</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25">https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25</a></p>
<h2>v0.3.24</h2>
<h2>Fixed</h2>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h2>v0.3.23</h2>
<h2>What's Changed</h2>
<ul>
<li>cherry-pick fix: streams awaiting capacity lockout in <a href="https://redirect.github.com/hyperium/h2/pull/734">hyperium/h2#734</a></li>
</ul>
<h2>v0.3.22</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>header_table_size(usize)</code> option to client and server builders.</li>
<li>Improve throughput when vectored IO is not available.</li>
<li>Update indexmap to 2.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/tottoto"><code>@​tottoto</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/714">hyperium/h2#714</a></li>
<li><a href="https://github.com/xiaoyawei"><code>@​xiaoyawei</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/712">hyperium/h2#712</a></li>
<li><a href="https://github.com/Protryon"><code>@​Protryon</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/719">hyperium/h2#719</a></li>
<li><a href="https://github.com/4JX"><code>@​4JX</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/638">hyperium/h2#638</a></li>
<li><a href="https://github.com/vuittont60"><code>@​vuittont60</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/724">hyperium/h2#724</a></li>
</ul>
<h2>v0.3.21</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix opening of new streams over peer's max concurrent limit.</li>
<li>Fix <code>RecvStream</code> to return data even if it has received a <code>CANCEL</code> stream error.</li>
<li>Update MSRV to 1.63.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/DDtKey"><code>@​DDtKey</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/703">hyperium/h2#703</a></li>
<li><a href="https://github.com/jwilm"><code>@​jwilm</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/707">hyperium/h2#707</a></li>
</ul>
<h2>v0.3.20</h2>
<h2>Bug Fixes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/blob/v0.3.26/CHANGELOG.md">h2's changelog</a>.</em></p>
<blockquote>
<h1>0.3.26 (April 3, 2024)</h1>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<h1>0.3.25 (March 15, 2024)</h1>
<ul>
<li>Improve performance decoding many headers.</li>
</ul>
<h1>0.3.24 (January 17, 2024)</h1>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h1>0.3.23 (January 10, 2024)</h1>
<ul>
<li>Backport fix from 0.4.1 for stream capacity assignment.</li>
</ul>
<h1>0.3.22 (November 15, 2023)</h1>
<ul>
<li>Add <code>header_table_size(usize)</code> option to client and server builders.</li>
<li>Improve throughput when vectored IO is not available.</li>
<li>Update indexmap to 2.</li>
</ul>
<h1>0.3.21 (August 21, 2023)</h1>
<ul>
<li>Fix opening of new streams over peer's max concurrent limit.</li>
<li>Fix <code>RecvStream</code> to return data even if it has received a <code>CANCEL</code> stream error.</li>
<li>Update MSRV to 1.63.</li>
</ul>
<h1>0.3.20 (June 26, 2023)</h1>
<ul>
<li>Fix panic if a server received a request with a <code>:status</code> pseudo header in the 1xx range.</li>
<li>Fix panic if a reset stream had pending push promises that were more than allowed.</li>
<li>Fix potential flow control overflow by subtraction, instead returning a connection error.</li>
</ul>
<h1>0.3.19 (May 12, 2023)</h1>
<ul>
<li>Fix counting reset streams when triggered by a GOAWAY.</li>
<li>Send <code>too_many_resets</code> in opaque debug data of GOAWAY when too many resets received.</li>
</ul>
<h1>0.3.18 (April 17, 2023)</h1>
<ul>
<li>Fix panic because of opposite check in <code>is_remote_local()</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/h2/commit/357127e279c06935830fe2140378312eac801494"><code>357127e</code></a> v0.3.26</li>
<li><a href="https://github.com/hyperium/h2/commit/1a357aaefc7243fdfa9442f45d90be17794a4004"><code>1a357aa</code></a> fix: limit number of CONTINUATION frames allowed</li>
<li><a href="https://github.com/hyperium/h2/commit/5b6c9e0da092728d702dff3607626aafb7809d77"><code>5b6c9e0</code></a> refactor: cleanup new unused warnings (<a href="https://redirect.github.com/hyperium/h2/issues/757">#757</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/3a798327211345b9b2bf797e2e4f3aca4e0ddfee"><code>3a79832</code></a> v0.3.25</li>
<li><a href="https://github.com/hyperium/h2/commit/94e80b1c72bec282bb5d13596803e6fb341fec4c"><code>94e80b1</code></a> perf: optimize header list size calculations (<a href="https://redirect.github.com/hyperium/h2/issues/750">#750</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/7243ab5854b2375213a5a2cdfd543f1d669661e2"><code>7243ab5</code></a> Prepare v0.3.24</li>
<li><a href="https://github.com/hyperium/h2/commit/d919cd6fd8e0f4f5d1f6282fab0b38a1b4bf999c"><code>d919cd6</code></a> streams: limit error resets for misbehaving connections</li>
<li><a href="https://github.com/hyperium/h2/commit/a7eb14a487c0094187314fca63cfe4de4d3d78ef"><code>a7eb14a</code></a> v0.3.23</li>
<li><a href="https://github.com/hyperium/h2/commit/b668c7fbe22e0cb4a76b0a67498cbb4d0aacbc75"><code>b668c7f</code></a> fix: streams awaiting capacity lockout (<a href="https://redirect.github.com/hyperium/h2/issues/730">#730</a>) (<a href="https://redirect.github.com/hyperium/h2/issues/734">#734</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/0f412d8b9c8d309966197873ad1d065adc23c794"><code>0f412d8</code></a> v0.3.22</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/h2/compare/v0.3.17...v0.3.26">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.17&new-version=0.3.26)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-05 15:57:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    build(deps): Bump h2 from 0.3.17 to 0.3.26 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.17 to 0.3.26.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/releases">h2's releases</a>.</em></p>
<blockquote>
<h2>v0.3.26</h2>
<h2>What's Changed</h2>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<p>See <a href="https://seanmonstar.com/blog/hyper-http2-continuation-flood/">https://seanmonstar.com/blog/hyper-http2-continuation-flood/</a> for more info.</p>
<h2>v0.3.25</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: optimize header list size calculations by <a href="https://github.com/Noah-Kennedy"><code>@​Noah-Kennedy</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/750">hyperium/h2#750</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25">https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25</a></p>
<h2>v0.3.24</h2>
<h2>Fixed</h2>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h2>v0.3.23</h2>
<h2>What's Changed</h2>
<ul>
<li>cherry-pick fix: streams awaiting capacity lockout in <a href="https://redirect.github.com/hyperium/h2/pull/734">hyperium/h2#734</a></li>
</ul>
<h2>v0.3.22</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>header_table_size(usize)</code> option to client and server builders.</li>
<li>Improve throughput when vectored IO is not available.</li>
<li>Update indexmap to 2.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/tottoto"><code>@​tottoto</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/714">hyperium/h2#714</a></li>
<li><a href="https://github.com/xiaoyawei"><code>@​xiaoyawei</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/712">hyperium/h2#712</a></li>
<li><a href="https://github.com/Protryon"><code>@​Protryon</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/719">hyperium/h2#719</a></li>
<li><a href="https://github.com/4JX"><code>@​4JX</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/638">hyperium/h2#638</a></li>
<li><a href="https://github.com/vuittont60"><code>@​vuittont60</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/724">hyperium/h2#724</a></li>
</ul>
<h2>v0.3.21</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix opening of new streams over peer's max concurrent limit.</li>
<li>Fix <code>RecvStream</code> to return data even if it has received a <code>CANCEL</code> stream error.</li>
<li>Update MSRV to 1.63.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/DDtKey"><code>@​DDtKey</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/703">hyperium/h2#703</a></li>
<li><a href="https://github.com/jwilm"><code>@​jwilm</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/707">hyperium/h2#707</a></li>
</ul>
<h2>v0.3.20</h2>
<h2>Bug Fixes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/blob/v0.3.26/CHANGELOG.md">h2's changelog</a>.</em></p>
<blockquote>
<h1>0.3.26 (April 3, 2024)</h1>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<h1>0.3.25 (March 15, 2024)</h1>
<ul>
<li>Improve performance decoding many headers.</li>
</ul>
<h1>0.3.24 (January 17, 2024)</h1>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h1>0.3.23 (January 10, 2024)</h1>
<ul>
<li>Backport fix from 0.4.1 for stream capacity assignment.</li>
</ul>
<h1>0.3.22 (November 15, 2023)</h1>
<ul>
<li>Add <code>header_table_size(usize)</code> option to client and server builders.</li>
<li>Improve throughput when vectored IO is not available.</li>
<li>Update indexmap to 2.</li>
</ul>
<h1>0.3.21 (August 21, 2023)</h1>
<ul>
<li>Fix opening of new streams over peer's max concurrent limit.</li>
<li>Fix <code>RecvStream</code> to return data even if it has received a <code>CANCEL</code> stream error.</li>
<li>Update MSRV to 1.63.</li>
</ul>
<h1>0.3.20 (June 26, 2023)</h1>
<ul>
<li>Fix panic if a server received a request with a <code>:status</code> pseudo header in the 1xx range.</li>
<li>Fix panic if a reset stream had pending push promises that were more than allowed.</li>
<li>Fix potential flow control overflow by subtraction, instead returning a connection error.</li>
</ul>
<h1>0.3.19 (May 12, 2023)</h1>
<ul>
<li>Fix counting reset streams when triggered by a GOAWAY.</li>
<li>Send <code>too_many_resets</code> in opaque debug data of GOAWAY when too many resets received.</li>
</ul>
<h1>0.3.18 (April 17, 2023)</h1>
<ul>
<li>Fix panic because of opposite check in <code>is_remote_local()</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/h2/commit/357127e279c06935830fe2140378312eac801494"><code>357127e</code></a> v0.3.26</li>
<li><a href="https://github.com/hyperium/h2/commit/1a357aaefc7243fdfa9442f45d90be17794a4004"><code>1a357aa</code></a> fix: limit number of CONTINUATION frames allowed</li>
<li><a href="https://github.com/hyperium/h2/commit/5b6c9e0da092728d702dff3607626aafb7809d77"><code>5b6c9e0</code></a> refactor: cleanup new unused warnings (<a href="https://redirect.github.com/hyperium/h2/issues/757">#757</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/3a798327211345b9b2bf797e2e4f3aca4e0ddfee"><code>3a79832</code></a> v0.3.25</li>
<li><a href="https://github.com/hyperium/h2/commit/94e80b1c72bec282bb5d13596803e6fb341fec4c"><code>94e80b1</code></a> perf: optimize header list size calculations (<a href="https://redirect.github.com/hyperium/h2/issues/750">#750</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/7243ab5854b2375213a5a2cdfd543f1d669661e2"><code>7243ab5</code></a> Prepare v0.3.24</li>
<li><a href="https://github.com/hyperium/h2/commit/d919cd6fd8e0f4f5d1f6282fab0b38a1b4bf999c"><code>d919cd6</code></a> streams: limit error resets for misbehaving connections</li>
<li><a href="https://github.com/hyperium/h2/commit/a7eb14a487c0094187314fca63cfe4de4d3d78ef"><code>a7eb14a</code></a> v0.3.23</li>
<li><a href="https://github.com/hyperium/h2/commit/b668c7fbe22e0cb4a76b0a67498cbb4d0aacbc75"><code>b668c7f</code></a> fix: streams awaiting capacity lockout (<a href="https://redirect.github.com/hyperium/h2/issues/730">#730</a>) (<a href="https://redirect.github.com/hyperium/h2/issues/734">#734</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/0f412d8b9c8d309966197873ad1d065adc23c794"><code>0f412d8</code></a> v0.3.22</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/h2/compare/v0.3.17...v0.3.26">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.17&new-version=0.3.26)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-05 15:56:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /samples/fabric/go-cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/437" class=".btn">#437</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /sdks/fabric/go-sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:22:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /core/network/fabric-interop-cc/libs/assetexchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:22:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.27.1 to 1.33.0 in /core/network/fabric-interop-cc/libs/testutils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.27.1 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.27.1&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:21:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/434" class=".btn">#434</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /core/network/fabric-interop-cc/libs/utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:21:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/433" class=".btn">#433</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.27.1 to 1.33.0 in /samples/fabric/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.27.1 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.27.1&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:21:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /samples/fabric/simpleassettransfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:21:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /samples/fabric/simplestatewithacl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:21:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /samples/fabric/simpleassetandinterop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:21:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    build(deps): Bump google.golang.org/protobuf from 1.30.0 to 1.33.0 in /common/protos-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.30.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.30.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 06:21:39 +0000 UTC
    </div>
</div>

