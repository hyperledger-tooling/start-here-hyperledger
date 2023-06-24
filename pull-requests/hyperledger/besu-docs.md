---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1349" class=".btn">#1349</a>
            </td>
            <td>
                <b>
                    Update versioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update versioning to make the [release process](https://wiki.hyperledger.org/display/BESU/Documentation+release+process) simpler.

Rename the `stable` version to the version number, so creating new versions doesn't require renaming the previous version. Keep the `stable` label and path for user-friendliness and so footer links and external links to the docs don't need to be changed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 20:30:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    Update index.md, fix display code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the snip code display

<img width="513" alt="Screenshot 2023-06-23 at 14 00 23" src="https://github.com/hyperledger/besu-docs/assets/17565440/69ccd916-df69-415c-bf57-cef42bdffe55">

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 06:59:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1343" class=".btn">#1343</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.1.15 to 9.1.16 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.1.15 to 9.1.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.1.16</h2>
<ul>
<li>Updated Indonesian translations</li>
<li>Ensure scroll bar follows color scheme of operating system</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.1.16+insiders-4.36.0 (2023-07-15)</p>
<ul>
<li>Added support for instant prefetching to speed up slow connections</li>
<li>Improved stability of anchor link removal in built-in typeset plugin</li>
<li>Improved performance of regular expressions in typeset plugin</li>
<li>Removed unnecessary import test for cairosvg in optimize plugin</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5590">#5590</a>: regular expression for anchor link removal too greedy</li>
</ul>
<p>mkdocs-material-9.1.16 (2023-07-15)</p>
<ul>
<li>Updated Indonesian translations</li>
<li>Ensure scroll bar follows color scheme of operating system</li>
</ul>
<p>mkdocs-material-9.1.15+insiders-4.35.3 (2023-06-01)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5579">#5579</a>: Abbreviations in headlines filtered by typeset plugin</li>
</ul>
<p>mkdocs-material-9.1.15+insiders-4.35.2 (2023-05-29)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5555">#5555</a>: Blog plugin crashes when computing readtime for emojis</li>
</ul>
<p>mkdocs-material-9.1.15 (2023-05-29)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5566">#5566</a>: Indicate color scheme to operating system</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5565">#5565</a>: Update Dockerfile to latest version of base image</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5554">#5554</a>: Add additional version tags (9, 9.1) to Docker image</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5536">#5536</a>: Strip tags of ARIA labels in table of contents</li>
</ul>
<p>mkdocs-material-9.1.14+insiders-4.35.1 (2023-05-20)</p>
<ul>
<li>Fixed internal handling of errors in social plugin</li>
</ul>
<p>mkdocs-material-9.1.14+insiders-4.35.0 (2023-05-20)</p>
<ul>
<li>Improve editing experience and stability of social plugin</li>
<li>Added support for custom layout syntax validation in social plugin</li>
<li>Added support for layer origin for easier placement in social plugin</li>
<li>Added support for in- and exclusion patterns in social plugin</li>
<li>Catch and print syntax errors in custom layouts</li>
</ul>
<p>mkdocs-material-9.1.14 (2023-05-20)</p>
<ul>
<li>Updated Armenian and Greek translations</li>
</ul>
<p>mkdocs-material-9.1.13+insiders-4.34.1 (2023-05-16)</p>
<ul>
<li>Disable social plugin debug mode by default on mkdocs build</li>
<li>Added warning in social plugin debug mode when font style couldn't be found</li>
<li>Set default concurrency of built-in multi-threaded plugins to CPUs - 1</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5521">#5521</a>: Social plugin triggers race condition when downloading fonts</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/bf28923c4318eb8180fd862229d494adad6794b1"><code>bf28923</code></a> Prepare 9.1.16 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/e18fd7cce035c61dfd919323747d4dc2809ee621"><code>e18fd7c</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0c45c6fd70a4c17a4647135384ca13e6d4b5efb5"><code>0c45c6f</code></a> Updated Premium sponsors</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/1c22ca42f25544f45e9dddac09266de0ee87f0a8"><code>1c22ca4</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/118904c216e0f074a5f285e4747b787292949490"><code>118904c</code></a> Updated Indonesian translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/d2f403495cba3610f3f4cb6767a9eb4ea24e8333"><code>d2f4034</code></a> Ensure color-scheme meta tag is set</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/1bbc7822d6973b718926b06ef136c3e6d26a7207"><code>1bbc782</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/9153aebe4405a97b23be50fe7c91f7919a60deb0"><code>9153aeb</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/7fa991c51be4efa1259555f3e12d95927234f186"><code>7fa991c</code></a> Updated Insiders changelog</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/530f84416e50e517991b6f1cd44ce8192421bce0"><code>530f844</code></a> Added support for using .mjs files in extra_javascript</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.1.15...9.1.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.1.15&new-version=9.1.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 23:58:56 +0000 UTC
    </div>
</div>

