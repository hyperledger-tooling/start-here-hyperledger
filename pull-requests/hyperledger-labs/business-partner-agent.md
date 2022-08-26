---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/819" class=".btn">#819</a>
            </td>
            <td>
                <b>
                    use websockets for events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - websocket for event handling
- added netty native libraries

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/819"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 15:34:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    Bump smartsquaregmbh/delete-old-packages from 0.4.0 to 0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [smartsquaregmbh/delete-old-packages](https://github.com/smartsquaregmbh/delete-old-packages) from 0.4.0 to 0.5.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/smartsquaregmbh/delete-old-packages/releases">smartsquaregmbh/delete-old-packages's releases</a>.</em></p>
<blockquote>
<h2>v0.5.0</h2>
<h4>:warning: This release includes breaking changes!</h4>
<ul>
<li><em>Breaking</em>: Removed <code>version</code> option.
<ul>
<li>To keep this package simple, this option has been removed. Very similar results can be achieved with <code>semver-pattern</code>.</li>
</ul>
</li>
<li><em>Potentially breaking</em>: Rewrite in TypeScript.</li>
<li>Support for ghcr.io packages. See the new section in the <a href="https://github.com/SmartsquareGmbH/delete-old-packages#ghcrio-packages">README</a>.</li>
<li>Improved error handling and logging.</li>
<li>New <code>type</code> option.</li>
</ul>
<blockquote>
<p>Since this release includes major changes and has not been tested as much as previous versions, it is marked as a pre-release. Please try it with the <code>dry-run</code> option and report bugs or missing features!</p>
</blockquote>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/53e0b59f56449a9fdbcec8dcc6d1b038b8a29992"><code>53e0b59</code></a> Bump version to 0.5.0</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/27998e516f375efe57cce37d8b9c4ce10495a790"><code>27998e5</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/237c4313ac8418bccec9cfb095312f56908d2ceb"><code>237c431</code></a> Update README</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/678055d997ba78aeb17fdfac019b7e14ad533fe2"><code>678055d</code></a> Update dependencies</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/2dd5dd734ccd2d1f4d038921270aaaaaf3cfdfe8"><code>2dd5dd7</code></a> Refactor a bit</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/a9319e534a8a97c5fe0053c63ba24209882998f0"><code>a9319e5</code></a> Validate user and organization input combination</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/1d029e77275be61a9e2d517e3e2f5248410a4169"><code>1d029e7</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/b04aafe88d0f3f9d3f2eece3ab4f9043d143d305"><code>b04aafe</code></a> Add cause to query package errors</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/de048edb051d2fd9daa6d47098ebe025d5b731e8"><code>de048ed</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/becea094ebba3952d40d01ffffb194ce205def1f"><code>becea09</code></a> Improve error handling</li>
<li>Additional commits viewable in <a href="https://github.com/smartsquaregmbh/delete-old-packages/compare/v0.4.0...v0.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smartsquaregmbh/delete-old-packages&package-manager=github_actions&previous-version=0.4.0&new-version=0.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/818"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 13:46:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/817" class=".btn">#817</a>
            </td>
            <td>
                <b>
                    fix 815 - partner deletion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes, remove presentation exchanges without loading them into memory first

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/817"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 15:46:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    convert logging config to yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                we need to overwrite logging config on the fly. this is easier with yaml files in the chart repo

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/816"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 12:01:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/813" class=".btn">#813</a>
            </td>
            <td>
                <b>
                    Bump docker/metadata-action from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [docker/metadata-action](https://github.com/docker/metadata-action) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/releases">docker/metadata-action's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<ul>
<li>Node 16 as default runtime by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/176">#176</a>)
<ul>
<li>This requires a minimum <a href="https://github.com/actions/runner/releases/tag/v2.285.0">Actions Runner</a> version of v2.285.0, which is by default available in GHES 3.4 or later.</li>
</ul>
</li>
<li>Do not sanitize before pattern matching by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/201">#201</a>)
<ul>
<li>Breaking change with <code>type=match</code> pattern matching</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v3.8.0...v4.0.0">https://github.com/docker/metadata-action/compare/v3.8.0...v4.0.0</a></p>
<h2>v3.8.0</h2>
<ul>
<li>Add attribute to enable/disable images by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/193">#193</a>)</li>
<li>Add <code>is_default_branch</code> global expression by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/192">#192</a> <a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/197">#197</a> <a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/198">#198</a>)</li>
<li>Update fixtures (dev) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/190">#190</a>)</li>
<li>Bump semver from 7.3.5 to 7.3.7 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/185">#185</a>)</li>
<li>Bump moment from 2.29.2 to 2.29.3 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/187">#187</a>)</li>
<li>Bump csv-parse from 4.16.3 to 5.0.4 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/195">#195</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v3.7.0...v3.8.0">https://github.com/docker/metadata-action/compare/v3.7.0...v3.8.0</a></p>
<h2>v3.7.0</h2>
<ul>
<li>Handle comments for multi-line inputs (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/172">#172</a>)</li>
<li>Missing <code>json</code> output in <code>action.yml</code> (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/167">#167</a>)</li>
<li>Update dev dependencies and workflow (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/175">#175</a>)</li>
<li>Bump minimist from 1.2.5 to 1.2.6 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/182">#182</a>)</li>
<li>Bump moment from 2.29.1 to 2.29.2 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/180">#180</a>)</li>
<li>Bump <code>@​actions/github</code> from 5.0.0 to 5.0.1 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/179">#179</a>)</li>
<li>Bump node-fetch from 2.6.1 to 2.6.7 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/173">#173</a>)</li>
</ul>
<h2>v3.6.2</h2>
<ul>
<li>Handle raw statement for pre-release (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/155">#155</a> <a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/156">#156</a>)</li>
</ul>
<h2>v3.6.1</h2>
<ul>
<li>Preserve quotes inside unquoted field (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/153">#153</a>)</li>
</ul>
<h2>v3.6.0</h2>
<ul>
<li><code>base_ref</code> global expression (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/142">#142</a>)</li>
<li>Trim tags and flavor inputs (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/143">#143</a>)</li>
<li>Bump <code>@​actions/core</code> from 1.5.0 to 1.6.0 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/135">#135</a>)</li>
<li>Bump ansi-regex from 5.0.0 to 5.0.1 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/134">#134</a>)</li>
<li>Bump tmpl from 1.0.4 to 1.0.5 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/132">#132</a>)</li>
<li>Bump csv-parse from 4.16.0 to 4.16.3 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/131">#131</a>)</li>
</ul>
<h2>v3.5.0</h2>
<ul>
<li>Add global expression <code>date</code> (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/121">#121</a>)</li>
<li>Bump <code>@​actions/core</code> from 1.4.0 to 1.5.0 (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/122">#122</a>)</li>
</ul>
<h2>v3.4.1</h2>
<ul>
<li>Only return edge if branch matches (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/115">#115</a>)</li>
</ul>
<h2>v3.4.0</h2>
<ul>
<li>PEP 440 support (<a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/108">#108</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Upgrade guide</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/blob/master/UPGRADE.md">docker/metadata-action's upgrade guide</a>.</em></p>
<blockquote>
<h1>Upgrade notes</h1>
<h2>v2 to v3</h2>
<ul>
<li>Repository has been moved to docker org. Replace <code>crazy-max/ghaction-docker-meta@v2</code> with <code>docker/metadata-action@v4</code></li>
<li>The default bake target has been changed: <code>ghaction-docker-meta</code> &gt; <code>docker-metadata-action</code></li>
</ul>
<h2>v1 to v2</h2>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#inputs">inputs</a>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-sha"><code>tag-sha</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-edge--tag-edge-branch"><code>tag-edge</code> / <code>tag-edge-branch</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-semver"><code>tag-semver</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-match--tag-match-group"><code>tag-match</code> / <code>tag-match-group</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-latest"><code>tag-latest</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-schedule"><code>tag-schedule</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-custom--tag-custom-only"><code>tag-custom</code> / <code>tag-custom-only</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#label-custom"><code>label-custom</code></a></li>
</ul>
</li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#basic-workflow">Basic workflow</a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#semver-workflow">Semver workflow</a></li>
</ul>
<h3>inputs</h3>
<table>
<thead>
<tr>
<th>New</th>
<th>Unchanged</th>
<th>Removed</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>tags</code></td>
<td><code>images</code></td>
<td><code>tag-sha</code></td>
</tr>
<tr>
<td><code>flavor</code></td>
<td><code>sep-tags</code></td>
<td><code>tag-edge</code></td>
</tr>
<tr>
<td><code>labels</code></td>
<td><code>sep-labels</code></td>
<td><code>tag-edge-branch</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-semver</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match-group</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-latest</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-schedule</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom-only</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>label-custom</code></td>
</tr>
</tbody>
</table>
<h4><code>tag-sha</code></h4>
<pre lang="yaml"><code>tags: |
  type=sha
</code></pre>
<h4><code>tag-edge</code> / <code>tag-edge-branch</code></h4>
<pre lang="yaml"><code>tags: |
  # default branch
  type=edge
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/metadata-action/commit/69f6fc9d46f2f8bf0d5491e4aabe0bb8c6a4678a"><code>69f6fc9</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/203">#203</a> from crazy-max/san-fix</li>
<li><a href="https://github.com/docker/metadata-action/commit/2f5b5ae8bf2725130d7ade554556e85077021427"><code>2f5b5ae</code></a> Sanitize tag earlier</li>
<li><a href="https://github.com/docker/metadata-action/commit/f206c36955d3cc6213c38fb3747d9ba4113e686a"><code>f206c36</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/202">#202</a> from crazy-max/v4-prep</li>
<li><a href="https://github.com/docker/metadata-action/commit/a20adfa74e16683029ddca858a830d46940bcde1"><code>a20adfa</code></a> readme: set metadata-action to v4</li>
<li><a href="https://github.com/docker/metadata-action/commit/26b9439ce3c3a94be4548b775c813dc6e9e618a2"><code>26b9439</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/201">#201</a> from crazy-max/fix-sanitization</li>
<li><a href="https://github.com/docker/metadata-action/commit/467883f452335596514beb1a02db7e09de6a08f7"><code>467883f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/metadata-action/issues/176">#176</a> from crazy-max/node-16</li>
<li><a href="https://github.com/docker/metadata-action/commit/5edf56f2c486f342f4319e9c0a1a79d59a474516"><code>5edf56f</code></a> Node 16 as default runtime</li>
<li><a href="https://github.com/docker/metadata-action/commit/678218f2be830b6011728d42a72a35714f423bcf"><code>678218f</code></a> Note about image name and tag sanitization</li>
<li><a href="https://github.com/docker/metadata-action/commit/e44c1fbe6ec0f8dbe5229eab51e84075fcca8799"><code>e44c1fb</code></a> Do not sanitize before pattern matching</li>
<li>See full diff in <a href="https://github.com/docker/metadata-action/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=docker/metadata-action&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/813"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 13:46:33 +0000 UTC
    </div>
</div>

