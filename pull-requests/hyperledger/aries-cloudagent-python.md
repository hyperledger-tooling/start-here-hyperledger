---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2689" class=".btn">#2689</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.0 to 1.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-28 16:45:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2688" class=".btn">#2688</a>
            </td>
            <td>
                <b>
                    Add unit tests for anoncreds revocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds unit testing for the anoncreds revocation module.

Tried to use the anoncred module as much as possible but when I was having too much trouble I mocked calls that loaded/created objects or converted forms. 

Mocked the database/wallet Entry responses a lot with basic classes. Couldn't find a better way to do this or an examples in the repo.

Coverage is 92%. I tried not to make the tests too brittle but wanted to have good coverage for my own understanding. I'm hoping this will help others trying to understand the code along with having a good testing layout for future refactoring or features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 22:25:10 +0000 UTC
    </div>
</div>

