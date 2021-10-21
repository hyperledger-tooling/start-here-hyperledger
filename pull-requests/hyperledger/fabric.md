---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2992" class=".btn">#2992</a>
            </td>
            <td>
                <b>
                    Bump babel from 2.3.4 to 2.9.1 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [babel](https://github.com/python-babel/babel) from 2.3.4 to 2.9.1.
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
&lt;li&gt;Additional commits viewable in &lt;a href=&quot;https://github.com/python-babel/babel/compare/2.3.4...v2.9.1&quot;&gt;compare view&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;/details&gt;

&lt;br /&gt;
</code></pre>


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=babel&package-manager=pip&previous-version=2.3.4&new-version=2.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 17:53:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2991" class=".btn">#2991</a>
            </td>
            <td>
                <b>
                    fix Windows SyncDir issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

closes #2984 

#### Type of change

- Bug fix

#### Description

On windows it's not valid to invoke Sync on a directory, it results in an error "Handle is invalid"

#### Additional details

As windows is there only as a development platform, removing the attempt to Sync on a dir restores the ability for Peer and Orderer to run natively on Windows Desktop platforms.

Included as well is ensuring the downloadable windows package contains .exe files so they are usable straight away (no extra rename once unpacked is required)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 08:58:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2990" class=".btn">#2990</a>
            </td>
            <td>
                <b>
                    Possible way of adding external builders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 14:48:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2989" class=".btn">#2989</a>
            </td>
            <td>
                <b>
                    Fix typo on terminal command 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix
- Documentation update

#### Description

Fix typo on terminal command 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 09:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2988" class=".btn">#2988</a>
            </td>
            <td>
                <b>
                    Check the package name on core/ledger/kvledger UT (#2987)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Check the package name not local file name including "fabric/"
on core/ledger/kvledger unit test

`core/ledger/kvledger` unit-test has been failed on a directory that not "fabric".

Signed-off-by: Justin Yang <justin.yang@themedium.io>

#### Type of change
- Test update

#### Description
Check the error message without "`fabric/`" in `core/ledger/kvledger/snapshot_test.go`
When you run the unit-test in a directory that is not "`fabric`", that unit-test will fail because of checking the filename starting "`fabric/`".

#### Additional details
* Problem
`core/ledger/kvledger/` unit test fails when running the unit-test in another directory, not `fabric/`

```
--- FAIL: TestGenerateSnapshotErrors (13.43s)
    --- FAIL: TestGenerateSnapshotErrors/block_store_returns_error (1.10s)
        snapshot_test.go:571:
            	Error Trace:	snapshot_test.go:571
            	Error:      	"leveldb: closed\ninternal leveldb error while obtaining db iterator\ngithub.com/hyperledger/fabric/common/ledger/util/leveldbhelper.(*DBHandle).GetIterator\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/util/leveldbhelper/leveldb_provider.go:262\ngithub.com/hyperledger/fabric/common/ledger/blkstorage.(*blockIndex).exportUniqueTxIDs\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/blkstorage/blockindex.go:304\ngithub.com/hyperledger/fabric/common/ledger/blkstorage.(*BlockStore).ExportTxIds\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/blkstorage/blockstore.go:105\ngithub.com/hyperledger/fabric/core/ledger/kvledger.(*kvLedger).generateSnapshot\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot.go:114\ngithub.com/hyperledger/fabric/core/ledger/kvledger.TestGenerateSnapshotErrors.func4\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot_test.go:567\ntesting.tRunner\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/testing/testing.go:1050\nruntime.goexit\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/runtime/asm_amd64.s:1373" does not contain "fabric/common/ledger/blkstorage/blockindex.go"
            	Test:       	TestGenerateSnapshotErrors/block_store_returns_error
    --- FAIL: TestGenerateSnapshotErrors/config_history_mgr_returns_error (1.32s)
        snapshot_test.go:581:
            	Error Trace:	snapshot_test.go:581
            	Error:      	"leveldb: closed\ninternal leveldb error while obtaining db iterator\ngithub.com/hyperledger/fabric/common/ledger/util/leveldbhelper.(*DBHandle).GetIterator\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/util/leveldbhelper/leveldb_provider.go:262\ngithub.com/hyperledger/fabric/core/ledger/confighistory.(*db).getNamespaceIterator\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/confighistory/db_helper.go:114\ngithub.com/hyperledger/fabric/core/ledger/confighistory.(*Retriever).ExportConfigHistory\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/confighistory/mgr.go:221\ngithub.com/hyperledger/fabric/core/ledger/kvledger.(*kvLedger).generateSnapshot\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot.go:120\ngithub.com/hyperledger/fabric/core/ledger/kvledger.TestGenerateSnapshotErrors.func5\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot_test.go:577\ntesting.tRunner\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/testing/testing.go:1050\nruntime.goexit\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/runtime/asm_amd64.s:1373" does not contain "fabric/core/ledger/confighistory/mgr.go"
            	Test:       	TestGenerateSnapshotErrors/config_history_mgr_returns_error

(...)

FAIL
coverage: 78.8% of statements
FAIL	github.com/hyperledger/fabric/core/ledger/kvledger	583.226s
```

* Reproduce procedure
1. `$ git clone https://github.com/hyperledger/fabric.git fabrictest` or `$ mv fabric fabrictest`
2. `$ cd fabrictest`
3. `$ make unit-test`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 15:15:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2985" class=".btn">#2985</a>
            </td>
            <td>
                <b>
                    Gateway endorsement retry logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rather than selecting one layout from the discovery endorsement plan and failing if one of the endorsers fails, this commit attempts to create a set of endorsements by retrying the proposal on other endorser until one of the layouts is satisfied.
Additionally, rather than connect to all peers in a channel once on first usage and then never update that cache, this commit adds support for later additions and removals to/from the cache and closing stale connections to peers.

Resolves #2914 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 15:20:08 +0000 UTC
    </div>
</div>

