---
layout: default
title: pluggable-hcs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pluggable-hcs
---

# pluggable-hcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pluggable-hcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Bump babel from 2.7.0 to 2.9.1 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [babel](https://github.com/python-babel/babel) from 2.7.0 to 2.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-babel/babel/releases">babel's releases</a>.</em></p>
<blockquote>
<h2>Version 2.9.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>The internal locale-data loading functions now validate the name of the locale file to be loaded and only allow files within Babel's data directory.  Thank you to Chris Lyne of Tenable, Inc. for discovering the issue!</li>
</ul>
<h2>Version 2.9.0</h2>
<h1>Upcoming version support changes</h1>
<ul>
<li>This version, Babel 2.9, is the last version of Babel to support Python 2.7, Python 3.4, and Python 3.5.</li>
</ul>
<h1>Improvements</h1>
<ul>
<li>CLDR: Use CLDR 37 – Aarni Koskela (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/734">#734</a>)</li>
<li>Dates: Handle ZoneInfo objects in get_timezone_location, get_timezone_name - Alessio Bogon (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/741">#741</a>)</li>
<li>Numbers: Add group_separator feature in number formatting - Abdullah Javed Nesar (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/726">#726</a>)</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>Dates: Correct default Format().timedelta format to 'long' to mute deprecation warnings – Aarni Koskela</li>
<li>Import: Simplify iteration code in &quot;import_cldr.py&quot; – Felix Schwarz</li>
<li>Import: Stop using deprecated ElementTree methods &quot;getchildren()&quot; and &quot;getiterator()&quot; – Felix Schwarz</li>
<li>Messages: Fix unicode printing error on Python 2 without TTY. – Niklas Hambüchen</li>
<li>Messages: Introduce invariant that _invalid_pofile() takes unicode line. – Niklas Hambüchen</li>
<li>Tests: fix tests when using Python 3.9 – Felix Schwarz</li>
<li>Tests: Remove deprecated 'sudo: false' from Travis configuration – Jon Dufresne</li>
<li>Tests: Support Py.test 6.x – Aarni Koskela</li>
<li>Utilities: LazyProxy: Handle AttributeError in specified func – Nikiforov Konstantin (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/724">#724</a>)</li>
<li>Utilities: Replace usage of parser.suite with ast.parse – Miro Hrončok</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>Update parse_number comments – Brad Martin (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/708">#708</a>)</li>
<li>Add <strong>iter</strong> to Catalog documentation – <a href="https://github.com/CyanNani123"><code>@​CyanNani123</code></a></li>
</ul>
<h2>Version 2.8.1</h2>
<p>This patch version only differs from 2.8.0 in that it backports in <a href="https://github-redirect.dependabot.com/python-babel/babel/issues/752">#752</a>.</p>
<h2>Version 2.8.0</h2>
<h1>Improvements</h1>
<ul>
<li>CLDR: Upgrade to CLDR 36.0 - Aarni Koskela (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/679">#679</a>)</li>
<li>Messages: Don't even open files with the &quot;ignore&quot; extraction method - <a href="https://github.com/sebleblanc"><code>@​sebleblanc</code></a> (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/678">#678</a>)</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>Numbers: Fix formatting very small decimals when quantization is disabled - Lev Lybin, <a href="https://github.com/miluChen"><code>@​miluChen</code></a> (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/662">#662</a>)</li>
<li>Messages: Attempt to sort all messages – Mario Frasca (<a href="https://github-redirect.dependabot.com/python-babel/babel/issues/651">#651</a>, <a href="https://github-redirect.dependabot.com/python-babel/babel/issues/606">#606</a>)</li>
</ul>
<h1>Docs</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-babel/babel/blob/master/CHANGES">babel's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.9.1</h2>
<p>Bugfixes</p>
<pre><code>
* The internal locale-data loading functions now validate the name of the locale file to be loaded and only
  allow files within Babel's data directory.  Thank you to Chris Lyne of Tenable, Inc. for discovering the issue!
<h2>Version 2.9.0</h2>
<p>Upcoming version support changes
</code></pre></p>
<ul>
<li>This version, Babel 2.9, is the last version of Babel to support Python 2.7, Python 3.4, and Python 3.5.</li>
</ul>
<p>Improvements</p>
<pre><code>
* CLDR: Use CLDR 37 – Aarni Koskela ([#734](https://github.com/python-babel/babel/issues/734))
* Dates: Handle ZoneInfo objects in get_timezone_location, get_timezone_name - Alessio Bogon ([#741](https://github.com/python-babel/babel/issues/741))
* Numbers: Add group_separator feature in number formatting - Abdullah Javed Nesar ([#726](https://github.com/python-babel/babel/issues/726))
<p>Bugfixes</p>
<pre><code>
* Dates: Correct default Format().timedelta format to 'long' to mute deprecation warnings – Aarni Koskela
* Import: Simplify iteration code in &amp;quot;import_cldr.py&amp;quot; – Felix Schwarz
* Import: Stop using deprecated ElementTree methods &amp;quot;getchildren()&amp;quot; and &amp;quot;getiterator()&amp;quot; – Felix Schwarz
* Messages: Fix unicode printing error on Python 2 without TTY. – Niklas Hambüchen
* Messages: Introduce invariant that _invalid_pofile() takes unicode line. – Niklas Hambüchen
* Tests: fix tests when using Python 3.9 – Felix Schwarz
* Tests: Remove deprecated 'sudo: false' from Travis configuration – Jon Dufresne
* Tests: Support Py.test 6.x – Aarni Koskela
* Utilities: LazyProxy: Handle AttributeError in specified func – Nikiforov Konstantin ([#724](https://github.com/python-babel/babel/issues/724))
* Utilities: Replace usage of parser.suite with ast.parse – Miro Hrončok

Documentation
&lt;/code&gt;&lt;/pre&gt;
&lt;ul&gt;
&lt;li&gt;Update parse_number comments – Brad Martin (&lt;a href=&quot;https://github-redirect.dependabot.com/python-babel/babel/issues/708&quot;&gt;#708&lt;/a&gt;)&lt;/li&gt;
&lt;li&gt;Add &lt;strong&gt;iter&lt;/strong&gt; to Catalog documentation – &lt;a href=&quot;https://github.com/CyanNani123&quot;&gt;&lt;code&gt;@​CyanNani123&lt;/code&gt;&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;h2&gt;Version 2.8.1&lt;/h2&gt;
&lt;p&gt;This is solely a patch release to make running tests on Py.test 6+ possible.&lt;/p&gt;
&lt;p&gt;Bugfixes&lt;/p&gt;
&lt;!-- raw HTML omitted --&gt;
&lt;/blockquote&gt;
&lt;p&gt;... (truncated)&lt;/p&gt;
&lt;/details&gt;
&lt;details&gt;
&lt;summary&gt;Commits&lt;/summary&gt;

&lt;ul&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/a99fa2474c808b51ebdabea18db871e389751559&quot;&gt;&lt;code&gt;a99fa24&lt;/code&gt;&lt;/a&gt; Use 2.9.0's setup.py for 2.9.1&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/60b33e083801109277cb068105251e76d0b7c14e&quot;&gt;&lt;code&gt;60b33e0&lt;/code&gt;&lt;/a&gt; Become 2.9.1&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/412015ef642bfcc0d8ba8f4d05cdbb6aac98d9b3&quot;&gt;&lt;code&gt;412015e&lt;/code&gt;&lt;/a&gt; Merge pull request &lt;a href=&quot;https://github-redirect.dependabot.com/python-babel/babel/issues/782&quot;&gt;#782&lt;/a&gt; from python-babel/locale-basename&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/5caf717ceca4bd235552362b4fbff88983c75d8c&quot;&gt;&lt;code&gt;5caf717&lt;/code&gt;&lt;/a&gt; Disallow special filenames on Windows&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/3a700b5b8b53606fd98ef8294a56f9510f7290f8&quot;&gt;&lt;code&gt;3a700b5&lt;/code&gt;&lt;/a&gt; Run locale identifiers through &lt;code&gt;os.path.basename()&lt;/code&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/5afe2b2f11dcdd6090c00231d342c2e9cd1bdaab&quot;&gt;&lt;code&gt;5afe2b2&lt;/code&gt;&lt;/a&gt; Merge pull request &lt;a href=&quot;https://github-redirect.dependabot.com/python-babel/babel/issues/754&quot;&gt;#754&lt;/a&gt; from python-babel/github-ci&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/58de8342f865df88697a4a166191e880e3c84d82&quot;&gt;&lt;code&gt;58de834&lt;/code&gt;&lt;/a&gt; Replace Travis + Appveyor with GitHub Actions (WIP)&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/d1bbc08e845d03d8e1f0dfa0e04983d755f39cb5&quot;&gt;&lt;code&gt;d1bbc08&lt;/code&gt;&lt;/a&gt; import_cldr: use logging; add -q option&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/156b7fb9f377ccf58c71cf01dc69fb10c7b69314&quot;&gt;&lt;code&gt;156b7fb&lt;/code&gt;&lt;/a&gt; Quiesce CLDR download progress bar if requested (or not a TTY)&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://github.com/python-babel/babel/commit/613dc1700f91c3d40b081948c0dd6023d8ece057&quot;&gt;&lt;code&gt;613dc17&lt;/code&gt;&lt;/a&gt; Make the import warnings about unsupported number systems less verbose&lt;/li&gt;
&lt;li&gt;Additional commits viewable in &lt;a href=&quot;https://github.com/python-babel/babel/compare/v2.7.0...v2.9.1&quot;&gt;compare view&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;/details&gt;

&lt;br /&gt;
</code></pre>


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=babel&package-manager=pip&previous-version=2.7.0&new-version=2.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pluggable-hcs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 18:43:22 +0000 UTC
    </div>
</div>

