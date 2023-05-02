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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1318" class=".btn">#1318</a>
            </td>
            <td>
                <b>
                    Bump plantuml-markdown from 3.9.0 to 3.9.1 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [plantuml-markdown](https://github.com/mikitex70/plantuml-markdown) from 3.9.0 to 3.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/releases">plantuml-markdown's releases</a>.</em></p>
<blockquote>
<h2>Fixed urllib3 warning about use of insecure connections</h2>
<p>When using a PlantUML server with self-signed certificates it is necessary to set the <code>insecure</code> configuration option to <code>true</code>, allowing for insecure connections.
But in this case 'urllib3' gives us a warning that it will appear on the rendered page; this release resolves this issue.
It also solves another small problem, when using other types of diagrams (such as <code>plantgantt</code>) with a PlantUML server.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/blob/master/CHANGELOG.md">plantuml-markdown's changelog</a>.</em></p>
<blockquote>
<h2>3.9.1 (2023-04-27)</h2>
<h3>Fix</h3>
<ul>
<li>
<p>Fixed handle of other diagram types with plantuml server. [Michele Tessaro]</p>
<p>When using a PlantUML server the handling of non-uml diagrams
(<code>startmindmap</code>, <code>startjson</code>, etc.) was building wrong open/close tags.</p>
</li>
<li>
<p>Fixed urllib3 warning in output page (fixes <a href="https://redirect.github.com/mikitex70/plantuml-markdown/issues/89">#89</a>) [Michele Tessaro]</p>
<p><code>urllib3</code> gives a warning when an insecure connection is used, and the
warning is included in the output page.
Now the warning is disabled if an insecure connection to a PlantUML
server is used.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/ab5ad5f0276bfede3b6da6b9e4856096ad65cddd"><code>ab5ad5f</code></a> chg: doc: updated the changelog</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/6fcc355a11bc0147b91aced9a3bbcb542d85c1c3"><code>6fcc355</code></a> chg: pkg: updated version for the new release</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/58e1b24140225c2ee65a66c2e73c7cffe2968529"><code>58e1b24</code></a> fix: usr: fixed handle of other diagram types with plantuml server</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/435ad49c111fdfe4c43cddf66b760c80960d2d6b"><code>435ad49</code></a> fix: usr: fixed urllib3 warning in output page (fixes <a href="https://redirect.github.com/mikitex70/plantuml-markdown/issues/89">#89</a>)</li>
<li>See full diff in <a href="https://github.com/mikitex70/plantuml-markdown/compare/3.9.0...3.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plantuml-markdown&package-manager=pip&previous-version=3.9.0&new-version=3.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-02 00:00:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1316" class=".btn">#1316</a>
            </td>
            <td>
                <b>
                    Updates for peering page.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [X] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [X] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [X] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change
 Minor edits for peering page 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 18:12:31 +0000 UTC
    </div>
</div>

