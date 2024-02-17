---
layout: default
title: aries-mobile-agent-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-react-native
---

# aries-mobile-agent-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1093" class=".btn">#1093</a>
            </td>
            <td>
                <b>
                    fix: test ids on wallet name edit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This change fixes some missing test IDs on the wallet name edit button and re-uses an existing component rather for a little more consistency in resuability.

# Related Issues

n/a

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 22:10:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1092" class=".btn">#1092</a>
            </td>
            <td>
                <b>
                    chore(deps): bump the all-actions group with 5 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 5 updates:

| Package | From | To |
| --- | --- | --- |
| [actions/setup-python](https://github.com/actions/setup-python) | `4` | `5` |
| [actions/cache](https://github.com/actions/cache) | `3` | `4` |
| [actions/setup-java](https://github.com/actions/setup-java) | `3` | `4` |
| [codecov/codecov-action](https://github.com/codecov/codecov-action) | `3` | `4` |
| [actions/upload-artifact](https://github.com/actions/upload-artifact) | `3` | `4` |

Updates `actions/setup-python` from 4 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-python/releases">actions/setup-python's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<h2>What's Changed</h2>
<p>In scope of this release, we update node version runtime from node16 to node20 (<a href="https://redirect.github.com/actions/setup-python/pull/772">actions/setup-python#772</a>). Besides, we update dependencies to the latest versions.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4.8.0...v5.0.0">https://github.com/actions/setup-python/compare/v4.8.0...v5.0.0</a></p>
<h2>v4.8.0</h2>
<h2>What's Changed</h2>
<p>In scope of this release we added support for GraalPy (<a href="https://redirect.github.com/actions/setup-python/pull/694">actions/setup-python#694</a>). You can use this snippet to set up GraalPy:</p>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v4
- uses: actions/setup-python@v4 
  with:
    python-version: 'graalpy-22.3' 
- run: python my_script.py
</code></pre>
<p>Besides, the release contains such changes as:</p>
<ul>
<li>Trim python version when reading from file by <a href="https://github.com/FerranPares"><code>@​FerranPares</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/628">actions/setup-python#628</a></li>
<li>Use non-deprecated versions in examples by <a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/724">actions/setup-python#724</a></li>
<li>Change deprecation comment to past tense by <a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/723">actions/setup-python#723</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.9.0 to 7.23.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/743">actions/setup-python#743</a></li>
<li>advanced-usage.md: Encourage the use actions/checkout@v4 by <a href="https://github.com/cclauss"><code>@​cclauss</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/729">actions/setup-python#729</a></li>
<li>Examples now use checkout@v4 by <a href="https://github.com/simonw"><code>@​simonw</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/738">actions/setup-python#738</a></li>
<li>Update actions/checkout to v4 by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/761">actions/setup-python#761</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/FerranPares"><code>@​FerranPares</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/628">actions/setup-python#628</a></li>
<li><a href="https://github.com/timfel"><code>@​timfel</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/694">actions/setup-python#694</a></li>
<li><a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/724">actions/setup-python#724</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4...v4.8.0">https://github.com/actions/setup-python/compare/v4...v4.8.0</a></p>
<h2>v4.7.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump word-wrap from 1.2.3 to 1.2.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/702">actions/setup-python#702</a></li>
<li>Add range validation for toml files by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/726">actions/setup-python#726</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4...v4.7.1">https://github.com/actions/setup-python/compare/v4...v4.7.1</a></p>
<h2>v4.7.0</h2>
<p>In scope of this release, the support for reading python version from pyproject.toml was added (<a href="https://redirect.github.com/actions/setup-python/pull/669">actions/setup-python#669</a>).</p>
<pre lang="yaml"><code>      - name: Setup Python
        uses: actions/setup-python@v4
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-python/commit/0a5c61591373683505ea898e09a3ea4f39ef2b9c"><code>0a5c615</code></a> Update action to node20 (<a href="https://redirect.github.com/actions/setup-python/issues/772">#772</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/0ae58361cdfd39e2950bed97a1e26aa20c3d8955"><code>0ae5836</code></a> Add example of GraalPy to docs (<a href="https://redirect.github.com/actions/setup-python/issues/773">#773</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/b64ffcaf5b410884ad320a9cfac8866006a109aa"><code>b64ffca</code></a> update actions/checkout to v4 (<a href="https://redirect.github.com/actions/setup-python/issues/761">#761</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/8d2896179abf658742de432b3f203d2c2d86a587"><code>8d28961</code></a> Examples now use checkout@v4 (<a href="https://redirect.github.com/actions/setup-python/issues/738">#738</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/7bc6abb01e0555719edc2dbca70a2fde309e5e56"><code>7bc6abb</code></a> advanced-usage.md: Encourage the use actions/checkout@v4 (<a href="https://redirect.github.com/actions/setup-python/issues/729">#729</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/e8111cec9d3dc15220d8a3b638f08419f57b906a"><code>e8111ce</code></a> Bump <code>@​babel/traverse</code> from 7.9.0 to 7.23.2 (<a href="https://redirect.github.com/actions/setup-python/issues/743">#743</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/a00ea43da65e7c04d2bdae58b3afecd77057eb9e"><code>a00ea43</code></a> add fix for graalpy ci (<a href="https://redirect.github.com/actions/setup-python/issues/741">#741</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/8635b1ccc5934e73ed3510980fd2e7790b85839b"><code>8635b1c</code></a> Change deprecation comment to past tense (<a href="https://redirect.github.com/actions/setup-python/issues/723">#723</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/f6cc428f535856f9c23558d01765a42a4d6cf758"><code>f6cc428</code></a> Use non-deprecated versions in examples (<a href="https://redirect.github.com/actions/setup-python/issues/724">#724</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/5f2af211d616f86005883b44826180b21abb4060"><code>5f2af21</code></a> Add GraalPy support (<a href="https://redirect.github.com/actions/setup-python/issues/694">#694</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-python/compare/v4...v5">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/cache` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/releases">actions/cache's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update action to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li>feat: save-always flag by <a href="https://github.com/to-s"><code>@​to-s</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li><a href="https://github.com/to-s"><code>@​to-s</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v4.0.0">https://github.com/actions/cache/compare/v3...v4.0.0</a></p>
<h2>v3.3.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Cache v3.3.3 by <a href="https://github.com/robherley"><code>@​robherley</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/robherley"><code>@​robherley</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.3">https://github.com/actions/cache/compare/v3...v3.3.3</a></p>
<h2>v3.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fixed readme with new segment timeout values by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1133">actions/cache#1133</a></li>
<li>Readme fixes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1134">actions/cache#1134</a></li>
<li>Updated description of the lookup-only input for main action by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1130">actions/cache#1130</a></li>
<li>Change two new actions mention as quoted text by <a href="https://github.com/bishal-pdMSFT"><code>@​bishal-pdMSFT</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1131">actions/cache#1131</a></li>
<li>Update Cross-OS Caching tips by <a href="https://github.com/pdotl"><code>@​pdotl</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1122">actions/cache#1122</a></li>
<li>Bazel example (Take <a href="https://redirect.github.com/actions/cache/issues/2">#2</a>️⃣) by <a href="https://github.com/vorburger"><code>@​vorburger</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li>Remove actions to add new PRs and issues to a project board by <a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li>Consume latest toolkit and fix dangling promise bug by <a href="https://github.com/chkimes"><code>@​chkimes</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li>Bump action version to 3.3.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vorburger"><code>@​vorburger</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li><a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li><a href="https://github.com/chkimes"><code>@​chkimes</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li><a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.2">https://github.com/actions/cache/compare/v3...v3.3.2</a></p>
<h2>v3.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Reduced download segment size to 128 MB and timeout to 10 minutes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1129">actions/cache#1129</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.1">https://github.com/actions/cache/compare/v3...v3.3.1</a></p>
<h2>v3.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bug: Permission is missing in cache delete example by <a href="https://github.com/kotokaze"><code>@​kotokaze</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1123">actions/cache#1123</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/blob/main/RELEASES.md">actions/cache's changelog</a>.</em></p>
<blockquote>
<h1>Releases</h1>
<h3>3.0.0</h3>
<ul>
<li>Updated minimum runner version support from node 12 -&gt; node 16</li>
</ul>
<h3>3.0.1</h3>
<ul>
<li>Added support for caching from GHES 3.5.</li>
<li>Fixed download issue for files &gt; 2GB during restore.</li>
</ul>
<h3>3.0.2</h3>
<ul>
<li>Added support for dynamic cache size cap on GHES.</li>
</ul>
<h3>3.0.3</h3>
<ul>
<li>Fixed avoiding empty cache save when no files are available for caching. (<a href="https://redirect.github.com/actions/cache/issues/624">issue</a>)</li>
</ul>
<h3>3.0.4</h3>
<ul>
<li>Fixed tar creation error while trying to create tar with path as <code>~/</code> home folder on <code>ubuntu-latest</code>. (<a href="https://redirect.github.com/actions/cache/issues/689">issue</a>)</li>
</ul>
<h3>3.0.5</h3>
<ul>
<li>Removed error handling by consuming actions/cache 3.0 toolkit, Now cache server error handling will be done by toolkit. (<a href="https://redirect.github.com/actions/cache/pull/834">PR</a>)</li>
</ul>
<h3>3.0.6</h3>
<ul>
<li>Fixed <a href="https://redirect.github.com/actions/cache/issues/809">#809</a> - zstd -d: no such file or directory error</li>
<li>Fixed <a href="https://redirect.github.com/actions/cache/issues/833">#833</a> - cache doesn't work with github workspace directory</li>
</ul>
<h3>3.0.7</h3>
<ul>
<li>Fixed <a href="https://redirect.github.com/actions/cache/issues/810">#810</a> - download stuck issue. A new timeout is introduced in the download process to abort the download if it gets stuck and doesn't finish within an hour.</li>
</ul>
<h3>3.0.8</h3>
<ul>
<li>Fix zstd not working for windows on gnu tar in issues <a href="https://redirect.github.com/actions/cache/issues/888">#888</a> and <a href="https://redirect.github.com/actions/cache/issues/891">#891</a>.</li>
<li>Allowing users to provide a custom timeout as input for aborting download of a cache segment using an environment variable <code>SEGMENT_DOWNLOAD_TIMEOUT_MINS</code>. Default is 60 minutes.</li>
</ul>
<h3>3.0.9</h3>
<ul>
<li>Enhanced the warning message for cache unavailablity in case of GHES.</li>
</ul>
<h3>3.0.10</h3>
<ul>
<li>Fix a bug with sorting inputs.</li>
<li>Update definition for restore-keys in README.md</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/cache/commit/13aacd865c20de90d75de3b17ebe84f7a17d57d2"><code>13aacd8</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1242">#1242</a> from to-s/main</li>
<li><a href="https://github.com/actions/cache/commit/53b35c543921fe2e8b288765ff817de9de8d906f"><code>53b35c5</code></a> Merge branch 'main' into main</li>
<li><a href="https://github.com/actions/cache/commit/65b8989fab3bb394817bdb845a453dff480c2b51"><code>65b8989</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1284">#1284</a> from takost/update-to-node-20</li>
<li><a href="https://github.com/actions/cache/commit/d0be34d54485f31ca2ccbe66e6ea3d96544a807b"><code>d0be34d</code></a> Fix dist</li>
<li><a href="https://github.com/actions/cache/commit/66cf064d47313d2cccf392d01bd10925da2bd072"><code>66cf064</code></a> Merge branch 'main' into update-to-node-20</li>
<li><a href="https://github.com/actions/cache/commit/1326563738ddb735c5f2ce85cba8c79f33b728cd"><code>1326563</code></a> Merge branch 'main' into main</li>
<li><a href="https://github.com/actions/cache/commit/e71876755e268d6cc25a5d3e3c46ae447e35290a"><code>e718767</code></a> Fix format</li>
<li><a href="https://github.com/actions/cache/commit/01229828ffa049a8dee4db27bcb23ed33f2b451f"><code>0122982</code></a> Apply workaround for earlyExit</li>
<li><a href="https://github.com/actions/cache/commit/3185ecfd6135856ca6d904ae032cff4f39b8b365"><code>3185ecf</code></a> Update &quot;only-&quot; actions to node20</li>
<li><a href="https://github.com/actions/cache/commit/25618a0a675e8447e5ffc8ed9b7ddb2aaf927f65"><code>25618a0</code></a> Bump version</li>
<li>Additional commits viewable in <a href="https://github.com/actions/cache/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/setup-java` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-java/releases">actions/setup-java's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>In the scope of this release, the version of the Node.js runtime was updated to 20. The majority of dependencies were updated to the latest versions. From now on, the code for the setup-java will run on Node.js 20 instead of Node.js 16.</p>
<h2>Breaking changes</h2>
<ul>
<li>Update Node.js runtime to version 20 by <a href="https://github.com/aparnajyothi-y"><code>@​aparnajyothi-y</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/558">actions/setup-java#558</a></li>
</ul>
<h2>Non-breaking changes</h2>
<ul>
<li>Adding support for microsoft openjdk 21.0.0 by <a href="https://github.com/ralfstuckert"><code>@​ralfstuckert</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/546">actions/setup-java#546</a></li>
<li>Update <code>@​actions/cache</code> dependency and documentation by <a href="https://github.com/IvanZosimov"><code>@​IvanZosimov</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/549">actions/setup-java#549</a></li>
<li>Implementation of the cache-dependency-path option to control caching dependency by <a href="https://github.com/itchyny"><code>@​itchyny</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/499">actions/setup-java#499</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ralfstuckert"><code>@​ralfstuckert</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/546">actions/setup-java#546</a></li>
<li><a href="https://github.com/itchyny"><code>@​itchyny</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/499">actions/setup-java#499</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-java/compare/v3...v4.0.0">https://github.com/actions/setup-java/compare/v3...v4.0.0</a></p>
<h2>v3.13.0</h2>
<h2>What's changed</h2>
<p>In the scope of this release, support for Dragonwell JDK was added by <a href="https://github.com/Accelerator1996"><code>@​Accelerator1996</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/532">actions/setup-java#532</a></p>
<pre lang="yaml"><code>steps:
 - name: Checkout
   uses: actions/checkout@v3
 - name: Setup-java
   uses: actions/setup-java@v3
   with:
     distribution: 'dragonwell'
     java-version: '17'
</code></pre>
<p>Several inaccuracies were also fixed:</p>
<ul>
<li>Fix XML namespaces wrongly using https by <a href="https://github.com/gnodet"><code>@​gnodet</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/503">actions/setup-java#503</a></li>
<li>Fix typo and remove unintentional(?) word by <a href="https://github.com/CyberFlameGO"><code>@​CyberFlameGO</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/518">actions/setup-java#518</a></li>
<li>Fix usage link within the README.md file by <a href="https://github.com/dassiorleando"><code>@​dassiorleando</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/525">actions/setup-java#525</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/CyberFlameGO"><code>@​CyberFlameGO</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/518">actions/setup-java#518</a></li>
<li><a href="https://github.com/dassiorleando"><code>@​dassiorleando</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/525">actions/setup-java#525</a></li>
<li><a href="https://github.com/gnodet"><code>@​gnodet</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/503">actions/setup-java#503</a></li>
<li><a href="https://github.com/Accelerator1996"><code>@​Accelerator1996</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/532">actions/setup-java#532</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-java/compare/v3...v3.13.0">https://github.com/actions/setup-java/compare/v3...v3.13.0</a></p>
<h2>v3.12.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-java/commit/387ac29b308b003ca37ba93a6cab5eb57c8f5f93"><code>387ac29</code></a> Upgrade Node to v20 (<a href="https://redirect.github.com/actions/setup-java/issues/558">#558</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/9eda6b51cc4f6ee99be3dd5537b85e389e47bda9"><code>9eda6b5</code></a> feat: implement cache-dependency-path option to control caching dependency (#...</li>
<li><a href="https://github.com/actions/setup-java/commit/78078da0cd035d0d177cc2cb696e05d96fba7d11"><code>78078da</code></a> Update <code>@​actions/cache</code> dependency and documentation (<a href="https://redirect.github.com/actions/setup-java/issues/549">#549</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/5caaba646e214abb5c4c808eb8fe13db519ab757"><code>5caaba6</code></a> add support for microsoft openjdk 21.0.0 (<a href="https://redirect.github.com/actions/setup-java/issues/546">#546</a>)</li>
<li>See full diff in <a href="https://github.com/actions/setup-java/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `codecov/codecov-action` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/releases">codecov/codecov-action's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<p>v4 of the Codecov Action uses the <a href="https://docs.codecov.com/docs/the-codecov-cli">CLI</a> as the underlying upload. The CLI has helped to power new features including local upload, the global upload token, and new upcoming features.</p>
<h2>Breaking Changes</h2>
<ul>
<li>The Codecov Action runs as a <code>node20</code> action due to <code>node16</code> deprecation. See <a href="https://github.blog/changelog/2023-09-22-github-actions-transitioning-from-node-16-to-node-20/">this post from GitHub</a> on how to migrate.</li>
<li>Tokenless uploading is unsupported. However, PRs made from forks to the upstream public repos will support tokenless (e.g. contributors to OS projects do not need the upstream repo's Codecov token). This <a href="https://docs.codecov.com/docs/adding-the-codecov-token#github-actions">doc</a> shows instructions on how to add the Codecov token.</li>
<li>OS platforms have been added, though some may not be automatically detected. To see a list of platforms, see our <a href="https://cli.codecov.io">CLI download page</a></li>
<li>Various arguments to the Action have been changed. Please be aware that the arguments match with the CLI's needs</li>
</ul>
<p><code>v3</code> versions and below will not have access to CLI features (e.g. global upload token, ATS).</p>
<h2>What's Changed</h2>
<ul>
<li>build(deps): bump openpgp from 5.8.0 to 5.9.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/985">codecov/codecov-action#985</a></li>
<li>build(deps): bump actions/checkout from 3.0.0 to 3.5.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1000">codecov/codecov-action#1000</a></li>
<li>build(deps): bump ossf/scorecard-action from 2.1.3 to 2.2.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1006">codecov/codecov-action#1006</a></li>
<li>build(deps): bump tough-cookie from 4.0.0 to 4.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1013">codecov/codecov-action#1013</a></li>
<li>build(deps-dev): bump word-wrap from 1.2.3 to 1.2.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1024">codecov/codecov-action#1024</a></li>
<li>build(deps): bump node-fetch from 3.3.1 to 3.3.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1031">codecov/codecov-action#1031</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.1.4 to 20.4.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1032">codecov/codecov-action#1032</a></li>
<li>build(deps): bump github/codeql-action from 1.0.26 to 2.21.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1033">codecov/codecov-action#1033</a></li>
<li>build commit,report and upload args based on codecovcli by <a href="https://github.com/dana-yaish"><code>@​dana-yaish</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/943">codecov/codecov-action#943</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.4.5 to 20.5.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1055">codecov/codecov-action#1055</a></li>
<li>build(deps): bump github/codeql-action from 2.21.2 to 2.21.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1051">codecov/codecov-action#1051</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.5.3 to 20.5.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1058">codecov/codecov-action#1058</a></li>
<li>chore(deps): update outdated deps by <a href="https://github.com/thomasrockhu-codecov"><code>@​thomasrockhu-codecov</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1059">codecov/codecov-action#1059</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.5.4 to 20.5.6 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1060">codecov/codecov-action#1060</a></li>
<li>build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 6.4.1 to 6.5.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1065">codecov/codecov-action#1065</a></li>
<li>build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 6.4.1 to 6.5.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1064">codecov/codecov-action#1064</a></li>
<li>build(deps): bump actions/checkout from 3.5.3 to 3.6.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1063">codecov/codecov-action#1063</a></li>
<li>build(deps-dev): bump eslint from 8.47.0 to 8.48.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1061">codecov/codecov-action#1061</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.5.6 to 20.5.7 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1062">codecov/codecov-action#1062</a></li>
<li>build(deps): bump openpgp from 5.9.0 to 5.10.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1066">codecov/codecov-action#1066</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.5.7 to 20.5.9 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1070">codecov/codecov-action#1070</a></li>
<li>build(deps): bump github/codeql-action from 2.21.4 to 2.21.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1069">codecov/codecov-action#1069</a></li>
<li>build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 6.5.0 to 6.6.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1072">codecov/codecov-action#1072</a></li>
<li>Update README.md by <a href="https://github.com/thomasrockhu-codecov"><code>@​thomasrockhu-codecov</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1073">codecov/codecov-action#1073</a></li>
<li>build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 6.5.0 to 6.6.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1071">codecov/codecov-action#1071</a></li>
<li>build(deps-dev): bump <code>@​vercel/ncc</code> from 0.36.1 to 0.38.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1074">codecov/codecov-action#1074</a></li>
<li>build(deps): bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1081">codecov/codecov-action#1081</a></li>
<li>build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 6.6.0 to 6.7.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1080">codecov/codecov-action#1080</a></li>
<li>build(deps): bump actions/checkout from 3.6.0 to 4.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1078">codecov/codecov-action#1078</a></li>
<li>build(deps): bump actions/upload-artifact from 3.1.2 to 3.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1077">codecov/codecov-action#1077</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.5.9 to 20.6.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1075">codecov/codecov-action#1075</a></li>
<li>build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 6.6.0 to 6.7.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1079">codecov/codecov-action#1079</a></li>
<li>build(deps-dev): bump eslint from 8.48.0 to 8.49.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1076">codecov/codecov-action#1076</a></li>
<li>use cli instead of node uploader by <a href="https://github.com/dana-yaish"><code>@​dana-yaish</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1068">codecov/codecov-action#1068</a></li>
<li>chore(release): 4.0.0-beta.1 by <a href="https://github.com/thomasrockhu-codecov"><code>@​thomasrockhu-codecov</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1084">codecov/codecov-action#1084</a></li>
<li>not adding -n if empty to do-upload command by <a href="https://github.com/dana-yaish"><code>@​dana-yaish</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1085">codecov/codecov-action#1085</a></li>
<li>4.0.0-beta.2 by <a href="https://github.com/thomasrockhu-codecov"><code>@​thomasrockhu-codecov</code></a> in <a href="https://redirect.github.com/codecov/codecov-action/pull/1086">codecov/codecov-action#1086</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/blob/main/CHANGELOG.md">codecov/codecov-action's changelog</a>.</em></p>
<blockquote>
<h2>4.0.0-beta.2</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/1085">#1085</a> not adding -n if empty to do-upload command</li>
</ul>
<h2>4.0.0-beta.1</h2>
<p><code>v4</code> represents a move from the <a href="https://github.com/codecov/uploader">universal uploader</a> to the <a href="https://github.com/codecov/codecov-cli">Codecov CLI</a>. Although this will unlock new features for our users, the CLI is not yet at feature parity with the universal uploader.</p>
<h3>Breaking Changes</h3>
<ul>
<li>No current support for <code>aarch64</code> and <code>alpine</code> architectures.</li>
<li>Tokenless uploading is unsuported</li>
<li>Various arguments to the Action have been removed</li>
</ul>
<h2>3.1.4</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/967">#967</a> Fix typo in README.md</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/971">#971</a> fix: add back in working dir</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/969">#969</a> fix: CLI option names for uploader</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/970">#970</a> build(deps-dev): bump <code>@​types/node</code> from 18.15.12 to 18.16.3</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/979">#979</a> build(deps-dev): bump <code>@​types/node</code> from 20.1.0 to 20.1.2</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/981">#981</a> build(deps-dev): bump <code>@​types/node</code> from 20.1.2 to 20.1.4</li>
</ul>
<h2>3.1.3</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/960">#960</a> fix: allow for aarch64 build</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/957">#957</a> build(deps-dev): bump jest-junit from 15.0.0 to 16.0.0</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/958">#958</a> build(deps): bump openpgp from 5.7.0 to 5.8.0</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/959">#959</a> build(deps-dev): bump <code>@​types/node</code> from 18.15.10 to 18.15.12</li>
</ul>
<h2>3.1.2</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/718">#718</a> Update README.md</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/851">#851</a> Remove unsupported path_to_write_report argument</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/898">#898</a> codeql-analysis.yml</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/901">#901</a> Update README to contain correct information - inputs and negate feature</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/955">#955</a> fix: add in all the extra arguments for uploader</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/819">#819</a> build(deps): bump openpgp from 5.4.0 to 5.5.0</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/835">#835</a> build(deps): bump node-fetch from 3.2.4 to 3.2.10</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/840">#840</a> build(deps): bump ossf/scorecard-action from 1.1.1 to 2.0.4</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/841">#841</a> build(deps): bump <code>@​actions/core</code> from 1.9.1 to 1.10.0</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/843">#843</a> build(deps): bump <code>@​actions/github</code> from 5.0.3 to 5.1.1</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/869">#869</a> build(deps): bump node-fetch from 3.2.10 to 3.3.0</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/872">#872</a> build(deps-dev): bump jest-junit from 13.2.0 to 15.0.0</li>
<li><a href="https://redirect.github.com/codecov/codecov-action/issues/879">#879</a> build(deps): bump decode-uri-component from 0.2.0 to 0.2.2</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/codecov/codecov-action/commit/e0b68c6749509c5f83f984dd99a76a1c1a231044"><code>e0b68c6</code></a> fix: show both token uses in readme (<a href="https://redirect.github.com/codecov/codecov-action/issues/1250">#1250</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/1f9f5573d12d0967fe14551018a4b25610226551"><code>1f9f557</code></a> Add all args (<a href="https://redirect.github.com/codecov/codecov-action/issues/1245">#1245</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/09686fcfcb6453414a5acd7f3a939670a7a77826"><code>09686fc</code></a> Update README.md (<a href="https://redirect.github.com/codecov/codecov-action/issues/1243">#1243</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/f30e4959ba63075080d4f7f90cacc18d9f3fafd7"><code>f30e495</code></a> fix: update action.yml (<a href="https://redirect.github.com/codecov/codecov-action/issues/1240">#1240</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/a7b945cea47ad44d8340fae2b004cb982191264f"><code>a7b945c</code></a> fix: allow for other archs (<a href="https://redirect.github.com/codecov/codecov-action/issues/1239">#1239</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/98ab2c591b94478f4c3606d68ff73601df85ec43"><code>98ab2c5</code></a> Update package.json (<a href="https://redirect.github.com/codecov/codecov-action/issues/1238">#1238</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/43235cc5aeeafd8aeb836fe7d647599acead161c"><code>43235cc</code></a> Update README.md (<a href="https://redirect.github.com/codecov/codecov-action/issues/1237">#1237</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/0cf8684c821546a4e0c8c9a4cf4f21a7a0c5014b"><code>0cf8684</code></a> chore(ci): bump to node20 (<a href="https://redirect.github.com/codecov/codecov-action/issues/1236">#1236</a>)</li>
<li><a href="https://github.com/codecov/codecov-action/commit/8e1e730371bf82c744e8ca9aa469e2b7011542ce"><code>8e1e730</code></a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 6.19.1 to 6.20.0 ...</li>
<li><a href="https://github.com/codecov/codecov-action/commit/61293af0e8288c75266030376a088c781ec81c18"><code>61293af</code></a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 6.19.1 to 6.20.0 (<a href="https://redirect.github.com/codecov/codecov-action/issues/1235">#1235</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/codecov/codecov-action/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/upload-artifact` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>The release of upload-artifact@v4 and download-artifact@v4 are major changes to the backend architecture of Artifacts. They have numerous performance and behavioral improvements.</p>
<p>ℹ️ However, this is a major update that includes breaking changes. Artifacts created with versions v3 and below are not compatible with the v4 actions. Uploads and downloads <em>must</em> use the same major actions versions. There are also key differences from previous versions that may require updates to your workflows.</p>
<p>For more information, please see:</p>
<ol>
<li>The <a href="https://github.blog/changelog/2023-12-14-github-actions-artifacts-v4-is-now-generally-available/">changelog</a> post.</li>
<li>The <a href="https://github.com/actions/upload-artifact/blob/main/README.md">README</a>.</li>
<li>The <a href="https://github.com/actions/upload-artifact/blob/main/docs/MIGRATION.md">migration documentation</a>.</li>
<li>As well as the underlying npm package, <a href="https://github.com/actions/toolkit/tree/main/packages/artifact"><code>@​actions/artifact</code></a> documentation.</li>
</ol>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vmjoseph"><code>@​vmjoseph</code></a> made their first contribution in <a href="https://redirect.github.com/actions/upload-artifact/pull/464">actions/upload-artifact#464</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v4.0.0">https://github.com/actions/upload-artifact/compare/v3...v4.0.0</a></p>
<h2>v3.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(github): remove trailing whitespaces by <a href="https://github.com/ljmf00"><code>@​ljmf00</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/313">actions/upload-artifact#313</a></li>
<li>Bump <code>@​actions/artifact</code> version to v1.1.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/436">actions/upload-artifact#436</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v3.1.3">https://github.com/actions/upload-artifact/compare/v3...v3.1.3</a></p>
<h2>v3.1.2</h2>
<ul>
<li>Update all <code>@actions/*</code> NPM packages to their latest versions- <a href="https://redirect.github.com/actions/upload-artifact/issues/374">#374</a></li>
<li>Update all dev dependencies to their most recent versions - <a href="https://redirect.github.com/actions/upload-artifact/issues/375">#375</a></li>
</ul>
<h2>v3.1.1</h2>
<ul>
<li>Update actions/core package to latest version to remove <code>set-output</code> deprecation warning <a href="https://redirect.github.com/actions/upload-artifact/issues/351">#351</a></li>
</ul>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​actions/artifact</code> to v1.1.0 (<a href="https://redirect.github.com/actions/upload-artifact/pull/327">actions/upload-artifact#327</a>)
<ul>
<li>Adds checksum headers on artifact upload (<a href="https://redirect.github.com/actions/toolkit/pull/1095">actions/toolkit#1095</a>) (<a href="https://redirect.github.com/actions/toolkit/pull/1063">actions/toolkit#1063</a>)</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/5d5d22a31266ced268874388b861e4b58bb5c2f3"><code>5d5d22a</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/515">#515</a> from actions/eggyhead/update-artifact-v2.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/f1e993d9663a03508e7fc0370c744c4b963f0044"><code>f1e993d</code></a> update artifact license</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4881bfd3f27855c63733d8cfff17721cc0ad611f"><code>4881bfd</code></a> updating dist:</li>
<li><a href="https://github.com/actions/upload-artifact/commit/a30777e2653648a0a7bbd3efb5c96ef9131b96cc"><code>a30777e</code></a> <a href="https://github.com/eggyhead"><code>@​eggyhead</code></a></li>
<li><a href="https://github.com/actions/upload-artifact/commit/3a8048248f2f288c271830f8ecf2a1c5d8eb0e9a"><code>3a80482</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/511">#511</a> from actions/robherley/migration-docs-typo</li>
<li><a href="https://github.com/actions/upload-artifact/commit/9d63e3f2f81d9dc4e13d83fc330408f8a94b79d1"><code>9d63e3f</code></a> Merge branch 'main' into robherley/migration-docs-typo</li>
<li><a href="https://github.com/actions/upload-artifact/commit/dfa1ab292d2fdd78d056187f11c568c16ab53de9"><code>dfa1ab2</code></a> fix typo with v3 artifact downloads in migration guide</li>
<li><a href="https://github.com/actions/upload-artifact/commit/d00351bf698398c17253d21cf8f90e57a344e14b"><code>d00351b</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/509">#509</a> from markmssd/patch-1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/707f5a7b71e0fb01c5df1e16e9679a3292606ef2"><code>707f5a7</code></a> Update limitation of <code>10</code> artifacts upload to <code>500</code></li>
<li><a href="https://github.com/actions/upload-artifact/commit/26f96dfa697d77e81fd5907df203aa23a56210a8"><code>26f96df</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/505">#505</a> from actions/robherley/merge-artifacts</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v3...v4">compare view</a></li>
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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 19:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1091" class=".btn">#1091</a>
            </td>
            <td>
                <b>
                    chore: add Dependabot configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Configure Dependabot to automatically maintain dependencies for GitHub Actions.
  - Check for updates once a week.
  - Group all updates into a single PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 17:15:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1090" class=".btn">#1090</a>
            </td>
            <td>
                <b>
                    feat: add loading info box during attestation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Adds an info box to communicate WIP during attestation proof request. Here's what it looks like:
![attestation_info_box](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/aaf566c8-375a-47cd-a290-c439c9295bbc)

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [ ] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 03:23:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1089" class=".btn">#1089</a>
            </td>
            <td>
                <b>
                    chore: add openwallet project proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

At the last Aries Bifold UG meeting, we ratified the decision to put forward a proposal to join the OpenWallet Foundation (OWF). This PR submits the said proposal for posterity. Once approved and merged, the next step will be to take the document and create a pull request against the OWF [project proposals](https://github.com/openwallet-foundation/project-proposals) and present to their technical committee.

A formatted version can be read here: https://hackmd.io/3d3_gSu_S5WNUij9hUZawA

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 23:36:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1088" class=".btn">#1088</a>
            </td>
            <td>
                <b>
                    feat:implement hide lists for credentials and contacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR introduces the feature of credential and contact hide lists. Supply a contact hide list with your configuration and when developer mode is not enabled, all contacts with that `alias` or `theirLabel` will be hidden. Same goes for credentials, using cred def IDs.

Here's what it looks like:
![hide_lists](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/3f164488-c898-4cb3-8883-c14efd1595f0)

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 21:37:12 +0000 UTC
    </div>
</div>

