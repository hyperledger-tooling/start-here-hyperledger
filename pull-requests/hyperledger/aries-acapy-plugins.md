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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/409" class=".btn">#409</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.2 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<h2>Changes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/JonathanPlasse"><code>@​JonathanPlasse</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/autinerd"><code>@​autinerd</code></a></li>
<li><a href="https://github.com/bersbersbers"><code>@​bersbersbers</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/ibraheemdev"><code>@​ibraheemdev</code></a></li>
<li><a href="https://github.com/jfrost-mo"><code>@​jfrost-mo</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.2</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>0.4.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>invalid-hash-returned</code> (<code>PLE0309</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10961">#10961</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-index-returned</code> (<code>PLE0305</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10962">#10962</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Allow <code>NoReturn</code>-like functions for <code>__str__</code>, <code>__len__</code>, etc. (<code>PLE0307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11017">#11017</a>)</li>
<li>Parser: Use empty range when there's &quot;gap&quot; in token source (<a href="https://redirect.github.com/astral-sh/ruff/pull/11032">#11032</a>)</li>
<li>[<code>ruff</code>] Ignore stub functions in <code>unused-async</code> (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11026">#11026</a>)</li>
<li>Parser: Expect indented case block instead of match stmt (<a href="https://redirect.github.com/astral-sh/ruff/pull/11033">#11033</a>)</li>
</ul>
<h2>0.4.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/77c93fd63c1c072501d297082aa59c741b2d5466"><code>77c93fd</code></a> Bump version to 0.4.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11151">#11151</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c9f5e3001da83a7e48aef21ef72d155c8928035"><code>1c9f5e3</code></a> Display the AST even with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/issues/11147">#11147</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/263a0d25edf0e56358a6132158d96f06bf94701b"><code>263a0d2</code></a> Use <code>macos-12</code> to build release wheels (<a href="https://redirect.github.com/astral-sh/ruff/issues/11146">#11146</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4738e199747cdfb7dd82d45b3bd23b715ad0d526"><code>4738e19</code></a> Remove unused lexical error types (<a href="https://redirect.github.com/astral-sh/ruff/issues/11145">#11145</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f428bd5052b9729cb25be4dd74c703308695edab"><code>f428bd5</code></a> Docs: mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11144">#11144</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4690890e9fc880489007ea557a0c7fcb190d9c73"><code>4690890</code></a> <code>ruff server</code>: In 'publish diagnostics' mode, document diagnostics are cleare...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/19baabba58c55d8c280b701dc5fb346ce19477bd"><code>19baabb</code></a> README: add Apache Superset to project list (<a href="https://redirect.github.com/astral-sh/ruff/issues/11136">#11136</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/cee38f39dfb7eaca22eda3c19a4d81adc4097105"><code>cee38f3</code></a> [<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11131">#11131</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e3fde2814655dd315683833c772d10e6cd55ba08"><code>e3fde28</code></a> [<code>flake8-pyi</code>] Allow overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (`PYI0...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c8849f9a8a2e2dcc0849f35fd5c39049a1e4a6e"><code>1c8849f</code></a> Use Matchit to Resolve Per-File Settings (<a href="https://redirect.github.com/astral-sh/ruff/issues/11111">#11111</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 05:12:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/408" class=".btn">#408</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.4.2 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/3702ba224ecffbcec30af640c149f231d90aebdb"><code>3702ba2</code></a> Prepare release 24.4.2 (<a href="https://redirect.github.com/psf/black/issues/4335">#4335</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4aaa8a9947d951eb1e69979c3c58e197adbe40f"><code>e4aaa8a</code></a> Fix incorrect f-string tokenization (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
<li><a href="https://github.com/psf/black/commit/ba88fc372eaed34abb33ea02d6860b185388d928"><code>ba88fc3</code></a> Simplify string tokenization regexes (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
<li><a href="https://github.com/psf/black/commit/5683242fd432d93c9c37540948a39afd06ea4f7d"><code>5683242</code></a> New release template</li>
<li><a href="https://github.com/psf/black/commit/e7fb048281a83733f0b162fc7fa85e48044ea9ec"><code>e7fb048</code></a> Prepare release 24.4.1 (<a href="https://redirect.github.com/psf/black/issues/4328">#4328</a>)</li>
<li><a href="https://github.com/psf/black/commit/3f0f8f1956646fd9f6fc47e133364c1352a478d1"><code>3f0f8f1</code></a> Support PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
<li><a href="https://github.com/psf/black/commit/2f88085da588d34286bc9a24e288de204f141243"><code>2f88085</code></a> Github Action: Directly install from repo if <code>export-subst</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
<li><a href="https://github.com/psf/black/commit/12ce3db077780ab01cc5ad1f92d5c85fcca3f54c"><code>12ce3db</code></a> Move changelog entry to right section (<a href="https://redirect.github.com/psf/black/issues/4326">#4326</a>)</li>
<li><a href="https://github.com/psf/black/commit/1354be2525e4910b8a0d7c46242eae76963db5d2"><code>1354be2</code></a> Add support to style function definitions with newlines before function stubs...</li>
<li><a href="https://github.com/psf/black/commit/f4b644b82f64d5aa2b8959277c9eb9ebcb16affe"><code>f4b644b</code></a> Prevent wrapping of multiline fstrings in parens (<a href="https://redirect.github.com/psf/black/issues/4325">#4325</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 05:11:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/407" class=".btn">#407</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.4.2 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/3702ba224ecffbcec30af640c149f231d90aebdb"><code>3702ba2</code></a> Prepare release 24.4.2 (<a href="https://redirect.github.com/psf/black/issues/4335">#4335</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4aaa8a9947d951eb1e69979c3c58e197adbe40f"><code>e4aaa8a</code></a> Fix incorrect f-string tokenization (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
<li><a href="https://github.com/psf/black/commit/ba88fc372eaed34abb33ea02d6860b185388d928"><code>ba88fc3</code></a> Simplify string tokenization regexes (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
<li><a href="https://github.com/psf/black/commit/5683242fd432d93c9c37540948a39afd06ea4f7d"><code>5683242</code></a> New release template</li>
<li><a href="https://github.com/psf/black/commit/e7fb048281a83733f0b162fc7fa85e48044ea9ec"><code>e7fb048</code></a> Prepare release 24.4.1 (<a href="https://redirect.github.com/psf/black/issues/4328">#4328</a>)</li>
<li><a href="https://github.com/psf/black/commit/3f0f8f1956646fd9f6fc47e133364c1352a478d1"><code>3f0f8f1</code></a> Support PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
<li><a href="https://github.com/psf/black/commit/2f88085da588d34286bc9a24e288de204f141243"><code>2f88085</code></a> Github Action: Directly install from repo if <code>export-subst</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
<li><a href="https://github.com/psf/black/commit/12ce3db077780ab01cc5ad1f92d5c85fcca3f54c"><code>12ce3db</code></a> Move changelog entry to right section (<a href="https://redirect.github.com/psf/black/issues/4326">#4326</a>)</li>
<li><a href="https://github.com/psf/black/commit/1354be2525e4910b8a0d7c46242eae76963db5d2"><code>1354be2</code></a> Add support to style function definitions with newlines before function stubs...</li>
<li><a href="https://github.com/psf/black/commit/f4b644b82f64d5aa2b8959277c9eb9ebcb16affe"><code>f4b644b</code></a> Prevent wrapping of multiline fstrings in parens (<a href="https://redirect.github.com/psf/black/issues/4325">#4325</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 05:11:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.2 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<h2>Changes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/JonathanPlasse"><code>@​JonathanPlasse</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/autinerd"><code>@​autinerd</code></a></li>
<li><a href="https://github.com/bersbersbers"><code>@​bersbersbers</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/ibraheemdev"><code>@​ibraheemdev</code></a></li>
<li><a href="https://github.com/jfrost-mo"><code>@​jfrost-mo</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.2</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>0.4.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>invalid-hash-returned</code> (<code>PLE0309</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10961">#10961</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-index-returned</code> (<code>PLE0305</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10962">#10962</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Allow <code>NoReturn</code>-like functions for <code>__str__</code>, <code>__len__</code>, etc. (<code>PLE0307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11017">#11017</a>)</li>
<li>Parser: Use empty range when there's &quot;gap&quot; in token source (<a href="https://redirect.github.com/astral-sh/ruff/pull/11032">#11032</a>)</li>
<li>[<code>ruff</code>] Ignore stub functions in <code>unused-async</code> (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11026">#11026</a>)</li>
<li>Parser: Expect indented case block instead of match stmt (<a href="https://redirect.github.com/astral-sh/ruff/pull/11033">#11033</a>)</li>
</ul>
<h2>0.4.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/77c93fd63c1c072501d297082aa59c741b2d5466"><code>77c93fd</code></a> Bump version to 0.4.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11151">#11151</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c9f5e3001da83a7e48aef21ef72d155c8928035"><code>1c9f5e3</code></a> Display the AST even with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/issues/11147">#11147</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/263a0d25edf0e56358a6132158d96f06bf94701b"><code>263a0d2</code></a> Use <code>macos-12</code> to build release wheels (<a href="https://redirect.github.com/astral-sh/ruff/issues/11146">#11146</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4738e199747cdfb7dd82d45b3bd23b715ad0d526"><code>4738e19</code></a> Remove unused lexical error types (<a href="https://redirect.github.com/astral-sh/ruff/issues/11145">#11145</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f428bd5052b9729cb25be4dd74c703308695edab"><code>f428bd5</code></a> Docs: mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11144">#11144</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4690890e9fc880489007ea557a0c7fcb190d9c73"><code>4690890</code></a> <code>ruff server</code>: In 'publish diagnostics' mode, document diagnostics are cleare...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/19baabba58c55d8c280b701dc5fb346ce19477bd"><code>19baabb</code></a> README: add Apache Superset to project list (<a href="https://redirect.github.com/astral-sh/ruff/issues/11136">#11136</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/cee38f39dfb7eaca22eda3c19a4d81adc4097105"><code>cee38f3</code></a> [<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11131">#11131</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e3fde2814655dd315683833c772d10e6cd55ba08"><code>e3fde28</code></a> [<code>flake8-pyi</code>] Allow overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (`PYI0...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c8849f9a8a2e2dcc0849f35fd5c39049a1e4a6e"><code>1c8849f</code></a> Use Matchit to Resolve Per-File Settings (<a href="https://redirect.github.com/astral-sh/ruff/issues/11111">#11111</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 05:10:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.4.2 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/3702ba224ecffbcec30af640c149f231d90aebdb"><code>3702ba2</code></a> Prepare release 24.4.2 (<a href="https://redirect.github.com/psf/black/issues/4335">#4335</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4aaa8a9947d951eb1e69979c3c58e197adbe40f"><code>e4aaa8a</code></a> Fix incorrect f-string tokenization (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
<li><a href="https://github.com/psf/black/commit/ba88fc372eaed34abb33ea02d6860b185388d928"><code>ba88fc3</code></a> Simplify string tokenization regexes (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
<li><a href="https://github.com/psf/black/commit/5683242fd432d93c9c37540948a39afd06ea4f7d"><code>5683242</code></a> New release template</li>
<li><a href="https://github.com/psf/black/commit/e7fb048281a83733f0b162fc7fa85e48044ea9ec"><code>e7fb048</code></a> Prepare release 24.4.1 (<a href="https://redirect.github.com/psf/black/issues/4328">#4328</a>)</li>
<li><a href="https://github.com/psf/black/commit/3f0f8f1956646fd9f6fc47e133364c1352a478d1"><code>3f0f8f1</code></a> Support PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
<li><a href="https://github.com/psf/black/commit/2f88085da588d34286bc9a24e288de204f141243"><code>2f88085</code></a> Github Action: Directly install from repo if <code>export-subst</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
<li><a href="https://github.com/psf/black/commit/12ce3db077780ab01cc5ad1f92d5c85fcca3f54c"><code>12ce3db</code></a> Move changelog entry to right section (<a href="https://redirect.github.com/psf/black/issues/4326">#4326</a>)</li>
<li><a href="https://github.com/psf/black/commit/1354be2525e4910b8a0d7c46242eae76963db5d2"><code>1354be2</code></a> Add support to style function definitions with newlines before function stubs...</li>
<li><a href="https://github.com/psf/black/commit/f4b644b82f64d5aa2b8959277c9eb9ebcb16affe"><code>f4b644b</code></a> Prevent wrapping of multiline fstrings in parens (<a href="https://redirect.github.com/psf/black/issues/4325">#4325</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 05:07:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/404" class=".btn">#404</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.2 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<h2>Changes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/JonathanPlasse"><code>@​JonathanPlasse</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/autinerd"><code>@​autinerd</code></a></li>
<li><a href="https://github.com/bersbersbers"><code>@​bersbersbers</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/ibraheemdev"><code>@​ibraheemdev</code></a></li>
<li><a href="https://github.com/jfrost-mo"><code>@​jfrost-mo</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.2</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>0.4.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>invalid-hash-returned</code> (<code>PLE0309</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10961">#10961</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-index-returned</code> (<code>PLE0305</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10962">#10962</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Allow <code>NoReturn</code>-like functions for <code>__str__</code>, <code>__len__</code>, etc. (<code>PLE0307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11017">#11017</a>)</li>
<li>Parser: Use empty range when there's &quot;gap&quot; in token source (<a href="https://redirect.github.com/astral-sh/ruff/pull/11032">#11032</a>)</li>
<li>[<code>ruff</code>] Ignore stub functions in <code>unused-async</code> (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11026">#11026</a>)</li>
<li>Parser: Expect indented case block instead of match stmt (<a href="https://redirect.github.com/astral-sh/ruff/pull/11033">#11033</a>)</li>
</ul>
<h2>0.4.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/77c93fd63c1c072501d297082aa59c741b2d5466"><code>77c93fd</code></a> Bump version to 0.4.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11151">#11151</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c9f5e3001da83a7e48aef21ef72d155c8928035"><code>1c9f5e3</code></a> Display the AST even with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/issues/11147">#11147</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/263a0d25edf0e56358a6132158d96f06bf94701b"><code>263a0d2</code></a> Use <code>macos-12</code> to build release wheels (<a href="https://redirect.github.com/astral-sh/ruff/issues/11146">#11146</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4738e199747cdfb7dd82d45b3bd23b715ad0d526"><code>4738e19</code></a> Remove unused lexical error types (<a href="https://redirect.github.com/astral-sh/ruff/issues/11145">#11145</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f428bd5052b9729cb25be4dd74c703308695edab"><code>f428bd5</code></a> Docs: mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11144">#11144</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4690890e9fc880489007ea557a0c7fcb190d9c73"><code>4690890</code></a> <code>ruff server</code>: In 'publish diagnostics' mode, document diagnostics are cleare...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/19baabba58c55d8c280b701dc5fb346ce19477bd"><code>19baabb</code></a> README: add Apache Superset to project list (<a href="https://redirect.github.com/astral-sh/ruff/issues/11136">#11136</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/cee38f39dfb7eaca22eda3c19a4d81adc4097105"><code>cee38f3</code></a> [<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11131">#11131</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e3fde2814655dd315683833c772d10e6cd55ba08"><code>e3fde28</code></a> [<code>flake8-pyi</code>] Allow overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (`PYI0...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c8849f9a8a2e2dcc0849f35fd5c39049a1e4a6e"><code>1c8849f</code></a> Use Matchit to Resolve Per-File Settings (<a href="https://redirect.github.com/astral-sh/ruff/issues/11111">#11111</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 05:06:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.4.2 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/3702ba224ecffbcec30af640c149f231d90aebdb"><code>3702ba2</code></a> Prepare release 24.4.2 (<a href="https://redirect.github.com/psf/black/issues/4335">#4335</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4aaa8a9947d951eb1e69979c3c58e197adbe40f"><code>e4aaa8a</code></a> Fix incorrect f-string tokenization (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
<li><a href="https://github.com/psf/black/commit/ba88fc372eaed34abb33ea02d6860b185388d928"><code>ba88fc3</code></a> Simplify string tokenization regexes (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
<li><a href="https://github.com/psf/black/commit/5683242fd432d93c9c37540948a39afd06ea4f7d"><code>5683242</code></a> New release template</li>
<li><a href="https://github.com/psf/black/commit/e7fb048281a83733f0b162fc7fa85e48044ea9ec"><code>e7fb048</code></a> Prepare release 24.4.1 (<a href="https://redirect.github.com/psf/black/issues/4328">#4328</a>)</li>
<li><a href="https://github.com/psf/black/commit/3f0f8f1956646fd9f6fc47e133364c1352a478d1"><code>3f0f8f1</code></a> Support PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
<li><a href="https://github.com/psf/black/commit/2f88085da588d34286bc9a24e288de204f141243"><code>2f88085</code></a> Github Action: Directly install from repo if <code>export-subst</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
<li><a href="https://github.com/psf/black/commit/12ce3db077780ab01cc5ad1f92d5c85fcca3f54c"><code>12ce3db</code></a> Move changelog entry to right section (<a href="https://redirect.github.com/psf/black/issues/4326">#4326</a>)</li>
<li><a href="https://github.com/psf/black/commit/1354be2525e4910b8a0d7c46242eae76963db5d2"><code>1354be2</code></a> Add support to style function definitions with newlines before function stubs...</li>
<li><a href="https://github.com/psf/black/commit/f4b644b82f64d5aa2b8959277c9eb9ebcb16affe"><code>f4b644b</code></a> Prevent wrapping of multiline fstrings in parens (<a href="https://redirect.github.com/psf/black/issues/4325">#4325</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 04:56:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.4.2 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/3702ba224ecffbcec30af640c149f231d90aebdb"><code>3702ba2</code></a> Prepare release 24.4.2 (<a href="https://redirect.github.com/psf/black/issues/4335">#4335</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4aaa8a9947d951eb1e69979c3c58e197adbe40f"><code>e4aaa8a</code></a> Fix incorrect f-string tokenization (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
<li><a href="https://github.com/psf/black/commit/ba88fc372eaed34abb33ea02d6860b185388d928"><code>ba88fc3</code></a> Simplify string tokenization regexes (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
<li><a href="https://github.com/psf/black/commit/5683242fd432d93c9c37540948a39afd06ea4f7d"><code>5683242</code></a> New release template</li>
<li><a href="https://github.com/psf/black/commit/e7fb048281a83733f0b162fc7fa85e48044ea9ec"><code>e7fb048</code></a> Prepare release 24.4.1 (<a href="https://redirect.github.com/psf/black/issues/4328">#4328</a>)</li>
<li><a href="https://github.com/psf/black/commit/3f0f8f1956646fd9f6fc47e133364c1352a478d1"><code>3f0f8f1</code></a> Support PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
<li><a href="https://github.com/psf/black/commit/2f88085da588d34286bc9a24e288de204f141243"><code>2f88085</code></a> Github Action: Directly install from repo if <code>export-subst</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
<li><a href="https://github.com/psf/black/commit/12ce3db077780ab01cc5ad1f92d5c85fcca3f54c"><code>12ce3db</code></a> Move changelog entry to right section (<a href="https://redirect.github.com/psf/black/issues/4326">#4326</a>)</li>
<li><a href="https://github.com/psf/black/commit/1354be2525e4910b8a0d7c46242eae76963db5d2"><code>1354be2</code></a> Add support to style function definitions with newlines before function stubs...</li>
<li><a href="https://github.com/psf/black/commit/f4b644b82f64d5aa2b8959277c9eb9ebcb16affe"><code>f4b644b</code></a> Prevent wrapping of multiline fstrings in parens (<a href="https://redirect.github.com/psf/black/issues/4325">#4325</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 04:51:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.2 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<h2>Changes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/JonathanPlasse"><code>@​JonathanPlasse</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/autinerd"><code>@​autinerd</code></a></li>
<li><a href="https://github.com/bersbersbers"><code>@​bersbersbers</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/ibraheemdev"><code>@​ibraheemdev</code></a></li>
<li><a href="https://github.com/jfrost-mo"><code>@​jfrost-mo</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.2</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>0.4.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>invalid-hash-returned</code> (<code>PLE0309</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10961">#10961</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-index-returned</code> (<code>PLE0305</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10962">#10962</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Allow <code>NoReturn</code>-like functions for <code>__str__</code>, <code>__len__</code>, etc. (<code>PLE0307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11017">#11017</a>)</li>
<li>Parser: Use empty range when there's &quot;gap&quot; in token source (<a href="https://redirect.github.com/astral-sh/ruff/pull/11032">#11032</a>)</li>
<li>[<code>ruff</code>] Ignore stub functions in <code>unused-async</code> (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11026">#11026</a>)</li>
<li>Parser: Expect indented case block instead of match stmt (<a href="https://redirect.github.com/astral-sh/ruff/pull/11033">#11033</a>)</li>
</ul>
<h2>0.4.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/77c93fd63c1c072501d297082aa59c741b2d5466"><code>77c93fd</code></a> Bump version to 0.4.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11151">#11151</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c9f5e3001da83a7e48aef21ef72d155c8928035"><code>1c9f5e3</code></a> Display the AST even with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/issues/11147">#11147</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/263a0d25edf0e56358a6132158d96f06bf94701b"><code>263a0d2</code></a> Use <code>macos-12</code> to build release wheels (<a href="https://redirect.github.com/astral-sh/ruff/issues/11146">#11146</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4738e199747cdfb7dd82d45b3bd23b715ad0d526"><code>4738e19</code></a> Remove unused lexical error types (<a href="https://redirect.github.com/astral-sh/ruff/issues/11145">#11145</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f428bd5052b9729cb25be4dd74c703308695edab"><code>f428bd5</code></a> Docs: mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11144">#11144</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4690890e9fc880489007ea557a0c7fcb190d9c73"><code>4690890</code></a> <code>ruff server</code>: In 'publish diagnostics' mode, document diagnostics are cleare...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/19baabba58c55d8c280b701dc5fb346ce19477bd"><code>19baabb</code></a> README: add Apache Superset to project list (<a href="https://redirect.github.com/astral-sh/ruff/issues/11136">#11136</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/cee38f39dfb7eaca22eda3c19a4d81adc4097105"><code>cee38f3</code></a> [<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11131">#11131</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e3fde2814655dd315683833c772d10e6cd55ba08"><code>e3fde28</code></a> [<code>flake8-pyi</code>] Allow overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (`PYI0...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c8849f9a8a2e2dcc0849f35fd5c39049a1e4a6e"><code>1c8849f</code></a> Use Matchit to Resolve Per-File Settings (<a href="https://redirect.github.com/astral-sh/ruff/issues/11111">#11111</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 04:50:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.4.2 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<h2>Changes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/JonathanPlasse"><code>@​JonathanPlasse</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/autinerd"><code>@​autinerd</code></a></li>
<li><a href="https://github.com/bersbersbers"><code>@​bersbersbers</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/ibraheemdev"><code>@​ibraheemdev</code></a></li>
<li><a href="https://github.com/jfrost-mo"><code>@​jfrost-mo</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.2</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>0.4.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>invalid-hash-returned</code> (<code>PLE0309</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10961">#10961</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-index-returned</code> (<code>PLE0305</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10962">#10962</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Allow <code>NoReturn</code>-like functions for <code>__str__</code>, <code>__len__</code>, etc. (<code>PLE0307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11017">#11017</a>)</li>
<li>Parser: Use empty range when there's &quot;gap&quot; in token source (<a href="https://redirect.github.com/astral-sh/ruff/pull/11032">#11032</a>)</li>
<li>[<code>ruff</code>] Ignore stub functions in <code>unused-async</code> (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11026">#11026</a>)</li>
<li>Parser: Expect indented case block instead of match stmt (<a href="https://redirect.github.com/astral-sh/ruff/pull/11033">#11033</a>)</li>
</ul>
<h2>0.4.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/77c93fd63c1c072501d297082aa59c741b2d5466"><code>77c93fd</code></a> Bump version to 0.4.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11151">#11151</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c9f5e3001da83a7e48aef21ef72d155c8928035"><code>1c9f5e3</code></a> Display the AST even with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/issues/11147">#11147</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/263a0d25edf0e56358a6132158d96f06bf94701b"><code>263a0d2</code></a> Use <code>macos-12</code> to build release wheels (<a href="https://redirect.github.com/astral-sh/ruff/issues/11146">#11146</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4738e199747cdfb7dd82d45b3bd23b715ad0d526"><code>4738e19</code></a> Remove unused lexical error types (<a href="https://redirect.github.com/astral-sh/ruff/issues/11145">#11145</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f428bd5052b9729cb25be4dd74c703308695edab"><code>f428bd5</code></a> Docs: mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11144">#11144</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4690890e9fc880489007ea557a0c7fcb190d9c73"><code>4690890</code></a> <code>ruff server</code>: In 'publish diagnostics' mode, document diagnostics are cleare...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/19baabba58c55d8c280b701dc5fb346ce19477bd"><code>19baabb</code></a> README: add Apache Superset to project list (<a href="https://redirect.github.com/astral-sh/ruff/issues/11136">#11136</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/cee38f39dfb7eaca22eda3c19a4d81adc4097105"><code>cee38f3</code></a> [<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11131">#11131</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e3fde2814655dd315683833c772d10e6cd55ba08"><code>e3fde28</code></a> [<code>flake8-pyi</code>] Allow overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (`PYI0...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c8849f9a8a2e2dcc0849f35fd5c39049a1e4a6e"><code>1c8849f</code></a> Use Matchit to Resolve Per-File Settings (<a href="https://redirect.github.com/astral-sh/ruff/issues/11111">#11111</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-26 04:48:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update ruff requirement from ^0.1.2 to ^0.4.2 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [ruff](https://github.com/astral-sh/ruff) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<h2>Changes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/JonathanPlasse"><code>@​JonathanPlasse</code></a></li>
<li><a href="https://github.com/KPCOFGS"><code>@​KPCOFGS</code></a></li>
<li><a href="https://github.com/KotlinIsland"><code>@​KotlinIsland</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/augustelalande"><code>@​augustelalande</code></a></li>
<li><a href="https://github.com/autinerd"><code>@​autinerd</code></a></li>
<li><a href="https://github.com/bersbersbers"><code>@​bersbersbers</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/ibraheemdev"><code>@​ibraheemdev</code></a></li>
<li><a href="https://github.com/jfrost-mo"><code>@​jfrost-mo</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.2</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-pyi</code>] Allow for overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (<code>PYI036</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11057">#11057</a>)</li>
<li>[<code>pyupgrade</code>] Catch usages of <code>&quot;%s&quot; % var</code> and provide an unsafe fix (<code>UP031</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11019">#11019</a>)</li>
<li>[<code>refurb</code>] Implement new rule that suggests min/max over <code>sorted()</code> (<code>FURB192</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10868">#10868</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Fix an issue with missing diagnostics for Neovim and Helix (<a href="https://redirect.github.com/astral-sh/ruff/pull/11092">#11092</a>)</li>
<li>Implement hover documentation for <code>noqa</code> codes (<a href="https://redirect.github.com/astral-sh/ruff/pull/11096">#11096</a>)</li>
<li>Introduce common Ruff configuration options with new server settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11062">#11062</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Use <code>macos-12</code> for building release wheels to enable macOS 11 compatibility (<a href="https://redirect.github.com/astral-sh/ruff/pull/11146">#11146</a>)</li>
<li>[<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11131">#11131</a>)</li>
<li>[<code>flake8-pyi</code>] Allow simple assignments to <code>None</code> in enum class scopes (<code>PYI026</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11128">#11128</a>)</li>
<li>[<code>flake8-simplify</code>] Avoid raising <code>SIM911</code> for non-<code>zip</code> attribute calls (<a href="https://redirect.github.com/astral-sh/ruff/pull/11126">#11126</a>)</li>
<li>[<code>refurb</code>] Avoid <code>operator.itemgetter</code> suggestion for single-item tuple (<a href="https://redirect.github.com/astral-sh/ruff/pull/11095">#11095</a>)</li>
<li>[<code>ruff</code>] Respect per-file-ignores for <code>RUF100</code> with no other diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/11058">#11058</a>)</li>
<li>[<code>ruff</code>] Fix async comprehension false positive (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11070">#11070</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Document explicitly disabling strict zip (<code>B905</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11040">#11040</a>)</li>
<li>[<code>flake8-type-checking</code>] Mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, and <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11144">#11144</a>)</li>
<li>[<code>isort</code>] Improve documentation around custom <code>isort</code> sections (<a href="https://redirect.github.com/astral-sh/ruff/pull/11050">#11050</a>)</li>
<li>[<code>pylint</code>] Fix documentation oversight for <code>invalid-X-returns</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11094">#11094</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use <code>matchit</code> to resolve per-file settings (<a href="https://redirect.github.com/astral-sh/ruff/pull/11111">#11111</a>)</li>
</ul>
<h2>0.4.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>invalid-hash-returned</code> (<code>PLE0309</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10961">#10961</a>)</li>
<li>[<code>pylint</code>] Implement <code>invalid-index-returned</code> (<code>PLE0305</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10962">#10962</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pylint</code>] Allow <code>NoReturn</code>-like functions for <code>__str__</code>, <code>__len__</code>, etc. (<code>PLE0307</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11017">#11017</a>)</li>
<li>Parser: Use empty range when there's &quot;gap&quot; in token source (<a href="https://redirect.github.com/astral-sh/ruff/pull/11032">#11032</a>)</li>
<li>[<code>ruff</code>] Ignore stub functions in <code>unused-async</code> (<code>RUF029</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11026">#11026</a>)</li>
<li>Parser: Expect indented case block instead of match stmt (<a href="https://redirect.github.com/astral-sh/ruff/pull/11033">#11033</a>)</li>
</ul>
<h2>0.4.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/77c93fd63c1c072501d297082aa59c741b2d5466"><code>77c93fd</code></a> Bump version to 0.4.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11151">#11151</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c9f5e3001da83a7e48aef21ef72d155c8928035"><code>1c9f5e3</code></a> Display the AST even with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/issues/11147">#11147</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/263a0d25edf0e56358a6132158d96f06bf94701b"><code>263a0d2</code></a> Use <code>macos-12</code> to build release wheels (<a href="https://redirect.github.com/astral-sh/ruff/issues/11146">#11146</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4738e199747cdfb7dd82d45b3bd23b715ad0d526"><code>4738e19</code></a> Remove unused lexical error types (<a href="https://redirect.github.com/astral-sh/ruff/issues/11145">#11145</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f428bd5052b9729cb25be4dd74c703308695edab"><code>f428bd5</code></a> Docs: mention <code>lint.typing-modules</code> in <code>TCH001</code>, <code>TCH002</code>, <code>TCH003</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11144">#11144</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4690890e9fc880489007ea557a0c7fcb190d9c73"><code>4690890</code></a> <code>ruff server</code>: In 'publish diagnostics' mode, document diagnostics are cleare...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/19baabba58c55d8c280b701dc5fb346ce19477bd"><code>19baabb</code></a> README: add Apache Superset to project list (<a href="https://redirect.github.com/astral-sh/ruff/issues/11136">#11136</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/cee38f39dfb7eaca22eda3c19a4d81adc4097105"><code>cee38f3</code></a> [<code>flake8-blind-expect</code>] Allow raise from in <code>BLE001</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11131">#11131</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e3fde2814655dd315683833c772d10e6cd55ba08"><code>e3fde28</code></a> [<code>flake8-pyi</code>] Allow overloaded <code>__exit__</code> and <code>__aexit__</code> definitions (`PYI0...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c8849f9a8a2e2dcc0849f35fd5c39049a1e4a6e"><code>1c8849f</code></a> Use Matchit to Resolve Per-File Settings (<a href="https://redirect.github.com/astral-sh/ruff/issues/11111">#11111</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.2...v0.4.2">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2024-04-26 04:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update black requirement from ~23.7.0 to ~24.4.2 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [black](https://github.com/psf/black) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.2</h2>
<p>This is a bugfix release to fix two regressions in the new f-string parser introduced in
24.4.1.</p>
<h3>Parser</h3>
<ul>
<li>Fix regression where certain complex f-strings failed to parse (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix bad performance on certain complex string literals (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
</ul>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/3702ba224ecffbcec30af640c149f231d90aebdb"><code>3702ba2</code></a> Prepare release 24.4.2 (<a href="https://redirect.github.com/psf/black/issues/4335">#4335</a>)</li>
<li><a href="https://github.com/psf/black/commit/e4aaa8a9947d951eb1e69979c3c58e197adbe40f"><code>e4aaa8a</code></a> Fix incorrect f-string tokenization (<a href="https://redirect.github.com/psf/black/issues/4332">#4332</a>)</li>
<li><a href="https://github.com/psf/black/commit/ba88fc372eaed34abb33ea02d6860b185388d928"><code>ba88fc3</code></a> Simplify string tokenization regexes (<a href="https://redirect.github.com/psf/black/issues/4331">#4331</a>)</li>
<li><a href="https://github.com/psf/black/commit/5683242fd432d93c9c37540948a39afd06ea4f7d"><code>5683242</code></a> New release template</li>
<li><a href="https://github.com/psf/black/commit/e7fb048281a83733f0b162fc7fa85e48044ea9ec"><code>e7fb048</code></a> Prepare release 24.4.1 (<a href="https://redirect.github.com/psf/black/issues/4328">#4328</a>)</li>
<li><a href="https://github.com/psf/black/commit/3f0f8f1956646fd9f6fc47e133364c1352a478d1"><code>3f0f8f1</code></a> Support PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
<li><a href="https://github.com/psf/black/commit/2f88085da588d34286bc9a24e288de204f141243"><code>2f88085</code></a> Github Action: Directly install from repo if <code>export-subst</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
<li><a href="https://github.com/psf/black/commit/12ce3db077780ab01cc5ad1f92d5c85fcca3f54c"><code>12ce3db</code></a> Move changelog entry to right section (<a href="https://redirect.github.com/psf/black/issues/4326">#4326</a>)</li>
<li><a href="https://github.com/psf/black/commit/1354be2525e4910b8a0d7c46242eae76963db5d2"><code>1354be2</code></a> Add support to style function definitions with newlines before function stubs...</li>
<li><a href="https://github.com/psf/black/commit/f4b644b82f64d5aa2b8959277c9eb9ebcb16affe"><code>f4b644b</code></a> Prevent wrapping of multiline fstrings in parens (<a href="https://redirect.github.com/psf/black/issues/4325">#4325</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.4.2">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2024-04-26 04:26:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    Create Automated Release Workflows 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There's some fairly complicated logic in a few places so I created a couple flow charts at `ReleaseWorkflows.md`.

Basically, this is a way to keep the plugins up to date with acapy releases automatically. If all the tests pass for a plugin it will be updated and be considered stable with acapy. If it doesn't then it won't be upgraded and will remain verified against an earlier release. A maintainer can create patch releases if a plugin which did fail for a release gets fixed before another version of acapy. A message is appended to the plugin description as well with the supported acapy version. I'm hoping this can be used to provide warnings in acapy when a plugin falls behind acapy.

There is some bash scripting. I tried to limit it as much as I could by utilizing the `repo_manager.py` script. The manager script has been changed slightly and some additional options for creating and parsing release information has added. The formatting for the release notes in RELEASES.md could be improved a bit more but I think it's good enough for now.

I had to do a bit of work for some tests after the upgrade but they all passing now so they will all be on version 0.12.0 of acapy initially. Two unit tests for rpc I removed. I couldn't figure out why they were only failing in the github action but not locally.

*** Note: *** I'm not sure if the bot will be able to create the release PR's for this repo. I have tried to use the org secret and replicated the same thing for my fork, so hopefully it does.

See initial PR https://github.com/hyperledger/aries-acapy-plugins/pull/387. Closed and wasn't able to re-open it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 20:06:01 +0000 UTC
    </div>
</div>

