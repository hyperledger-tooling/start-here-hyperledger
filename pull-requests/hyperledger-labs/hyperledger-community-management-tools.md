---
layout: default
title: hyperledger-community-management-tools
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hyperledger-community-management-tools
---

# hyperledger-community-management-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hyperledger-community-management-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hyperledger-community-management-tools/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    Bump jinja2 from 2.11.3 to 3.1.3 in /org-repo-info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jinja2](https://github.com/pallets/jinja) from 2.11.3 to 3.1.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/releases">jinja2's releases</a>.</em></p>
<blockquote>
<h2>3.1.3</h2>
<p>This is a fix release for the 3.1.x feature branch.</p>
<ul>
<li>Fix for <a href="https://github.com/pallets/jinja/security/advisories/GHSA-h5c8-rqwp-cp95">GHSA-h5c8-rqwp-cp95</a>. You are affected if you are using <code>xmlattr</code> and passing user input as attribute keys.</li>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/15?closed=1">https://github.com/pallets/jinja/milestone/15?closed=1</a></li>
</ul>
<h2>3.1.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/jinja/releases/tag/3.1.0">3.1.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-2">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/13?closed=1">https://github.com/pallets/jinja/milestone/13?closed=1</a></li>
</ul>
<h2>3.1.1</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-1">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/12?closed=1">https://github.com/pallets/jinja/milestone/12?closed=1</a></li>
</ul>
<h2>3.1.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated features. The 3.1.x branch is now the supported bugfix branch, the 3.0.x branch has become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades. We also encourage upgrading to MarkupSafe 2.1.1, the latest version at this time.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-0">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/8?closed=1">https://github.com/pallets/jinja/milestone/8?closed=1</a></li>
<li>MarkupSafe changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1</a></li>
</ul>
<h2>3.0.3</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-3">https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-3</a></li>
</ul>
<h2>3.0.2</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-2">https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-2</a></li>
</ul>
<h2>3.0.1</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-1">https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-1</a></li>
</ul>
<h2>3.0.0</h2>
<p>New major versions of all the core Pallets libraries, including Jinja 3.0, have been released! :tada:</p>
<ul>
<li>Read the announcement on our blog: <a href="https://palletsprojects.com/blog/flask-2-0-released/">https://palletsprojects.com/blog/flask-2-0-released/</a></li>
<li>Read the full list of changes: <a href="https://jinja.palletsprojects.com/changes/#version-3-0-0">https://jinja.palletsprojects.com/changes/#version-3-0-0</a></li>
<li>Retweet the announcement on Twitter: <a href="https://twitter.com/PalletsTeam/status/1392266507296514048">https://twitter.com/PalletsTeam/status/1392266507296514048</a></li>
<li>Follow our blog, Twitter, or GitHub to see future announcements.</li>
</ul>
<p>This represents a significant amount of work, and there are quite a few changes. Be sure to carefully read the changelog, and use tools such as pip-compile and Dependabot to pin your dependencies and control your updates.</p>
<h2>3.0.0rc2</h2>
<p>Fixes an issue with the deprecated <code>Markup</code> subclass, <a href="https://redirect.github.com/pallets/jinja/issues/1401">#1401</a>.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0">https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0</a></li>
</ul>
<h2>3.0.0rc1</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0">https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/blob/main/CHANGES.rst">jinja2's changelog</a>.</em></p>
<blockquote>
<h2>Version 3.1.3</h2>
<p>Released 2024-01-10</p>
<ul>
<li>Fix compiler error when checking if required blocks in parent templates are
empty. :pr:<code>1858</code></li>
<li><code>xmlattr</code> filter does not allow keys with spaces. GHSA-h5c8-rqwp-cp95</li>
<li>Make error messages stemming from invalid nesting of <code>{% trans %}</code> blocks
more helpful. :pr:<code>1918</code></li>
</ul>
<h2>Version 3.1.2</h2>
<p>Released 2022-04-28</p>
<ul>
<li>Add parameters to <code>Environment.overlay</code> to match <code>__init__</code>.
:issue:<code>1645</code></li>
<li>Handle race condition in <code>FileSystemBytecodeCache</code>. :issue:<code>1654</code></li>
</ul>
<h2>Version 3.1.1</h2>
<p>Released 2022-03-25</p>
<ul>
<li>The template filename on Windows uses the primary path separator.
:issue:<code>1637</code></li>
</ul>
<h2>Version 3.1.0</h2>
<p>Released 2022-03-24</p>
<ul>
<li>
<p>Drop support for Python 3.6. :pr:<code>1534</code></p>
</li>
<li>
<p>Remove previously deprecated code. :pr:<code>1544</code></p>
<ul>
<li><code>WithExtension</code> and <code>AutoEscapeExtension</code> are built-in now.</li>
<li><code>contextfilter</code> and <code>contextfunction</code> are replaced by
<code>pass_context</code>. <code>evalcontextfilter</code> and
<code>evalcontextfunction</code> are replaced by <code>pass_eval_context</code>.
<code>environmentfilter</code> and <code>environmentfunction</code> are replaced
by <code>pass_environment</code>.</li>
<li><code>Markup</code> and <code>escape</code> should be imported from MarkupSafe.</li>
<li>Compiled templates from very old Jinja versions may need to be
recompiled.</li>
<li>Legacy resolve mode for <code>Context</code> subclasses is no longer
supported. Override <code>resolve_or_missing</code> instead of</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/jinja/commit/d9de4bb215fd1cc8092a410fb834c7c4060b1fc1"><code>d9de4bb</code></a> release version 3.1.3</li>
<li><a href="https://github.com/pallets/jinja/commit/50124e16561f17f6c1ec85a692f6551418971cdc"><code>50124e1</code></a> skip test pypi</li>
<li><a href="https://github.com/pallets/jinja/commit/9ea7222ef3f184480be0d0884e30ccfb4172b17b"><code>9ea7222</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/da703f7aae36b1e88baaa20de334d7ff6378fdde"><code>da703f7</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/bce174692547464512383ec40e0f8338b8811983"><code>bce1746</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/7277d8068be593deab3555c7c14f974ada373af1"><code>7277d80</code></a> update pre-commit hooks</li>
<li><a href="https://github.com/pallets/jinja/commit/5c8a10522421270f66376a24ec8e0d6812bc4b14"><code>5c8a105</code></a> Make nested-trans-block exceptions nicer (<a href="https://redirect.github.com/pallets/jinja/issues/1918">#1918</a>)</li>
<li><a href="https://github.com/pallets/jinja/commit/19a55db3b411343309f2faaffaedbb089e841895"><code>19a55db</code></a> Make nested-trans-block exceptions nicer</li>
<li><a href="https://github.com/pallets/jinja/commit/716795349a41d4983a9a4771f7d883c96ea17be7"><code>7167953</code></a> Merge pull request from GHSA-h5c8-rqwp-cp95</li>
<li><a href="https://github.com/pallets/jinja/commit/7dd3680e6eea0d77fde024763657aa4d884ddb23"><code>7dd3680</code></a> xmlattr filter disallows keys with spaces</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/jinja/compare/2.11.3...3.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jinja2&package-manager=pip&previous-version=2.11.3&new-version=3.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/hyperledger-community-management-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 17:49:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hyperledger-community-management-tools/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    Bump jinja2 from 2.11.3 to 3.1.3 in /list-old-repos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jinja2](https://github.com/pallets/jinja) from 2.11.3 to 3.1.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/releases">jinja2's releases</a>.</em></p>
<blockquote>
<h2>3.1.3</h2>
<p>This is a fix release for the 3.1.x feature branch.</p>
<ul>
<li>Fix for <a href="https://github.com/pallets/jinja/security/advisories/GHSA-h5c8-rqwp-cp95">GHSA-h5c8-rqwp-cp95</a>. You are affected if you are using <code>xmlattr</code> and passing user input as attribute keys.</li>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/15?closed=1">https://github.com/pallets/jinja/milestone/15?closed=1</a></li>
</ul>
<h2>3.1.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/jinja/releases/tag/3.1.0">3.1.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-2">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/13?closed=1">https://github.com/pallets/jinja/milestone/13?closed=1</a></li>
</ul>
<h2>3.1.1</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-1">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/12?closed=1">https://github.com/pallets/jinja/milestone/12?closed=1</a></li>
</ul>
<h2>3.1.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated features. The 3.1.x branch is now the supported bugfix branch, the 3.0.x branch has become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades. We also encourage upgrading to MarkupSafe 2.1.1, the latest version at this time.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-0">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/8?closed=1">https://github.com/pallets/jinja/milestone/8?closed=1</a></li>
<li>MarkupSafe changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1</a></li>
</ul>
<h2>3.0.3</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-3">https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-3</a></li>
</ul>
<h2>3.0.2</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-2">https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-2</a></li>
</ul>
<h2>3.0.1</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-1">https://jinja.palletsprojects.com/en/3.0.x/changes/#version-3-0-1</a></li>
</ul>
<h2>3.0.0</h2>
<p>New major versions of all the core Pallets libraries, including Jinja 3.0, have been released! :tada:</p>
<ul>
<li>Read the announcement on our blog: <a href="https://palletsprojects.com/blog/flask-2-0-released/">https://palletsprojects.com/blog/flask-2-0-released/</a></li>
<li>Read the full list of changes: <a href="https://jinja.palletsprojects.com/changes/#version-3-0-0">https://jinja.palletsprojects.com/changes/#version-3-0-0</a></li>
<li>Retweet the announcement on Twitter: <a href="https://twitter.com/PalletsTeam/status/1392266507296514048">https://twitter.com/PalletsTeam/status/1392266507296514048</a></li>
<li>Follow our blog, Twitter, or GitHub to see future announcements.</li>
</ul>
<p>This represents a significant amount of work, and there are quite a few changes. Be sure to carefully read the changelog, and use tools such as pip-compile and Dependabot to pin your dependencies and control your updates.</p>
<h2>3.0.0rc2</h2>
<p>Fixes an issue with the deprecated <code>Markup</code> subclass, <a href="https://redirect.github.com/pallets/jinja/issues/1401">#1401</a>.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0">https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0</a></li>
</ul>
<h2>3.0.0rc1</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0">https://jinja.palletsprojects.com/en/master/changes/#version-3-0-0</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/blob/main/CHANGES.rst">jinja2's changelog</a>.</em></p>
<blockquote>
<h2>Version 3.1.3</h2>
<p>Released 2024-01-10</p>
<ul>
<li>Fix compiler error when checking if required blocks in parent templates are
empty. :pr:<code>1858</code></li>
<li><code>xmlattr</code> filter does not allow keys with spaces. GHSA-h5c8-rqwp-cp95</li>
<li>Make error messages stemming from invalid nesting of <code>{% trans %}</code> blocks
more helpful. :pr:<code>1918</code></li>
</ul>
<h2>Version 3.1.2</h2>
<p>Released 2022-04-28</p>
<ul>
<li>Add parameters to <code>Environment.overlay</code> to match <code>__init__</code>.
:issue:<code>1645</code></li>
<li>Handle race condition in <code>FileSystemBytecodeCache</code>. :issue:<code>1654</code></li>
</ul>
<h2>Version 3.1.1</h2>
<p>Released 2022-03-25</p>
<ul>
<li>The template filename on Windows uses the primary path separator.
:issue:<code>1637</code></li>
</ul>
<h2>Version 3.1.0</h2>
<p>Released 2022-03-24</p>
<ul>
<li>
<p>Drop support for Python 3.6. :pr:<code>1534</code></p>
</li>
<li>
<p>Remove previously deprecated code. :pr:<code>1544</code></p>
<ul>
<li><code>WithExtension</code> and <code>AutoEscapeExtension</code> are built-in now.</li>
<li><code>contextfilter</code> and <code>contextfunction</code> are replaced by
<code>pass_context</code>. <code>evalcontextfilter</code> and
<code>evalcontextfunction</code> are replaced by <code>pass_eval_context</code>.
<code>environmentfilter</code> and <code>environmentfunction</code> are replaced
by <code>pass_environment</code>.</li>
<li><code>Markup</code> and <code>escape</code> should be imported from MarkupSafe.</li>
<li>Compiled templates from very old Jinja versions may need to be
recompiled.</li>
<li>Legacy resolve mode for <code>Context</code> subclasses is no longer
supported. Override <code>resolve_or_missing</code> instead of</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/jinja/commit/d9de4bb215fd1cc8092a410fb834c7c4060b1fc1"><code>d9de4bb</code></a> release version 3.1.3</li>
<li><a href="https://github.com/pallets/jinja/commit/50124e16561f17f6c1ec85a692f6551418971cdc"><code>50124e1</code></a> skip test pypi</li>
<li><a href="https://github.com/pallets/jinja/commit/9ea7222ef3f184480be0d0884e30ccfb4172b17b"><code>9ea7222</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/da703f7aae36b1e88baaa20de334d7ff6378fdde"><code>da703f7</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/bce174692547464512383ec40e0f8338b8811983"><code>bce1746</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/7277d8068be593deab3555c7c14f974ada373af1"><code>7277d80</code></a> update pre-commit hooks</li>
<li><a href="https://github.com/pallets/jinja/commit/5c8a10522421270f66376a24ec8e0d6812bc4b14"><code>5c8a105</code></a> Make nested-trans-block exceptions nicer (<a href="https://redirect.github.com/pallets/jinja/issues/1918">#1918</a>)</li>
<li><a href="https://github.com/pallets/jinja/commit/19a55db3b411343309f2faaffaedbb089e841895"><code>19a55db</code></a> Make nested-trans-block exceptions nicer</li>
<li><a href="https://github.com/pallets/jinja/commit/716795349a41d4983a9a4771f7d883c96ea17be7"><code>7167953</code></a> Merge pull request from GHSA-h5c8-rqwp-cp95</li>
<li><a href="https://github.com/pallets/jinja/commit/7dd3680e6eea0d77fde024763657aa4d884ddb23"><code>7dd3680</code></a> xmlattr filter disallows keys with spaces</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/jinja/compare/2.11.3...3.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jinja2&package-manager=pip&previous-version=2.11.3&new-version=3.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/hyperledger-community-management-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 17:45:22 +0000 UTC
    </div>
</div>

