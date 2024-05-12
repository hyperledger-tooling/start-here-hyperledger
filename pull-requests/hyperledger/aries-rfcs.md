---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/832" class=".btn">#832</a>
            </td>
            <td>
                <b>
                    RFC 0829: VDR Proxy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A VDR ([verifiable data registry]) is a place where DIDs and objects related to
DIDs (such as [Hyperledger AnonCreds] objects) are stored such that they can be
resolved. The VDR Proxy protocol defined by this RFC is a DIDComm protocol that
can be used by a DIDComm agent to request another agent resolve VDR URIs
([Uniform Resource Identifier]s) and return the resolved objects to the
requesting agent. The protocol is a simple client/server protocol, supporting
the ability to request and receive back multiple resolutions in a single exchange.

[VDR]: https://www.w3.org/TR/did-core/#dfn-verifiable-data-registry
[verifiable data registry]: https://www.w3.org/TR/did-core/#dfn-verifiable-data-registry
[Hyperledger AnonCreds]: https://www.hyperledger.org/projects/anoncreds
[Uniform Resource Identifier]: https://en.wikipedia.org/wiki/Uniform_Resource_Identifier


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-12 14:20:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.5.10 to 9.5.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.5.10 to 9.5.21.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.5.21</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7133">#7133</a>: Ensure latest version of Mermaid.js is used</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7125">#7125</a>: Added warning for dotfiles in info plugin</li>
</ul>
<p>Thanks to <a href="https://github.com/kamilkrzyskow"><code>@​kamilkrzyskow</code></a> for their contributions</p>
<h2>mkdocs-material-9.5.20</h2>
<ul>
<li>Fixed deprecation warning in privacy plugin (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7119">#7119</a>: Tags plugin emits deprecation warning (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7118">#7118</a>: Social plugin crashes if fonts are disabled (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7085">#7085</a>: Social plugin crashes on Windows when downloading fonts</li>
</ul>
<h2>mkdocs-material-9.5.19</h2>
<ul>
<li>Updated MkDocs to 1.6 and limited version to &lt; 2</li>
<li>Updated Docker image to latest Alpine Linux</li>
<li>Removed <code>setup.py</code>, now that GitHub fully understands <code>pyproject.toml</code></li>
<li>Improved interop of social plugin with third-party MkDocs themes</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7099">#7099</a>: Blog reading time not rendered correctly for Japanese</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7097">#7097</a>: Improved resilience of tags plugin when no tags are given</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7090">#7090</a>: Active tab indicator in nested content tabs rendering bug</li>
</ul>
<h2>mkdocs-material-9.5.18</h2>
<ul>
<li>Refactored tooltips implementation to fix positioning issues</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7044">#7044</a>: Rendering glitch when hovering contributor avatar in Chrome</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7043">#7043</a>: Highlighted lines in code blocks cutoff on mobile</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6910">#6910</a>: Incorrect position of tooltip for page status in sidebar</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6760">#6760</a>: Incorrect position and overly long tooltip in tables</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6488">#6488</a>: Incorrect position and cutoff tooltip in content tabs</li>
</ul>
<h2>mkdocs-material-9.5.17</h2>
<ul>
<li>Updated Serbian translations</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7003">#7003</a>: Confusing keyboard interaction for palette toggle</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7001">#7001</a>: Blog posts now show time by default (9.5.16 regression)</li>
<li>Fixed edge case in backport of social plugin font loading logic</li>
</ul>
<p>Thanks to <a href="https://github.com/stcksmsh"><code>@​stcksmsh</code></a> for their contributions.</p>
<h2>mkdocs-material-9.5.16</h2>
<ul>
<li>Updated Russian translations</li>
<li>Improved error handling and reporting in social plugin</li>
<li>Improved error handling and reporting in privacy plugin</li>
<li>Fixed blog plugin not allowing to use time in format strings</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6983">#6983</a>: Social plugin crashes because of Google Fonts API change</li>
</ul>
<p>Thanks to <a href="https://github.com/kamilkrzyskow"><code>@​kamilkrzyskow</code></a>, <a href="https://github.com/Guts"><code>@​Guts</code></a>, <a href="https://github.com/szg-alex-payne"><code>@​szg-alex-payne</code></a> and <a href="https://github.com/natakazakova"><code>@​natakazakova</code></a> for their contributions</p>
<h2>mkdocs-material-9.5.15</h2>
<ul>
<li>Reverted fix for transparent iframes (9.5.14)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6929">#6929</a>: Interference of social plugin and auto dark mode</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6938">#6938</a>: Giscus shows dark background in light mode (9.5.14 regression)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.5.21 (2024-05-03)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7133">#7133</a>: Ensure latest version of Mermaid.js is used</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7125">#7125</a>: Added warning for dotfiles in info plugin</li>
</ul>
<p>mkdocs-material-9.5.20 (2024-04-29)</p>
<ul>
<li>Fixed deprecation warning in privacy plugin (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7119">#7119</a>: Tags plugin emits deprecation warning (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7118">#7118</a>: Social plugin crashes if fonts are disabled (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7085">#7085</a>: Social plugin crashes on Windows when downloading fonts</li>
</ul>
<p>mkdocs-material-9.5.19+insiders-4.53.8 (2024-04-26)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7052">#7052</a>: Preview extension automatically including all pages</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7051">#7051</a>: Instant previews mounting on footnote references</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5165">#5165</a>: Improved tooltips not mounting in sidebar for typeset plugin</li>
</ul>
<p>mkdocs-material-9.5.19+insiders-4.53.7 (2024-04-25)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7060">#7060</a>: Incorrect resolution of translation when using static-i18n</li>
</ul>
<p>mkdocs-material-9.5.19 (2024-04-25)</p>
<ul>
<li>Updated MkDocs to 1.6 and limited version to &lt; 2</li>
<li>Updated Docker image to latest Alpine Linux</li>
<li>Removed setup.py, now that GitHub fully understands pyproject.toml</li>
<li>Improved interop of social plugin with third-party MkDocs themes</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7099">#7099</a>: Blog reading time not rendered correctly for Japanese</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7097">#7097</a>: Improved resilience of tags plugin when no tags are given</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7090">#7090</a>: Active tab indicator in nested content tabs rendering bug</li>
</ul>
<p>mkdocs-material-9.5.18 (2024-04-16)</p>
<ul>
<li>Refactored tooltips implementation to fix positioning issues</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7044">#7044</a>: Rendering glitch when hovering contributor avatar in Chrome</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7043">#7043</a>: Highlighted lines in code blocks cutoff on mobile</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6910">#6910</a>: Incorrect position of tooltip for page status in sidebar</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6760">#6760</a>: Incorrect position and overly long tooltip in tables</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6488">#6488</a>: Incorrect position and cutoff tooltip in content tabs</li>
</ul>
<p>mkdocs-material-9.5.17+insiders-4.53.6 (2024-04-05)</p>
<ul>
<li>Ensure working directory is set for projects when using projects plugin</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6970">#6970</a>: Incorrect relative paths in git submodules with projects plugin</li>
</ul>
<p>mkdocs-material-9.5.17+insiders-4.53.5 (2024-04-02)</p>
<ul>
<li>Fixed social plugin crashing when no colors are specified in palettes</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/d1161b431f391c3be2bf3617b8c62c2477309ff6"><code>d1161b4</code></a> Prepare 9.5.21 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/aef6175f04244870e7c356d00a48a19e0cde90db"><code>aef6175</code></a> Added type selection to icon and emoji search</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/b0c5fe6aeffabb270465604e50582e8cdea9889c"><code>b0c5fe6</code></a> Updated JSON schema (<a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7150">#7150</a>)</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0e0a678b7849db824a6a18b55a595e927a5c28cc"><code>0e0a678</code></a> Merge pull request <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7142">#7142</a> from kamilkrzyskow/info-dotfile-warning</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/75d87eaf7ea696cccf99b96c915412b16ea3f079"><code>75d87ea</code></a> Widen Mermaid.js import to 10.x (current major version)</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f724bb901a18bc0813ab38a716536d3bf7212435"><code>f724bb9</code></a> Add warning for dotfiles in info plugin</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/5cb3117f50c78abfef6817b72cb09910decd272b"><code>5cb3117</code></a> Prepare 9.5.20 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/47527797b576b64161dcb066e86abbef3f38df3d"><code>4752779</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/e90871f210b5d281da5c238b9e67917fe9222585"><code>e90871f</code></a> Fixed social plugin crashing on Windows when downloading fonts (<a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7085">#7085</a>) (<a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7117">#7117</a>)</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/ff49d740249490d79b4300c0a21bbb2f191037f8"><code>ff49d74</code></a> Fixed deprecation warning in privacy plugin</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.5.10...9.5.21">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.5.10&new-version=9.5.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 17:28:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    Bump mike from 2.0.0 to 2.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mike](https://github.com/jimporter/mike) from 2.0.0 to 2.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jimporter/mike/releases">mike's releases</a>.</em></p>
<blockquote>
<h2>v2.1.1</h2>
<h3>Bug fixes</h3>
<ul>
<li>Support using environment variables for <code>INHERIT</code> when injecting the <code>mike</code> plugin into <code>mkdocs.yml</code></li>
</ul>
<h2>v2.1.0</h2>
<h3>New features</h3>
<ul>
<li>When calling <code>set-default</code>, you can now pass <code>--allow-undefined</code> to set the default to a version that doesn't exist yet</li>
<li>Add global-level <code>-q</code> / <code>--quiet</code> option to suppress warning messages</li>
<li>Add support for handling <code>!relative</code> in <code>mkdocs.yml</code></li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>When loading an MkDocs config, mike now runs the <code>startup</code> and <code>shutdown</code> events</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jimporter/mike/blob/master/CHANGES.md">mike's changelog</a>.</em></p>
<blockquote>
<h2>v2.1.1 (2024-05-03)</h2>
<h3>Bug fixes</h3>
<ul>
<li>Support using environment variables for <code>INHERIT</code> when injecting the <code>mike</code>
plugin into <code>mkdocs.yml</code></li>
</ul>
<hr />
<h2>v2.1.0 (2024-05-01)</h2>
<h3>New features</h3>
<ul>
<li>When calling <code>set-default</code>, you can now pass <code>--allow-undefined</code> to set the
default to a version that doesn't exist yet</li>
<li>Add global-level <code>-q</code> / <code>--quiet</code> option to suppress warning messages</li>
<li>Add support for handling <code>!relative</code> in <code>mkdocs.yml</code></li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>When loading an MkDocs config, mike now runs the <code>startup</code> and <code>shutdown</code>
events</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jimporter/mike/commit/0bdfe24c20fb0774652230a7abe8466b98098da4"><code>0bdfe24</code></a> Update version to 2.1.1</li>
<li><a href="https://github.com/jimporter/mike/commit/3351d5feabff8ee107f4ad6d1f86055843c7dbf1"><code>3351d5f</code></a> Expand environment variables when injecting the mike plugin; resolves <a href="https://redirect.github.com/jimporter/mike/issues/217">#217</a></li>
<li><a href="https://github.com/jimporter/mike/commit/e4d83eda046b1dea0493f91fcacbf86634c93db5"><code>e4d83ed</code></a> Update version to 2.2.0.dev0</li>
<li><a href="https://github.com/jimporter/mike/commit/6e6cfbb9a3e78d2ab2a529b72b84e8918c101f6c"><code>6e6cfbb</code></a> Update version to 2.1.0</li>
<li><a href="https://github.com/jimporter/mike/commit/5773be928d1a6e99e61755df0d73a8b2ce16660f"><code>5773be9</code></a> Fix CI</li>
<li><a href="https://github.com/jimporter/mike/commit/7904925595827ccba3908775b2f9b5add3ae9030"><code>7904925</code></a> Further tests for deserializing Python objects during <code>inject_plugin</code></li>
<li><a href="https://github.com/jimporter/mike/commit/01219bddfeea16f8d6dd6d65d0d84581cf183a3f"><code>01219bd</code></a> Allow arbitrary Python object in YAML config</li>
<li><a href="https://github.com/jimporter/mike/commit/ac7b2403cacb0a16892ce915478bac70bd7faf39"><code>ac7b240</code></a> Handle <code>!relative</code> (and any future constructors) in mkdocs.yml; resolves <a href="https://redirect.github.com/jimporter/mike/issues/199">#199</a></li>
<li><a href="https://github.com/jimporter/mike/commit/fdcc9126b5ded0a273f7d3be3dd1d698f53157ec"><code>fdcc912</code></a> Add <code>--quiet</code> option; resolves <a href="https://redirect.github.com/jimporter/mike/issues/210">#210</a></li>
<li><a href="https://github.com/jimporter/mike/commit/a39ea731c810627341980f4e28b0b5afa55c1c08"><code>a39ea73</code></a> Add <code>set-default --allow-undefined</code>; see <a href="https://redirect.github.com/jimporter/mike/issues/210">#210</a></li>
<li>Additional commits viewable in <a href="https://github.com/jimporter/mike/compare/v2.0.0...v2.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mike&package-manager=pip&previous-version=2.0.0&new-version=2.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 17:28:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    chore: updating dependabot file to support gha and python packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 16:15:55 +0000 UTC
    </div>
</div>

