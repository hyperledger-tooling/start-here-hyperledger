---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2528" class=".btn">#2528</a>
            </td>
            <td>
                <b>
                    Bump regex from 1.1.0 to 1.5.6 in /libnullpay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [regex](https://github.com/rust-lang/regex) from 1.1.0 to 1.5.6.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/regex/blob/master/CHANGELOG.md">regex's changelog</a>.</em></p>
<blockquote>
<h1>1.5.6 (2022-05-20)</h1>
<p>This release includes a few bug fixes, including a bug that produced incorrect
matches when a non-greedy <code>?</code> operator was used.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/680">#680</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/680">rust-lang/regex#680</a>):
Fixes a bug where <code>[[:alnum:][:^ascii:]]</code> dropped <code>[:alnum:]</code> from the class.</li>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/859">#859</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/859">rust-lang/regex#859</a>):
Fixes a bug where <code>Hir::is_match_empty</code> returned <code>false</code> for <code>\b</code>.</li>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/862">#862</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/862">rust-lang/regex#862</a>):
Fixes a bug where 'ab??' matches 'ab' instead of 'a' in 'ab'.</li>
</ul>
<h1>1.5.5 (2022-03-08)</h1>
<p>This releases fixes a security bug in the regex compiler. This bug permits a
vector for a denial-of-service attack in cases where the regex being compiled
is untrusted. There are no known problems where the regex is itself trusted,
including in cases of untrusted haystacks.</p>
<ul>
<li><a href="https://github.com/rust-lang/regex/security/advisories/GHSA-m5pq-gvj9-9vr8">SECURITY #GHSA-m5pq-gvj9-9vr8</a>:
Fixes a bug in the regex compiler where empty sub-expressions subverted the
existing mitigations in place to enforce a size limit on compiled regexes.
The Rust Security Response WG published an advisory about this:
<a href="https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw">https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw</a></li>
</ul>
<h1>1.5.4 (2021-05-06)</h1>
<p>This release fixes another compilation failure when building regex. This time,
the fix is for when the <code>pattern</code> feature is enabled, which only works on
nightly Rust. CI has been updated to test this case.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/772">#772</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/pull/772">rust-lang/regex#772</a>):
Fix build when <code>pattern</code> feature is enabled.</li>
</ul>
<h1>1.5.3 (2021-05-01)</h1>
<p>This releases fixes a bug when building regex with only the <code>unicode-perl</code>
feature. It turns out that while CI was building this configuration, it wasn't
actually failing the overall build on a failed compilation.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">#769</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">rust-lang/regex#769</a>):
Fix build in <code>regex-syntax</code> when only the <code>unicode-perl</code> feature is enabled.</li>
</ul>
<h1>1.5.2 (2021-05-01)</h1>
<p>This release fixes a performance bug when Unicode word boundaries are used.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/regex/commit/9aef5b1edc2a436244b936db53a03ed6d720e87e"><code>9aef5b1</code></a> 1.5.6</li>
<li><a href="https://github.com/rust-lang/regex/commit/2931b070fd9b525dec95c2b4c91f8b9ee500239e"><code>2931b07</code></a> syntax: bump minimum regex-syntax version to 0.6.26</li>
<li><a href="https://github.com/rust-lang/regex/commit/b41bde0b854e3cd1018f55e5dcd80c09b418d6c4"><code>b41bde0</code></a> regex-syntax-0.6.26</li>
<li><a href="https://github.com/rust-lang/regex/commit/d98da65bb3df16836f1181c6f7e4f03c3af1d5a5"><code>d98da65</code></a> changelog: 1.5.6</li>
<li><a href="https://github.com/rust-lang/regex/commit/1c19619672c2ef16dc9f64fec38af5719c4ec06c"><code>1c19619</code></a> syntax: fix literal extraction for 'ab??'</li>
<li><a href="https://github.com/rust-lang/regex/commit/88a2a62d861d189faae539990f63cb9cf195bd8c"><code>88a2a62</code></a> syntax: fix 'is_match_empty' predicate</li>
<li><a href="https://github.com/rust-lang/regex/commit/72f09f1aeb0ff3f703b1afdbdd21f5ff63162fb4"><code>72f09f1</code></a> syntax: fix ascii class union bug</li>
<li><a href="https://github.com/rust-lang/regex/commit/b5372864e2df6a2f5e543a556a62197f50ca3650"><code>b537286</code></a> doc: fix some typos</li>
<li><a href="https://github.com/rust-lang/regex/commit/258bdf798a14f50529c1665e84cc8a3a9e2c90fc"><code>258bdf7</code></a> changelog: 1.5.5</li>
<li><a href="https://github.com/rust-lang/regex/commit/d130381b150756ba7e5940efdc6ebdf47f4febc0"><code>d130381</code></a> 1.5.5</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/regex/compare/1.1.0...1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=regex&package-manager=cargo&previous-version=1.1.0&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 21:13:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2527" class=".btn">#2527</a>
            </td>
            <td>
                <b>
                    Bump regex from 1.3.7 to 1.5.5 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [regex](https://github.com/rust-lang/regex) from 1.3.7 to 1.5.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/regex/blob/master/CHANGELOG.md">regex's changelog</a>.</em></p>
<blockquote>
<h1>1.5.5 (2022-03-08)</h1>
<p>This releases fixes a security bug in the regex compiler. This bug permits a
vector for a denial-of-service attack in cases where the regex being compiled
is untrusted. There are no known problems where the regex is itself trusted,
including in cases of untrusted haystacks.</p>
<ul>
<li><a href="https://github.com/rust-lang/regex/security/advisories/GHSA-m5pq-gvj9-9vr8">SECURITY #GHSA-m5pq-gvj9-9vr8</a>:
Fixes a bug in the regex compiler where empty sub-expressions subverted the
existing mitigations in place to enforce a size limit on compiled regexes.
The Rust Security Response WG published an advisory about this:
<a href="https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw">https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw</a></li>
</ul>
<h1>1.5.4 (2021-05-06)</h1>
<p>This release fixes another compilation failure when building regex. This time,
the fix is for when the <code>pattern</code> feature is enabled, which only works on
nightly Rust. CI has been updated to test this case.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/772">#772</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/pull/772">rust-lang/regex#772</a>):
Fix build when <code>pattern</code> feature is enabled.</li>
</ul>
<h1>1.5.3 (2021-05-01)</h1>
<p>This releases fixes a bug when building regex with only the <code>unicode-perl</code>
feature. It turns out that while CI was building this configuration, it wasn't
actually failing the overall build on a failed compilation.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">#769</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">rust-lang/regex#769</a>):
Fix build in <code>regex-syntax</code> when only the <code>unicode-perl</code> feature is enabled.</li>
</ul>
<h1>1.5.2 (2021-05-01)</h1>
<p>This release fixes a performance bug when Unicode word boundaries are used.
Namely, for certain regexes on certain inputs, it's possible for the lazy DFA
to stop searching (causing a fallback to a slower engine) when it doesn't
actually need to.</p>
<p>[PR <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/768">#768</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/pull/768">rust-lang/regex#768</a>) fixes the bug, which was
originally reported in
<a href="https://github-redirect.dependabot.com/BurntSushi/ripgrep/issues/1860">ripgrep#1860</a>.</p>
<h1>1.5.1 (2021-04-30)</h1>
<p>This is a patch release that fixes a compilation error when the <code>perf-literal</code>
feature is not enabled.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/regex/commit/d130381b150756ba7e5940efdc6ebdf47f4febc0"><code>d130381</code></a> 1.5.5</li>
<li><a href="https://github.com/rust-lang/regex/commit/ae70b41d4f46641dbc45c7a4f87954aea356283e"><code>ae70b41</code></a> security: fix denial-of-service bug in compiler</li>
<li><a href="https://github.com/rust-lang/regex/commit/b92ffd5471018419ec48dbdef32757424439f065"><code>b92ffd5</code></a> cargo: use SPDX license format</li>
<li><a href="https://github.com/rust-lang/regex/commit/f6e52dafdee305d16d6778e7bfe935bd9a6ae38b"><code>f6e52da</code></a> syntax: fix 'unused' warnings</li>
<li><a href="https://github.com/rust-lang/regex/commit/5197f21287344d2994f9cf06758a3ea30f5a26c3"><code>5197f21</code></a> fuzz: do not use inherits in Cargo.toml</li>
<li><a href="https://github.com/rust-lang/regex/commit/3662851482327e3642940981298150c93718de3c"><code>3662851</code></a> doc: fix typo</li>
<li><a href="https://github.com/rust-lang/regex/commit/63ee6699a27b294774af0154862e5cc35b495ee6"><code>63ee669</code></a> syntax/doc: fix 'their' typo</li>
<li><a href="https://github.com/rust-lang/regex/commit/d6bc7a4c3b58e1d618024aaededa722df32fa6e8"><code>d6bc7a4</code></a> readme: remove broken badge</li>
<li><a href="https://github.com/rust-lang/regex/commit/bd7466034f8cccc3b0918201d1eb099cc8be3c56"><code>bd74660</code></a> fuzz: try to fix build issue</li>
<li><a href="https://github.com/rust-lang/regex/commit/bd0a14231b8848669e0d257ba55526f62756c749"><code>bd0a142</code></a> readme: fix badges</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/regex/compare/regex-1.3.7...1.5.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=regex&package-manager=cargo&previous-version=1.3.7&new-version=1.5.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 21:13:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2526" class=".btn">#2526</a>
            </td>
            <td>
                <b>
                    Bump regex from 1.3.1 to 1.5.5 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [regex](https://github.com/rust-lang/regex) from 1.3.1 to 1.5.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/regex/blob/master/CHANGELOG.md">regex's changelog</a>.</em></p>
<blockquote>
<h1>1.5.5 (2022-03-08)</h1>
<p>This releases fixes a security bug in the regex compiler. This bug permits a
vector for a denial-of-service attack in cases where the regex being compiled
is untrusted. There are no known problems where the regex is itself trusted,
including in cases of untrusted haystacks.</p>
<ul>
<li><a href="https://github.com/rust-lang/regex/security/advisories/GHSA-m5pq-gvj9-9vr8">SECURITY #GHSA-m5pq-gvj9-9vr8</a>:
Fixes a bug in the regex compiler where empty sub-expressions subverted the
existing mitigations in place to enforce a size limit on compiled regexes.
The Rust Security Response WG published an advisory about this:
<a href="https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw">https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw</a></li>
</ul>
<h1>1.5.4 (2021-05-06)</h1>
<p>This release fixes another compilation failure when building regex. This time,
the fix is for when the <code>pattern</code> feature is enabled, which only works on
nightly Rust. CI has been updated to test this case.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/772">#772</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/pull/772">rust-lang/regex#772</a>):
Fix build when <code>pattern</code> feature is enabled.</li>
</ul>
<h1>1.5.3 (2021-05-01)</h1>
<p>This releases fixes a bug when building regex with only the <code>unicode-perl</code>
feature. It turns out that while CI was building this configuration, it wasn't
actually failing the overall build on a failed compilation.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">#769</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">rust-lang/regex#769</a>):
Fix build in <code>regex-syntax</code> when only the <code>unicode-perl</code> feature is enabled.</li>
</ul>
<h1>1.5.2 (2021-05-01)</h1>
<p>This release fixes a performance bug when Unicode word boundaries are used.
Namely, for certain regexes on certain inputs, it's possible for the lazy DFA
to stop searching (causing a fallback to a slower engine) when it doesn't
actually need to.</p>
<p>[PR <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/768">#768</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/pull/768">rust-lang/regex#768</a>) fixes the bug, which was
originally reported in
<a href="https://github-redirect.dependabot.com/BurntSushi/ripgrep/issues/1860">ripgrep#1860</a>.</p>
<h1>1.5.1 (2021-04-30)</h1>
<p>This is a patch release that fixes a compilation error when the <code>perf-literal</code>
feature is not enabled.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/regex/commit/d130381b150756ba7e5940efdc6ebdf47f4febc0"><code>d130381</code></a> 1.5.5</li>
<li><a href="https://github.com/rust-lang/regex/commit/ae70b41d4f46641dbc45c7a4f87954aea356283e"><code>ae70b41</code></a> security: fix denial-of-service bug in compiler</li>
<li><a href="https://github.com/rust-lang/regex/commit/b92ffd5471018419ec48dbdef32757424439f065"><code>b92ffd5</code></a> cargo: use SPDX license format</li>
<li><a href="https://github.com/rust-lang/regex/commit/f6e52dafdee305d16d6778e7bfe935bd9a6ae38b"><code>f6e52da</code></a> syntax: fix 'unused' warnings</li>
<li><a href="https://github.com/rust-lang/regex/commit/5197f21287344d2994f9cf06758a3ea30f5a26c3"><code>5197f21</code></a> fuzz: do not use inherits in Cargo.toml</li>
<li><a href="https://github.com/rust-lang/regex/commit/3662851482327e3642940981298150c93718de3c"><code>3662851</code></a> doc: fix typo</li>
<li><a href="https://github.com/rust-lang/regex/commit/63ee6699a27b294774af0154862e5cc35b495ee6"><code>63ee669</code></a> syntax/doc: fix 'their' typo</li>
<li><a href="https://github.com/rust-lang/regex/commit/d6bc7a4c3b58e1d618024aaededa722df32fa6e8"><code>d6bc7a4</code></a> readme: remove broken badge</li>
<li><a href="https://github.com/rust-lang/regex/commit/bd7466034f8cccc3b0918201d1eb099cc8be3c56"><code>bd74660</code></a> fuzz: try to fix build issue</li>
<li><a href="https://github.com/rust-lang/regex/commit/bd0a14231b8848669e0d257ba55526f62756c749"><code>bd0a142</code></a> readme: fix badges</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/regex/compare/1.3.1...1.5.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=regex&package-manager=cargo&previous-version=1.3.1&new-version=1.5.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 21:09:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2525" class=".btn">#2525</a>
            </td>
            <td>
                <b>
                    Bump regex from 1.3.1 to 1.5.6 in /experimental/plugins/postgres_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [regex](https://github.com/rust-lang/regex) from 1.3.1 to 1.5.6.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/regex/blob/master/CHANGELOG.md">regex's changelog</a>.</em></p>
<blockquote>
<h1>1.5.6 (2022-05-20)</h1>
<p>This release includes a few bug fixes, including a bug that produced incorrect
matches when a non-greedy <code>?</code> operator was used.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/680">#680</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/680">rust-lang/regex#680</a>):
Fixes a bug where <code>[[:alnum:][:^ascii:]]</code> dropped <code>[:alnum:]</code> from the class.</li>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/859">#859</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/859">rust-lang/regex#859</a>):
Fixes a bug where <code>Hir::is_match_empty</code> returned <code>false</code> for <code>\b</code>.</li>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/862">#862</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/862">rust-lang/regex#862</a>):
Fixes a bug where 'ab??' matches 'ab' instead of 'a' in 'ab'.</li>
</ul>
<h1>1.5.5 (2022-03-08)</h1>
<p>This releases fixes a security bug in the regex compiler. This bug permits a
vector for a denial-of-service attack in cases where the regex being compiled
is untrusted. There are no known problems where the regex is itself trusted,
including in cases of untrusted haystacks.</p>
<ul>
<li><a href="https://github.com/rust-lang/regex/security/advisories/GHSA-m5pq-gvj9-9vr8">SECURITY #GHSA-m5pq-gvj9-9vr8</a>:
Fixes a bug in the regex compiler where empty sub-expressions subverted the
existing mitigations in place to enforce a size limit on compiled regexes.
The Rust Security Response WG published an advisory about this:
<a href="https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw">https://groups.google.com/g/rustlang-security-announcements/c/NcNNL1Jq7Yw</a></li>
</ul>
<h1>1.5.4 (2021-05-06)</h1>
<p>This release fixes another compilation failure when building regex. This time,
the fix is for when the <code>pattern</code> feature is enabled, which only works on
nightly Rust. CI has been updated to test this case.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/772">#772</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/pull/772">rust-lang/regex#772</a>):
Fix build when <code>pattern</code> feature is enabled.</li>
</ul>
<h1>1.5.3 (2021-05-01)</h1>
<p>This releases fixes a bug when building regex with only the <code>unicode-perl</code>
feature. It turns out that while CI was building this configuration, it wasn't
actually failing the overall build on a failed compilation.</p>
<ul>
<li>[BUG <a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">#769</a>](<a href="https://github-redirect.dependabot.com/rust-lang/regex/issues/769">rust-lang/regex#769</a>):
Fix build in <code>regex-syntax</code> when only the <code>unicode-perl</code> feature is enabled.</li>
</ul>
<h1>1.5.2 (2021-05-01)</h1>
<p>This release fixes a performance bug when Unicode word boundaries are used.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/regex/commit/9aef5b1edc2a436244b936db53a03ed6d720e87e"><code>9aef5b1</code></a> 1.5.6</li>
<li><a href="https://github.com/rust-lang/regex/commit/2931b070fd9b525dec95c2b4c91f8b9ee500239e"><code>2931b07</code></a> syntax: bump minimum regex-syntax version to 0.6.26</li>
<li><a href="https://github.com/rust-lang/regex/commit/b41bde0b854e3cd1018f55e5dcd80c09b418d6c4"><code>b41bde0</code></a> regex-syntax-0.6.26</li>
<li><a href="https://github.com/rust-lang/regex/commit/d98da65bb3df16836f1181c6f7e4f03c3af1d5a5"><code>d98da65</code></a> changelog: 1.5.6</li>
<li><a href="https://github.com/rust-lang/regex/commit/1c19619672c2ef16dc9f64fec38af5719c4ec06c"><code>1c19619</code></a> syntax: fix literal extraction for 'ab??'</li>
<li><a href="https://github.com/rust-lang/regex/commit/88a2a62d861d189faae539990f63cb9cf195bd8c"><code>88a2a62</code></a> syntax: fix 'is_match_empty' predicate</li>
<li><a href="https://github.com/rust-lang/regex/commit/72f09f1aeb0ff3f703b1afdbdd21f5ff63162fb4"><code>72f09f1</code></a> syntax: fix ascii class union bug</li>
<li><a href="https://github.com/rust-lang/regex/commit/b5372864e2df6a2f5e543a556a62197f50ca3650"><code>b537286</code></a> doc: fix some typos</li>
<li><a href="https://github.com/rust-lang/regex/commit/258bdf798a14f50529c1665e84cc8a3a9e2c90fc"><code>258bdf7</code></a> changelog: 1.5.5</li>
<li><a href="https://github.com/rust-lang/regex/commit/d130381b150756ba7e5940efdc6ebdf47f4febc0"><code>d130381</code></a> 1.5.5</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/regex/compare/1.3.1...1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=regex&package-manager=cargo&previous-version=1.3.1&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 21:09:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2524" class=".btn">#2524</a>
            </td>
            <td>
                <b>
                    Bump socket2 from 0.3.11 to 0.3.19 in /experimental/plugins/postgres_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [socket2](https://github.com/rust-lang/socket2) from 0.3.11 to 0.3.19.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/socket2/blob/master/CHANGELOG.md">socket2's changelog</a>.</em></p>
<blockquote>
<h1>0.4.5</h1>
<h2>Changed</h2>
<ul>
<li>Replace <code>winapi</code> dependency with <code>windows-sys</code>
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/303">rust-lang/socket2#303</a>).</li>
</ul>
<h2>Added</h2>
<ul>
<li><code>Socket::join_ssm_v4</code> and <code>Socket::leave_ssm_v4</code>
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/298">rust-lang/socket2#298</a>).</li>
<li><code>Socket::set_recv_tos</code> and <code>Socket::recv_tos</code>
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/299">rust-lang/socket2#299</a>).</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>Fix OpenBSD build
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/291">rust-lang/socket2#291</a>).</li>
<li>Fix OpenBSD build
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/291">rust-lang/socket2#291</a>).</li>
</ul>
<h1>0.4.4</h1>
<h2>Fixed</h2>
<ul>
<li>Libc v0.2.114 fixed an issue where <code>ip_mreqn</code> where was not defined for Linux
s390x.</li>
</ul>
<h1>0.4.3 (yanked)</h1>
<h2>Added</h2>
<ul>
<li><code>Socket::set_fib</code>: sets <code>SO_SETFIB</code> (<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/271">rust-lang/socket2#271</a>).</li>
<li><code>Socket::attach_filter</code>, <code>SO_ATTACH_FILTER</code> (<a href="https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232">https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232</a>).</li>
<li><code>Socket::detach_filter</code>, <code>SO_DETACH_FILTER</code> (<a href="https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232">https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232</a>).</li>
<li><code>Socket::{header_included, set_header_included}</code>: sets or gets <code>IP_HDRINCL</code>
(<a href="https://github.com/rust-lang/socket2/commit/f9e882ee53c0b4e89c5043b6d709af95c9db5599">https://github.com/rust-lang/socket2/commit/f9e882ee53c0b4e89c5043b6d709af95c9db5599</a>).</li>
<li><code>Socket::{cork, set_cork}</code>: sets or gets <code>TCP_CORK</code>
(<a href="https://github.com/rust-lang/socket2/commit/50f31f18aac8fd6ef277df2906adeeed9fa391de">https://github.com/rust-lang/socket2/commit/50f31f18aac8fd6ef277df2906adeeed9fa391de</a>).</li>
<li><code>Socket::{quickack, set_quickack}</code>: sets or gets <code>TCP_QUICKACK</code>
(<a href="https://github.com/rust-lang/socket2/commit/849eee2abc5d5170d2d3bc635386a2ba13b04530">https://github.com/rust-lang/socket2/commit/849eee2abc5d5170d2d3bc635386a2ba13b04530</a>).</li>
<li><code>Socket::{thin_linear_timeouts, set_thin_linear_timeouts}</code>: sets or gets
<code>TCP_THIN_LINEAR_TIMEOUTS</code>
(<a href="https://github.com/rust-lang/socket2/commit/24c231ca463a17f51e53e7a554c7915a95bdbcc7">https://github.com/rust-lang/socket2/commit/24c231ca463a17f51e53e7a554c7915a95bdbcc7</a>).</li>
<li><code>Socket::{join_multicast_v4_n, leave_multicast_v4_n}</code>: extends the existing
multicast API by allowing an index to be used (in addition to an address)
(<a href="https://github.com/rust-lang/socket2/commit/750f83618b967c620bbfdf6ca04de7362bdb42b5">https://github.com/rust-lang/socket2/commit/750f83618b967c620bbfdf6ca04de7362bdb42b5</a>).</li>
</ul>
<h1>0.4.2</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/socket2/commit/c991f802642525dcf063c253b6fcaa5d6f4c8cb6"><code>c991f80</code></a> Release v0.3.19</li>
<li><a href="https://github.com/rust-lang/socket2/commit/1dfd15d8f3626eb91ff6238155d3bfbfaed59cf5"><code>1dfd15d</code></a> Add Socket::(bind_)device</li>
<li><a href="https://github.com/rust-lang/socket2/commit/beeebd01b8ff5c73924df09cd78bea5c47b1acd0"><code>beeebd0</code></a> Release v0.3.18</li>
<li><a href="https://github.com/rust-lang/socket2/commit/a0053b522c363a07972935cbd6cb36b6b824638b"><code>a0053b5</code></a> Backport redox compilation to 0.3</li>
<li><a href="https://github.com/rust-lang/socket2/commit/3b4214da98dd344db97f1a7d5d48da18e14d2aba"><code>3b4214d</code></a> Fix compilation on Haiku</li>
<li><a href="https://github.com/rust-lang/socket2/commit/7312f81e94c22bb90fbe1acd76b294fc5e91e6ec"><code>7312f81</code></a> Release v0.3.17</li>
<li><a href="https://github.com/rust-lang/socket2/commit/930c9a9803df565a6733f4c6b5b1b198282c7b33"><code>930c9a9</code></a> Additional Linux socket options</li>
<li><a href="https://github.com/rust-lang/socket2/commit/06a25107c7fc6797370e990d213ffb28fa4992af"><code>06a2510</code></a> [0.3] Update cfg-if to 1.0</li>
<li><a href="https://github.com/rust-lang/socket2/commit/73d54bb3366474aa011a7760b186d3d799347ca1"><code>73d54bb</code></a> Release v0.3.16</li>
<li><a href="https://github.com/rust-lang/socket2/commit/d2c15de84991947b6577bea92763efe0a2eecf28"><code>d2c15de</code></a> Don't assume memory layout of std::net::SocketAddr</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/socket2/compare/0.3.11...v0.3.19">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket2&package-manager=cargo&previous-version=0.3.11&new-version=0.3.19)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:54:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2523" class=".btn">#2523</a>
            </td>
            <td>
                <b>
                    Bump socket2 from 0.3.11 to 0.3.19 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [socket2](https://github.com/rust-lang/socket2) from 0.3.11 to 0.3.19.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/socket2/blob/master/CHANGELOG.md">socket2's changelog</a>.</em></p>
<blockquote>
<h1>0.4.5</h1>
<h2>Changed</h2>
<ul>
<li>Replace <code>winapi</code> dependency with <code>windows-sys</code>
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/303">rust-lang/socket2#303</a>).</li>
</ul>
<h2>Added</h2>
<ul>
<li><code>Socket::join_ssm_v4</code> and <code>Socket::leave_ssm_v4</code>
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/298">rust-lang/socket2#298</a>).</li>
<li><code>Socket::set_recv_tos</code> and <code>Socket::recv_tos</code>
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/299">rust-lang/socket2#299</a>).</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>Fix OpenBSD build
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/291">rust-lang/socket2#291</a>).</li>
<li>Fix OpenBSD build
(<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/291">rust-lang/socket2#291</a>).</li>
</ul>
<h1>0.4.4</h1>
<h2>Fixed</h2>
<ul>
<li>Libc v0.2.114 fixed an issue where <code>ip_mreqn</code> where was not defined for Linux
s390x.</li>
</ul>
<h1>0.4.3 (yanked)</h1>
<h2>Added</h2>
<ul>
<li><code>Socket::set_fib</code>: sets <code>SO_SETFIB</code> (<a href="https://github-redirect.dependabot.com/rust-lang/socket2/pull/271">rust-lang/socket2#271</a>).</li>
<li><code>Socket::attach_filter</code>, <code>SO_ATTACH_FILTER</code> (<a href="https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232">https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232</a>).</li>
<li><code>Socket::detach_filter</code>, <code>SO_DETACH_FILTER</code> (<a href="https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232">https://github.com/rust-lang/socket2/commit/6601ed132b37d6e9d178b34918bfb0b236800232</a>).</li>
<li><code>Socket::{header_included, set_header_included}</code>: sets or gets <code>IP_HDRINCL</code>
(<a href="https://github.com/rust-lang/socket2/commit/f9e882ee53c0b4e89c5043b6d709af95c9db5599">https://github.com/rust-lang/socket2/commit/f9e882ee53c0b4e89c5043b6d709af95c9db5599</a>).</li>
<li><code>Socket::{cork, set_cork}</code>: sets or gets <code>TCP_CORK</code>
(<a href="https://github.com/rust-lang/socket2/commit/50f31f18aac8fd6ef277df2906adeeed9fa391de">https://github.com/rust-lang/socket2/commit/50f31f18aac8fd6ef277df2906adeeed9fa391de</a>).</li>
<li><code>Socket::{quickack, set_quickack}</code>: sets or gets <code>TCP_QUICKACK</code>
(<a href="https://github.com/rust-lang/socket2/commit/849eee2abc5d5170d2d3bc635386a2ba13b04530">https://github.com/rust-lang/socket2/commit/849eee2abc5d5170d2d3bc635386a2ba13b04530</a>).</li>
<li><code>Socket::{thin_linear_timeouts, set_thin_linear_timeouts}</code>: sets or gets
<code>TCP_THIN_LINEAR_TIMEOUTS</code>
(<a href="https://github.com/rust-lang/socket2/commit/24c231ca463a17f51e53e7a554c7915a95bdbcc7">https://github.com/rust-lang/socket2/commit/24c231ca463a17f51e53e7a554c7915a95bdbcc7</a>).</li>
<li><code>Socket::{join_multicast_v4_n, leave_multicast_v4_n}</code>: extends the existing
multicast API by allowing an index to be used (in addition to an address)
(<a href="https://github.com/rust-lang/socket2/commit/750f83618b967c620bbfdf6ca04de7362bdb42b5">https://github.com/rust-lang/socket2/commit/750f83618b967c620bbfdf6ca04de7362bdb42b5</a>).</li>
</ul>
<h1>0.4.2</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/socket2/commit/c991f802642525dcf063c253b6fcaa5d6f4c8cb6"><code>c991f80</code></a> Release v0.3.19</li>
<li><a href="https://github.com/rust-lang/socket2/commit/1dfd15d8f3626eb91ff6238155d3bfbfaed59cf5"><code>1dfd15d</code></a> Add Socket::(bind_)device</li>
<li><a href="https://github.com/rust-lang/socket2/commit/beeebd01b8ff5c73924df09cd78bea5c47b1acd0"><code>beeebd0</code></a> Release v0.3.18</li>
<li><a href="https://github.com/rust-lang/socket2/commit/a0053b522c363a07972935cbd6cb36b6b824638b"><code>a0053b5</code></a> Backport redox compilation to 0.3</li>
<li><a href="https://github.com/rust-lang/socket2/commit/3b4214da98dd344db97f1a7d5d48da18e14d2aba"><code>3b4214d</code></a> Fix compilation on Haiku</li>
<li><a href="https://github.com/rust-lang/socket2/commit/7312f81e94c22bb90fbe1acd76b294fc5e91e6ec"><code>7312f81</code></a> Release v0.3.17</li>
<li><a href="https://github.com/rust-lang/socket2/commit/930c9a9803df565a6733f4c6b5b1b198282c7b33"><code>930c9a9</code></a> Additional Linux socket options</li>
<li><a href="https://github.com/rust-lang/socket2/commit/06a25107c7fc6797370e990d213ffb28fa4992af"><code>06a2510</code></a> [0.3] Update cfg-if to 1.0</li>
<li><a href="https://github.com/rust-lang/socket2/commit/73d54bb3366474aa011a7760b186d3d799347ca1"><code>73d54bb</code></a> Release v0.3.16</li>
<li><a href="https://github.com/rust-lang/socket2/commit/d2c15de84991947b6577bea92763efe0a2eecf28"><code>d2c15de</code></a> Don't assume memory layout of std::net::SocketAddr</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/socket2/compare/0.3.11...v0.3.19">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket2&package-manager=cargo&previous-version=0.3.11&new-version=0.3.19)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:53:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2522" class=".btn">#2522</a>
            </td>
            <td>
                <b>
                    Bump hyper from 0.12.35 to 0.12.36 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [hyper](https://github.com/hyperium/hyper) from 0.12.35 to 0.12.36.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/blob/v0.12.36/CHANGELOG.md">hyper's changelog</a>.</em></p>
<blockquote>
<h3>v0.12.36 (2021-02-17)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> allow client GET requests with explicit body headers (<a href="https://github.com/hyperium/hyper/commit/23fc8b0806e7fde435ca00479cd5e3c8c5bdeee7">23fc8b08</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/1925">#1925</a>)</li>
<li><strong>dependencies:</strong> use correct minimum versions (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/1974">#1974</a>) (<a href="https://github.com/hyperium/hyper/commit/90c1e8f44cb40d0eb1a2b36b2893e8bb5f970a96">90c1e8f4</a>)</li>
<li><strong>http1:</strong> fix server misinterpretting multiple Transfer-Encoding headers (<a href="https://github.com/hyperium/hyper/commit/f605125067562174920206e57cb589d31e2afb4b">f6051250</a>)</li>
<li><strong>server:</strong> allow <code>Server::local_addr</code> to be called with custom executor (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2009">#2009</a>) (<a href="https://github.com/hyperium/hyper/commit/da16ed62a3f478800f7a44c49acca4b109e4448b">da16ed62</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>client:</strong>
<ul>
<li>add resolve timeout to HttpConnector (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/1994">#1994</a>) (<a href="https://github.com/hyperium/hyper/commit/d4ee6996bf99eda110a067a80b5b7967fec6af48">d4ee6996</a>)</li>
<li>Add connect timeout to HttpConnector (<a href="https://github.com/hyperium/hyper/commit/3d676fb775a8291cab1491a2c7a9a7f247749e63">3d676fb7</a>)</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper/commit/4c82565f5a233b4f72ab6c745e9892d41b1bc274"><code>4c82565</code></a> v0.12.36</li>
<li><a href="https://github.com/hyperium/hyper/commit/6d9003d85bc650d5d7f548f7896cefb4e4f5c20b"><code>6d9003d</code></a> chore(lib): fix new unused variable lint</li>
<li><a href="https://github.com/hyperium/hyper/commit/f605125067562174920206e57cb589d31e2afb4b"><code>f605125</code></a> fix(http1): fix server misinterpretting multiple Transfer-Encoding headers</li>
<li><a href="https://github.com/hyperium/hyper/commit/a115c30f1c869a0027dc73157f11adf66b113dbb"><code>a115c30</code></a> chore(lib): allow deprecations in 0.12.x builds</li>
<li><a href="https://github.com/hyperium/hyper/commit/d4ee6996bf99eda110a067a80b5b7967fec6af48"><code>d4ee699</code></a> feat(client): add resolve timeout to HttpConnector (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/1994">#1994</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/da16ed62a3f478800f7a44c49acca4b109e4448b"><code>da16ed6</code></a> fix(server): allow <code>Server::local_addr</code> to be called with custom executor (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2">#2</a>...</li>
<li><a href="https://github.com/hyperium/hyper/commit/3d676fb775a8291cab1491a2c7a9a7f247749e63"><code>3d676fb</code></a> feat(client): Add connect timeout to HttpConnector</li>
<li><a href="https://github.com/hyperium/hyper/commit/90c1e8f44cb40d0eb1a2b36b2893e8bb5f970a96"><code>90c1e8f</code></a> fix(dependencies): use correct minimum versions (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/1974">#1974</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/4d188d17b36d840c624781d276c959a3ef4a1a63"><code>4d188d1</code></a> chore(ci): update MSRV to 1.31 (parking_lot uses 2018 edition)</li>
<li>See full diff in <a href="https://github.com/hyperium/hyper/compare/v0.12.35...v0.12.36">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyper&package-manager=cargo&previous-version=0.12.35&new-version=0.12.36)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:51:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2521" class=".btn">#2521</a>
            </td>
            <td>
                <b>
                    Bump hyper from 0.12.35 to 0.14.3 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [hyper](https://github.com/hyperium/hyper) from 0.12.35 to 0.14.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/releases">hyper's releases</a>.</em></p>
<blockquote>
<h2>v0.14.3</h2>
<h2>Bug Fixes</h2>
<ul>
<li>
<p><strong>client:</strong> HTTP/1 client &quot;Transfer-Encoding&quot; repair code would panic (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2410">#2410</a>) (<a href="https://github.com/hyperium/hyper/commit/2c8121f1735aa8efeb0d5e4ef595363c373ba470">2c8121f1</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2409">#2409</a>)</p>
</li>
<li>
<p><strong>http1:</strong> fix server misinterpretting multiple Transfer-Encoding headers (<a href="https://github.com/hyperium/hyper/commit/8f93123efef5c1361086688fe4f34c83c89cec02">8f93123e</a>)</p>
<p>See <a href="https://github.com/hyperium/hyper/security/advisories/GHSA-6hfq-h8hq-87mf">https://github.com/hyperium/hyper/security/advisories/GHSA-6hfq-h8hq-87mf</a></p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>body:</strong>
<ul>
<li>reexport <code>hyper::body::SizeHint</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2404">#2404</a>) (<a href="https://github.com/hyperium/hyper/commit/9956587f83428a5dbe338ba0b55c1dc0bce8c282">9956587f</a>)</li>
<li>add <code>send_trailers</code> to Body channel's <code>Sender</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2387">#2387</a>) (<a href="https://github.com/hyperium/hyper/commit/bf8d74ad1cf7d0b33b470b1e61625ebac56f9c4c">bf8d74ad</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2260">#2260</a>)</li>
</ul>
</li>
<li><strong>ffi:</strong>
<ul>
<li>add HYPERE_INVALID_PEER_MESSAGE error code for parse errors (<a href="https://github.com/hyperium/hyper/commit/1928682b33f98244435ba6d574677546205a15ec">1928682b</a>)</li>
<li>Initial unstable C API for hyper (<a href="https://github.com/hyperium/hyper/commit/3ae1581a539b67363bd87d9d8fc8635a204eec5d">3ae1581a</a>)</li>
</ul>
</li>
</ul>
<h2>v0.14.2</h2>
<h2>Features</h2>
<ul>
<li><strong>client:</strong> expose <code>connect</code> types without proto feature (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2377">#2377</a>) (<a href="https://github.com/hyperium/hyper/commit/73a59e5fc7ddedcb7cbd91e97b33385fde57aa10">73a59e5f</a>)</li>
<li><strong>server:</strong> expose <code>Accept</code> without httpX features (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2382">#2382</a>) (<a href="https://github.com/hyperium/hyper/commit/a6d4fcbee65bebf461291def75f4c512ec62a664">a6d4fcbe</a>)</li>
</ul>
<h2>v0.14.1</h2>
<ul>
<li>Fixes building documentation.</li>
</ul>
<h2>v0.14.0</h2>
<p>Blog post: <a href="https://seanmonstar.com/post/638320652536922112/hyper-v014">https://seanmonstar.com/post/638320652536922112/hyper-v014</a></p>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong> log socket option errors instead of returning error (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2361">#2361</a>) (<a href="https://github.com/hyperium/hyper/commit/dad5c8792fec7b586b41b5237bc161d8f0c09f72">dad5c879</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2359">#2359</a>)</li>
<li><strong>http1:</strong>
<ul>
<li>ignore chunked trailers (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2357">#2357</a>) (<a href="https://github.com/hyperium/hyper/commit/1dd761c87de226261599ff2518fe9d231ba1c82d">1dd761c8</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2171">#2171</a>)</li>
<li>ending close-delimited body should close (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2322">#2322</a>) (<a href="https://github.com/hyperium/hyper/commit/71f340242120f1ea52c7446b4bae37b894b83912">71f34024</a>)</li>
</ul>
</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>client:</strong>
<ul>
<li>change DNS Resolver to resolve to SocketAddrs (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2346">#2346</a>) (<a href="https://github.com/hyperium/hyper/commit/b4e24332a0cd44068a806081d51686f50c086056">b4e24332</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/1937">#1937</a>)</li>
<li>Make <code>client</code> an optional feature (<a href="https://github.com/hyperium/hyper/commit/4e55583d30a597884883f1a51b678f5c57c76765">4e55583d</a>)</li>
</ul>
</li>
<li><strong>http1:</strong> Make HTTP/1 support an optional feature (<a href="https://github.com/hyperium/hyper/commit/2a19ab74ed69bc776da25544e98979c9fb6e1834">2a19ab74</a>)</li>
<li><strong>http2:</strong> Make HTTP/2 support an optional feature (<a href="https://github.com/hyperium/hyper/commit/b819b428d314f2203642a015545967601b8e518a">b819b428</a>)</li>
<li><strong>lib:</strong>
<ul>
<li>Upgrade to Tokio 1.0, Bytes 1.0, http-body 0.4 (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2369">#2369</a>) (<a href="https://github.com/hyperium/hyper/commit/fad42acc79b54ce38adf99c58c894f29fa2665ad">fad42acc</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2370">#2370</a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/blob/master/CHANGELOG.md">hyper's changelog</a>.</em></p>
<blockquote>
<h3>v0.14.3 (2021-02-05)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> HTTP/1 client &quot;Transfer-Encoding&quot; repair code would panic (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2410">#2410</a>) (<a href="https://github.com/hyperium/hyper/commit/2c8121f1735aa8efeb0d5e4ef595363c373ba470">2c8121f1</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2409">#2409</a>)</li>
<li><strong>http1:</strong> fix server misinterpretting multiple Transfer-Encoding headers (<a href="https://github.com/hyperium/hyper/commit/8f93123efef5c1361086688fe4f34c83c89cec02">8f93123e</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>body:</strong>
<ul>
<li>reexport <code>hyper::body::SizeHint</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2404">#2404</a>) (<a href="https://github.com/hyperium/hyper/commit/9956587f83428a5dbe338ba0b55c1dc0bce8c282">9956587f</a>)</li>
<li>add <code>send_trailers</code> to Body channel's <code>Sender</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2387">#2387</a>) (<a href="https://github.com/hyperium/hyper/commit/bf8d74ad1cf7d0b33b470b1e61625ebac56f9c4c">bf8d74ad</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2260">#2260</a>)</li>
</ul>
</li>
<li><strong>ffi:</strong>
<ul>
<li>add HYPERE_INVALID_PEER_MESSAGE error code for parse errors (<a href="https://github.com/hyperium/hyper/commit/1928682b33f98244435ba6d574677546205a15ec">1928682b</a>)</li>
<li>Initial C API for hyper (<a href="https://github.com/hyperium/hyper/commit/3ae1581a539b67363bd87d9d8fc8635a204eec5d">3ae1581a</a>)</li>
</ul>
</li>
</ul>
<h3>v0.14.2 (2020-12-29)</h3>
<h4>Features</h4>
<ul>
<li><strong>client:</strong> expose <code>connect</code> types without proto feature (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2377">#2377</a>) (<a href="https://github.com/hyperium/hyper/commit/73a59e5fc7ddedcb7cbd91e97b33385fde57aa10">73a59e5f</a>)</li>
<li><strong>server:</strong> expose <code>Accept</code> without httpX features (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2382">#2382</a>) (<a href="https://github.com/hyperium/hyper/commit/a6d4fcbee65bebf461291def75f4c512ec62a664">a6d4fcbe</a>)</li>
</ul>
<h3>v0.14.1 (2020-12-23)</h3>
<ul>
<li>Fixes building documentation.</li>
</ul>
<h2>v0.14.0 (2020-12-23)</h2>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> log socket option errors instead of returning error (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2361">#2361</a>) (<a href="https://github.com/hyperium/hyper/commit/dad5c8792fec7b586b41b5237bc161d8f0c09f72">dad5c879</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2359">#2359</a>)</li>
<li><strong>http1:</strong>
<ul>
<li>ignore chunked trailers (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2357">#2357</a>) (<a href="https://github.com/hyperium/hyper/commit/1dd761c87de226261599ff2518fe9d231ba1c82d">1dd761c8</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2171">#2171</a>)</li>
<li>ending close-delimited body should close (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2322">#2322</a>) (<a href="https://github.com/hyperium/hyper/commit/71f340242120f1ea52c7446b4bae37b894b83912">71f34024</a>)</li>
</ul>
</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>client:</strong>
<ul>
<li>change DNS Resolver to resolve to SocketAddrs (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2346">#2346</a>) (<a href="https://github.com/hyperium/hyper/commit/b4e24332a0cd44068a806081d51686f50c086056">b4e24332</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/1937">#1937</a>)</li>
<li>Make <code>client</code> an optional feature (<a href="https://github.com/hyperium/hyper/commit/4e55583d30a597884883f1a51b678f5c57c76765">4e55583d</a>)</li>
</ul>
</li>
<li><strong>http1:</strong> Make HTTP/1 support an optional feature (<a href="https://github.com/hyperium/hyper/commit/2a19ab74ed69bc776da25544e98979c9fb6e1834">2a19ab74</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper/commit/48d4594930da4e227039cfa254411b85c98b63c5"><code>48d4594</code></a> v0.14.3</li>
<li><a href="https://github.com/hyperium/hyper/commit/8f93123efef5c1361086688fe4f34c83c89cec02"><code>8f93123</code></a> fix(http1): fix server misinterpretting multiple Transfer-Encoding headers</li>
<li><a href="https://github.com/hyperium/hyper/commit/4d2125c67c8087de863f74278a017c4caf37e6a9"><code>4d2125c</code></a> perf(body): specialize BufList::copy_to_bytes (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2413">#2413</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/5e8238c1b8d6351d42546a4423cf5598def1c35e"><code>5e8238c</code></a> docs(body): warn about no length check in aggregate (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2415">#2415</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/43412a950f2052e7865eb596c1d39067b2002a94"><code>43412a9</code></a> refactor(lib): Switch from pin-project to pin-project-lite</li>
<li><a href="https://github.com/hyperium/hyper/commit/9dff00425dc4463a3277cad739dba4d935364851"><code>9dff004</code></a> refactor(lib): Use cfg(all(...)) instead of multiple cfg attributes</li>
<li><a href="https://github.com/hyperium/hyper/commit/2c8121f1735aa8efeb0d5e4ef595363c373ba470"><code>2c8121f</code></a> fix(client): HTTP/1 client &quot;Transfer-Encoding&quot; repair code would panic (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2410">#2410</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/1928682b33f98244435ba6d574677546205a15ec"><code>1928682</code></a> feat(ffi): add HYPERE_INVALID_PEER_MESSAGE error code for parse errors</li>
<li><a href="https://github.com/hyperium/hyper/commit/237b2ce08341266b62a8d1cfa974779c511a0710"><code>237b2ce</code></a> refactor(lib): Remove useless uses of Pin (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2405">#2405</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/9956587f83428a5dbe338ba0b55c1dc0bce8c282"><code>9956587</code></a> feat(body): reexport <code>hyper::body::SizeHint</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2404">#2404</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/hyper/compare/v0.12.35...v0.14.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyper&package-manager=cargo&previous-version=0.12.35&new-version=0.14.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:49:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2520" class=".btn">#2520</a>
            </td>
            <td>
                <b>
                    Bump rusqlite from 0.25.3 to 0.25.4 in /libindy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [rusqlite](https://github.com/rusqlite/rusqlite) from 0.25.3 to 0.25.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rusqlite/rusqlite/commit/f4f95f8caf9fd53bffd0c19530be2484c644cc16"><code>f4f95f8</code></a> Backport fix of closure lifetime issue to v0.25.x</li>
<li>See full diff in <a href="https://github.com/rusqlite/rusqlite/compare/v0.25.3...v0.25.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rusqlite&package-manager=cargo&previous-version=0.25.3&new-version=0.25.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2519" class=".btn">#2519</a>
            </td>
            <td>
                <b>
                    Bump bumpalo from 3.2.0 to 3.10.0 in /scripts/test_zmq
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [bumpalo](https://github.com/fitzgen/bumpalo) from 3.2.0 to 3.10.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/fitzgen/bumpalo/blob/main/CHANGELOG.md">bumpalo's changelog</a>.</em></p>
<blockquote>
<h2>3.10.0</h2>
<p>Released 2022-06-01.</p>
<h3>Added</h3>
<ul>
<li>Implement <code>bumpalo::collections::FromIteratorIn</code> for <code>Option</code> and <code>Result</code>,
just like <code>core</code> does for <code>FromIterator</code>.</li>
<li>Implement <code>bumpalo::collections::FromIteratorIn</code> for <code>bumpalo::boxed::Box&lt;'a, [T]&gt;</code>.</li>
<li>Added running tests under MIRI in CI for additional confidence in unsafe code.</li>
<li>Publicly exposed <code>bumpalo::collections::Vec::drain_filter</code> since the
corresponding <code>std::vec::Vec</code> method has stabilized.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>Bump::new</code> will not allocate a backing chunk until the first allocation
inside the bump arena now.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Properly account for alignment changes when growing or shrinking an existing
allocation.</li>
<li>Removed all internal integer-to-pointer casts, to play better with UB checkers
like MIRI.</li>
</ul>
<hr />
<h2>3.9.1</h2>
<p>Released 2022-01-06.</p>
<h3>Fixed</h3>
<ul>
<li>Fixed link to logo in docs and README.md</li>
</ul>
<hr />
<h2>3.9.0</h2>
<p>Released 2022-01-05.</p>
<h3>Changed</h3>
<ul>
<li>
<p>The minimum supported Rust version (MSRV) has been raised to Rust 1.54.0.</p>
</li>
<li>
<p><code>bumpalo::collections::Vec&lt;T&gt;</code> implements relevant traits for all arrays of
any size <code>N</code> via const generics. Previously, it was just arrays up to length
32. Similar for <code>bumpalo::boxed::Box&lt;[T; N]&gt;</code>.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/fitzgen/bumpalo/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=bumpalo&package-manager=cargo&previous-version=3.2.0&new-version=3.10.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:28:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2518" class=".btn">#2518</a>
            </td>
            <td>
                <b>
                    Bump generic-array from 0.12.3 to 0.12.4 in /libnullpay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [generic-array](https://github.com/fizyk20/generic-array) from 0.12.3 to 0.12.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/fizyk20/generic-array/blob/0.12.4/CHANGELOG.md">generic-array's changelog</a>.</em></p>
<blockquote>
<ul>
<li>
<p><strong><code>0.12.4</code></strong></p>
<ul>
<li>Fix unsoundness in the <code>arr!</code> macro.</li>
</ul>
</li>
<li>
<p><strong><code>0.12.0</code></strong></p>
<ul>
<li>Allow trailing commas in <code>arr!</code> macro.</li>
<li><strong>BREAKING</strong>: Serialize <code>GenericArray</code> using <code>serde</code> tuples, instead of variable-length sequences. This may not be compatible with old serialized data.</li>
</ul>
</li>
<li>
<p><strong><code>0.11.0</code></strong></p>
<ul>
<li><strong>BREAKING</strong> Redesign <code>GenericSequence</code> with an emphasis on use in generic type parameters.</li>
<li>Add <code>MappedGenericSequence</code> and <code>FunctionalSequence</code>
<ul>
<li>Implements optimized <code>map</code>, <code>zip</code> and <code>fold</code> for <code>GenericArray</code>, <code>&amp;GenericArray</code> and <code>&amp;mut GenericArray</code></li>
</ul>
</li>
<li><strong>BREAKING</strong> Remove <code>map_ref</code>, <code>zip_ref</code> and <code>map_slice</code>
<ul>
<li><code>map_slice</code> is now equivalent to <code>GenericArray::from_iter(slice.iter().map(...))</code></li>
</ul>
</li>
</ul>
</li>
<li>
<p><strong><code>0.10.0</code></strong></p>
<ul>
<li>Add <code>GenericSequence</code>, <code>Lengthen</code>, <code>Shorten</code>, <code>Split</code> and <code>Concat</code> traits.</li>
<li>Redefine <code>transmute</code> to avert errors.</li>
</ul>
</li>
<li>
<p><strong><code>0.9.0</code></strong></p>
<ul>
<li>Rewrite construction methods to be well-defined in panic situations, correctly dropping elements.</li>
<li><code>NoDrop</code> crate replaced by <code>ManuallyDrop</code> as it became stable in Rust core.</li>
<li>Add optimized <code>map</code>/<code>map_ref</code> and <code>zip</code>/<code>zip_ref</code> methods to <code>GenericArray</code></li>
</ul>
</li>
<li>
<p><strong><code>0.8.0</code></strong></p>
<ul>
<li>Implement <code>AsRef</code>, <code>AsMut</code>, <code>Borrow</code>, <code>BorrowMut</code>, <code>Hash</code> for <code>GenericArray</code></li>
<li>Update <code>serde</code> to <code>1.0</code></li>
<li>Update <code>typenum</code></li>
<li>Make macro <code>arr!</code> non-cloning</li>
<li>Implement <code>From&lt;[T; N]&gt;</code> up to <code>N=32</code></li>
<li>Fix <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/45">#45</a></li>
</ul>
</li>
<li>
<p><strong><code>0.7.0</code></strong></p>
<ul>
<li>Upgrade <code>serde</code> to <code>0.9</code></li>
<li>Make <code>serde</code> with <code>no_std</code></li>
<li>Implement <code>PartialOrd</code>/<code>Ord</code> for <code>GenericArray</code></li>
</ul>
</li>
<li>
<p><strong><code>0.6.0</code></strong></p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/30">#30</a></li>
<li>Implement <code>Default</code> for <code>GenericArray</code></li>
<li>Implement <code>LowerHex</code> and <code>UpperHex</code> for <code>GenericArray&lt;u8, N&gt;</code></li>
<li>Use <code>precision</code> formatting field in hex representation</li>
<li>Add <code>as_slice</code>, <code>as_mut_slice</code></li>
<li>Remove <code>GenericArray::new</code> in favor of <code>Default</code> trait</li>
<li>Add <code>from_slice</code> and <code>from_mut_slice</code></li>
<li><code>no_std</code> and <code>core</code> for crate.</li>
</ul>
</li>
<li>
<p><strong><code>0.5.0</code></strong></p>
<ul>
<li>Update <code>serde</code></li>
<li>remove <code>no_std</code> feature, fixed <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/19">#19</a></li>
</ul>
</li>
<li>
<p><strong><code>0.4.0</code></strong></p>
<ul>
<li>Re-export <code>typenum</code></li>
</ul>
</li>
<li>
<p><strong><code>0.3.0</code></strong></p>
<ul>
<li>Implement <code>IntoIter</code> for <code>GenericArray</code></li>
<li>Add <code>map</code> method</li>
<li>Add optional <code>serde</code> (de)serialization support feature.</li>
</ul>
</li>
<li>
<p><strong><code>&lt; 0.3.0</code></strong></p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/fizyk20/generic-array/commit/42843cdb6c24ef3684494617e78745a62a64a29c"><code>42843cd</code></a> Bump version</li>
<li><a href="https://github.com/fizyk20/generic-array/commit/59dad415731e76d01022c9e347e67d52468fccb6"><code>59dad41</code></a> Fixed lifetime unsoundness in <code>arr</code> macro.</li>
<li>See full diff in <a href="https://github.com/fizyk20/generic-array/compare/0.12.3...0.12.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=generic-array&package-manager=cargo&previous-version=0.12.3&new-version=0.12.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:19:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2517" class=".btn">#2517</a>
            </td>
            <td>
                <b>
                    Bump generic-array from 0.12.3 to 0.12.4 in /libindy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [generic-array](https://github.com/fizyk20/generic-array) from 0.12.3 to 0.12.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/fizyk20/generic-array/blob/0.12.4/CHANGELOG.md">generic-array's changelog</a>.</em></p>
<blockquote>
<ul>
<li>
<p><strong><code>0.12.4</code></strong></p>
<ul>
<li>Fix unsoundness in the <code>arr!</code> macro.</li>
</ul>
</li>
<li>
<p><strong><code>0.12.0</code></strong></p>
<ul>
<li>Allow trailing commas in <code>arr!</code> macro.</li>
<li><strong>BREAKING</strong>: Serialize <code>GenericArray</code> using <code>serde</code> tuples, instead of variable-length sequences. This may not be compatible with old serialized data.</li>
</ul>
</li>
<li>
<p><strong><code>0.11.0</code></strong></p>
<ul>
<li><strong>BREAKING</strong> Redesign <code>GenericSequence</code> with an emphasis on use in generic type parameters.</li>
<li>Add <code>MappedGenericSequence</code> and <code>FunctionalSequence</code>
<ul>
<li>Implements optimized <code>map</code>, <code>zip</code> and <code>fold</code> for <code>GenericArray</code>, <code>&amp;GenericArray</code> and <code>&amp;mut GenericArray</code></li>
</ul>
</li>
<li><strong>BREAKING</strong> Remove <code>map_ref</code>, <code>zip_ref</code> and <code>map_slice</code>
<ul>
<li><code>map_slice</code> is now equivalent to <code>GenericArray::from_iter(slice.iter().map(...))</code></li>
</ul>
</li>
</ul>
</li>
<li>
<p><strong><code>0.10.0</code></strong></p>
<ul>
<li>Add <code>GenericSequence</code>, <code>Lengthen</code>, <code>Shorten</code>, <code>Split</code> and <code>Concat</code> traits.</li>
<li>Redefine <code>transmute</code> to avert errors.</li>
</ul>
</li>
<li>
<p><strong><code>0.9.0</code></strong></p>
<ul>
<li>Rewrite construction methods to be well-defined in panic situations, correctly dropping elements.</li>
<li><code>NoDrop</code> crate replaced by <code>ManuallyDrop</code> as it became stable in Rust core.</li>
<li>Add optimized <code>map</code>/<code>map_ref</code> and <code>zip</code>/<code>zip_ref</code> methods to <code>GenericArray</code></li>
</ul>
</li>
<li>
<p><strong><code>0.8.0</code></strong></p>
<ul>
<li>Implement <code>AsRef</code>, <code>AsMut</code>, <code>Borrow</code>, <code>BorrowMut</code>, <code>Hash</code> for <code>GenericArray</code></li>
<li>Update <code>serde</code> to <code>1.0</code></li>
<li>Update <code>typenum</code></li>
<li>Make macro <code>arr!</code> non-cloning</li>
<li>Implement <code>From&lt;[T; N]&gt;</code> up to <code>N=32</code></li>
<li>Fix <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/45">#45</a></li>
</ul>
</li>
<li>
<p><strong><code>0.7.0</code></strong></p>
<ul>
<li>Upgrade <code>serde</code> to <code>0.9</code></li>
<li>Make <code>serde</code> with <code>no_std</code></li>
<li>Implement <code>PartialOrd</code>/<code>Ord</code> for <code>GenericArray</code></li>
</ul>
</li>
<li>
<p><strong><code>0.6.0</code></strong></p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/30">#30</a></li>
<li>Implement <code>Default</code> for <code>GenericArray</code></li>
<li>Implement <code>LowerHex</code> and <code>UpperHex</code> for <code>GenericArray&lt;u8, N&gt;</code></li>
<li>Use <code>precision</code> formatting field in hex representation</li>
<li>Add <code>as_slice</code>, <code>as_mut_slice</code></li>
<li>Remove <code>GenericArray::new</code> in favor of <code>Default</code> trait</li>
<li>Add <code>from_slice</code> and <code>from_mut_slice</code></li>
<li><code>no_std</code> and <code>core</code> for crate.</li>
</ul>
</li>
<li>
<p><strong><code>0.5.0</code></strong></p>
<ul>
<li>Update <code>serde</code></li>
<li>remove <code>no_std</code> feature, fixed <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/19">#19</a></li>
</ul>
</li>
<li>
<p><strong><code>0.4.0</code></strong></p>
<ul>
<li>Re-export <code>typenum</code></li>
</ul>
</li>
<li>
<p><strong><code>0.3.0</code></strong></p>
<ul>
<li>Implement <code>IntoIter</code> for <code>GenericArray</code></li>
<li>Add <code>map</code> method</li>
<li>Add optional <code>serde</code> (de)serialization support feature.</li>
</ul>
</li>
<li>
<p><strong><code>&lt; 0.3.0</code></strong></p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/fizyk20/generic-array/commit/42843cdb6c24ef3684494617e78745a62a64a29c"><code>42843cd</code></a> Bump version</li>
<li><a href="https://github.com/fizyk20/generic-array/commit/59dad415731e76d01022c9e347e67d52468fccb6"><code>59dad41</code></a> Fixed lifetime unsoundness in <code>arr</code> macro.</li>
<li>See full diff in <a href="https://github.com/fizyk20/generic-array/compare/0.12.3...0.12.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=generic-array&package-manager=cargo&previous-version=0.12.3&new-version=0.12.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:18:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2516" class=".btn">#2516</a>
            </td>
            <td>
                <b>
                    Bump generic-array from 0.12.3 to 0.12.4 in /scripts/test_zmq
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [generic-array](https://github.com/fizyk20/generic-array) from 0.12.3 to 0.12.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/fizyk20/generic-array/blob/0.12.4/CHANGELOG.md">generic-array's changelog</a>.</em></p>
<blockquote>
<ul>
<li>
<p><strong><code>0.12.4</code></strong></p>
<ul>
<li>Fix unsoundness in the <code>arr!</code> macro.</li>
</ul>
</li>
<li>
<p><strong><code>0.12.0</code></strong></p>
<ul>
<li>Allow trailing commas in <code>arr!</code> macro.</li>
<li><strong>BREAKING</strong>: Serialize <code>GenericArray</code> using <code>serde</code> tuples, instead of variable-length sequences. This may not be compatible with old serialized data.</li>
</ul>
</li>
<li>
<p><strong><code>0.11.0</code></strong></p>
<ul>
<li><strong>BREAKING</strong> Redesign <code>GenericSequence</code> with an emphasis on use in generic type parameters.</li>
<li>Add <code>MappedGenericSequence</code> and <code>FunctionalSequence</code>
<ul>
<li>Implements optimized <code>map</code>, <code>zip</code> and <code>fold</code> for <code>GenericArray</code>, <code>&amp;GenericArray</code> and <code>&amp;mut GenericArray</code></li>
</ul>
</li>
<li><strong>BREAKING</strong> Remove <code>map_ref</code>, <code>zip_ref</code> and <code>map_slice</code>
<ul>
<li><code>map_slice</code> is now equivalent to <code>GenericArray::from_iter(slice.iter().map(...))</code></li>
</ul>
</li>
</ul>
</li>
<li>
<p><strong><code>0.10.0</code></strong></p>
<ul>
<li>Add <code>GenericSequence</code>, <code>Lengthen</code>, <code>Shorten</code>, <code>Split</code> and <code>Concat</code> traits.</li>
<li>Redefine <code>transmute</code> to avert errors.</li>
</ul>
</li>
<li>
<p><strong><code>0.9.0</code></strong></p>
<ul>
<li>Rewrite construction methods to be well-defined in panic situations, correctly dropping elements.</li>
<li><code>NoDrop</code> crate replaced by <code>ManuallyDrop</code> as it became stable in Rust core.</li>
<li>Add optimized <code>map</code>/<code>map_ref</code> and <code>zip</code>/<code>zip_ref</code> methods to <code>GenericArray</code></li>
</ul>
</li>
<li>
<p><strong><code>0.8.0</code></strong></p>
<ul>
<li>Implement <code>AsRef</code>, <code>AsMut</code>, <code>Borrow</code>, <code>BorrowMut</code>, <code>Hash</code> for <code>GenericArray</code></li>
<li>Update <code>serde</code> to <code>1.0</code></li>
<li>Update <code>typenum</code></li>
<li>Make macro <code>arr!</code> non-cloning</li>
<li>Implement <code>From&lt;[T; N]&gt;</code> up to <code>N=32</code></li>
<li>Fix <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/45">#45</a></li>
</ul>
</li>
<li>
<p><strong><code>0.7.0</code></strong></p>
<ul>
<li>Upgrade <code>serde</code> to <code>0.9</code></li>
<li>Make <code>serde</code> with <code>no_std</code></li>
<li>Implement <code>PartialOrd</code>/<code>Ord</code> for <code>GenericArray</code></li>
</ul>
</li>
<li>
<p><strong><code>0.6.0</code></strong></p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/30">#30</a></li>
<li>Implement <code>Default</code> for <code>GenericArray</code></li>
<li>Implement <code>LowerHex</code> and <code>UpperHex</code> for <code>GenericArray&lt;u8, N&gt;</code></li>
<li>Use <code>precision</code> formatting field in hex representation</li>
<li>Add <code>as_slice</code>, <code>as_mut_slice</code></li>
<li>Remove <code>GenericArray::new</code> in favor of <code>Default</code> trait</li>
<li>Add <code>from_slice</code> and <code>from_mut_slice</code></li>
<li><code>no_std</code> and <code>core</code> for crate.</li>
</ul>
</li>
<li>
<p><strong><code>0.5.0</code></strong></p>
<ul>
<li>Update <code>serde</code></li>
<li>remove <code>no_std</code> feature, fixed <a href="https://github-redirect.dependabot.com/fizyk20/generic-array/issues/19">#19</a></li>
</ul>
</li>
<li>
<p><strong><code>0.4.0</code></strong></p>
<ul>
<li>Re-export <code>typenum</code></li>
</ul>
</li>
<li>
<p><strong><code>0.3.0</code></strong></p>
<ul>
<li>Implement <code>IntoIter</code> for <code>GenericArray</code></li>
<li>Add <code>map</code> method</li>
<li>Add optional <code>serde</code> (de)serialization support feature.</li>
</ul>
</li>
<li>
<p><strong><code>&lt; 0.3.0</code></strong></p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/fizyk20/generic-array/commit/42843cdb6c24ef3684494617e78745a62a64a29c"><code>42843cd</code></a> Bump version</li>
<li><a href="https://github.com/fizyk20/generic-array/commit/59dad415731e76d01022c9e347e67d52468fccb6"><code>59dad41</code></a> Fixed lifetime unsoundness in <code>arr</code> macro.</li>
<li>See full diff in <a href="https://github.com/fizyk20/generic-array/compare/0.12.3...0.12.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=generic-array&package-manager=cargo&previous-version=0.12.3&new-version=0.12.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2515" class=".btn">#2515</a>
            </td>
            <td>
                <b>
                    Bump crossbeam-utils from 0.8.1 to 0.8.8 in /libindy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [crossbeam-utils](https://github.com/crossbeam-rs/crossbeam) from 0.8.1 to 0.8.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/crossbeam-rs/crossbeam/releases">crossbeam-utils's releases</a>.</em></p>
<blockquote>
<h2>crossbeam-utils 0.8.8</h2>
<ul>
<li>Fix a bug when unstable <code>loom</code> support is enabled. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/787">#787</a>)</li>
</ul>
<h2>crossbeam-utils 0.8.7</h2>
<ul>
<li>Add <code>AtomicCell&lt;{i*,u*}&gt;::{fetch_max,fetch_min}</code>. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/785">#785</a>)</li>
<li>Add <code>AtomicCell&lt;{i*,u*,bool}&gt;::fetch_nand</code>. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/785">#785</a>)</li>
<li>Fix unsoundness of <code>AtomicCell&lt;{i,u}64&gt;</code> arithmetics on 32-bit targets that support <code>Atomic{I,U}64</code> (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/781">#781</a>)</li>
</ul>
<h2>crossbeam-utils 0.8.6</h2>
<ul>
<li>Re-add <code>AtomicCell&lt;{i,u}64&gt;::{fetch_add,fetch_sub,fetch_and,fetch_or,fetch_xor}</code> that were accidentally removed in <del>0.8.0</del> 0.7.1 on targets that do not support <code>Atomic{I,U}64</code>. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/767">#767</a>)</li>
<li>Re-add <code>AtomicCell&lt;{i,u}128&gt;::{fetch_add,fetch_sub,fetch_and,fetch_or,fetch_xor}</code> that were accidentally removed in <del>0.8.0</del> 0.7.1. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/767">#767</a>)</li>
</ul>
<h2>crossbeam-utils 0.8.5</h2>
<ul>
<li>Add <code>AtomicCell::fetch_update</code> (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/704">#704</a>)</li>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/698">#698</a>)</li>
</ul>
<h2>crossbeam-utils 0.8.4</h2>
<ul>
<li>Bump <code>loom</code> dependency to version 0.5. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/686">#686</a>)</li>
</ul>
<h2>crossbeam-utils 0.8.3</h2>
<ul>
<li>Make <code>loom</code> dependency optional. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/666">#666</a>)</li>
</ul>
<h2>crossbeam-utils 0.8.2</h2>
<ul>
<li>Deprecate <code>AtomicCell::compare_and_swap</code>. Use <code>AtomicCell::compare_exchange</code> instead. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/619">#619</a>)</li>
<li>Add <code>Parker::park_deadline</code>. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/563">#563</a>)</li>
<li>Improve implementation of <code>CachePadded</code>. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/636">#636</a>)</li>
<li>Add unstable support for <code>loom</code>. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/487">#487</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/5b4d80835a68c47ab4b8842b3e46618c9ed7c3cb"><code>5b4d808</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/800">#800</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/6fa72466ce222ed6b4c47c1d7ce4d9cf51cdf5e1"><code>6fa7246</code></a> Prepare for the next release</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/8efcd0261c326c42a06579fa9be53d3ea32185d4"><code>8efcd02</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/798">#798</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/baedeb003eae35c5cfa9b702948b5ab29fe5b33a"><code>baedeb0</code></a> channel: Do not panic on very large timeout</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/113daf45a4a5586af87aa5db0962edda51905f9e"><code>113daf4</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/799">#799</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/5cb7cac9f230ca2449c9f6553d43af72b3cf87ec"><code>5cb7cac</code></a> Update no_atomic.rs</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/0081fcc510e602948faffbf5efa67925836f8b52"><code>0081fcc</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/789">#789</a> <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/797">#797</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/7b2d65fa21c9742c83f4a7e606418872405ad7d4"><code>7b2d65f</code></a> Update to stabilized const_fn_trait_bound</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/bd75c3c45edb78a731956c01458b75e5b69a8146"><code>bd75c3c</code></a> Add force_push to ArrayQueue</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/b11f1a83e6362589979a4c58c79895cc936b09fb"><code>b11f1a8</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/793">#793</a></li>
<li>Additional commits viewable in <a href="https://github.com/crossbeam-rs/crossbeam/compare/crossbeam-utils-0.8.1...crossbeam-utils-0.8.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=crossbeam-utils&package-manager=cargo&previous-version=0.8.1&new-version=0.8.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:03:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2514" class=".btn">#2514</a>
            </td>
            <td>
                <b>
                    Bump zeroize_derive from 1.0.0 to 1.3.2 in /scripts/test_zmq
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [zeroize_derive](https://github.com/RustCrypto/utils) from 1.0.0 to 1.3.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/RustCrypto/utils/blob/master/zeroize/CHANGELOG.md">zeroize_derive's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<p>All notable changes to this project will be documented in this file.</p>
<p>The format is based on <a href="https://keepachangelog.com/en/1.0.0/">Keep a Changelog</a>,
and this project adheres to <a href="https://semver.org/spec/v2.0.0.html">Semantic Versioning</a>.</p>
<h2>1.5.5 (2022-04-30)</h2>
<h3>Added</h3>
<ul>
<li>Impl <code>Zeroize</code> for std::ffi::CString (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/759">#759</a>)</li>
<li><code>AsRef&lt;T&gt;</code> and <code>AsMut&lt;T&gt;</code> impls for <code>Zeroizing</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/761">#761</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/759">#759</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/759">RustCrypto/utils#759</a>
<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/761">#761</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/761">RustCrypto/utils#761</a></p>
<h2>1.5.4 (2022-03-16)</h2>
<h3>Added</h3>
<ul>
<li>Nightly-only upport for zeroizing ARM64 SIMD registers (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/749">#749</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/749">#749</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/749">RustCrypto/utils#749</a></p>
<h2>1.5.3 (2022-02-25)</h2>
<h3>Fixed</h3>
<ul>
<li>Deriving <code>ZeroizeOnDrop</code> on <code>DerefMut</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/739">#739</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/739">#739</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/739">RustCrypto/utils#739</a></p>
<h2>1.5.2 (2022-01-31) [YANKED]</h2>
<h3>Fixed</h3>
<ul>
<li>Ambiguous method for <code>AssertZeroizeOnDrop</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/725">#725</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/725">#725</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/725">RustCrypto/utils#725</a></p>
<h2>1.5.1 (2022-01-27) [YANKED]</h2>
<h3>Fixed</h3>
<ul>
<li>Double <code>mut</code> on <code>AssertZeroizeOnDrop</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/719">#719</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/719">#719</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/719">RustCrypto/utils#719</a></p>
<h2>1.5.0 (2022-01-14) [YANKED]</h2>
<h3>Added</h3>
<ul>
<li><code>Zeroize</code> impls for <code>PhantomData</code>, <code>PhantomPinned</code>, and tuples with 0-10 elements (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/660">#660</a>)</li>
<li><code>#[zeroize(bound = &quot;T: MyTrait&quot;)]</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/663">#663</a>)</li>
<li><code>ZeroizeOnDrop</code> trait and custom derive (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/699">#699</a>, <a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/700">#700</a>, <a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/703">#703</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/660">#660</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/660">RustCrypto/utils#660</a>
<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/663">#663</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/663">RustCrypto/utils#663</a>
<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/699">#699</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/699">RustCrypto/utils#699</a>
<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/700">#700</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/700">RustCrypto/utils#700</a>
<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/703">#703</a>: <a href="https://github-redirect.dependabot.com/RustCrypto/utils/pull/703">RustCrypto/utils#703</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/RustCrypto/utils/commit/25167758af1fcbb8f5ee00c8d8097a50269635f5"><code>2516775</code></a> Test and fix min versions build (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/737">#737</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/d1efec578f726109042a0a66d18c81f49f13ca66"><code>d1efec5</code></a> Fix min deps versions (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/732">#732</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/c603767380b71ad013ca92c19d7e69b8014b62e0"><code>c603767</code></a> zeroize v1.5.2 (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/726">#726</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/ba4e7e732dea2c9adaf6fa4803362cd9a2b1adfe"><code>ba4e7e7</code></a> Fix ambiguous method for <code>AssertZeroizeOnDrop</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/725">#725</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/a37fa8d3f56de3bc8c217ffa15579aef322bebcc"><code>a37fa8d</code></a> zeroize v1.5.1 (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/721">#721</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/44bed6eab24fea3496f746498ee5c0f755d1e60c"><code>44bed6e</code></a> Fix double <code>mut</code> on <code>AssertZeroizeOnDrop</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/719">#719</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/73ad6a6fb26e30483580f71c98b901d27803565e"><code>73ad6a6</code></a> zeroize_derive v1.3.1 (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/716">#716</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/ca1632522a6fbcc055bbf6daebdde9eaf31df047"><code>ca16325</code></a> Remove <code>ZeroizeOnDrop</code> implementation for <code>#[zeroize(drop)]</code> (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/715">#715</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/5092abf78885af06423ad3381c84263e59c02a37"><code>5092abf</code></a> zeroize v1.5.0 (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/713">#713</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/cf0901abe343e35e8b7c70030eaa45de4f6a45f3"><code>cf0901a</code></a> zeroize_derive v1.3.0 (<a href="https://github-redirect.dependabot.com/RustCrypto/utils/issues/712">#712</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/RustCrypto/utils/compare/base64ct-v1.0.0...zeroize_derive-v1.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zeroize_derive&package-manager=cargo&previous-version=1.0.0&new-version=1.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:56:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2513" class=".btn">#2513</a>
            </td>
            <td>
                <b>
                    Bump linked-hash-map from 0.5.1 to 0.5.4 in /cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [linked-hash-map](https://github.com/contain-rs/linked-hash-map) from 0.5.1 to 0.5.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/contain-rs/linked-hash-map/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=linked-hash-map&package-manager=cargo&previous-version=0.5.1&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:52:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2512" class=".btn">#2512</a>
            </td>
            <td>
                <b>
                    Bump linked-hash-map from 0.5.2 to 0.5.4 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [linked-hash-map](https://github.com/contain-rs/linked-hash-map) from 0.5.2 to 0.5.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/contain-rs/linked-hash-map/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=linked-hash-map&package-manager=cargo&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:52:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2511" class=".btn">#2511</a>
            </td>
            <td>
                <b>
                    Bump sodiumoxide from 0.0.16 to 0.2.5 in /libindy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [sodiumoxide](https://github.com/sodiumoxide/sodiumoxide) from 0.0.16 to 0.2.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sodiumoxide/sodiumoxide/blob/master/CHANGELOG.md">sodiumoxide's changelog</a>.</em></p>
<blockquote>
<h1>0.2.5 (Oct 11, 2019)</h1>
<ul>
<li>Fix Digest PartialEq (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/381">#381</a>)</li>
<li>Fix compiler warnings (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/380">#380</a>)</li>
<li>Use copy_from_slice instead of manual loop where possible (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/378">#378</a>)</li>
</ul>
<h1>0.2.4 (Sep 3, 2019)</h1>
<ul>
<li>Fixed erronoeus dependency on older libsodium-sys</li>
<li>Fixed use of deprecated try! macro (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/369">#369</a>)</li>
</ul>
<h1>0.2.3 (Sep 1, 2019)</h1>
<ul>
<li>Allow reusing Vec for secretstream (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/357">#357</a>)</li>
<li>Replace mem::uninitialized with MaybeUninit (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/350">#350</a>, <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/356">#356</a>)</li>
<li>Fix warning about deprecated uint64_t (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/358">#358</a>)</li>
<li>Fix path to ./configure script (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/355">#355</a>)</li>
<li>Add API to derive Ed25519 public keys from secret keys (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/345">#345</a>)</li>
<li>Add DEP_SODIUM_INCLUDE &amp; DEP_SODIUM_LIB env variables (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/344">#344</a>)</li>
<li>Update libsodium to 1.0.18 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/342">#342</a>)</li>
</ul>
<h1>0.2.2 (May 16, 2019)</h1>
<ul>
<li>Bundle libsodium .a .lib for win &amp; cygwin (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/332">#332</a>)</li>
<li>Add <code>AsRef&lt;[u8]&gt;</code> for newtypes (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/323">#323</a>)</li>
<li>Implement memory locking and unlocking (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/324">#324</a>)</li>
<li>Add convenience functions for pwhash() and derive_key() (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/309">#309</a>)</li>
</ul>
<h1>0.2.1 (March 1, 2019)</h1>
<ul>
<li>Remove statik option from pkg_config usage (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/296">#296</a>)</li>
<li>Fix struct alignments that are not correctly recognized by bindgen (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/304">#304</a>)</li>
<li>Add streaming calculation of ed25519 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/237">#237</a>)</li>
<li>Update libsodium to 1.0.17 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/306">#306</a>)</li>
<li>Add support for secretstream (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/301">#301</a>)</li>
<li>Expose randombytes_uniform (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/311">#311</a>)</li>
<li>Use stable rustc to check fmt in TravisCI (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/314">#314</a>)</li>
<li>Reduce deps to build on linux from 61 -&gt; to 48 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/312">#312</a>)</li>
<li>Add instructions how to compile for armv7-unknown-linux-musleabihf (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/294">#294</a>)</li>
<li>Add use-pkg-config feature (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/315">#315</a>)</li>
</ul>
<h1>0.2.0 (December 2, 2018)</h1>
<ul>
<li>Add binding for sodium_add function (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/210">#210</a>)</li>
<li>Add bindings for crypto_generichash (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/196">#196</a>)</li>
<li>Add #[derive(Clone)] to State struct in hash_macros.rs (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/228">#228</a>)</li>
<li>Add bindings for keypair_from_seed for authenticated encryption (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/230">#230</a>)</li>
<li>Instruct OSX users to install pkg-config in README (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/243">#243</a>)</li>
<li>Mark libsodium-sys as a member of workspace (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/247">#247</a>)</li>
<li>Update README w/ Clang + Sodium version (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/248">#248</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/c85a6a225b8de81f740134c8e0fa1d018b6f4adf"><code>c85a6a2</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/383">#383</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/7ad5913a096fe00cafa9ba7bd99a76c421df7d77"><code>7ad5913</code></a> update dependency on libsodium-sys for 0.2.5 release</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/b1184d89d3d5d7413e3659fce68eea4a7386f14b"><code>b1184d8</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/382">#382</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/3d190afdb3c731a5c525a8b24c2a4b647f1c9f83"><code>3d190af</code></a> Prepare for 0.2.5 release</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/02737158ba4e487bf0cdbd4c7c2e94d234ad2fe2"><code>0273715</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/381">#381</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/fae052b834b097ced9a89a8fff8466e18f383070"><code>fae052b</code></a> Fix Digest PartialEq</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/fbfe0392ed569d8da8f17af5bbad2905e2518449"><code>fbfe039</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/380">#380</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/b59850bc4f1df0651a5b4d8a4d8d7611f9ece2c2"><code>b59850b</code></a> Fix compiler warnings</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/a2bf6681b8f7d7176c55a500e0a7b89f65774139"><code>a2bf668</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/378">#378</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/0e661b83df9817db2abe6a44cd23a9c800ab9d17"><code>0e661b8</code></a> (fmt) remove redundant newline</li>
<li>Additional commits viewable in <a href="https://github.com/sodiumoxide/sodiumoxide/compare/sodiumoxide-0.0.16...0.2.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sodiumoxide&package-manager=cargo&previous-version=0.0.16&new-version=0.2.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2510" class=".btn">#2510</a>
            </td>
            <td>
                <b>
                    Bump sodiumoxide from 0.0.16 to 0.2.5 in /experimental/plugins/postgres_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [sodiumoxide](https://github.com/sodiumoxide/sodiumoxide) from 0.0.16 to 0.2.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sodiumoxide/sodiumoxide/blob/master/CHANGELOG.md">sodiumoxide's changelog</a>.</em></p>
<blockquote>
<h1>0.2.5 (Oct 11, 2019)</h1>
<ul>
<li>Fix Digest PartialEq (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/381">#381</a>)</li>
<li>Fix compiler warnings (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/380">#380</a>)</li>
<li>Use copy_from_slice instead of manual loop where possible (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/378">#378</a>)</li>
</ul>
<h1>0.2.4 (Sep 3, 2019)</h1>
<ul>
<li>Fixed erronoeus dependency on older libsodium-sys</li>
<li>Fixed use of deprecated try! macro (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/369">#369</a>)</li>
</ul>
<h1>0.2.3 (Sep 1, 2019)</h1>
<ul>
<li>Allow reusing Vec for secretstream (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/357">#357</a>)</li>
<li>Replace mem::uninitialized with MaybeUninit (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/350">#350</a>, <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/356">#356</a>)</li>
<li>Fix warning about deprecated uint64_t (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/358">#358</a>)</li>
<li>Fix path to ./configure script (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/355">#355</a>)</li>
<li>Add API to derive Ed25519 public keys from secret keys (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/345">#345</a>)</li>
<li>Add DEP_SODIUM_INCLUDE &amp; DEP_SODIUM_LIB env variables (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/344">#344</a>)</li>
<li>Update libsodium to 1.0.18 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/342">#342</a>)</li>
</ul>
<h1>0.2.2 (May 16, 2019)</h1>
<ul>
<li>Bundle libsodium .a .lib for win &amp; cygwin (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/332">#332</a>)</li>
<li>Add <code>AsRef&lt;[u8]&gt;</code> for newtypes (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/323">#323</a>)</li>
<li>Implement memory locking and unlocking (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/324">#324</a>)</li>
<li>Add convenience functions for pwhash() and derive_key() (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/309">#309</a>)</li>
</ul>
<h1>0.2.1 (March 1, 2019)</h1>
<ul>
<li>Remove statik option from pkg_config usage (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/296">#296</a>)</li>
<li>Fix struct alignments that are not correctly recognized by bindgen (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/304">#304</a>)</li>
<li>Add streaming calculation of ed25519 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/237">#237</a>)</li>
<li>Update libsodium to 1.0.17 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/306">#306</a>)</li>
<li>Add support for secretstream (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/301">#301</a>)</li>
<li>Expose randombytes_uniform (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/311">#311</a>)</li>
<li>Use stable rustc to check fmt in TravisCI (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/314">#314</a>)</li>
<li>Reduce deps to build on linux from 61 -&gt; to 48 (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/312">#312</a>)</li>
<li>Add instructions how to compile for armv7-unknown-linux-musleabihf (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/294">#294</a>)</li>
<li>Add use-pkg-config feature (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/315">#315</a>)</li>
</ul>
<h1>0.2.0 (December 2, 2018)</h1>
<ul>
<li>Add binding for sodium_add function (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/210">#210</a>)</li>
<li>Add bindings for crypto_generichash (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/196">#196</a>)</li>
<li>Add #[derive(Clone)] to State struct in hash_macros.rs (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/228">#228</a>)</li>
<li>Add bindings for keypair_from_seed for authenticated encryption (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/230">#230</a>)</li>
<li>Instruct OSX users to install pkg-config in README (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/243">#243</a>)</li>
<li>Mark libsodium-sys as a member of workspace (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/247">#247</a>)</li>
<li>Update README w/ Clang + Sodium version (<a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/248">#248</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/c85a6a225b8de81f740134c8e0fa1d018b6f4adf"><code>c85a6a2</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/383">#383</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/7ad5913a096fe00cafa9ba7bd99a76c421df7d77"><code>7ad5913</code></a> update dependency on libsodium-sys for 0.2.5 release</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/b1184d89d3d5d7413e3659fce68eea4a7386f14b"><code>b1184d8</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/382">#382</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/3d190afdb3c731a5c525a8b24c2a4b647f1c9f83"><code>3d190af</code></a> Prepare for 0.2.5 release</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/02737158ba4e487bf0cdbd4c7c2e94d234ad2fe2"><code>0273715</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/381">#381</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/fae052b834b097ced9a89a8fff8466e18f383070"><code>fae052b</code></a> Fix Digest PartialEq</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/fbfe0392ed569d8da8f17af5bbad2905e2518449"><code>fbfe039</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/380">#380</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/b59850bc4f1df0651a5b4d8a4d8d7611f9ece2c2"><code>b59850b</code></a> Fix compiler warnings</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/a2bf6681b8f7d7176c55a500e0a7b89f65774139"><code>a2bf668</code></a> Merge <a href="https://github-redirect.dependabot.com/sodiumoxide/sodiumoxide/issues/378">#378</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/0e661b83df9817db2abe6a44cd23a9c800ab9d17"><code>0e661b8</code></a> (fmt) remove redundant newline</li>
<li>Additional commits viewable in <a href="https://github.com/sodiumoxide/sodiumoxide/compare/sodiumoxide-0.0.16...0.2.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sodiumoxide&package-manager=cargo&previous-version=0.0.16&new-version=0.2.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:49:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2509" class=".btn">#2509</a>
            </td>
            <td>
                <b>
                    Bump crossbeam-deque from 0.8.0 to 0.8.1 in /libindy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [crossbeam-deque](https://github.com/crossbeam-rs/crossbeam) from 0.8.0 to 0.8.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/crossbeam-rs/crossbeam/releases">crossbeam-deque's releases</a>.</em></p>
<blockquote>
<h2>crossbeam-deque 0.8.1</h2>
<ul>
<li>Fix deque steal race condition. (<a href="https://github.com/crossbeam-rs/crossbeam/security/advisories/GHSA-pqqp-xmhj-wgcw">https://github.com/crossbeam-rs/crossbeam/security/advisories/GHSA-pqqp-xmhj-wgcw</a>)</li>
<li>Add <code>Stealer::len</code> method. (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/708">#708</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/crossbeam-rs/crossbeam/blob/master/CHANGELOG.md">crossbeam-deque's changelog</a>.</em></p>
<blockquote>
<h1>Version 0.8.1</h1>
<ul>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/698">#698</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/0e2a930eac3586ab52498413310c45af6c67d830"><code>0e2a930</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/727">#727</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/36a606b33b158200e0b3eb49b196f2178d9ea78b"><code>36a606b</code></a> Prepare for the next release</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/3e72cde559641a3b1cf3ded0c9d9859d491a2d71"><code>3e72cde</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/726">#726</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/2653a6cfe7f8756d27f53d51cc84fcabf5d1d549"><code>2653a6c</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/722">#722</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/cb4db4cbd54427203c9358fe5b4dfb2994085461"><code>cb4db4c</code></a> clippy</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/f2cae5c64da01430e985760173442b54ae49b4e0"><code>f2cae5c</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/723">#723</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/703d73959208745197460ee8bb0337fec184272e"><code>703d739</code></a> Update list of targets that do not support Atomic*64</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/b552900e63904275837807cd09b3dd326216892b"><code>b552900</code></a> remove <code>array!</code>, use const to shorten array.</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/b1a24d31997160573028bed15aca4bb6b1454497"><code>b1a24d3</code></a> Use <code>array-macro</code> to simplify <code>AtomicCell</code> <code>LOCKS</code></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/800ca61b40fa1f014cd16d5941df5d5a45804f89"><code>800ca61</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/718">#718</a></li>
<li>Additional commits viewable in <a href="https://github.com/crossbeam-rs/crossbeam/compare/crossbeam-deque-0.8.0...crossbeam-deque-0.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=crossbeam-deque&package-manager=cargo&previous-version=0.8.0&new-version=0.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2508" class=".btn">#2508</a>
            </td>
            <td>
                <b>
                    Bump crossbeam-deque from 0.7.2 to 0.7.4 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [crossbeam-deque](https://github.com/crossbeam-rs/crossbeam) from 0.7.2 to 0.7.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/crossbeam-rs/crossbeam/blob/master/CHANGELOG.md">crossbeam-deque's changelog</a>.</em></p>
<blockquote>
<h1>Version 0.8.1</h1>
<ul>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/698">#698</a>)</li>
</ul>
<h1>Version 0.8.0</h1>
<ul>
<li>Bump the minimum supported Rust version to 1.36.</li>
<li>Bump <code>crossbeam-channel</code> to <code>0.5</code>.</li>
<li>Bump <code>crossbeam-deque</code> to <code>0.8</code>.</li>
<li>Bump <code>crossbeam-epoch</code> to <code>0.9</code>.</li>
<li>Bump <code>crossbeam-queue</code> to <code>0.3</code>.</li>
<li>Bump <code>crossbeam-utils</code> to <code>0.8</code>.</li>
</ul>
<h1>Version 0.7.3</h1>
<ul>
<li>Fix breakage with nightly feature due to <a href="https://github-redirect.dependabot.com/rust-lang/rust/issues/65214">rust-lang/rust#65214</a>.</li>
<li>Bump <code>crossbeam-channel</code> to <code>0.4</code>.</li>
<li>Bump <code>crossbeam-epoch</code> to <code>0.8</code>.</li>
<li>Bump <code>crossbeam-queue</code> to <code>0.2</code>.</li>
<li>Bump <code>crossbeam-utils</code> to <code>0.7</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/048513769238eda1876bcc61b131b2ece32f87dd"><code>0485137</code></a> Prepare for the next release</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/180b462b021ea02af4209da385f3c037508c64fc"><code>180b462</code></a> Fix deque steal race condition</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/48b13dc43cf19e0544d03d16f4b3da3d8b23f076"><code>48b13dc</code></a> Bump crossbeam-channel to v0.4.4</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/679dac8e1cef3b0c05d8ac7b9c33aa52a9f193e3"><code>679dac8</code></a> Bump crossbeam-channel to v0.4.3</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/f652c6adc96353b9ad530d3271345562296b6eb1"><code>f652c6a</code></a> Change crossbeam-channel's license to MIT OR Apache-2.0.</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/149a3c93895538080fb4cc2884def30111059ffc"><code>149a3c9</code></a> Release crossbeam-queue 0.2.3</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/18363b5b3e063a940db92c54fdb6f4a0538413f4"><code>18363b5</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/476">#476</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/e32c891f376332828852fa2eb5626a831b395e28"><code>e32c891</code></a> Release new versions</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/6d6591a0e1c4d1d540d7289d27c21ec7f1689aa6"><code>6d6591a</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/474">#474</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/528c3caadb2f4f5f0d0327de35404ad077636345"><code>528c3ca</code></a> Undo bump of rand as it bumps MSRV</li>
<li>Additional commits viewable in <a href="https://github.com/crossbeam-rs/crossbeam/compare/crossbeam-deque-0.7.2...crossbeam-deque-0.7.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=crossbeam-deque&package-manager=cargo&previous-version=0.7.2&new-version=0.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2507" class=".btn">#2507</a>
            </td>
            <td>
                <b>
                    Bump crossbeam-deque from 0.7.3 to 0.7.4 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [crossbeam-deque](https://github.com/crossbeam-rs/crossbeam) from 0.7.3 to 0.7.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/crossbeam-rs/crossbeam/blob/master/CHANGELOG.md">crossbeam-deque's changelog</a>.</em></p>
<blockquote>
<h1>Version 0.8.1</h1>
<ul>
<li>Support targets that do not have atomic CAS on stable Rust (<a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/698">#698</a>)</li>
</ul>
<h1>Version 0.8.0</h1>
<ul>
<li>Bump the minimum supported Rust version to 1.36.</li>
<li>Bump <code>crossbeam-channel</code> to <code>0.5</code>.</li>
<li>Bump <code>crossbeam-deque</code> to <code>0.8</code>.</li>
<li>Bump <code>crossbeam-epoch</code> to <code>0.9</code>.</li>
<li>Bump <code>crossbeam-queue</code> to <code>0.3</code>.</li>
<li>Bump <code>crossbeam-utils</code> to <code>0.8</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/048513769238eda1876bcc61b131b2ece32f87dd"><code>0485137</code></a> Prepare for the next release</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/180b462b021ea02af4209da385f3c037508c64fc"><code>180b462</code></a> Fix deque steal race condition</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/48b13dc43cf19e0544d03d16f4b3da3d8b23f076"><code>48b13dc</code></a> Bump crossbeam-channel to v0.4.4</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/679dac8e1cef3b0c05d8ac7b9c33aa52a9f193e3"><code>679dac8</code></a> Bump crossbeam-channel to v0.4.3</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/f652c6adc96353b9ad530d3271345562296b6eb1"><code>f652c6a</code></a> Change crossbeam-channel's license to MIT OR Apache-2.0.</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/149a3c93895538080fb4cc2884def30111059ffc"><code>149a3c9</code></a> Release crossbeam-queue 0.2.3</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/18363b5b3e063a940db92c54fdb6f4a0538413f4"><code>18363b5</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/476">#476</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/e32c891f376332828852fa2eb5626a831b395e28"><code>e32c891</code></a> Release new versions</li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/6d6591a0e1c4d1d540d7289d27c21ec7f1689aa6"><code>6d6591a</code></a> Merge <a href="https://github-redirect.dependabot.com/crossbeam-rs/crossbeam/issues/474">#474</a></li>
<li><a href="https://github.com/crossbeam-rs/crossbeam/commit/528c3caadb2f4f5f0d0327de35404ad077636345"><code>528c3ca</code></a> Undo bump of rand as it bumps MSRV</li>
<li>Additional commits viewable in <a href="https://github.com/crossbeam-rs/crossbeam/compare/crossbeam-0.7.3...crossbeam-deque-0.7.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=crossbeam-deque&package-manager=cargo&previous-version=0.7.3&new-version=0.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 18:24:15 +0000 UTC
    </div>
</div>

