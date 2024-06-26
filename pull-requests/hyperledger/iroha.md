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
                PR <a href="https://github.com/hyperledger/iroha/pull/4772" class=".btn">#4772</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump mypy from 1.10.0 to 1.10.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mypy](https://github.com/python/mypy) from 1.10.0 to 1.10.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python/mypy/blob/master/CHANGELOG.md">mypy's changelog</a>.</em></p>
<blockquote>
<h4>Mypy 1.10.1</h4>
<ul>
<li>Fix error reporting on cached run after uninstallation of third party library (Shantanu, PR <a href="https://redirect.github.com/python/mypy/pull/17420">17420</a>)</li>
</ul>
<h4>Acknowledgements</h4>
<p>Thanks to all mypy contributors who contributed to this release:</p>
<ul>
<li>Alex Waygood</li>
<li>Ali Hamdan</li>
<li>Edward Paget</li>
<li>Evgeniy Slobodkin</li>
<li>Hashem</li>
<li>hesam</li>
<li>Hugo van Kemenade</li>
<li>Ihor</li>
<li>James Braza</li>
<li>Jelle Zijlstra</li>
<li>jhance</li>
<li>Jukka Lehtosalo</li>
<li>Loïc Simon</li>
<li>Marc Mueller</li>
<li>Matthieu Devlin</li>
<li>Michael R. Crusoe</li>
<li>Nikita Sobolev</li>
<li>Oskari Lehto</li>
<li>Riccardo Di Maio</li>
<li>Richard Si</li>
<li>roberfi</li>
<li>Roman Solomatin</li>
<li>Sam Xifaras</li>
<li>Shantanu</li>
<li>Spencer Brown</li>
<li>Srinivas Lade</li>
<li>Tamir Duberstein</li>
<li>youkaichao</li>
</ul>
<p>I’d also like to thank my employer, Dropbox, for supporting mypy development.</p>
<h2>Mypy 1.9</h2>
<p>We’ve just uploaded mypy 1.9 to the Python Package Index (<a href="https://pypi.org/project/mypy/">PyPI</a>). Mypy is a static type checker for Python. This release includes new features, performance improvements and bug fixes. You can install it as follows:</p>
<pre><code>python3 -m pip install -U mypy
</code></pre>
<p>You can read the full documentation for this release on <a href="http://mypy.readthedocs.io">Read the Docs</a>.</p>
<h4>Breaking Changes</h4>
<p>Because the version of typeshed we use in mypy 1.9 doesn't support 3.7, neither does mypy 1.9. (Jared Hance, PR <a href="https://redirect.github.com/python/mypy/pull/16883">16883</a>)</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python/mypy/commit/c28b5257b528f65a028e7d0dbecbcd81c7997356"><code>c28b525</code></a> [1.10 backport] Fix error reporting on cached run after uninstallation of thi...</li>
<li>See full diff in <a href="https://github.com/python/mypy/compare/v1.10.0...v1.10.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mypy&package-manager=pip&previous-version=1.10.0&new-version=1.10.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-25 16:55:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4771" class=".btn">#4771</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_json from 1.0.117 to 1.0.118
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.117 to 1.0.118.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.118</h2>
<ul>
<li>Implement Hash for serde_json::Value (<a href="https://redirect.github.com/serde-rs/json/issues/1127">#1127</a>, thanks <a href="https://github.com/edwardycl"><code>@​edwardycl</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/c4f24f3be29a3d096d3ac7b1d5594777a613ec0d"><code>c4f24f3</code></a> Release 1.0.118</li>
<li><a href="https://github.com/serde-rs/json/commit/51d94ebdc07127de22fb655bdcf6a01d119492d5"><code>51d94eb</code></a> Combine Map's Hash into one impl</li>
<li><a href="https://github.com/serde-rs/json/commit/5e7bedc0a0e19ecda1c15a412ab7c69569f4aa84"><code>5e7bedc</code></a> Touch up PR 1127</li>
<li><a href="https://github.com/serde-rs/json/commit/0af2bdae9483a9c54f8e032fcbf357dbe7803c49"><code>0af2bda</code></a> Resolve semicolon_if_nothing_returned pedantic clippy lint from PR 1127</li>
<li><a href="https://github.com/serde-rs/json/commit/eb0330a178e0c179321101fbcbb5cb7530a2a3e5"><code>eb0330a</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1127">#1127</a> from edwardycl/hash</li>
<li><a href="https://github.com/serde-rs/json/commit/24d868f4e9be428afa1c744f8218a32660a1e0bf"><code>24d868f</code></a> Another lexical const that is unused, though not in test</li>
<li><a href="https://github.com/serde-rs/json/commit/4c894eaa18181860f3f5cf3fb11e18d4ee454120"><code>4c894ea</code></a> Delete unused associated constant from lexical</li>
<li><a href="https://github.com/serde-rs/json/commit/fa8aa223c66018cae73efa57fd276af329a343f4"><code>fa8aa22</code></a> Fill in ignore reasons in all #[ignore] attributes</li>
<li><a href="https://github.com/serde-rs/json/commit/c9b9f88c1add99e20fefcd377a29b00715b4e8c3"><code>c9b9f88</code></a> Run more of test suite in preserve_order mode</li>
<li><a href="https://github.com/serde-rs/json/commit/b83d243e711b65e32925510343df566080776dd5"><code>b83d243</code></a> Ignore large_digit_groups pedantic clippy lint in test</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/json/compare/v1.0.117...v1.0.118">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.117&new-version=1.0.118)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-25 16:32:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4768" class=".btn">#4768</a>
            </td>
            <td>
                <b>
                    docs(md): fix typos in CONTRIBUTING, iroha_2_whitepaper, hot-reload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs(md): fix typos in CONTRIBUTING, iroha_2_whitepaper, hot-reload
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-25 09:47:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4766" class=".btn">#4766</a>
            </td>
            <td>
                <b>
                    chore(deps): bump uuid from 1.8.0 to 1.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [uuid](https://github.com/uuid-rs/uuid) from 1.8.0 to 1.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/uuid-rs/uuid/releases">uuid's releases</a>.</em></p>
<blockquote>
<h2>1.9.0</h2>
<h2><code>Uuid::now_v7()</code> is guaranteed to be monotonic</h2>
<p>Before this release, <code>Uuid::now_v7()</code> would only use the millisecond-precision timestamp for ordering. It now also uses a global 42-bit counter that's re-initialized each millisecond so that the following will always pass:</p>
<pre lang="rust"><code>let a = Uuid::now_v7();
let b = Uuid::now_v7();
<p>assert!(a &lt; b);
</code></pre></p>
<h2>What's Changed</h2>
<ul>
<li>Add a get_node_id method for v1 and v6 UUIDs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/748">uuid-rs/uuid#748</a></li>
<li>Update atomic and zerocopy to latest by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/750">uuid-rs/uuid#750</a></li>
<li>Add repository field to uuid-macro-internal crate by <a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/752">uuid-rs/uuid#752</a></li>
<li>update docs to updated RFC (from 4122 to 9562) by <a href="https://github.com/Mikopet"><code>@​Mikopet</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/753">uuid-rs/uuid#753</a></li>
<li>Support counters in v7 UUIDs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/755">uuid-rs/uuid#755</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a> made their first contribution in <a href="https://redirect.github.com/uuid-rs/uuid/pull/752">uuid-rs/uuid#752</a></li>
<li><a href="https://github.com/Mikopet"><code>@​Mikopet</code></a> made their first contribution in <a href="https://redirect.github.com/uuid-rs/uuid/pull/753">uuid-rs/uuid#753</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/uuid-rs/uuid/compare/1.8.0...1.9.0">https://github.com/uuid-rs/uuid/compare/1.8.0...1.9.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/uuid-rs/uuid/commit/4a129e728174a340ac2772f3cc6310ba77d1969f"><code>4a129e7</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/760">#760</a> from uuid-rs/cargo/1.9.0</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/6bfee6ba82ad8e7a0155f3161157dc3ea3a5d552"><code>6bfee6b</code></a> prepare for 1.9.0 release</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/62b7145d95913642298d5a954314ea28a199fa78"><code>62b7145</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/759">#759</a> from uuid-rs/chore/v7-counter-cleanup</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/62e968c92b464c81a73b6002ab66a32c4bdad9ad"><code>62e968c</code></a> clean up new Timestamp APIs</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/49319a7ff766dc7c7638c0226294beebd45f6762"><code>49319a7</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/758">#758</a> from uuid-rs/chore/test-overflow</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/47b9130ada093391db900b03e53f716310ae1ca0"><code>47b9130</code></a> ensure v7 methods don't overflow on max values</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/0c561e3443191065b724e8f8eb7b116f08d4e181"><code>0c561e3</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/757">#757</a> from uuid-rs/ci/more-miri</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/252770be2f824e2cb4a2f68cb5980e0b7bd4b6cc"><code>252770b</code></a> expand miri tests to cover all features</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/e62647f7623f8663f806ec69d8264fbfb836a6e3"><code>e62647f</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/755">#755</a> from uuid-rs/feat/v7-counter</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/c270b3d66ae809517663ffeb38d56e004c517f7f"><code>c270b3d</code></a> improve testing for contexts</li>
<li>Additional commits viewable in <a href="https://github.com/uuid-rs/uuid/compare/1.8.0...1.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uuid&package-manager=cargo&previous-version=1.8.0&new-version=1.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-24 16:40:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4765" class=".btn">#4765</a>
            </td>
            <td>
                <b>
                    fix: restore RawGenesisTransaction schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
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
        Created At 2024-06-24 08:30:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4764" class=".btn">#4764</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.66 to 2.0.68
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.66 to 2.0.68.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.68</h2>
<ul>
<li>Improve panic location when <code>parse_quote!</code> parses invalid syntax (<a href="https://redirect.github.com/dtolnay/syn/issues/1690">#1690</a>, thanks <a href="https://github.com/stepancheg"><code>@​stepancheg</code></a>)</li>
<li>More efficient peek implementation for <code>Group</code> and <code>Lifetime</code> (<a href="https://redirect.github.com/dtolnay/syn/issues/1687">#1687</a>)</li>
</ul>
<h2>2.0.67</h2>
<ul>
<li>Produce more accurate error message locations for errors located at the end of a nested group (<a href="https://redirect.github.com/dtolnay/syn/issues/1679">#1679</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1680">#1680</a>)</li>
<li>Support peeking <code>LitCStr</code> in ParseStream::peek (<a href="https://redirect.github.com/dtolnay/syn/issues/1682">#1682</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/ecb0429297d3da2f20ab8559e41ddf8a2137d83b"><code>ecb0429</code></a> Release 2.0.68</li>
<li><a href="https://github.com/dtolnay/syn/commit/37edbd23908006e77c42dae3e64f13f53470c5b6"><code>37edbd2</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1690">#1690</a> from stepancheg/track-called</li>
<li><a href="https://github.com/dtolnay/syn/commit/43387720a3d52db3c148e5383cd6d9ef3b766611"><code>4338772</code></a> track-caller in parse_quote_spanned</li>
<li><a href="https://github.com/dtolnay/syn/commit/537b0c58f4d00c1f412fb83d258900843f65814e"><code>537b0c5</code></a> Update test suite to nightly-2024-06-22</li>
<li><a href="https://github.com/dtolnay/syn/commit/b088d5c2242478edb5b07e5a7221c37507287840"><code>b088d5c</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1688">#1688</a> from dtolnay/peeklit</li>
<li><a href="https://github.com/dtolnay/syn/commit/9b4e478a98aeb90a113eeac2bf882402c8574dfb"><code>9b4e478</code></a> Relocate Lit peek impls into lit module</li>
<li><a href="https://github.com/dtolnay/syn/commit/38f2ddb7632a39d7ef98a836369acaf8fb9babf1"><code>38f2ddb</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1687">#1687</a> from dtolnay/fastpeek</li>
<li><a href="https://github.com/dtolnay/syn/commit/ef20bfdfbf32c06a4930b26d683b61defb34b043"><code>ef20bfd</code></a> Optimize the peek impl of Group and Lifetime</li>
<li><a href="https://github.com/dtolnay/syn/commit/4b6c96a642be81c8020e0d4a6502b91facf5026e"><code>4b6c96a</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1686">#1686</a> from dtolnay/isempty</li>
<li><a href="https://github.com/dtolnay/syn/commit/87d57920513951b05a4dd64a39d1d8a39c314624"><code>87d5792</code></a> Reword explanation of ParseBuffer::is_empty</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.66...2.0.68">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.66&new-version=2.0.68)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-24 05:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4761" class=".btn">#4761</a>
            </td>
            <td>
                <b>
                    chore: move back to the upstream displaydoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Now that the displaydoc has released a version which fixed the nightly warnings, we can migrate back to it.

(We were previously using a git version because of #4567)

### Checklist

- [ ] make ci pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 18:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4759" class=".btn">#4759</a>
            </td>
            <td>
                <b>
                    chore(deps): bump proc-macro2 from 1.0.85 to 1.0.86
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [proc-macro2](https://github.com/dtolnay/proc-macro2) from 1.0.85 to 1.0.86.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/proc-macro2/releases">proc-macro2's releases</a>.</em></p>
<blockquote>
<h2>1.0.86</h2>
<ul>
<li>Documentation improvements</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/aa9476b27932ae1b1b50bbfe0530b3b261fc1b72"><code>aa9476b</code></a> Release 1.0.86</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/19613587b70633e8bd383dd2fc29856d2d080f45"><code>1961358</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/466">#466</a> from dtolnay/buildrs</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/e1bd2cc29da09be421555bb0e1156c5e2b87df5d"><code>e1bd2cc</code></a> Bring build script comments up to date</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/5b271279521e11ac6eada5435e5a8d87f46d3619"><code>5b27127</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/465">#465</a> from dtolnay/ignorereason</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/0da4629757024ac6dac1680ba3be44bac24af809"><code>0da4629</code></a> Fill in ignore reasons in all #[ignore] attributes</li>
<li>See full diff in <a href="https://github.com/dtolnay/proc-macro2/compare/1.0.85...1.0.86">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=proc-macro2&package-manager=cargo&previous-version=1.0.85&new-version=1.0.86)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-21 17:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4757" class=".btn">#4757</a>
            </td>
            <td>
                <b>
                    fix!: Upgrade executor in separate transaction in genesis block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

`GenesisBlock` now have two transactions, first with single `Upgrade` instruction to set executor, and second with all other instructions. If there are no other instructions, second transaction will be omitted.

### Linked issue

Closes #4743

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
        Created At 2024-06-21 12:09:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4752" class=".btn">#4752</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.8.0 to 25.9.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.8.0 to 25.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.9.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.9.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v25.9.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.9.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.9.0..v25.9.1">v25.9.1 - 2024-06-20</a></h3>
<ul>
<li>Change <code>pydecimal</code> type hint for <code>min_value</code>, <code>max_value</code> to allow <code>int</code>s. Thanks <a href="https://github.com/parsariyahi"><code>@​parsariyahi</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v25.8.0..v25.9.0">v25.9.0 - 2024-06-20</a></h3>
<ul>
<li>Add support for Nigerian Yoruba names and surnames (<code>yo_NG</code>). Thanks <a href="https://github.com/5uru"><code>@​5uru</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/fb42357d0ac30c0fdba200d5339f8fe9f9ce6f81"><code>fb42357</code></a> Bump version: 25.9.0 → 25.9.1</li>
<li><a href="https://github.com/joke2k/faker/commit/7c391c45d840c9b7ea29e723fee6cbfd6ba08d24"><code>7c391c4</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/10c2ba35cda949188c460464f46e79ee0236d605"><code>10c2ba3</code></a> Fix typing on <code>pydecimal</code></li>
<li><a href="https://github.com/joke2k/faker/commit/d0bfbfbf7a30b1831bf466cfb48ac627bb090b15"><code>d0bfbfb</code></a> Change <code>pydecimal</code> type hint for <code>min_value</code>, <code>max_value</code> to <code>numbers.Number</code>...</li>
<li><a href="https://github.com/joke2k/faker/commit/c49ef43bf5ac8ccaaded6ff02866e9eabdaa27b5"><code>c49ef43</code></a> Bump version: 25.8.0 → 25.9.0</li>
<li><a href="https://github.com/joke2k/faker/commit/f375cbc42d8dd973aa170207dbe2e2ab2ea945c3"><code>f375cbc</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/fc329ad841d45967ff3cda49d06c9399d5f56299"><code>fc329ad</code></a> 💄 format code</li>
<li><a href="https://github.com/joke2k/faker/commit/84766274e5476f7698df00bc7e7ba3c3c99ad82f"><code>8476627</code></a> Added support for Nigerian Yoruba names and surnames (yo_NG) (<a href="https://redirect.github.com/joke2k/faker/issues/2054">#2054</a>)</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.8.0...v25.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.8.0&new-version=25.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-20 16:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4750" class=".btn">#4750</a>
            </td>
            <td>
                <b>
                    ci: Modify CodeQuality job branch checkout variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
Attempt to fix `CodeQuality` workflow `checkout` actions that always points to repository defaults branch even if PR is coming from not-default branch.

### Linked issue
https://github.com/orgs/community/discussions/66784
https://github.com/orgs/community/discussions/25220

### Benefits

Perhaps will fix `CodeQuality` workflow.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 11:29:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4747" class=".btn">#4747</a>
            </td>
            <td>
                <b>
                    chore(deps): bump curve25519-dalek from 4.1.2 to 4.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [curve25519-dalek](https://github.com/dalek-cryptography/curve25519-dalek) from 4.1.2 to 4.1.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/5312a0311ec40df95be953eacfa8a11b9a34bc54"><code>5312a03</code></a> curve: Bump version to 4.1.3 (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/660">#660</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/b4f9e4df92a4689fb59e312a21f940ba06ba7013"><code>b4f9e4d</code></a> SECURITY: fix timing variability in backend/serial/u32/scalar.rs (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/661">#661</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/415892acf1cdf9161bd6a4c99bc2f4cb8fae5e6a"><code>415892a</code></a> SECURITY: fix timing variability in backend/serial/u64/scalar.rs (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/659">#659</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/56bf398d0caed63ef1d1edfbd35eb5335132aba2"><code>56bf398</code></a> Updates license field to valid SPDX format (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/647">#647</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/9252fa5c0d09054fed4ac4d649e63c40fad7abaf"><code>9252fa5</code></a> Mitigate check-cfg until MSRV 1.77 (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/652">#652</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/1efe6a93b176c4389b78e81e52b2cf85d728aac6"><code>1efe6a9</code></a> Fix a minor typo in signing.rs (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/649">#649</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/cc3421a22fa7ee1f557cbe9243b450da53bbe962"><code>cc3421a</code></a> Indicate that the rand_core feature is required (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/641">#641</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/858c4ca8ae03d33fe8b71b4504c4d3f5ff5b45c0"><code>858c4ca</code></a> Address new nightly clippy unnecessary qualifications (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/639">#639</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/31ccb6705067d68782cb135e23c79b640a6a06ee"><code>31ccb67</code></a> Remove platforms in favor using CARGO_CFG_TARGET_POINTER_WIDTH (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/636">#636</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/19c7f4a5d5e577adc9cc65a837abef9ed7ebf0a4"><code>19c7f4a</code></a> Fix new nightly redundant import lint warns (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/638">#638</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dalek-cryptography/curve25519-dalek/compare/curve25519-4.1.2...curve25519-4.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=curve25519-dalek&package-manager=cargo&previous-version=4.1.2&new-version=4.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-19 16:09:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4746" class=".btn">#4746</a>
            </td>
            <td>
                <b>
                    chore(deps): bump url from 2.5.1 to 2.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [url](https://github.com/servo/rust-url) from 2.5.1 to 2.5.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/servo/rust-url/commit/54346fa288e16b25b71c45149d7067c752b450e0"><code>54346fa</code></a> Revert &quot;Reimplement idna on top of ICU4X&quot; (<a href="https://redirect.github.com/servo/rust-url/issues/946">#946</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/dcfbed3e90b4bbbb70f121f802f1d9b25adb8f89"><code>dcfbed3</code></a> Update idna to 1.0.1 (<a href="https://redirect.github.com/servo/rust-url/issues/945">#945</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/467ef63969f477ee44b7456bb450fba95af25780"><code>467ef63</code></a> fix panic on <code>xn--55555577</code> (<a href="https://redirect.github.com/servo/rust-url/issues/940">#940</a>)</li>
<li>See full diff in <a href="https://github.com/servo/rust-url/compare/v2.5.1...v2.5.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url&package-manager=cargo&previous-version=2.5.1&new-version=2.5.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-19 16:08:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4745" class=".btn">#4745</a>
            </td>
            <td>
                <b>
                    refactor: send blocks to observing peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport of #4392 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 13:00:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4744" class=".btn">#4744</a>
            </td>
            <td>
                <b>
                    fix(sumeragi): early exit from handle_block_sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Exit early from `handle_block_sync` if received block is the same or has smaller or equal view change index.

## Benefits

Improve performance of block sync by avoid doing work where not necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 11:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4742" class=".btn">#4742</a>
            </td>
            <td>
                <b>
                    refactor: move permission migration into executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description


### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

we no longer depend on the `ExecutorDataModel::permissions` being correct. 
It's just for users to query it the same way as `ExecutorDataModel::custom_instruction` is

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
        Created At 2024-06-19 07:51:17 +0000 UTC
    </div>
</div>

