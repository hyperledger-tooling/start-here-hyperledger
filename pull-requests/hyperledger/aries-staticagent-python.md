---
layout: default
title: aries-staticagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-staticagent-python
---

# aries-staticagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-staticagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Bump addressable from 2.7.0 to 2.8.0 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [addressable](https://github.com/sporkmonger/addressable) from 2.7.0 to 2.8.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sporkmonger/addressable/blob/main/CHANGELOG.md">addressable's changelog</a>.</em></p>
<blockquote>
<h1>Addressable 2.8.0</h1>
<ul>
<li>fixes ReDoS vulnerability in Addressable::Template#match</li>
<li>no longer replaces <code>+</code> with spaces in queries for non-http(s) schemes</li>
<li>fixed encoding ipv6 literals</li>
<li>the <code>:compacted</code> flag for <code>normalized_query</code> now dedupes parameters</li>
<li>fix broken <code>escape_component</code> alias</li>
<li>dropping support for Ruby 2.0 and 2.1</li>
<li>adding Ruby 3.0 compatibility for development tasks</li>
<li>drop support for <code>rack-mount</code> and remove Addressable::Template#generate</li>
<li>performance improvements</li>
<li>switch CI/CD to GitHub Actions</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sporkmonger/addressable/commit/6469a232c0f1892809ff66737370c765d574e16c"><code>6469a23</code></a> Updating gemspec again</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/24336385de0261571b3adaad0431459edb420c79"><code>2433638</code></a> Merge branch 'main' of github.com:sporkmonger/addressable into main</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/e9c76b889789c75d7073c17b0ab557635d3f6704"><code>e9c76b8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sporkmonger/addressable/issues/378">#378</a> from ashmaroli/flat-map</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/56c5cf7ece9223ff4240e07078cc26d3adbbbd30"><code>56c5cf7</code></a> Update the gemspec</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/c1fed1ca0a44c448e74d761fd44ed94869199807"><code>c1fed1c</code></a> Require a non-vulnerable rake</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/0d8a3127e35886ce9284810a7f2438bff6b43cbc"><code>0d8a312</code></a> Adding note about ReDoS vulnerability</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/89c76130ce255c601f642a018cb5fb5a80e679a7"><code>89c7613</code></a> Merge branch 'template-regexp' into main</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/cf8884f815c96b646c796f707bf768cf6eb65543"><code>cf8884f</code></a> Note about alias fix</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/bb03f7112e8e478240a0f96e1cc7428159b41586"><code>bb03f71</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/sporkmonger/addressable/issues/371">#371</a> from charleystran/add_missing_encode_component_doc_entry</li>
<li><a href="https://github.com/sporkmonger/addressable/commit/6d1d8094a66cbf932ecf69db6850bc9edaf86de0"><code>6d1d809</code></a> Adding note about :compacted normalization</li>
<li>Additional commits viewable in <a href="https://github.com/sporkmonger/addressable/compare/addressable-2.7.0...addressable-2.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=addressable&package-manager=bundler&previous-version=2.7.0&new-version=2.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-staticagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 06:52:36 +0000 UTC
    </div>
</div>

