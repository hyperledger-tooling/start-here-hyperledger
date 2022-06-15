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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Bump miow from 0.2.1 to 0.2.2 in /core/relay
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 21:12:18 +0000 UTC
    </div>
</div>

