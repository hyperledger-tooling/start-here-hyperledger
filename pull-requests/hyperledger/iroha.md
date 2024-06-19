---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4744" class=".btn">#4744</a>
            </td>
            <td>
                <b>
                    fix(sumeragi): early exit from handle_block_sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Exit early from `handle_block_sync` if received block is the same or has smaller or equal view change index.

## Benefits

Improve performance of block sync by avoid doing work where not necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 11:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4742" class=".btn">#4742</a>
            </td>
            <td>
                <b>
                    refactor: move permission migration into executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description


### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

we no longer depend on the `ExecutorDataModel::permissions` being correct. 
It's just for users to query it the same way as `ExecutorDataModel::custom_instruction` is

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 07:51:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4741" class=".btn">#4741</a>
            </td>
            <td>
                <b>
                    refactor!: fix naming convention for assets and permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 12:07:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4740" class=".btn">#4740</a>
            </td>
            <td>
                <b>
                    fix: fix unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

Fix failing unit tests.

Checked tests locally to verify if errors are resolved.

```
cargo test --all-features --no-fail-fast --workspace --exclude iroha_executor
```

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 11:52:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4739" class=".btn">#4739</a>
            </td>
            <td>
                <b>
                    refactor!: Supply `SignedBlock` instead of `SignedTransaction` to peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

This is first part of #4696:
* Added `topology` field to `genesis.json`
* Changed `kagami genesis sign` to generate `SignedBlock`
* Adapted `iroha_swarm` to those changes

Planned changes for next PRs:
* Provide hash of genesis block to all peers (#4555)
* Allow multiple peers to submit genesis

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 11:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4738" class=".btn">#4738</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump flake8 from 7.0.0 to 7.1.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [flake8](https://github.com/pycqa/flake8) from 7.0.0 to 7.1.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/PyCQA/flake8/commit/65a38c42a7f1a05ff8d99b313160754fc9b7a0d8"><code>65a38c4</code></a> Release 7.1.0</li>
<li><a href="https://github.com/PyCQA/flake8/commit/34c97e046a459b0682c82660f16c620369abd6b7"><code>34c97e0</code></a> Merge pull request <a href="https://redirect.github.com/pycqa/flake8/issues/1939">#1939</a> from PyCQA/new-pycodestyle</li>
<li><a href="https://github.com/PyCQA/flake8/commit/defd315175b7b77472affb61a410e5720dabdc1a"><code>defd315</code></a> latest pycodestyle</li>
<li><a href="https://github.com/PyCQA/flake8/commit/408d4d695c71b0b232cea576876e757c87a3379c"><code>408d4d6</code></a> Merge pull request <a href="https://redirect.github.com/pycqa/flake8/issues/1930">#1930</a> from mzagol/patch-1</li>
<li><a href="https://github.com/PyCQA/flake8/commit/866ad729c64eea359960a8ac4e3f1201104ee55c"><code>866ad72</code></a> Add --extend-exclude to the TOC</li>
<li><a href="https://github.com/PyCQA/flake8/commit/33e508307ac4545a45472fdc32c6eaadbc7b9580"><code>33e5083</code></a> Merge pull request <a href="https://redirect.github.com/pycqa/flake8/issues/1923">#1923</a> from Viicos/entry-points-docs</li>
<li><a href="https://github.com/PyCQA/flake8/commit/6659b213c9aa8fa49235e13a365fcd34f58cbc6b"><code>6659b21</code></a> Fix toctree ordering in index</li>
<li><a href="https://github.com/PyCQA/flake8/commit/ba0f56610adbd4d8733772ce1c63efcab1b70079"><code>ba0f566</code></a> Use explicit external references</li>
<li><a href="https://github.com/PyCQA/flake8/commit/350f2545fd3ec75640a1605e4995a2f921e8b38b"><code>350f254</code></a> Use explicit external references</li>
<li><a href="https://github.com/PyCQA/flake8/commit/49f52a8598d8a934b07f367a1b3ad87dbe51be5b"><code>49f52a8</code></a> Update documentation regarding entry points</li>
<li>Additional commits viewable in <a href="https://github.com/pycqa/flake8/compare/7.0.0...7.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=flake8&package-manager=pip&previous-version=7.0.0&new-version=7.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 16:55:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4737" class=".btn">#4737</a>
            </td>
            <td>
                <b>
                    chore(deps): bump docker/build-push-action from 4 to 6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [docker/build-push-action](https://github.com/docker/build-push-action) from 4 to 6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v6.0.0</h2>
<ul>
<li>Export build record and generate <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">build summary</a> by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1120">docker/build-push-action#1120</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.24.0 to 0.26.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1132">docker/build-push-action#1132</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1136">docker/build-push-action#1136</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1138">docker/build-push-action#1138</a></li>
<li>Bump braces from 3.0.2 to 3.0.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1137">docker/build-push-action#1137</a></li>
</ul>
<blockquote>
<p>[!NOTE]
This major release adds support for generating <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">Build summary</a> and exporting build record for your build. You can disable this feature by setting <a href="https://docs.docker.com/build/ci/github-actions/build-summary/#disable-job-summary"> <code>DOCKER_BUILD_NO_SUMMARY: true</code> environment variable in your workflow</a>.</p>
</blockquote>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0">https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0</a></p>
<h2>v5.4.0</h2>
<ul>
<li>Show builder information before building by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1128">docker/build-push-action#1128</a></li>
<li>Handle attestations correctly with provenance and sbom inputs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1086">docker/build-push-action#1086</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.19.0 to 0.24.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1088">docker/build-push-action#1088</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1105">docker/build-push-action#1105</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1121">docker/build-push-action#1121</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1127">docker/build-push-action#1127</a></li>
<li>Bump undici from 5.28.3 to 5.28.4 in <a href="https://redirect.github.com/docker/build-push-action/pull/1090">docker/build-push-action#1090</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0">https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0</a></p>
<h2>v5.3.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1080">docker/build-push-action#1080</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0">https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0</a></p>
<h2>v5.2.0</h2>
<ul>
<li>Disable quotes detection for <code>outputs</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1074">docker/build-push-action#1074</a></li>
<li>Warn about ignored inputs by <a href="https://github.com/favonia"><code>@​favonia</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1019">docker/build-push-action#1019</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.14.0 to 0.18.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1070">docker/build-push-action#1070</a></li>
<li>Bump undici from 5.26.3 to 5.28.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1057">docker/build-push-action#1057</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0">https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0</a></p>
<h2>v5.1.0</h2>
<ul>
<li>Add <code>annotations</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/992">docker/build-push-action#992</a></li>
<li>Add <code>secret-envs</code> input by <a href="https://github.com/elias-lundgren"><code>@​elias-lundgren</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/980">docker/build-push-action#980</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.17.3 to 7.23.2 in <a href="https://redirect.github.com/docker/build-push-action/pull/991">docker/build-push-action#991</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.13.0-rc.1 to 0.14.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/990">docker/build-push-action#990</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1006">docker/build-push-action#1006</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0">https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0</a></p>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/954">docker/build-push-action#954</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/959">docker/build-push-action#959</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0">https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0</a></p>
<h2>v4.2.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/c382f710d39a5bb4e430307530a720f50c2d3318"><code>c382f71</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1120">#1120</a> from crazy-max/build-summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/5a5b70d974381b812e448a9ea8efef0c0781e8a7"><code>5a5b70d</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/dc24cf9e252ee3b05f80a1637b2950c11d305b3d"><code>dc24cf9</code></a> don't generate summary for cloud driver</li>
<li><a href="https://github.com/docker/build-push-action/commit/667cb22c52a8762431790112e70ef7f545dbf2d2"><code>667cb22</code></a> DOCKER_BUILD_NO_SUMMARY env to disable summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/d880b1964b626c7ac1763e83768e139202071136"><code>d880b19</code></a> generate build summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/e51051ad0baf1cdf23788f7f0980f675806b580e"><code>e51051a</code></a> export build record and upload artifact</li>
<li><a href="https://github.com/docker/build-push-action/commit/86c2bd00318427a320d2cee5bbc61251df6f647e"><code>86c2bd0</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1137">#1137</a> from docker/dependabot/npm_and_yarn/braces-3.0.3</li>
<li><a href="https://github.com/docker/build-push-action/commit/268d2b16117932ad41015c96fbc27a7641533625"><code>268d2b1</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1138">#1138</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/2b8dc7f52914dfdd416618a1f33d11277b7d64d2"><code>2b8dc7f</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/840c12be1707e3d7115f8d61da2c8b78442cc538"><code>840c12b</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.25.1 to 0.26.0</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v4...v6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=docker/build-push-action&package-manager=github_actions&previous-version=4&new-version=6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 16:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4736" class=".btn">#4736</a>
            </td>
            <td>
                <b>
                    chore(deps): bump derive_more from 0.99.17 to 0.99.18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [derive_more](https://github.com/JelteF/derive_more) from 0.99.17 to 0.99.18.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/JelteF/derive_more/blob/v0.99.18/CHANGELOG.md">derive_more's changelog</a>.</em></p>
<blockquote>
<h2>0.99.18 - 2024-06-15</h2>
<ul>
<li>Update syn to version 2.x</li>
<li>Bump minimum supported rust version to 1.65</li>
</ul>
<h2>0.99.10 - 2020-09-11</h2>
<h3>Improvements</h3>
<ul>
<li><code>From</code> supports additional types for conversion: <code>#[from(types(u8, u16))]</code>.</li>
</ul>
<h2>0.99.7 - 2020-05-16</h2>
<h3>Fixes</h3>
<ul>
<li>Fix generic derives for <code>MulAssign</code></li>
</ul>
<h3>Improvements</h3>
<ul>
<li>When specifying specific features of the crate to only enable specific
derives, the <code>extra-traits</code> feature of  <code>syn</code> is not always enabled
when those the specified features do not require it. This should speed up
compile time of <code>syn</code> when this feature is not needed.</li>
</ul>
<h2>0.99.6 - 2020-05-13</h2>
<h3>Improvements</h3>
<ul>
<li>Make sure output of derives is deterministic, for better support in
rust-analyzer</li>
</ul>
<h2>0.99.5 - 2020-03-28</h2>
<h3>New features</h3>
<ul>
<li>Support for deriving <code>Error</code>!!! (many thanks to <a href="https://github.com/ffuugoo"><code>@​ffuugoo</code></a> and <a href="https://github.com/tyranron"><code>@​tyranron</code></a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>
<p>Fix generic bounds for <code>Deref</code> and <code>DerefMut</code> with <code>forward</code>, i.e. put <code>Deref</code>
bound on whole type, so on <code>where Box&lt;T&gt;: Deref</code> instead of on <code>T: Deref</code>.
(<a href="https://redirect.github.com/JelteF/derive_more/issues/114">#107</a>)</p>
</li>
<li>
<p>The <code>tests</code> directory is now correctly included in the crate (requested by
Debian package maintainers)</p>
</li>
</ul>
<h2>0.99.4 - 2020-03-28</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/JelteF/derive_more/commit/678a4735bc540b7363c6dadddc4bb273fdf74468"><code>678a473</code></a> chore: Release derive_more version 0.99.18</li>
<li><a href="https://github.com/JelteF/derive_more/commit/fcde5568cb2a815b8d85fceb6dd8fd56750d2b25"><code>fcde556</code></a> Include example published package</li>
<li><a href="https://github.com/JelteF/derive_more/commit/89cbd82959034284f7a2eeffb1976bc41a75b95f"><code>89cbd82</code></a> Remove track_caller feature detection because msrv was bumped</li>
<li><a href="https://github.com/JelteF/derive_more/commit/db36f6dade1cf512ff71961882bda6467a639a31"><code>db36f6d</code></a> Fix question marks</li>
<li><a href="https://github.com/JelteF/derive_more/commit/f0c2530255b21d9f791ee6e4acb6375c2becc641"><code>f0c2530</code></a> fmt</li>
<li><a href="https://github.com/JelteF/derive_more/commit/461db95716ac91f60ee4877bb94c474b5fa25ca7"><code>461db95</code></a> Fix issue when compiling on 1.65</li>
<li><a href="https://github.com/JelteF/derive_more/commit/39ad36fd7117acb0a8140d3aa63899ecc46b53c6"><code>39ad36f</code></a> Update changelog for v0.99.18</li>
<li><a href="https://github.com/JelteF/derive_more/commit/57b6e1746e1ddf4c67e16b5e82f12e19ef02a3d5"><code>57b6e17</code></a> Update to syn 2</li>
<li><a href="https://github.com/JelteF/derive_more/commit/ea4fa940033682ca16e1040688963011404d02a0"><code>ea4fa94</code></a> Fix tests</li>
<li><a href="https://github.com/JelteF/derive_more/commit/ab82aef0bf0c4f4e5cc837e3de3a78a373bc922b"><code>ab82aef</code></a> Ignore error doctests as it still contains old backtrace logic</li>
<li>Additional commits viewable in <a href="https://github.com/JelteF/derive_more/compare/v0.99.17...v0.99.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=derive_more&package-manager=cargo&previous-version=0.99.17&new-version=0.99.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 16:04:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4734" class=".btn">#4734</a>
            </td>
            <td>
                <b>
                    refactor: Make domain structure shallow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-15 22:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4732" class=".btn">#4732</a>
            </td>
            <td>
                <b>
                    refactor: Make the metadata dynamic via implementing JsonString
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

* Removed MetadataValueBox
* Added JsonString

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

* Closes #4353  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 09:56:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4731" class=".btn">#4731</a>
            </td>
            <td>
                <b>
                    fix!: remove on-chain parameters from config and remove NewParameter ISI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

* remove `NewParametere` ISI
* remove on-chain parameters from configuration
* strong type on-chain parameters
* removed `MetadataLimits` and `LenghtLimits` as built-in on-chain parameters (they can be defined as custom)

Next PR will introduce Custom parameters

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 09:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4730" class=".btn">#4730</a>
            </td>
            <td>
                <b>
                    fix: update schema.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Add missing types into the schema.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 08:58:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4728" class=".btn">#4728</a>
            </td>
            <td>
                <b>
                    fix: Introduce p2p idle timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport of #4398.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4267 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

No problem with connectivity on rc20.

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 14:20:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4725" class=".btn">#4725</a>
            </td>
            <td>
                <b>
                    fix: Make `iroha_smart_contract_utils` `log` and `dbg` functions work outside of wasm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

This PR adds support for `iroha_smart_contract_utils`'s `log` and `dbg` functions to be used outside of wasm. This allows writing tests to be ran against the host target and to still use those wasm-specific functions.

Both implementations just print the requested object to stderr.

As a drive-by, this also makes sure to run wasm tests from `iroha_smart_contract_utils`, which was omitted in CI for some time.

### Linked issue

Fixes #4721

### Benefits

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 11:56:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4724" class=".btn">#4724</a>
            </td>
            <td>
                <b>
                    refactor(genesis)!: remove _id and _file suffix from genesis fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 11:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4723" class=".btn">#4723</a>
            </td>
            <td>
                <b>
                    fix(swarm): remove `_id` suffix from docker-compose files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 10:57:16 +0000 UTC
    </div>
</div>

