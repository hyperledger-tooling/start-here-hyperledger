---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    chore(deps): update rstest requirement from 0.18 to 0.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [rstest](https://github.com/la10736/rstest) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/la10736/rstest/releases">rstest's releases</a>.</em></p>
<blockquote>
<h2>0.21.0</h2>
<p>Use <code>crate-name</code> feature to enable the crate rename support (enabled by default)</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/la10736/rstest/blob/master/CHANGELOG.md">rstest's changelog</a>.</em></p>
<blockquote>
<h2>[0.21.0] 2024/6/1</h2>
<h3>Changed</h3>
<ul>
<li>Add feature <code>crate-name</code> enabled by default to opt-in crate rename
support. See <a href="https://redirect.github.com/la10736/rstest/issues/258">#258</a></li>
</ul>
<h2>[0.20.0] 2024/5/30</h2>
<h3>Add</h3>
<ul>
<li>Implemented <code>#[by_ref]</code> attribute to take get a local lifetime for test arguments.
See <a href="https://redirect.github.com/la10736/rstest/issues/241">#241</a> for more details. Thanks to
<a href="https://github.com/narpfel"><code>@​narpfel</code></a> for suggesting it and useful discussions.</li>
<li>Support for import <code>rstest</code> with another name. See <a href="https://redirect.github.com/la10736/rstest/issues/221">#221</a></li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Don't remove Lifetimes from test function if any. See <a href="https://redirect.github.com/la10736/rstest/issues/230">#230</a>
<a href="https://redirect.github.com/la10736/rstest/issues/241">#241</a> for more details.</li>
<li><a href="https://doc.rust-lang.org/std/path/struct.PathBuf.html"><code>PathBuf</code></a> does no longer need to be
in scope when using <code>#[files]</code> (see <a href="https://redirect.github.com/la10736/rstest/pull/242">#242</a>)</li>
<li><code>#[from(now::accept::also::path::for::fixture)]</code> See <a href="https://redirect.github.com/la10736/rstest/issues/246">#246</a>
for more details</li>
</ul>
<h2>[0.19.0] 2024/4/9</h2>
<h3>Changed</h3>
<ul>
<li>Defined <code>rust-version</code> for each crate (see <a href="https://redirect.github.com/la10736/rstest/issues/227">#227</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>
<p><code>#[once]</code> fixtures now require the returned type to be
<a href="https://doc.rust-lang.org/std/marker/trait.Sync.html"><code>Sync</code></a> to prevent UB
when tests are executed in parallel. (see <a href="https://redirect.github.com/la10736/rstest/issues/235">#235</a>
for more details)</p>
</li>
<li>
<p><code>#[future(awt)]</code> and <code>#[awt]</code> now properly handle mutable (<code>mut</code>) parameters by treating futures as immutable and
treating the awaited rebinding as mutable.</p>
</li>
</ul>
<h2>[0.18.2] 2023/8/13</h2>
<h3>Changed</h3>
<ul>
<li>Now <code>#[files]</code> accept also parent folders (see <a href="https://redirect.github.com/la10736/rstest/issues/205">#205</a>
for more details).</li>
</ul>
<h2>[0.18.1] 2023/7/5</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/la10736/rstest/commit/38da6bfb9640763727778c07225228ebf405500e"><code>38da6bf</code></a> Prepare 0.21.0 Release</li>
<li><a href="https://github.com/la10736/rstest/commit/ca69788392e8b45f371939525d949b97e5b93673"><code>ca69788</code></a> bump version rstest_test to 0.13.0</li>
<li><a href="https://github.com/la10736/rstest/commit/b6b43c6740381ddbda6bf88276a3946c8e02f049"><code>b6b43c6</code></a> Clean chackoutlist</li>
<li><a href="https://github.com/la10736/rstest/commit/fef4f7b4f4eb1e0eb1c40b8554bdcb32b96e4a1e"><code>fef4f7b</code></a> Implemented Opt-in crate-name support Fix <a href="https://redirect.github.com/la10736/rstest/issues/258">#258</a></li>
<li><a href="https://github.com/la10736/rstest/commit/236be92a8a7b376669c7e5c18e29cc2e4e85f84c"><code>236be92</code></a> Build should use build tests target</li>
<li><a href="https://github.com/la10736/rstest/commit/8fde5be94fb6918492189c3f55528bd1e7962d01"><code>8fde5be</code></a> Prepare next changelog</li>
<li><a href="https://github.com/la10736/rstest/commit/f29e6346fee09a8854e20aa4c13a50da094fde30"><code>f29e634</code></a> Dependency should have a n explicit version to be published</li>
<li><a href="https://github.com/la10736/rstest/commit/e27ad2a4db085c714b9a98012683721f0fd5cb3d"><code>e27ad2a</code></a> Removed empty section</li>
<li><a href="https://github.com/la10736/rstest/commit/386779448365f5bb8620f404ad485b5a82a261be"><code>3867794</code></a> Fixed docs</li>
<li><a href="https://github.com/la10736/rstest/commit/b90fb8e0923b394223b72ab1ef63367959abfcba"><code>b90fb8e</code></a> Fix checkout list</li>
<li>Additional commits viewable in <a href="https://github.com/la10736/rstest/compare/v0.18.0...v0.21.0">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 11:45:24 +0000 UTC
    </div>
</div>

