---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4833" class=".btn">#4833</a>
            </td>
            <td>
                <b>
                    refactor: query filters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                # Description

This PR introduces a lot of changes to the query subsystem. I tried to make the changes gradually in smaller PRs, but it ended up being very intertwined =(

## Summary of changes
- Queries are now split into two categories: iterable queries which return sequences of results and singular queries that return a single value. They are now fully disjoint traits stored in different Box enums, as they require very different handling.
- Query filters (aka predicates) are now typed depending on the type of the iterable query they are applied to (#4569). Instead of a single `PredicateBox` there is a predicate type for each queryable type (like `AccountPredicateBox`), with `CompountPredicate<T>` providing the logical operations on top.
- A new rust DSL to construct the predicates is introduced. It is designed to look very close to how one would write an `Iterator::filter` closure (`|obj| obj.field.inner_field.starts_with("hello")`) and is inspired by diesel's DSL.
- HTTP clients and wasm code (smart contracts, triggers and executor) are now using a common query builder struct, generic over a new `QueryExecutor` trait
- The HTTP API is majorly revamped to pass all of the params as scale-encoded values. This simplifies the torii handler, makes it more type-safe (can't add pagination to singular query) and allows sharing more code with wasm
- All of the queries that can be implemented as filtered versions of other queries are now removed. Here's a rough google table I made to keep track of all of them: https://docs.google.com/spreadsheets/d/1Cx9cU4wLk1ZyIa3Igx0NN9azl9dfqcXXMJMLKTMxes4/edit?usp=sharing

### The primary key question

Currently we have a bunch of queries that give you an object using its Primary Key (like `FindAccountById`). They can be implemented by filtering a basis query that returns all objects of such type (like `FindAllAccounts`). However, with naïve implementation (which this PR currently does) this would result in `O(n)` complexity instead of `O(log n)` that we currently have.

There is a way to do these lookups fast: just pattern-match the filter on the shape `|obj| obj.id.eq(expected_id)` and use the primary key index instead of linear scan. We can even use a similar approach to speed up other types of queries, if deemed necessary.

However, merging it as-is would mean that the primary queries would be slow. I can probably add the PK queries back for now, if that's unacceptable.

## Future work

These are improvements I see that can be made to this PR, but I would prefer them to be implemented in separate PRs. I'll convent them to issues when this PR gets closer to getting merged.

Perf:
- the Primary Key optimization (see above)
- make queries truly lazy (put them into the query store without collecting them all in a vec); Needs investigation whether that'll actually be beneficial and some clever implementation (need to store an iterator with lifetime tied to iroha state snapshot).

Ergonomics:
- `client::account::all()` is unfortunate, seeing as how most of the queries would be "all" with filters now
- provide helpers like `client::domain::by_id`, with them still relying on filtered queries
- `impl Into<String>` for ids (#4832)

Misc:
- `Display` representations for queries & filters (right now printing them with `Debug`)
- check that the iterable query continuation is executed by the same authority as the one that started it

## Linked issue

Closes #4569, #4720, #3720, #3671.

## Checklist

I still have a lot of doc strings, an overview of the predicate DSL implementation and some tests to write, hence marking this PR as a draft.

- [ ] add more docs and remove all the `#[warn(missing_docs)]`
- [ ] add more tests of the DSL
- [ ] add a test checking the validation performed on `SignedQueryCandidate`
- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-10 17:29:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4831" class=".btn">#4831</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tomlkit from 0.12.5 to 0.13.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [tomlkit](https://github.com/sdispater/tomlkit) from 0.12.5 to 0.13.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-poetry/tomlkit/blob/master/CHANGELOG.md">tomlkit's changelog</a>.</em></p>
<blockquote>
<h2>[0.13.0] - 2024-07-10</h2>
<h3>Changed</h3>
<ul>
<li>Expect a tomlkit-specific error instead of <code>TypeError</code> from a custom encoder. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/355">#355</a>)</li>
<li>Drop support for Python older than 3.8. Remove 3.7 from the CI matrix.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix the incompatiblity with 3.13 because of the <code>datetime.replace()</code> change. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/333">#333</a>)</li>
<li>Revert the change of parsing out-of-order tables. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/347">#347</a>)</li>
<li>Keep the nested out-of-order table. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/361">#361</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-poetry/tomlkit/commit/4d06dff4bc4a1cc16e0f600f71df8f41724efcec"><code>4d06dff</code></a> chore: bump version to 0.13.0</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/85aaf7a9231030fc3455048d78bfdabfe0a0a937"><code>85aaf7a</code></a> fix: keep the nested out of order table (<a href="https://redirect.github.com/sdispater/tomlkit/issues/366">#366</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/f12ece324fc376d0f863717005ba6acc5f9d8933"><code>f12ece3</code></a> chore(deps-dev): bump zipp from 3.15.0 to 3.19.1 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/365">#365</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/f4b2f74d2a4e19ee8bebd94b874c8c47699a169f"><code>f4b2f74</code></a> chore(deps-dev): bump requests from 2.31.0 to 2.32.2 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/364">#364</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/0747884431425b45071b696fd6ffe806d59304bb"><code>0747884</code></a> chore(deps-dev): bump urllib3 from 2.0.7 to 2.2.2 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/363">#363</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/d55d837d0b139bd48567ac90204baccb8ce0cbd9"><code>d55d837</code></a> fix: Remove 3.7 from the CI matrix</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/49daa69df84db37ab3e9ec365c3a9590d5455646"><code>49daa69</code></a> chore(deps-dev): bump certifi from 2024.2.2 to 2024.7.4 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/362">#362</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/cce567ca4c1455d948d68c0fa32f7eb9196b9be3"><code>cce567c</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/sdispater/tomlkit/issues/359">#359</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/400057ba17dbf562fa4fe01fc26b40d7112690e4"><code>400057b</code></a> fix: <code>tomlkit</code> 0.12.5 : Encoder contract interferes with external <code>TypeError</code>...</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/22676f9a79228df216d79ba98209b98c2313c31c"><code>22676f9</code></a> Update tests action (<a href="https://redirect.github.com/sdispater/tomlkit/issues/357">#357</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/sdispater/tomlkit/compare/0.12.5...0.13.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tomlkit&package-manager=pip&previous-version=0.12.5&new-version=0.13.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-10 16:39:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4828" class=".btn">#4828</a>
            </td>
            <td>
                <b>
                    fix: Keep voting block if possible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Implements idea from https://github.com/hyperledger/iroha/pull/4518#discussion_r1612185825:

> Maybe we can be smarter about when to reject incoming block? Like checking signatures, height, hashes this checks doesn’t need ability to modify state.

This is relatively small change which I think will keep voting block in most cases (however not in all).

---

Alternative approach might be to change our state block to accumulate changes localy and take write lock just before applying changes. However it will require large refactoring and might affect performance.

### Linked issue

Closes #4643

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 17:53:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4826" class=".btn">#4826</a>
            </td>
            <td>
                <b>
                    chore(deps): bump clap from 4.5.8 to 4.5.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [clap](https://github.com/clap-rs/clap) from 4.5.8 to 4.5.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/releases">clap's releases</a>.</em></p>
<blockquote>
<h2>v4.5.9</h2>
<h2>[4.5.9] - 2024-07-09</h2>
<h3>Fixes</h3>
<ul>
<li><em>(error)</em> When defining a custom help flag, be sure to suggest it like we do the built-in one</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/blob/master/CHANGELOG.md">clap's changelog</a>.</em></p>
<blockquote>
<h2>[4.5.9] - 2024-07-09</h2>
<h3>Fixes</h3>
<ul>
<li><em>(error)</em> When defining a custom help flag, be sure to suggest it like we do the built-in one</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/clap-rs/clap/commit/43e73682835653ac48f32cc786514553d697c693"><code>43e7368</code></a> chore: Release</li>
<li><a href="https://github.com/clap-rs/clap/commit/f00dafa690479e562ef22c3ed82f17726213ee32"><code>f00dafa</code></a> docs: Update changelog</li>
<li><a href="https://github.com/clap-rs/clap/commit/da1093a4f4cd1abba7de0b86f39319ab86913420"><code>da1093a</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/5574">#5574</a> from zanieb/zb/try-help-custom</li>
<li><a href="https://github.com/clap-rs/clap/commit/2eb842cc3bc1fb5f04156efa816003ef803d5254"><code>2eb842c</code></a> feat: Show user defined help flags in hints</li>
<li><a href="https://github.com/clap-rs/clap/commit/b24deb101f7e12660b8b19d6b3979df87ffe065d"><code>b24deb1</code></a> test: Add coverage for help flag hints</li>
<li><a href="https://github.com/clap-rs/clap/commit/866d7d14d33a3ef1f010222f004815b5cd8c15ef"><code>866d7d1</code></a> chore(deps): Update compatible (dev) (<a href="https://redirect.github.com/clap-rs/clap/issues/5560">#5560</a>)</li>
<li><a href="https://github.com/clap-rs/clap/commit/d14bbc95317eb87a115f56c455bdab6ba19342ff"><code>d14bbc9</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/5567">#5567</a> from epage/c</li>
<li><a href="https://github.com/clap-rs/clap/commit/5448020b188899601d641a2684833073aba0a669"><code>5448020</code></a> fix: Install shells for CI</li>
<li><a href="https://github.com/clap-rs/clap/commit/1c5a625ad0303e2407c8ab83ea7d37795e69a3a5"><code>1c5a625</code></a> fix: Fix wrong <code>cfg(linux)</code></li>
<li><a href="https://github.com/clap-rs/clap/commit/2d2d1f498731d2ab70e8f15fed3765a856d52732"><code>2d2d1f4</code></a> chore: Bump completest</li>
<li>Additional commits viewable in <a href="https://github.com/clap-rs/clap/compare/v4.5.8...v4.5.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clap&package-manager=cargo&previous-version=4.5.8&new-version=4.5.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 16:58:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4825" class=".btn">#4825</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.69 to 2.0.70
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.69 to 2.0.70.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.70</h2>
<ul>
<li>Improve parenthesization of closures, jumps, ranges, chained comparisons, and let (<a href="https://redirect.github.com/dtolnay/syn/issues/1694">#1694</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1695">#1695</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1698">#1698</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1699">#1699</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1700">#1700</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/5c67e2689791db44258d99402ae6d05b1898d9a3"><code>5c67e26</code></a> Release 2.0.70</li>
<li><a href="https://github.com/dtolnay/syn/commit/935c1e1817d411a02d09d2315ed533df12f70ace"><code>935c1e1</code></a> Configure out more full-only expression kinds in print_expr</li>
<li><a href="https://github.com/dtolnay/syn/commit/e664375b4981637a490f1f30dd252536371ef2cc"><code>e664375</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1704">#1704</a> from dtolnay/fixup</li>
<li><a href="https://github.com/dtolnay/syn/commit/f1daf234e942ffda27ed45ec67aa6cd984081c2a"><code>f1daf23</code></a> Enable expression fixups in 'derive' mode</li>
<li><a href="https://github.com/dtolnay/syn/commit/678dbc2e50904de7b80f10f4d355be5536a8bceb"><code>678dbc2</code></a> Update test suite to nightly-2024-07-08</li>
<li><a href="https://github.com/dtolnay/syn/commit/628e2f7003d17ae0c02d0da076577001e62015a3"><code>628e2f7</code></a> Ignore needless_update clippy lint</li>
<li><a href="https://github.com/dtolnay/syn/commit/c3e378cdda142d83f14055661001d39533199f3f"><code>c3e378c</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1703">#1703</a> from dtolnay/cast</li>
<li><a href="https://github.com/dtolnay/syn/commit/d47e532913bb9138cc47a6a3756aeead9ad2d08a"><code>d47e532</code></a> Rearrange logic of FixupContext precedence methods</li>
<li><a href="https://github.com/dtolnay/syn/commit/9809f716e3aa0b3223489860f29385afcd04b5f8"><code>9809f71</code></a> Incorporate parenthesization of casts into FixupContext</li>
<li><a href="https://github.com/dtolnay/syn/commit/ff022f529241e536c75ecd79ee155518723c1460"><code>ff022f5</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1702">#1702</a> from dtolnay/preclet</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.69...2.0.70">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.69&new-version=2.0.70)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 16:57:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4824" class=".btn">#4824</a>
            </td>
            <td>
                <b>
                    chore(deps): bump uuid from 1.9.1 to 1.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [uuid](https://github.com/uuid-rs/uuid) from 1.9.1 to 1.10.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/uuid-rs/uuid/releases">uuid's releases</a>.</em></p>
<blockquote>
<h2>1.10.0</h2>
<h2>Deprecations</h2>
<p>This release deprecates and renames the following functions:</p>
<ul>
<li><code>Builder::from_rfc4122_timestamp</code> -&gt; <code>Builder::from_gregorian_timestamp</code></li>
<li><code>Builder::from_sorted_rfc4122_timestamp</code> -&gt; <code>Builder::from_sorted_gregorian_timestamp</code></li>
<li><code>Timestamp::from_rfc4122</code> -&gt; <code>Timestamp::from_gregorian</code></li>
<li><code>Timestamp::to_rfc4122</code> -&gt; <code>Timestamp::to_gregorian</code></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Use const identifier in uuid macro by <a href="https://github.com/Vrajs16"><code>@​Vrajs16</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/764">uuid-rs/uuid#764</a></li>
<li>Rename most methods referring to RFC4122 by <a href="https://github.com/Mikopet"><code>@​Mikopet</code></a> / <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/765">uuid-rs/uuid#765</a></li>
<li>prepare for 1.10.0 release by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/766">uuid-rs/uuid#766</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Vrajs16"><code>@​Vrajs16</code></a> made their first contribution in <a href="https://redirect.github.com/uuid-rs/uuid/pull/764">uuid-rs/uuid#764</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/uuid-rs/uuid/compare/1.9.1...1.10.0">https://github.com/uuid-rs/uuid/compare/1.9.1...1.10.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/uuid-rs/uuid/commit/4b4c590ae323b683a7ba80f05c83d3002ddc2fc5"><code>4b4c590</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/766">#766</a> from uuid-rs/cargo/1.10.0</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/68eff326408ea269253aa0ba8f6cb3ac4099f894"><code>68eff32</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/765">#765</a> from uuid-rs/chore/time-fn-deprecations</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/3d5384da4bfb2f35ad4426440d285e4a13c8c011"><code>3d5384d</code></a> update docs and deprecation messages for timestamp fns</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/de50f2091f05a973b4e8ca2f7eddd03459b1b680"><code>de50f20</code></a> renaming rfc4122 functions</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/4a8841792a8bb7007d23a54fa866adc5cec79425"><code>4a88417</code></a> prepare for 1.10.0 release</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/66b4fcef14862bc5d8d45acb9f6683a37fa5ecb4"><code>66b4fce</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/764">#764</a> from Vrajs16/main</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/8896e26c421a8b9a7a935acf83d291df40256de9"><code>8896e26</code></a> Use expr instead of ident</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/09973d6aff62b61ec35f577a757148007deb5f05"><code>09973d6</code></a> Added changes</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/6edf3e8cd59351589622daf1f2634870d90896e3"><code>6edf3e8</code></a> Use const identifer in uuid macro</li>
<li>See full diff in <a href="https://github.com/uuid-rs/uuid/compare/1.9.1...1.10.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uuid&package-manager=cargo&previous-version=1.9.1&new-version=1.10.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 16:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4823" class=".btn">#4823</a>
            </td>
            <td>
                <b>
                    chore(deps): bump darling from 0.20.9 to 0.20.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [darling](https://github.com/TedDriggs/darling) from 0.20.9 to 0.20.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/TedDriggs/darling/releases">darling's releases</a>.</em></p>
<blockquote>
<h2>v0.20.10</h2>
<ul>
<li>Add <code>#[allow(clippy::manual_unwrap_or_default)]</code> to all generated impls to avoid causing clippy fails in crates using <code>darling</code> <a href="https://redirect.github.com/TedDriggs/darling/pull/296">#296</a></li>
<li>Properly initialize <code>attrs</code> magic field in derived <code>FromAttributes</code> impls <a href="https://redirect.github.com/TedDriggs/darling/pull/297">#297</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/TedDriggs/darling/blob/master/CHANGELOG.md">darling's changelog</a>.</em></p>
<blockquote>
<h2>v0.20.10 (July 9, 2024)</h2>
<ul>
<li>Add <code>#[allow(clippy::manual_unwrap_or_default)]</code> to all generated impls to avoid causing clippy fails in crates using <code>darling</code> <a href="https://redirect.github.com/TedDriggs/darling/pull/296">#296</a></li>
<li>Properly initialize <code>attrs</code> magic field in derived <code>FromAttributes</code> impls <a href="https://redirect.github.com/TedDriggs/darling/pull/297">#297</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/TedDriggs/darling/commits/v0.20.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=darling&package-manager=cargo&previous-version=0.20.9&new-version=0.20.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 16:54:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4822" class=".btn">#4822</a>
            </td>
            <td>
                <b>
                    fix(docker): propagate SIGTERM to irohad
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4783 

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 15:18:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4819" class=".btn">#4819</a>
            </td>
            <td>
                <b>
                    chore(deps): bump trybuild from 1.0.96 to 1.0.97
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [trybuild](https://github.com/dtolnay/trybuild) from 1.0.96 to 1.0.97.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/trybuild/releases">trybuild's releases</a>.</em></p>
<blockquote>
<h2>1.0.97</h2>
<ul>
<li>Normalize number of types listed in <em>&quot;the following other types implement trait&quot;</em> diagnostics (<a href="https://redirect.github.com/dtolnay/trybuild/issues/277">#277</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/trybuild/commit/daeef9c9b0b0da1c63eb9e2ce2b2cc816e0ddc8c"><code>daeef9c</code></a> Release 1.0.97</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/207b0a51a72de39d66aa09d4884ac8fbe2e529b7"><code>207b0a5</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/278">#278</a> from dtolnay/rustflags</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/1b8d4bdf0718bfe4719039ad2d3d53c9f5ccdab5"><code>1b8d4bd</code></a> Combine all rustflags into cargo --config arg</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/ef6893bf616cc6fd97264118473e45fbfeb27217"><code>ef6893b</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/277">#277</a> from dtolnay/nothers</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/883a38daa03e97053180f70e0b7b6446f1b7724a"><code>883a38d</code></a> Ignore comparison_chain clippy lint</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/f3b1dab3275e628d4e0b486d494fd820eb7bb559"><code>f3b1dab</code></a> Normalize the effect of --verbose on '$N others' diagnostic</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/6184f60b31cf9547f2a2697c57a5852fc186d996"><code>6184f60</code></a> Add test of 'following other types' diagnostic</li>
<li>See full diff in <a href="https://github.com/dtolnay/trybuild/compare/1.0.96...1.0.97">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=trybuild&package-manager=cargo&previous-version=1.0.96&new-version=1.0.97)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:04:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4818" class=".btn">#4818</a>
            </td>
            <td>
                <b>
                    chore(deps): bump async-trait from 0.1.80 to 0.1.81
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [async-trait](https://github.com/dtolnay/async-trait) from 0.1.80 to 0.1.81.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/async-trait/releases">async-trait's releases</a>.</em></p>
<blockquote>
<h2>0.1.81</h2>
<ul>
<li>Turn off unneeded features of <code>syn</code> dependency (<a href="https://redirect.github.com/dtolnay/async-trait/issues/272">#272</a>, thanks <a href="https://github.com/klensy"><code>@​klensy</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/async-trait/commit/383f65f138963391a41d25ed7e2857fa002c5742"><code>383f65f</code></a> Release 0.1.81</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/4ec740e1dddab158a46f59271245984d1b92794d"><code>4ec740e</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/273">#273</a> from dtolnay/cloneimpls</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/b6c606384471c26a06852c0586304965237c0b95"><code>b6c6063</code></a> Ignore trivially_copy_pass_by_ref pedantic clippy lint</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/315fd9005c8294ecf2d9cce84d1d5a53da656b19"><code>315fd90</code></a> Turn off syn/clone-impls feature</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/94a3165a30a225c2d78425e4c68fc5ec67929a98"><code>94a3165</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/272">#272</a> from klensy/syn-f</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/2fac9405c8d3ecf8c08b0085ec338b72a643e43c"><code>2fac940</code></a> syn: remove derive feature</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/4a00d732460d37e219755bfc6db132b42b8c4af1"><code>4a00d73</code></a> Work around dead code warning in test</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/dba15b5a73f34a2fd96361a2fa8993ba412a43e1"><code>dba15b5</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/270">#270</a> from dtolnay/objsafety</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/d28c95b2037901ff4c36b631054d463f675f991c"><code>d28c95b</code></a> Former where_clauses_object_safety lint is now hard error</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/78a5922b4a9e81c72676dbeb9ea3bac50535864b"><code>78a5922</code></a> Fill in ignore reasons in all #[ignore] attributes</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/async-trait/compare/0.1.80...0.1.81">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async-trait&package-manager=cargo&previous-version=0.1.80&new-version=0.1.81)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:03:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4817" class=".btn">#4817</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.68 to 2.0.69
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.68 to 2.0.69.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.69</h2>
<ul>
<li>Correctly parenthesize labeled loops inside a break value (<a href="https://redirect.github.com/dtolnay/syn/issues/1692">#1692</a>)</li>
<li>Add <code>Punctuated::get</code> and <code>get_mut</code> (<a href="https://redirect.github.com/dtolnay/syn/issues/1693">#1693</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/d4a0ff556fe1bbcaa77ebc37d24cc1bdaf5eac3a"><code>d4a0ff5</code></a> Release 2.0.69</li>
<li><a href="https://github.com/dtolnay/syn/commit/0f7213407fb59cca90a1097747868b68b32ff020"><code>0f72134</code></a> Improve precedence variant name of sum and product operators</li>
<li><a href="https://github.com/dtolnay/syn/commit/06f34fce1a62e75fbd0400b93181ff989e16505b"><code>06f34fc</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1693">#1693</a> from dtolnay/get</li>
<li><a href="https://github.com/dtolnay/syn/commit/a4438571c902aae659ff568419fa4af029b5c0b0"><code>a443857</code></a> Add Punctuated::get and get_mut</li>
<li><a href="https://github.com/dtolnay/syn/commit/f0dfdbd9af41fe75ee6054daca545d80a4374a32"><code>f0dfdbd</code></a> Update test suite to nightly-2024-07-05</li>
<li><a href="https://github.com/dtolnay/syn/commit/1560f9a2ac7937fee688eaa98ad009caaeef323c"><code>1560f9a</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1692">#1692</a> from dtolnay/break</li>
<li><a href="https://github.com/dtolnay/syn/commit/4e71c1caa413122a644f9e3fcb8222dfc20d9f8d"><code>4e71c1c</code></a> Parenthesize labeled loops inside break value</li>
<li><a href="https://github.com/dtolnay/syn/commit/93931a4f243665a1e50748072b9fac1adbcebb7c"><code>93931a4</code></a> Add fixup test for break with leading label</li>
<li><a href="https://github.com/dtolnay/syn/commit/cc5e64e4143099699c5c7f20791c563e71395455"><code>cc5e64e</code></a> Update test suite to nightly-2024-06-29</li>
<li><a href="https://github.com/dtolnay/syn/commit/2bbf612a945f94860be6197c1efc76f8e3ae9e6c"><code>2bbf612</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1691">#1691</a> from dtolnay/postfix</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.68...2.0.69">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.68&new-version=2.0.69)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4816" class=".btn">#4816</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.203 to 1.0.204
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.203 to 1.0.204.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.204</h2>
<ul>
<li>Apply #[diagnostic::on_unimplemented] attribute on Rust 1.78+ to suggest adding serde derive or enabling a &quot;serde&quot; feature flag in dependencies (<a href="https://redirect.github.com/serde-rs/serde/issues/2767">#2767</a>, thanks <a href="https://github.com/weiznich"><code>@​weiznich</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/18dcae0a77632fb4767a420c550cb41991f750b8"><code>18dcae0</code></a> Release 1.0.204</li>
<li><a href="https://github.com/serde-rs/serde/commit/58c307f9cc28a19d73a0e2869f6addf9a8a329f9"><code>58c307f</code></a> Alphabetize list of rustc-check-cfg</li>
<li><a href="https://github.com/serde-rs/serde/commit/8cc4809414a83de0d41eac38ecfa1040e088b61e"><code>8cc4809</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2769">#2769</a> from dtolnay/onunimpl</li>
<li><a href="https://github.com/serde-rs/serde/commit/1179158defc5351467cbd2c340b7e1498391bce4"><code>1179158</code></a> Update ui test with diagnostic::on_unimplemented from PR 2767</li>
<li><a href="https://github.com/serde-rs/serde/commit/91aa40e749620f31bf7db01c772e672f023136b5"><code>91aa40e</code></a> Add ui test of unsatisfied serde trait bound</li>
<li><a href="https://github.com/serde-rs/serde/commit/595019e979ebed5452b550bf901abcab2cf4e945"><code>595019e</code></a> Cut test_suite from workspace members in old toolchain CI jobs</li>
<li><a href="https://github.com/serde-rs/serde/commit/b0d7917f88978eda264f8fbac13b46ece35f5348"><code>b0d7917</code></a> Pull in trybuild 'following types implement trait' fix</li>
<li><a href="https://github.com/serde-rs/serde/commit/8e6637a1e44c30dffd37322a7107d434cd751722"><code>8e6637a</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2767">#2767</a> from weiznich/feature/diagnostic_on_unimplemented</li>
<li><a href="https://github.com/serde-rs/serde/commit/694fe0595358aa0857120a99041d99975b1a8a70"><code>694fe05</code></a> Use the <code>#[diagnostic::on_unimplemented]</code> attribute when possible</li>
<li><a href="https://github.com/serde-rs/serde/commit/f3dfd2a2375d9caf15a18ec657dde51a32caf6ed"><code>f3dfd2a</code></a> Suppress dead code warning in test of unit struct remote derive</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/serde/compare/v1.0.203...v1.0.204">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.203&new-version=1.0.204)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:02:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4812" class=".btn">#4812</a>
            </td>
            <td>
                <b>
                    feat!: speicfy on-chain parameters explicitly in genesis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Currently it's not possible to submit genesis which doesn't pass under default parameter values (i.e. large genesis). 
This PR fixes that allowing to specify parameters inside genesis.json so that they are applied before processing rest of instructions.

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4810" class=".btn">#4810</a>
            </td>
            <td>
                <b>
                    refactor!: rename wasm to smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

The fact that we work with wasm smart contracts is a sort of implementation detail.
Let's not specify implementation details in the API.


### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

If we change from wasm to some other VM, we will have a reduced effect on the API.
If we don't it is implied that we use wasm, so no harm done there

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 08:50:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4808" class=".btn">#4808</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_with from 3.8.2 to 3.8.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_with](https://github.com/jonasbb/serde_with) from 3.8.2 to 3.8.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonasbb/serde_with/releases">serde_with's releases</a>.</em></p>
<blockquote>
<h2>serde_with v3.8.3</h2>
<h3>Fixed</h3>
<ul>
<li>Fix compile issues when dependency <code>schemars_0_8</code> is used with the <code>preserve_order</code> features (<a href="https://redirect.github.com/jonasbb/serde_with/issues/762">#762</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonasbb/serde_with/commit/1c4b022e6018fbf1f9cb2e897bae519f91ed6908"><code>1c4b022</code></a> Bump version to v3.8.3 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/765">#765</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/7de983895c0dcbf8598676f52b987a0026f7d816"><code>7de9838</code></a> Bump version to v3.8.3</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/19bfe182439616416f0fc17b1fac134e1b29e537"><code>19bfe18</code></a> Make code compile with <code>schemars_0_8/preserve_order</code> enabled (<a href="https://redirect.github.com/jonasbb/serde_with/issues/764">#764</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/4c8c2db1105da0408c89330e0bcfc7ac4818975c"><code>4c8c2db</code></a> Make code compile with <code>schemars_0_8/preserve_order</code> enabled</li>
<li>See full diff in <a href="https://github.com/jonasbb/serde_with/compare/v3.8.2...v3.8.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_with&package-manager=cargo&previous-version=3.8.2&new-version=3.8.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-05 16:29:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4807" class=".btn">#4807</a>
            </td>
            <td>
                <b>
                    fix: Check that authority owns domain to transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

When transfer `domain` from `source` account:
* Fixed check in executor that `authority` owns `domain` (previously it checked that `source` owns `domain`, but it is not needed since it is checked in iroha_core)
* Improved error message for check that `source` owns `domain` in iroha_core

### Linked issue

Closes #4751

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-05 14:53:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4806" class=".btn">#4806</a>
            </td>
            <td>
                <b>
                    feat: include parameters into generated genesis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Include parameters into default genesis.json.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

While parameters may have default values i still think it's useful to include them into default genesis as an example.
I've got contacted by our QA and they didn't have a way to know how new parameters are expressed in the genesis.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->
<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-05 09:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4805" class=".btn">#4805</a>
            </td>
            <td>
                <b>
                    refactor(client): allow turbofish with multiple `Instruction`s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Converts `impl Instruction` to an explicit type parameter in functions accepting multiple instructions.

### Benefits

Lets users avoid converting heterogeneous instructions to `InstructionBox`es in a separate variable before submitting to a client, which is more ergonomic.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-05 09:13:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4804" class=".btn">#4804</a>
            </td>
            <td>
                <b>
                    fix: Fix failing tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Fix those tests:
* `iroha::mod integration::upgrade::migration_should_cause_upgrade_event`
* `iroha_core queue::tests::queue_throttling`
* `iroha_core smartcontracts::isi::query::tests::asset_store`
* `parity_scale_cli::bin/parity_scale_cli tests::decode_account_sample`
* `parity_scale_cli::bin/parity_scale_cli tests::decode_domain_sample`

### Linked issue

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 12:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4802" class=".btn">#4802</a>
            </td>
            <td>
                <b>
                    fix: Smarter transaction expire logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 07:05:24 +0000 UTC
    </div>
</div>

