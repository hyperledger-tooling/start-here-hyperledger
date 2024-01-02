---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump tj-actions/changed-files from 40 to 41 in /.github/workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [tj-actions/changed-files](https://github.com/tj-actions/changed-files) from 40 to 41.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tj-actions/changed-files/releases">tj-actions/changed-files's releases</a>.</em></p>
<blockquote>
<h2>v41</h2>
<h1>Changes in v41.0.1</h1>
<h2>What's Changed</h2>
<ul>
<li>Upgraded to v41 by <a href="https://github.com/tj-actions-bot"><code>@​tj-actions-bot</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1811">tj-actions/changed-files#1811</a></li>
<li>chore(deps): update dependency eslint-plugin-prettier to v5.1.2 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1813">tj-actions/changed-files#1813</a></li>
<li>fix: update characters escaped by safe output by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1815">tj-actions/changed-files#1815</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/tj-actions/changed-files/compare/v41...v41.0.1">https://github.com/tj-actions/changed-files/compare/v41...v41.0.1</a></p>
<hr />
<h1>Changes in v41.0.0</h1>
<h2>🔥 🔥 BREAKING CHANGE 🔥 🔥</h2>
<p>A new <code>safe_output</code> input is now available to prevent outputting unsafe filename characters (Enabled by default). This would escape characters in the filename that could be used for command injection.</p>
<blockquote>
<p>[!NOTE]
This can be disabled by setting the <code>safe_output</code> to false this comes with a recommendation to store all outputs generated in an environment variable first before using them.</p>
</blockquote>
<h4>Example</h4>
<pre lang="yaml"><code>...
    - name: Get changed files
      id: changed-files
      uses: tj-actions/changed-files@v40
      with:
        safe_output: false # set to false because we are using an environment variable to store the output and avoid command injection.
<pre><code>- name: List all added files
  env:
    ADDED_FILES: ${{ steps.changed-files.outputs.added_files }}
  run: |
    for file in &amp;quot;$ADDED_FILES&amp;quot;; do
      echo &amp;quot;$file was added&amp;quot;
    done
</code></pre>
<p>...
</code></pre></p>
<h2>What's Changed</h2>
<ul>
<li>chore(deps): update typescript-eslint monorepo to v6.15.0 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1801">tj-actions/changed-files#1801</a></li>
<li>Upgraded to v40.2.3 by <a href="https://github.com/tj-actions-bot"><code>@​tj-actions-bot</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1800">tj-actions/changed-files#1800</a></li>
<li>chore(deps): update dependency eslint-plugin-prettier to v5.1.0 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1802">tj-actions/changed-files#1802</a></li>
<li>chore(deps): lock file maintenance by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1803">tj-actions/changed-files#1803</a></li>
<li>chore(deps): update dependency eslint-plugin-prettier to v5.1.1 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1804">tj-actions/changed-files#1804</a></li>
<li>fix: update safe output regex and the docs by <a href="https://github.com/tj-actions-bot"><code>@​tj-actions-bot</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1805">tj-actions/changed-files#1805</a></li>
<li>Revert &quot;chore(deps): update actions/download-artifact action to v4&quot; by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1806">tj-actions/changed-files#1806</a></li>
<li>Update README.md by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1808">tj-actions/changed-files#1808</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tj-actions/changed-files/blob/main/HISTORY.md">tj-actions/changed-files's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h1><a href="https://github.com/tj-actions/changed-files/compare/v41.0.0...v41.0.1">41.0.1</a> - (2023-12-24)</h1>
<h2><!-- raw HTML omitted -->🐛 Bug Fixes</h2>
<ul>
<li>Update characters escaped by safe output (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1815">#1815</a>) (<a href="https://github.com/tj-actions/changed-files/commit/716b1e13042866565e00e85fd4ec490e186c4a2f">716b1e1</a>)  - (Tonye Jack)</li>
</ul>
<h2><!-- raw HTML omitted -->⚙️ Miscellaneous Tasks</h2>
<ul>
<li><strong>deps:</strong> Update dependency eslint-plugin-prettier to v5.1.2 (<a href="https://github.com/tj-actions/changed-files/commit/7aaf10d9eef19e8a2432a967b88124171152caaf">7aaf10d</a>)  - (renovate[bot])</li>
</ul>
<h2><!-- raw HTML omitted -->⬆️ Upgrades</h2>
<ul>
<li>Upgraded to v41 (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1811">#1811</a>)</li>
</ul>
<p>Co-authored-by: jackton1 <a href="mailto:jackton1@users.noreply.github.com">jackton1@users.noreply.github.com</a> (<a href="https://github.com/tj-actions/changed-files/commit/cc08e170f4447237bcaf8acaacfa615b9cb86612">cc08e17</a>)  - (tj-actions[bot])</p>
<h1><a href="https://github.com/tj-actions/changed-files/compare/v40.2.3...v41.0.0">41.0.0</a> - (2023-12-23)</h1>
<h2><!-- raw HTML omitted -->🐛 Bug Fixes</h2>
<ul>
<li>Update safe output regex and the docs (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1805">#1805</a>) (<a href="https://github.com/tj-actions/changed-files/commit/ff2f6e6b91913a7be42be1b5917330fe442f2ede">ff2f6e6</a>)  - (tj-actions[bot])</li>
</ul>
<h2><!-- raw HTML omitted -->⏪ Reverts</h2>
<ul>
<li>Revert &quot;chore(deps): update actions/download-artifact action to v4&quot; (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1806">#1806</a>)</li>
</ul>
<p>(<a href="https://github.com/tj-actions/changed-files/commit/4f573fed06c9abb5da4c72f75c1c320718114ff7">4f573fe</a>)  - (Tonye Jack)</p>
<h2><!-- raw HTML omitted -->🔄 Update</h2>
<ul>
<li>Update README.md (<a href="https://github.com/tj-actions/changed-files/commit/6e79d6e3dbe48946636c2939c80ff5c84ff7f9fe">6e79d6e</a>)  - (Tonye Jack)</li>
<li>Update README.md (<a href="https://github.com/tj-actions/changed-files/commit/d13ac1942fb3c1d7d32017915bb082cebe8a272a">d13ac19</a>)  - (Tonye Jack)</li>
<li>Update README.md (<a href="https://github.com/tj-actions/changed-files/commit/bb89f97963be96b39e1a303e64d5b91a1af4c340">bb89f97</a>)  - (Tonye Jack)</li>
<li>Updated README.md (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1810">#1810</a>)</li>
</ul>
<p>Co-authored-by: renovate[bot] <!-- raw HTML omitted --> (<a href="https://github.com/tj-actions/changed-files/commit/1864078d0afadf68ba489e671ecc09fefe8b70ab">1864078</a>)  - (tj-actions[bot])</p>
<ul>
<li>Update README.md (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1808">#1808</a>)</li>
</ul>
<p>(<a href="https://github.com/tj-actions/changed-files/commit/47371c50e97c089212d9eb92ca26c8453224e78e">47371c5</a>)  - (Tonye Jack)</p>
<h2><!-- raw HTML omitted -->📝 Other</h2>
<ul>
<li>Merge pull request from GHSA-mcph-m25j-8j63</li>
</ul>
<ul>
<li>
<p>feat: add <code>safe_output</code> input enabled by default</p>
</li>
<li>
<p>fix: migrate README to safe uses of interpolation</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tj-actions/changed-files/commit/716b1e13042866565e00e85fd4ec490e186c4a2f"><code>716b1e1</code></a> fix: update characters escaped by safe output (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1815">#1815</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/7aaf10d9eef19e8a2432a967b88124171152caaf"><code>7aaf10d</code></a> chore(deps): update dependency eslint-plugin-prettier to v5.1.2</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/cc08e170f4447237bcaf8acaacfa615b9cb86612"><code>cc08e17</code></a> Upgraded to v41 (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1811">#1811</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/6e79d6e3dbe48946636c2939c80ff5c84ff7f9fe"><code>6e79d6e</code></a> Update README.md</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/d13ac1942fb3c1d7d32017915bb082cebe8a272a"><code>d13ac19</code></a> Update README.md</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/bb89f97963be96b39e1a303e64d5b91a1af4c340"><code>bb89f97</code></a> Update README.md</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/1864078d0afadf68ba489e671ecc09fefe8b70ab"><code>1864078</code></a> Updated README.md (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1810">#1810</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/f495a0321d3fffa62da2573adf70b77d5eb2f57a"><code>f495a03</code></a> chore(deps): lock file maintenance</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/47371c50e97c089212d9eb92ca26c8453224e78e"><code>47371c5</code></a> Update README.md (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1808">#1808</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/4f573fed06c9abb5da4c72f75c1c320718114ff7"><code>4f573fe</code></a> Revert &quot;chore(deps): update actions/download-artifact action to v4&quot; (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1806">#1806</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tj-actions/changed-files/compare/v40...v41">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tj-actions/changed-files&package-manager=github_actions&previous-version=40&new-version=41)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-02 16:53:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    Update repo manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the script to handle spaces, comments and extra sections. Made small adjustment to oid4vci libraries. Upgraded askar to ~3.0 globally.

Ran the script to update dependencies.

Removed the common development files part of the script. I thought they would be the same for every plugin but I'm already seeing them be customized in @Jsyro latest PR.

Also changed the script to loop over sections. Made it smaller and easier to maintain. Still a bit over work could be done to use the same code for the main vs integration test sections. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-30 00:45:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.0 to 1.5.1 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.0 to 1.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.1 - Security Release</h2>
<p>This is a minor security release to fix a potential DoS for applications that allow the use of symmetric keys with pbkdf2.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix X22519 import/export from PEM by <a href="https://github.com/achamayou"><code>@​achamayou</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li>Read the Docs now requires a config file by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/335">latchset/jwcrypto#335</a></li>
<li>chore: refactor for removing pdb symbols by <a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
<li>Fix potential DoS issue with p2c header by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/336">latchset/jwcrypto#336</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/achamayou"><code>@​achamayou</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li><a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/8ae0df6538b8d8aa52e82105ec5132d289ad9ddd"><code>8ae0df6</code></a> Version 1.5.1</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/066d13f2dbac3c0be7aa2a3023189980d56b86ab"><code>066d13f</code></a> Update Security Policy</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d2655d370586cb830e49acfb450f87598da60be8"><code>d2655d3</code></a> Fix potential DoS issue with p2c header</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/6ee0e8915a22f2aed5346ec8a0116ce1cc64349a"><code>6ee0e89</code></a> chore: arg renamed</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d64536b102049c6b08bd8ce155a6bf578c653bfa"><code>d64536b</code></a> chore: refactor for removing pdb symbols</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/ac40895d57422ec4e93cd7c53d430b532448687d"><code>ac40895</code></a> Read the Docs now requires a config file</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/4c900198a25bbe0c71a9d3a09c8c378920f40887"><code>4c90019</code></a> Fix X25519 import/export from PEM</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.0&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-28 16:49:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.0 to 1.5.1 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.0 to 1.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.1 - Security Release</h2>
<p>This is a minor security release to fix a potential DoS for applications that allow the use of symmetric keys with pbkdf2.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix X22519 import/export from PEM by <a href="https://github.com/achamayou"><code>@​achamayou</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li>Read the Docs now requires a config file by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/335">latchset/jwcrypto#335</a></li>
<li>chore: refactor for removing pdb symbols by <a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
<li>Fix potential DoS issue with p2c header by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/336">latchset/jwcrypto#336</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/achamayou"><code>@​achamayou</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li><a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/8ae0df6538b8d8aa52e82105ec5132d289ad9ddd"><code>8ae0df6</code></a> Version 1.5.1</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/066d13f2dbac3c0be7aa2a3023189980d56b86ab"><code>066d13f</code></a> Update Security Policy</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d2655d370586cb830e49acfb450f87598da60be8"><code>d2655d3</code></a> Fix potential DoS issue with p2c header</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/6ee0e8915a22f2aed5346ec8a0116ce1cc64349a"><code>6ee0e89</code></a> chore: arg renamed</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d64536b102049c6b08bd8ce155a6bf578c653bfa"><code>d64536b</code></a> chore: refactor for removing pdb symbols</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/ac40895d57422ec4e93cd7c53d430b532448687d"><code>ac40895</code></a> Read the Docs now requires a config file</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/4c900198a25bbe0c71a9d3a09c8c378920f40887"><code>4c90019</code></a> Fix X25519 import/export from PEM</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.0&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-28 16:49:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.0 to 1.5.1 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.0 to 1.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.1 - Security Release</h2>
<p>This is a minor security release to fix a potential DoS for applications that allow the use of symmetric keys with pbkdf2.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix X22519 import/export from PEM by <a href="https://github.com/achamayou"><code>@​achamayou</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li>Read the Docs now requires a config file by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/335">latchset/jwcrypto#335</a></li>
<li>chore: refactor for removing pdb symbols by <a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
<li>Fix potential DoS issue with p2c header by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/336">latchset/jwcrypto#336</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/achamayou"><code>@​achamayou</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li><a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/8ae0df6538b8d8aa52e82105ec5132d289ad9ddd"><code>8ae0df6</code></a> Version 1.5.1</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/066d13f2dbac3c0be7aa2a3023189980d56b86ab"><code>066d13f</code></a> Update Security Policy</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d2655d370586cb830e49acfb450f87598da60be8"><code>d2655d3</code></a> Fix potential DoS issue with p2c header</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/6ee0e8915a22f2aed5346ec8a0116ce1cc64349a"><code>6ee0e89</code></a> chore: arg renamed</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d64536b102049c6b08bd8ce155a6bf578c653bfa"><code>d64536b</code></a> chore: refactor for removing pdb symbols</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/ac40895d57422ec4e93cd7c53d430b532448687d"><code>ac40895</code></a> Read the Docs now requires a config file</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/4c900198a25bbe0c71a9d3a09c8c378920f40887"><code>4c90019</code></a> Fix X25519 import/export from PEM</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.0&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-28 16:49:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.0 to 1.5.1 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.0 to 1.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.1 - Security Release</h2>
<p>This is a minor security release to fix a potential DoS for applications that allow the use of symmetric keys with pbkdf2.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix X22519 import/export from PEM by <a href="https://github.com/achamayou"><code>@​achamayou</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li>Read the Docs now requires a config file by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/335">latchset/jwcrypto#335</a></li>
<li>chore: refactor for removing pdb symbols by <a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
<li>Fix potential DoS issue with p2c header by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/336">latchset/jwcrypto#336</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/achamayou"><code>@​achamayou</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li><a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/8ae0df6538b8d8aa52e82105ec5132d289ad9ddd"><code>8ae0df6</code></a> Version 1.5.1</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/066d13f2dbac3c0be7aa2a3023189980d56b86ab"><code>066d13f</code></a> Update Security Policy</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d2655d370586cb830e49acfb450f87598da60be8"><code>d2655d3</code></a> Fix potential DoS issue with p2c header</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/6ee0e8915a22f2aed5346ec8a0116ce1cc64349a"><code>6ee0e89</code></a> chore: arg renamed</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d64536b102049c6b08bd8ce155a6bf578c653bfa"><code>d64536b</code></a> chore: refactor for removing pdb symbols</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/ac40895d57422ec4e93cd7c53d430b532448687d"><code>ac40895</code></a> Read the Docs now requires a config file</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/4c900198a25bbe0c71a9d3a09c8c378920f40887"><code>4c90019</code></a> Fix X25519 import/export from PEM</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.0&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-28 16:47:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.0 to 1.5.1 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.0 to 1.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.1 - Security Release</h2>
<p>This is a minor security release to fix a potential DoS for applications that allow the use of symmetric keys with pbkdf2.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix X22519 import/export from PEM by <a href="https://github.com/achamayou"><code>@​achamayou</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li>Read the Docs now requires a config file by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/335">latchset/jwcrypto#335</a></li>
<li>chore: refactor for removing pdb symbols by <a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
<li>Fix potential DoS issue with p2c header by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/336">latchset/jwcrypto#336</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/achamayou"><code>@​achamayou</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/334">latchset/jwcrypto#334</a></li>
<li><a href="https://github.com/peppelinux"><code>@​peppelinux</code></a> made their first contribution in <a href="https://redirect.github.com/latchset/jwcrypto/pull/330">latchset/jwcrypto#330</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/8ae0df6538b8d8aa52e82105ec5132d289ad9ddd"><code>8ae0df6</code></a> Version 1.5.1</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/066d13f2dbac3c0be7aa2a3023189980d56b86ab"><code>066d13f</code></a> Update Security Policy</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d2655d370586cb830e49acfb450f87598da60be8"><code>d2655d3</code></a> Fix potential DoS issue with p2c header</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/6ee0e8915a22f2aed5346ec8a0116ce1cc64349a"><code>6ee0e89</code></a> chore: arg renamed</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/d64536b102049c6b08bd8ce155a6bf578c653bfa"><code>d64536b</code></a> chore: refactor for removing pdb symbols</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/ac40895d57422ec4e93cd7c53d430b532448687d"><code>ac40895</code></a> Read the Docs now requires a config file</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/4c900198a25bbe0c71a9d3a09c8c378920f40887"><code>4c90019</code></a> Fix X25519 import/export from PEM</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.0...v1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.0&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-28 16:46:19 +0000 UTC
    </div>
</div>

