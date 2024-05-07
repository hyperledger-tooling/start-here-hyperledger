---
layout: default
title: aries-agent-controller
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/aries-agent-controller
---

# aries-agent-controller <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/aries-agent-controller){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aries-agent-controller/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Bump jinja2 from 3.1.2 to 3.1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jinja2](https://github.com/pallets/jinja) from 3.1.2 to 3.1.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/releases">jinja2's releases</a>.</em></p>
<blockquote>
<h2>3.1.4</h2>
<p>This is the Jinja 3.1.4 security release, which fixes security issues and bugs but does not otherwise change behavior and should not result in breaking changes.</p>
<p>PyPI: <a href="https://pypi.org/project/Jinja2/3.1.4/">https://pypi.org/project/Jinja2/3.1.4/</a>
Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-4">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-4</a></p>
<ul>
<li>The <code>xmlattr</code> filter does not allow keys with <code>/</code> solidus, <code>&gt;</code> greater-than sign, or <code>=</code> equals sign, in addition to disallowing spaces. Regardless of any validation done by Jinja, user input should never be used as keys to this filter, or must be separately validated first. GHSA-h75v-3vvj-5mfj</li>
</ul>
<h2>3.1.3</h2>
<p>This is a fix release for the 3.1.x feature branch.</p>
<ul>
<li>Fix for <a href="https://github.com/pallets/jinja/security/advisories/GHSA-h5c8-rqwp-cp95">GHSA-h5c8-rqwp-cp95</a>. You are affected if you are using <code>xmlattr</code> and passing user input as attribute keys.</li>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/15?closed=1">https://github.com/pallets/jinja/milestone/15?closed=1</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/blob/main/CHANGES.rst">jinja2's changelog</a>.</em></p>
<blockquote>
<h2>Version 3.1.4</h2>
<p>Released 2024-05-05</p>
<ul>
<li>The <code>xmlattr</code> filter does not allow keys with <code>/</code> solidus, <code>&gt;</code>
greater-than sign, or <code>=</code> equals sign, in addition to disallowing spaces.
Regardless of any validation done by Jinja, user input should never be used
as keys to this filter, or must be separately validated first.
:ghsa:<code>h75v-3vvj-5mfj</code></li>
</ul>
<h2>Version 3.1.3</h2>
<p>Released 2024-01-10</p>
<ul>
<li>Fix compiler error when checking if required blocks in parent templates are
empty. :pr:<code>1858</code></li>
<li><code>xmlattr</code> filter does not allow keys with spaces. :ghsa:<code>h5c8-rqwp-cp95</code></li>
<li>Make error messages stemming from invalid nesting of <code>{% trans %}</code> blocks
more helpful. :pr:<code>1918</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/jinja/commit/dd4a8b5466d8790540c181590b14db4d4d889d57"><code>dd4a8b5</code></a> release version 3.1.4</li>
<li><a href="https://github.com/pallets/jinja/commit/0668239dc6b44ef38e7a6c9f91f312fd4ca581cb"><code>0668239</code></a> Merge pull request from GHSA-h75v-3vvj-5mfj</li>
<li><a href="https://github.com/pallets/jinja/commit/d655030770081e2dfe46f90e27620472a502289d"><code>d655030</code></a> disallow invalid characters in keys to xmlattr filter</li>
<li><a href="https://github.com/pallets/jinja/commit/a7863ba9d3521f1450f821119c50d19d7ecea329"><code>a7863ba</code></a> add ghsa links</li>
<li><a href="https://github.com/pallets/jinja/commit/b5c98e78c2ee7d2bf0aa06d29ed9bf7082de9cf4"><code>b5c98e7</code></a> start version 3.1.4</li>
<li><a href="https://github.com/pallets/jinja/commit/da3a9f0b804199845fcb76f2e08748bdaeba93ee"><code>da3a9f0</code></a> update project files (<a href="https://redirect.github.com/pallets/jinja/issues/1968">#1968</a>)</li>
<li><a href="https://github.com/pallets/jinja/commit/0ee5eb41d1a2d7d9a05a02dc26dd70e63aaaeeb1"><code>0ee5eb4</code></a> satisfy formatter, linter, and strict mypy</li>
<li><a href="https://github.com/pallets/jinja/commit/20477c63575175196bfc8103f223cc9f5642595d"><code>20477c6</code></a> update project files (<a href="https://redirect.github.com/pallets/jinja/issues/5457">#5457</a>)</li>
<li><a href="https://github.com/pallets/jinja/commit/e491223739dedbb1f4fc6a71340c1484e149d947"><code>e491223</code></a> update pyyaml dev dependency</li>
<li><a href="https://github.com/pallets/jinja/commit/36f98854c721f98ba103f97f65a8a098da5af0d7"><code>36f9885</code></a> fix pr link</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/jinja/compare/3.1.2...3.1.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jinja2&package-manager=pip&previous-version=3.1.2&new-version=3.1.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/aries-agent-controller/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 20:30:41 +0000 UTC
    </div>
</div>

