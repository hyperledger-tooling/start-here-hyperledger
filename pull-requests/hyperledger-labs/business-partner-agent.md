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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/854" class=".btn">#854</a>
            </td>
            <td>
                <b>
                    Bump docker/build-push-action from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [docker/build-push-action](https://github.com/docker/build-push-action) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<blockquote>
<p><strong>Warning</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://github-redirect.dependabot.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Revert disable provenance by default if not set by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://github-redirect.dependabot.com/docker/build-push-action/pull/784">docker/build-push-action#784</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v3.3.1...v4.0.0">https://github.com/docker/build-push-action/compare/v3.3.1...v4.0.0</a></p>
<h2>v3.3.1</h2>
<ul>
<li>Disable provenance by default if not set by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/781">#781</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v3.3.0...v3.3.1">https://github.com/docker/build-push-action/compare/v3.3.0...v3.3.1</a></p>
<h2>v3.3.0</h2>
<blockquote>
<p><strong>Warning</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://github-redirect.dependabot.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Add <code>attests</code>, <code>provenance</code> and <code>sbom</code> inputs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/746">#746</a> <a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/759">#759</a>)</li>
<li>Log GitHub Actions runtime token access controls by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/707">#707</a>)</li>
<li>Examples moved to <a href="https://docs.docker.com/build/ci/github-actions/examples/">docs website</a> by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/718">#718</a>)</li>
<li>Bump minimatch from 3.0.4 to 3.1.2 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/732">#732</a>)</li>
<li>Bump csv-parse from 5.3.0 to 5.3.3 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/729">#729</a>)</li>
<li>Bump json5 from 2.2.0 to 2.2.3 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/749">#749</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v3.2.0...v3.3.0">https://github.com/docker/build-push-action/compare/v3.2.0...v3.3.0</a></p>
<h2>v3.2.0</h2>
<ul>
<li>Remove workaround for <code>setOutput</code> by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/704">#704</a>)</li>
<li>Docs: fix Git context link and add more details about subdir support by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/685">#685</a>)</li>
<li>Docs: named context by <a href="https://github.com/baibaratsky"><code>@​baibaratsky</code></a> and <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/665">#665</a>)</li>
<li>Bump <code>@​actions/core</code> from 1.9.0 to 1.10.0 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/667">#667</a> <a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/695">#695</a>)</li>
<li>Bump <code>@​actions/github</code> from 5.0.3 to 5.1.1 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/696">#696</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v3.1.1...v3.2.0">https://github.com/docker/build-push-action/compare/v3.1.1...v3.2.0</a></p>
<h2>v3.1.1</h2>
<ul>
<li>Fix GitHub token not passed with Git context if subdir defined by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/663">#663</a>)</li>
<li>Replace deprecated <code>fs.rmdir</code> with <code>fs.rm</code> by <a href="https://github.com/bendrucker"><code>@​bendrucker</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/657">#657</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v3.1.0...v3.1.1">https://github.com/docker/build-push-action/compare/v3.1.0...v3.1.1</a></p>
<h2>v3.1.0</h2>
<ul>
<li><code>no-cache-filters</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/653">#653</a>)</li>
<li>Bump <code>@​actions/github</code> from 5.0.1 to 5.0.3 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/619">#619</a>)</li>
<li>Bump <code>@​actions/core</code> from 1.6.0 to 1.9.0 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/620">#620</a> <a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/637">#637</a>)</li>
<li>Bump csv-parse from 5.0.4 to 5.3.0 (<a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/623">#623</a> <a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/650">#650</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v3.0.0...v3.1.0">https://github.com/docker/build-push-action/compare/v3.0.0...v3.1.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/3b5e8027fcad23fda98b2e3ac259d8d67585f671"><code>3b5e802</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/build-push-action/issues/784">#784</a> from crazy-max/enable-provenance</li>
<li><a href="https://github.com/docker/build-push-action/commit/02d3266a89e5dfed960723e6127886a5adc7eb2f"><code>02d3266</code></a> update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/f403dafe18abeb00b9d5976ab285a9f457520f29"><code>f403daf</code></a> revert disable provenance by default if not set</li>
<li>See full diff in <a href="https://github.com/docker/build-push-action/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=docker/build-push-action&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-31 13:10:56 +0000 UTC
    </div>
</div>

