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
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2531" class=".btn">#2531</a>
            </td>
            <td>
                <b>
                    Bump ordered-float from 1.0.1 to 1.1.1 in /cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [ordered-float](https://github.com/reem/rust-ordered-float) from 1.0.1 to 1.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/reem/rust-ordered-float/releases">ordered-float's releases</a>.</em></p>
<blockquote>
<h2>v1.1.1</h2>
<ul>
<li>Make assignment operators panic safe (<a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/71">#71</a>). This fixes a bug that could cause undefined behavior in safe code.</li>
</ul>
<h2>v1.1.0</h2>
<ul>
<li>Implement Sum and Product traits for NotNan (<a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/65">#65</a>).</li>
<li>Implement Neg and Zero traits for OrderedFloat (<a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/60">#60</a>, <a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/66">#66</a>).</li>
<li>Implement Add, Sub, Mul, and Div traits for OrderedFloat.</li>
</ul>
<h2>v1.0.2</h2>
<ul>
<li>Implement <code>FromStr</code> (<a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/53">#53</a>)</li>
<li>Internal refactoring (<a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/55">#55</a>)</li>
<li>Fix for <code>no_std</code> builds (<a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/59">#59</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/reem/rust-ordered-float/commit/ebbbb4711e9d20954136bedc4f4a74e89bb455ae"><code>ebbbb47</code></a> Version 1.1.1</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/da4a8dd49300740a434c095a9c4b408d2415cc08"><code>da4a8dd</code></a> Make assignment operators panic safe</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/96672a8af0782f1b85e7b5e36272cd8aa107303f"><code>96672a8</code></a> Version 1.1.0</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/70848787afb5b4983c3e6cc3e2e4b09ca66d3a25"><code>7084878</code></a> impl Add/Sub/Mul/Div for OrderedFloat</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/57e16fdd5d39d9a54bb84257792cfc1be9b1fd26"><code>57e16fd</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/66">#66</a> from Uriopass/patch-1</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/9a241dc1d72f9d716829fa8a46786fc301afa6a9"><code>9a241dc</code></a> Add Zero impl for OrderedFloat</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/90f4ca8d63b6271c9594260a92ddf588af94c862"><code>90f4ca8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/65">#65</a> from bennofs/master</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/eae40333bd122dc5d74566f142f3351e1e618ffc"><code>eae4033</code></a> Add Sum/Product impls for NotNan</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/06afbc94f6390a0d31f2e395546f49dd75b6f1bd"><code>06afbc9</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/reem/rust-ordered-float/issues/60">#60</a> from wookietreiber/topic/neg</li>
<li><a href="https://github.com/reem/rust-ordered-float/commit/9013e4c202c9f424df70d1dc2b0e0bae1424d2a3"><code>9013e4c</code></a> adds neg for ordered float</li>
<li>Additional commits viewable in <a href="https://github.com/reem/rust-ordered-float/compare/v1.0.1...v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ordered-float&package-manager=cargo&previous-version=1.0.1&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-08 22:34:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2530" class=".btn">#2530</a>
            </td>
            <td>
                <b>
                    Bump miow from 0.2.1 to 0.2.2 in /vcx/libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [miow](https://github.com/yoshuawuyts/miow) from 0.2.1 to 0.2.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/yoshuawuyts/miow/commit/6fd7b9cfb5f5998dc6772803354b05815e579bb8"><code>6fd7b9c</code></a> Bump version to 0.2.2</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/550efc2e9608b72e971d659a01f2d02a3a27e1bc"><code>550efc2</code></a> Merge branch 'fix-sockaddr-convertion-v0.2.x' into 0.2.x</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/ca8db5365495d6da42b2f26f2062fb5e12b6c329"><code>ca8db53</code></a> Stop using from_ne_bytes to be compatible with Rust &lt; 1.32.0</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/3e217e34994923c4ef99aa3209aa9448b9e8b798"><code>3e217e3</code></a> Bump net2 dep to 0.2.36 without invalid SocketAddr convertion</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/27b77cc870b922d305015841978b581ceb18e3b9"><code>27b77cc</code></a> Adapt to winapi 0.2</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/2783715269d56a0020160179c0f2ba883d12d874"><code>2783715</code></a> Safely convert SocketAddr into raw SOCKADDR</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/f6662ef11d1aac309aea5a6548c1a2d35c1de6e9"><code>f6662ef</code></a> Clarify wording of license information in README.</li>
<li>See full diff in <a href="https://github.com/yoshuawuyts/miow/compare/0.2.1...0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=miow&package-manager=cargo&previous-version=0.2.1&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-08 21:00:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2529" class=".btn">#2529</a>
            </td>
            <td>
                <b>
                    Bump miow from 0.2.1 to 0.2.2 in /vcx/dummy-cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [miow](https://github.com/yoshuawuyts/miow) from 0.2.1 to 0.2.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/yoshuawuyts/miow/commit/6fd7b9cfb5f5998dc6772803354b05815e579bb8"><code>6fd7b9c</code></a> Bump version to 0.2.2</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/550efc2e9608b72e971d659a01f2d02a3a27e1bc"><code>550efc2</code></a> Merge branch 'fix-sockaddr-convertion-v0.2.x' into 0.2.x</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/ca8db5365495d6da42b2f26f2062fb5e12b6c329"><code>ca8db53</code></a> Stop using from_ne_bytes to be compatible with Rust &lt; 1.32.0</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/3e217e34994923c4ef99aa3209aa9448b9e8b798"><code>3e217e3</code></a> Bump net2 dep to 0.2.36 without invalid SocketAddr convertion</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/27b77cc870b922d305015841978b581ceb18e3b9"><code>27b77cc</code></a> Adapt to winapi 0.2</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/2783715269d56a0020160179c0f2ba883d12d874"><code>2783715</code></a> Safely convert SocketAddr into raw SOCKADDR</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/f6662ef11d1aac309aea5a6548c1a2d35c1de6e9"><code>f6662ef</code></a> Clarify wording of license information in README.</li>
<li>See full diff in <a href="https://github.com/yoshuawuyts/miow/compare/0.2.1...0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=miow&package-manager=cargo&previous-version=0.2.1&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-08 21:00:00 +0000 UTC
    </div>
</div>

