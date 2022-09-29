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
                PR <a href="https://github.com/hyperledger/iroha/pull/2798" class=".btn">#2798</a>
            </td>
            <td>
                <b>
                    [ci] #2781: add codecov commit parent feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Sign-off-by: BAStos525 <jungle.vas@yandex.ru>

### Description of the Change
1. Add `parent_commit` option to Codecov Upload Action with the branch SHA:

```
The commit SHA of the parent for which you are uploading coverage.
```
2. Temporarily disable codecov report upload as artifact Actions.

### Issue
Codecov Action bot doesn't show the correct diff between the head and PR branches.

### Benefits
`parent_commit` option could help to currently determine the right head branch merge commit.

### Possible Drawbacks
None, but it still could be not work.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 12:54:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2788" class=".btn">#2788</a>
            </td>
            <td>
                <b>
                    [fix] #2787: Notify every listener to shutdown on panic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Shanin Roman <shanin1000@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Replaced `.notify_one()` with `.notify_waiters()` in order to notify every waiter about shutdown.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2787.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Iroha actually shutdown. 

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

There is still possibility of deadlock if `.notified().await` would be called after `.notify_waiters()` was called, but this seems to be very unlikely case , because either start warp (in this case waiters would be ready) or warp not started yet (int this case nothing will prevent iroha from shutdown).

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

```
cargo test --package iroha --lib -- tests::iroha_should_notify_on_panic --exact --nocapture
```

### Alternate Designs *[optional]*

- Replace `Notify` channel with different sync primitive.
- Every `waiter` must call `.notify_one()` after receiving notification: more verbose, but solve case of possible deadlock. 

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 14:05:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2785" class=".btn">#2785</a>
            </td>
            <td>
                <b>
                    [ci]: move jobs to github runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
Replace self-hosted runners inside `tests` workflows with the default `ubuntu-latest` Gihub Runners.

### Issue
Some long tests are failed on self-hosted runners due to undetected reason.

### Benefits
Long tests should not be failed when they are run on the deault GH Runners.

### Possible Drawbacks
Should be none, but we have to re-implement self-hosted runners.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 07:22:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    Bump protobuf from 3.15.0 to 3.18.3 in /docs/source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [protobuf](https://github.com/protocolbuffers/protobuf) from 3.15.0 to 3.18.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf's releases</a>.</em></p>
<blockquote>
<h2>Protocol Buffers v3.18.3</h2>
<h1>C++</h1>
<ul>
<li>Reduce memory consumption of MessageSet parsing</li>
<li>This release addresses a <a href="https://github.com/protocolbuffers/protobuf/security/advisories/GHSA-8gq9-2x98-w8hf">Security Advisory for C++ and Python users</a></li>
</ul>
<h2>Protocol Buffers v3.16.1</h2>
<h1>Java</h1>
<ul>
<li>Improve performance characteristics of UnknownFieldSet parsing (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
</ul>
<h2>Protocol Buffers v3.18.2</h2>
<h1>Java</h1>
<ul>
<li>Improve performance characteristics of UnknownFieldSet parsing (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
</ul>
<h2>Protocol Buffers v3.18.1</h2>
<h1>Python</h1>
<ul>
<li>Update setup.py to reflect that we now require at least Python 3.5 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8989">#8989</a>)</li>
<li>Performance fix for DynamicMessage: force GetRaw() to be inlined (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9023">#9023</a>)</li>
</ul>
<h1>Ruby</h1>
<ul>
<li>Update ruby_generator.cc to allow proto2 imports in proto3 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9003">#9003</a>)</li>
</ul>
<h2>Protocol Buffers v3.18.0</h2>
<h1>C++</h1>
<ul>
<li>Fix warnings raised by clang 11 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8664">#8664</a>)</li>
<li>Make StringPiece constructible from std::string_view (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8707">#8707</a>)</li>
<li>Add missing capability attributes for LLVM 12 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8714">#8714</a>)</li>
<li>Stop using std::iterator (deprecated in C++17). (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8741">#8741</a>)</li>
<li>Move field_access_listener from libprotobuf-lite to libprotobuf (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8775">#8775</a>)</li>
<li>Fix <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/7047">#7047</a> Safely handle setlocale (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8735">#8735</a>)</li>
<li>Remove deprecated version of SetTotalBytesLimit() (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8794">#8794</a>)</li>
<li>Support arena allocation of google::protobuf::AnyMetadata (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8758">#8758</a>)</li>
<li>Fix undefined symbol error around SharedCtor() (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8827">#8827</a>)</li>
<li>Fix default value of enum(int) in json_util with proto2 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8835">#8835</a>)</li>
<li>Better Smaller ByteSizeLong</li>
<li>Introduce event filters for inject_field_listener_events</li>
<li>Reduce memory usage of DescriptorPool</li>
<li>For lazy fields copy serialized form when allowed.</li>
<li>Re-introduce the InlinedStringField class</li>
<li>v2 access listener</li>
<li>Reduce padding in the proto's ExtensionRegistry map.</li>
<li>GetExtension performance optimizations</li>
<li>Make tracker a static variable rather than call static functions</li>
<li>Support extensions in field access listener</li>
<li>Annotate MergeFrom for field access listener</li>
<li>Fix incomplete types for field access listener</li>
<li>Add map_entry/new_map_entry to SpecificField in MessageDifferencer. They
record the map items which are different in MessageDifferencer's reporter.</li>
<li>Reduce binary size due to fieldless proto messages</li>
<li>TextFormat: ParseInfoTree supports getting field end location in addition to
start.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/a902b39270841beafc307dfa709610aa1cac2f06"><code>a902b39</code></a> No-op whitespace change</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/ae62acd7293e5a80378faeaac67b3baadba810d5"><code>ae62acd</code></a> Updating version.json and repo version numbers to: 18.3</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/f43ac49b91007501ce1683967b04dcfb47183478"><code>f43ac49</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10542">#10542</a> from deannagarcia/3.18.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/9efdf55814add154d3c2646652f527a51d4a21ea"><code>9efdf55</code></a> Add missing includes</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/d1635e1496f51e0d5653d856211e8821bc47adc4"><code>d1635e1</code></a> Apply patch</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/5b37c91d62d7fe097253ac64518b993b096e9386"><code>5b37c91</code></a> Update version.json with &quot;lts&quot;: true (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10534">#10534</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/c39d622dba8343c50876770e6c2cc580781f6264"><code>c39d622</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10529">#10529</a> from protocolbuffers/deannagarcia-patch-5</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/f77d3b643209437f186755737499a841886706cd"><code>f77d3b6</code></a> Update version.json</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/8178b06523f67923f538c479c148af765b09b628"><code>8178b06</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/10503">#10503</a> from deannagarcia/3.18.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/24ca839fffdd2f795acb26686a312de9892f2c6b"><code>24ca839</code></a> Add version file</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.15.0...v3.18.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobuf&package-manager=pip&previous-version=3.15.0&new-version=3.18.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 23:13:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2782" class=".btn">#2782</a>
            </td>
            <td>
                <b>
                    [ci] #2778: Client config check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

* Added kagami sub-command to generate valid client config
* Added ci check
* New config was tested with `iroha_client_cli` and it works. Current config on `iroha2-dev` is not working

### Issue

* Closes #2778 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

* CI check for corrent client config
* Automatic way to generate valid config

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

None

### Usage Examples or Tests

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

```bash
scripts/check.sh client
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 14:24:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2779" class=".btn">#2779</a>
            </td>
            <td>
                <b>
                    [documentation] #2544: Tutorial doctests, a version without API changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

Same as [2603](https://github.com/hyperledger/iroha/pull/2603) except the API changes.
Adds example that mirrors tutorial examples, so that changes in the API can be propagated by directly taking them from GitHub.

### Issue

Addresses https://github.com/hyperledger/iroha/issues/2544

### Benefits

Direct connection to tutorial

### Possible Drawbacks

More code to test

### Usage Examples or Tests *[optional]*

`cargo run --example tutorial`

### Alternate Designs

As a test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 17:10:46 +0000 UTC
    </div>
</div>

