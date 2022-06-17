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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Bump futures-task from 0.3.5 to 0.3.21 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [futures-task](https://github.com/rust-lang/futures-rs) from 0.3.5 to 0.3.21.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/futures-rs/releases">futures-task's releases</a>.</em></p>
<blockquote>
<h2>0.3.21</h2>
<ul>
<li>Fix potential data race in <code>FlattenUnordered</code> that introduced in 0.3.20 (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2566">#2566</a>)</li>
</ul>
<h2>0.3.20</h2>
<ul>
<li>Fix stacked borrows violations when <code>-Zmiri-tag-raw-pointers</code> is enabled. This raises MSRV of <code>futures-task</code> to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2548">#2548</a>, <a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2550">#2550</a>)</li>
<li>Change <code>FuturesUnordered</code> to respect yielding from future (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2551">#2551</a>)</li>
<li>Add <code>StreamExt::{flatten_unordered, flat_map_unordered}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2083">#2083</a>)</li>
</ul>
<h2>0.3.19</h2>
<ul>
<li>Remove unstable <code>read-initializer</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2534">#2534</a>)</li>
<li>Fix panic in <code>FuturesUnordered</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2535">#2535</a>)</li>
<li>Fix compatibility issue with <code>FuturesUnordered</code> and tokio's cooperative scheduling (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2527">#2527</a>)</li>
<li>Add <code>StreamExt::count</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2495">#2495</a>)</li>
</ul>
<h2>0.3.18</h2>
<ul>
<li>Fix unusable <code>Sink</code> implementation on <code>stream::Scan</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2499">#2499</a>)</li>
<li>Make <code>task::noop_waker_ref</code> available without <code>std</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2505">#2505</a>)</li>
<li>Add async <code>LineWriter</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2477">#2477</a>)</li>
<li>Remove dependency on <code>proc-macro-hack</code>. This raises MSRV of utility crates to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2520">#2520</a>)</li>
</ul>
<h2>0.3.17</h2>
<ul>
<li>Use <code>FuturesOrdered</code> in <code>join_all</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2412">#2412</a>)</li>
<li>Add <code>{future, stream}::poll_immediate</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2452">#2452</a>)</li>
<li>Add <code>stream_select!</code> macro (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2262">#2262</a>)</li>
<li>Implement <code>Default</code> for <code>OptionFuture</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2471">#2471</a>)</li>
<li>Add <code>Peekable::{peek_mut, poll_peek_mut}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2488">#2488</a>)</li>
<li>Add <code>BufReader::seek_relative</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2489">#2489</a>)</li>
</ul>
<h2>0.3.16</h2>
<ul>
<li>Add <code>TryStreamExt::try_chunks</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2438">#2438</a>)</li>
<li>Add <code>StreamExt::{all, any}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2460">#2460</a>)</li>
<li>Add <code>stream::select_with_strategy</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2450">#2450</a>)</li>
<li>Update to new <code>io_slice_advance</code> interface (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2454">#2454</a>)</li>
</ul>
<h2>0.3.15</h2>
<ul>
<li>Use <code>#[proc_macro]</code> at Rust 1.45+ to fix an issue where proc macros don't work with rust-analyzer (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2407">#2407</a>)</li>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2400">#2400</a>)</li>
<li>futures-test: Add async <code>#[test]</code> function attribute (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2409">#2409</a>)</li>
<li>Add <code>stream::abortable</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2410">#2410</a>)</li>
<li>Add <code>FuturesUnordered::clear</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2415">#2415</a>)</li>
<li>Implement <code>IntoIterator</code> for <code>FuturesUnordered</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2423">#2423</a>)</li>
<li>Implement <code>Send</code> and <code>Sync</code> for <code>FuturesUnordered</code> iterators (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2416">#2416</a>)</li>
<li>Make <code>FuturesUnordered::iter_pin_ref</code> public (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2423">#2423</a>)</li>
<li>Add <code>SelectAll::clear</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2430">#2430</a>)</li>
<li>Add <code>SelectAll::{iter, iter_mut}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2428">#2428</a>)</li>
<li>Implement <code>IntoIterator</code> for <code>SelectAll</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2428">#2428</a>)</li>
<li>Implement <code>Clone</code> for <code>WeakShared</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2396">#2396</a>)</li>
</ul>
<h2>0.3.14</h2>
<ul>
<li>Add <code>future::SelectAll::into_inner</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2363">#2363</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/futures-rs/blob/master/CHANGELOG.md">futures-task's changelog</a>.</em></p>
<blockquote>
<h1>0.3.21 - 2022-02-06</h1>
<ul>
<li>Fix potential data race in <code>FlattenUnordered</code> that introduced in 0.3.20 (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2566">#2566</a>)</li>
</ul>
<h1>0.3.20 - 2022-02-06</h1>
<p>NOTE: This release has been yanked due to a bug fixed in 0.3.21.</p>
<ul>
<li>Fix stacked borrows violations when <code>-Zmiri-tag-raw-pointers</code> is enabled. This raises MSRV of <code>futures-task</code> to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2548">#2548</a>, <a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2550">#2550</a>)</li>
<li>Change <code>FuturesUnordered</code> to respect yielding from future (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2551">#2551</a>)</li>
<li>Add <code>StreamExt::{flatten_unordered, flat_map_unordered}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2083">#2083</a>)</li>
</ul>
<h1>0.3.19 - 2021-12-18</h1>
<ul>
<li>Remove unstable <code>read-initializer</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2534">#2534</a>)</li>
<li>Fix panic in <code>FuturesUnordered</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2535">#2535</a>)</li>
<li>Fix compatibility issue with <code>FuturesUnordered</code> and tokio's cooperative scheduling (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2527">#2527</a>)</li>
<li>Add <code>StreamExt::count</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2495">#2495</a>)</li>
</ul>
<h1>0.3.18 - 2021-11-23</h1>
<p>NOTE: This release has been yanked. See <a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2529">#2529</a> for details.</p>
<ul>
<li>Fix unusable <code>Sink</code> implementation on <code>stream::Scan</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2499">#2499</a>)</li>
<li>Make <code>task::noop_waker_ref</code> available without <code>std</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2505">#2505</a>)</li>
<li>Add async <code>LineWriter</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2477">#2477</a>)</li>
<li>Remove dependency on <code>proc-macro-hack</code>. This raises MSRV of utility crates to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2520">#2520</a>)</li>
</ul>
<h1>0.3.17 - 2021-08-30</h1>
<ul>
<li>Use <code>FuturesOrdered</code> in <code>join_all</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2412">#2412</a>)</li>
<li>Add <code>{future, stream}::poll_immediate</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2452">#2452</a>)</li>
<li>Add <code>stream_select!</code> macro (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2262">#2262</a>)</li>
<li>Implement <code>Default</code> for <code>OptionFuture</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2471">#2471</a>)</li>
<li>Add <code>Peekable::{peek_mut, poll_peek_mut}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2488">#2488</a>)</li>
<li>Add <code>BufReader::seek_relative</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2489">#2489</a>)</li>
</ul>
<h1>0.3.16 - 2021-07-23</h1>
<ul>
<li>Add <code>TryStreamExt::try_chunks</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2438">#2438</a>)</li>
<li>Add <code>StreamExt::{all, any}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2460">#2460</a>)</li>
<li>Add <code>stream::select_with_strategy</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2450">#2450</a>)</li>
<li>Update to new <code>io_slice_advance</code> interface (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2454">#2454</a>)</li>
</ul>
<h1>0.3.15 - 2021-05-11</h1>
<ul>
<li>Use <code>#[proc_macro]</code> at Rust 1.45+ to fix an issue where proc macros don't work with rust-analyzer (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2407">#2407</a>)</li>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2400">#2400</a>)</li>
<li>futures-test: Add async <code>#[test]</code> function attribute (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2409">#2409</a>)</li>
<li>Add <code>stream::abortable</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2410">#2410</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/futures-rs/commit/fc1e3250219170e31cddb8857a276cba7dd08d44"><code>fc1e325</code></a> Release 0.3.21</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/20279ebbfcd326e83161e44a2cf5afe1bfc3b074"><code>20279eb</code></a> <code>FlattenUnordered</code>: improve wakers behavior (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2566">#2566</a>)</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/75dca5ae7fabe6b7073558a8fc6793ee5caa7057"><code>75dca5a</code></a> Fix MSRV in futures-task readme</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/55281c8c8de6308ba97ce8b4ffd754ba204409a0"><code>55281c8</code></a> Release 0.3.20</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/591b982af835fc5e0ffb5104bbb9e942b2ed0631"><code>591b982</code></a> Redefine executor and compat modules in futures crate (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2564">#2564</a>)</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/94b508bfcb1d1f986f34f9b12d799e5a73f65f22"><code>94b508b</code></a> Basic <code>StreamExt::{flatten_unordered, flat_map_unordered}</code> impls (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2083">#2083</a>)</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/dca16fafa597d8e0075a7b693904c6f2ce0322a4"><code>dca16fa</code></a> Do not auto-create PR on fork</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/a9795a9243b0e6b836f71cbe9661bbb35bb17a7f"><code>a9795a9</code></a> Automatically creates PR when no_atomic_cas.rs needs to be updated</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/4841888d68eb8a7796ccd9c9f7a9dc677586e054"><code>4841888</code></a> Update comments in build scripts</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/85706b6d67aa30e1f8380f8101c14cf43be7500e"><code>85706b6</code></a> Clean up ci/no_atomic_cas.sh</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/futures-rs/compare/0.3.5...0.3.21">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=futures-task&package-manager=cargo&previous-version=0.3.5&new-version=0.3.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:10:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Bump futures-util from 0.3.5 to 0.3.21 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [futures-util](https://github.com/rust-lang/futures-rs) from 0.3.5 to 0.3.21.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/futures-rs/releases">futures-util's releases</a>.</em></p>
<blockquote>
<h2>0.3.21</h2>
<ul>
<li>Fix potential data race in <code>FlattenUnordered</code> that introduced in 0.3.20 (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2566">#2566</a>)</li>
</ul>
<h2>0.3.20</h2>
<ul>
<li>Fix stacked borrows violations when <code>-Zmiri-tag-raw-pointers</code> is enabled. This raises MSRV of <code>futures-task</code> to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2548">#2548</a>, <a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2550">#2550</a>)</li>
<li>Change <code>FuturesUnordered</code> to respect yielding from future (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2551">#2551</a>)</li>
<li>Add <code>StreamExt::{flatten_unordered, flat_map_unordered}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2083">#2083</a>)</li>
</ul>
<h2>0.3.19</h2>
<ul>
<li>Remove unstable <code>read-initializer</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2534">#2534</a>)</li>
<li>Fix panic in <code>FuturesUnordered</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2535">#2535</a>)</li>
<li>Fix compatibility issue with <code>FuturesUnordered</code> and tokio's cooperative scheduling (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2527">#2527</a>)</li>
<li>Add <code>StreamExt::count</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2495">#2495</a>)</li>
</ul>
<h2>0.3.18</h2>
<ul>
<li>Fix unusable <code>Sink</code> implementation on <code>stream::Scan</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2499">#2499</a>)</li>
<li>Make <code>task::noop_waker_ref</code> available without <code>std</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2505">#2505</a>)</li>
<li>Add async <code>LineWriter</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2477">#2477</a>)</li>
<li>Remove dependency on <code>proc-macro-hack</code>. This raises MSRV of utility crates to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2520">#2520</a>)</li>
</ul>
<h2>0.3.17</h2>
<ul>
<li>Use <code>FuturesOrdered</code> in <code>join_all</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2412">#2412</a>)</li>
<li>Add <code>{future, stream}::poll_immediate</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2452">#2452</a>)</li>
<li>Add <code>stream_select!</code> macro (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2262">#2262</a>)</li>
<li>Implement <code>Default</code> for <code>OptionFuture</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2471">#2471</a>)</li>
<li>Add <code>Peekable::{peek_mut, poll_peek_mut}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2488">#2488</a>)</li>
<li>Add <code>BufReader::seek_relative</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2489">#2489</a>)</li>
</ul>
<h2>0.3.16</h2>
<ul>
<li>Add <code>TryStreamExt::try_chunks</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2438">#2438</a>)</li>
<li>Add <code>StreamExt::{all, any}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2460">#2460</a>)</li>
<li>Add <code>stream::select_with_strategy</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2450">#2450</a>)</li>
<li>Update to new <code>io_slice_advance</code> interface (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2454">#2454</a>)</li>
</ul>
<h2>0.3.15</h2>
<ul>
<li>Use <code>#[proc_macro]</code> at Rust 1.45+ to fix an issue where proc macros don't work with rust-analyzer (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2407">#2407</a>)</li>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2400">#2400</a>)</li>
<li>futures-test: Add async <code>#[test]</code> function attribute (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2409">#2409</a>)</li>
<li>Add <code>stream::abortable</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2410">#2410</a>)</li>
<li>Add <code>FuturesUnordered::clear</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2415">#2415</a>)</li>
<li>Implement <code>IntoIterator</code> for <code>FuturesUnordered</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2423">#2423</a>)</li>
<li>Implement <code>Send</code> and <code>Sync</code> for <code>FuturesUnordered</code> iterators (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2416">#2416</a>)</li>
<li>Make <code>FuturesUnordered::iter_pin_ref</code> public (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2423">#2423</a>)</li>
<li>Add <code>SelectAll::clear</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2430">#2430</a>)</li>
<li>Add <code>SelectAll::{iter, iter_mut}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2428">#2428</a>)</li>
<li>Implement <code>IntoIterator</code> for <code>SelectAll</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2428">#2428</a>)</li>
<li>Implement <code>Clone</code> for <code>WeakShared</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2396">#2396</a>)</li>
</ul>
<h2>0.3.14</h2>
<ul>
<li>Add <code>future::SelectAll::into_inner</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2363">#2363</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/futures-rs/blob/master/CHANGELOG.md">futures-util's changelog</a>.</em></p>
<blockquote>
<h1>0.3.21 - 2022-02-06</h1>
<ul>
<li>Fix potential data race in <code>FlattenUnordered</code> that introduced in 0.3.20 (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2566">#2566</a>)</li>
</ul>
<h1>0.3.20 - 2022-02-06</h1>
<p>NOTE: This release has been yanked due to a bug fixed in 0.3.21.</p>
<ul>
<li>Fix stacked borrows violations when <code>-Zmiri-tag-raw-pointers</code> is enabled. This raises MSRV of <code>futures-task</code> to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2548">#2548</a>, <a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2550">#2550</a>)</li>
<li>Change <code>FuturesUnordered</code> to respect yielding from future (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2551">#2551</a>)</li>
<li>Add <code>StreamExt::{flatten_unordered, flat_map_unordered}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2083">#2083</a>)</li>
</ul>
<h1>0.3.19 - 2021-12-18</h1>
<ul>
<li>Remove unstable <code>read-initializer</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2534">#2534</a>)</li>
<li>Fix panic in <code>FuturesUnordered</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2535">#2535</a>)</li>
<li>Fix compatibility issue with <code>FuturesUnordered</code> and tokio's cooperative scheduling (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2527">#2527</a>)</li>
<li>Add <code>StreamExt::count</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2495">#2495</a>)</li>
</ul>
<h1>0.3.18 - 2021-11-23</h1>
<p>NOTE: This release has been yanked. See <a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2529">#2529</a> for details.</p>
<ul>
<li>Fix unusable <code>Sink</code> implementation on <code>stream::Scan</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2499">#2499</a>)</li>
<li>Make <code>task::noop_waker_ref</code> available without <code>std</code> feature (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2505">#2505</a>)</li>
<li>Add async <code>LineWriter</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2477">#2477</a>)</li>
<li>Remove dependency on <code>proc-macro-hack</code>. This raises MSRV of utility crates to 1.45. (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2520">#2520</a>)</li>
</ul>
<h1>0.3.17 - 2021-08-30</h1>
<ul>
<li>Use <code>FuturesOrdered</code> in <code>join_all</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2412">#2412</a>)</li>
<li>Add <code>{future, stream}::poll_immediate</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2452">#2452</a>)</li>
<li>Add <code>stream_select!</code> macro (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2262">#2262</a>)</li>
<li>Implement <code>Default</code> for <code>OptionFuture</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2471">#2471</a>)</li>
<li>Add <code>Peekable::{peek_mut, poll_peek_mut}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2488">#2488</a>)</li>
<li>Add <code>BufReader::seek_relative</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2489">#2489</a>)</li>
</ul>
<h1>0.3.16 - 2021-07-23</h1>
<ul>
<li>Add <code>TryStreamExt::try_chunks</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2438">#2438</a>)</li>
<li>Add <code>StreamExt::{all, any}</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2460">#2460</a>)</li>
<li>Add <code>stream::select_with_strategy</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2450">#2450</a>)</li>
<li>Update to new <code>io_slice_advance</code> interface (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2454">#2454</a>)</li>
</ul>
<h1>0.3.15 - 2021-05-11</h1>
<ul>
<li>Use <code>#[proc_macro]</code> at Rust 1.45+ to fix an issue where proc macros don't work with rust-analyzer (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2407">#2407</a>)</li>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2400">#2400</a>)</li>
<li>futures-test: Add async <code>#[test]</code> function attribute (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2409">#2409</a>)</li>
<li>Add <code>stream::abortable</code> (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2410">#2410</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/futures-rs/commit/fc1e3250219170e31cddb8857a276cba7dd08d44"><code>fc1e325</code></a> Release 0.3.21</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/20279ebbfcd326e83161e44a2cf5afe1bfc3b074"><code>20279eb</code></a> <code>FlattenUnordered</code>: improve wakers behavior (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2566">#2566</a>)</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/75dca5ae7fabe6b7073558a8fc6793ee5caa7057"><code>75dca5a</code></a> Fix MSRV in futures-task readme</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/55281c8c8de6308ba97ce8b4ffd754ba204409a0"><code>55281c8</code></a> Release 0.3.20</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/591b982af835fc5e0ffb5104bbb9e942b2ed0631"><code>591b982</code></a> Redefine executor and compat modules in futures crate (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2564">#2564</a>)</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/94b508bfcb1d1f986f34f9b12d799e5a73f65f22"><code>94b508b</code></a> Basic <code>StreamExt::{flatten_unordered, flat_map_unordered}</code> impls (<a href="https://github-redirect.dependabot.com/rust-lang/futures-rs/issues/2083">#2083</a>)</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/dca16fafa597d8e0075a7b693904c6f2ce0322a4"><code>dca16fa</code></a> Do not auto-create PR on fork</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/a9795a9243b0e6b836f71cbe9661bbb35bb17a7f"><code>a9795a9</code></a> Automatically creates PR when no_atomic_cas.rs needs to be updated</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/4841888d68eb8a7796ccd9c9f7a9dc677586e054"><code>4841888</code></a> Update comments in build scripts</li>
<li><a href="https://github.com/rust-lang/futures-rs/commit/85706b6d67aa30e1f8380f8101c14cf43be7500e"><code>85706b6</code></a> Clean up ci/no_atomic_cas.sh</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/futures-rs/compare/0.3.5...0.3.21">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=futures-util&package-manager=cargo&previous-version=0.3.5&new-version=0.3.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:02:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Added Fabric Node SDK Unit Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added Fabric Node SDK unit tests for Interoperable Helper and Relay.
2. Fixed docs links.
3. Fixed bug in house-token exchange corda workflow.
4. Adding clean vendor before building go chaincodes.

Closes #280 #246 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 07:45:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    Bump net2 from 0.2.34 to 0.2.37 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [net2](https://github.com/deprecrated/net2-rs) from 0.2.34 to 0.2.37.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/deprecrated/net2-rs/commit/a18347549413975fbbeb5567165f163e5f60a627"><code>a183475</code></a> Release v0.2.37</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/6081dff94aa3128f0742c24e3925a6f8e7f5de53"><code>6081dff</code></a> haiku: Fix sockaddr_in/sockaddr_in6; Solves <a href="https://github-redirect.dependabot.com/deprecrated/net2-rs/issues/108">#108</a></li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/71708b75d672f5f2430a1edb326d67ed14d87a51"><code>71708b7</code></a> Release v0.2.36</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/49b43f277afb1caf5104fcbe02bef581f7444686"><code>49b43f2</code></a> Do not assume memory layout of std::net::SocketAddr</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/77a6eb4d5eb36adc81ee21ab7ffebc62fdf2ab88"><code>77a6eb4</code></a> Release v0.2.35</li>
<li><a href="https://github.com/deprecrated/net2-rs/commit/eeeab131cb52790df3bedeac46e889feab8f83e3"><code>eeeab13</code></a> Add support for Haiku</li>
<li>See full diff in <a href="https://github.com/deprecrated/net2-rs/compare/0.2.34...0.2.37">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=net2&package-manager=cargo&previous-version=0.2.34&new-version=0.2.37)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 00:54:18 +0000 UTC
    </div>
</div>

