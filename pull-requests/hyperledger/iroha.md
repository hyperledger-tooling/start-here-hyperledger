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
                PR <a href="https://github.com/hyperledger/iroha/pull/1905" class=".btn">#1905</a>
            </td>
            <td>
                <b>
                    [refactor] #1893: Split `data_model` lib.rs file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Split `data_model/src/lib.rs` file into separate ones. Just moved some modules into its own files.

Reading `data_model/src/lib.rs` file shouldn't have gotten any worse, cause every module is completely independent from each other

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Resolves #1893 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now it's easier to read and navigate in `data_model` crate

<!-- What benefits will be realized by the code change? -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-12 12:59:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1901" class=".btn">#1901</a>
            </td>
            <td>
                <b>
                    Gh wf readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
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

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-02-11 06:57:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1900" class=".btn">#1900</a>
            </td>
            <td>
                <b>
                    Bump protobuf from 3.5.1 to 3.15.0 in /docs/source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [protobuf](https://github.com/protocolbuffers/protobuf) from 3.5.1 to 3.15.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf's releases</a>.</em></p>
<blockquote>
<h2>Protocol Buffers v3.15.0</h2>
<h1>Protocol Compiler</h1>
<ul>
<li>Optional fields for proto3 are enabled by default, and no longer require
the --experimental_allow_proto3_optional flag.</li>
</ul>
<h1>C++</h1>
<ul>
<li>MessageDifferencer: fixed bug when using custom ignore with multiple
unknown fields</li>
<li>Use init_seg in MSVC to push initialization to an earlier phase.</li>
<li>Runtime no longer triggers -Wsign-compare warnings.</li>
<li>Fixed -Wtautological-constant-out-of-range-compare warning.</li>
<li>DynamicCastToGenerated works for nullptr input for even if RTTI is disabled</li>
<li>Arena is refactored and optimized.</li>
<li>Clarified/specified that the exact value of Arena::SpaceAllocated() is an
implementation detail users must not rely on. It should not be used in
unit tests.</li>
<li>Change the signature of Any::PackFrom() to return false on error.</li>
<li>Add fast reflection getter API for strings.</li>
<li>Constant initialize the global message instances</li>
<li>Avoid potential for missed wakeup in UnknownFieldSet</li>
<li>Now Proto3 Oneof fields have &quot;has&quot; methods for checking their presence in
C++.</li>
<li>Bugfix for NVCC</li>
<li>Return early in _InternalSerialize for empty maps.</li>
<li>Adding functionality for outputting map key values in proto path logging
output (does not affect comparison logic) and stop printing 'value' in the
path. The modified print functionality is in the
MessageDifferencer::StreamReporter.</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8129">protocolbuffers/protobuf#8129</a></li>
<li>Ensure that null char symbol, package and file names do not result in a
crash.</li>
<li>Constant initialize the global message instances</li>
<li>Pretty print 'max' instead of numeric values in reserved ranges.</li>
<li>Removed remaining instances of std::is_pod, which is deprecated in C++20.</li>
<li>Changes to reduce code size for unknown field handling by making uncommon
cases out of line.</li>
<li>Fix std::is_pod deprecated in C++20 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/7180">#7180</a>)</li>
<li>Fix some -Wunused-parameter warnings (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8053">#8053</a>)</li>
<li>Fix detecting file as directory on zOS issue <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8051">#8051</a> (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8052">#8052</a>)</li>
<li>Don't include sys/param.h for _BYTE_ORDER (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8106">#8106</a>)</li>
<li>remove CMAKE_THREAD_LIBS_INIT from pkgconfig CFLAGS (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8154">#8154</a>)</li>
<li>Fix TextFormatMapTest.DynamicMessage issue#5136 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8159">#8159</a>)</li>
<li>Fix for compiler warning issue#8145 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8160">#8160</a>)</li>
<li>fix: support deprecated enums for GCC &lt; 6 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8164">#8164</a>)</li>
<li>Fix some warning when compiling with Visual Studio 2019 on x64 target (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8125">#8125</a>)</li>
</ul>
<h1>Python</h1>
<ul>
<li>Provided an override for the reverse() method that will reverse the internal
collection directly instead of using the other methods of the BaseContainer.</li>
<li>MessageFactory.CreateProtoype can be overridden to customize class creation.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/ae50d9b9902526efd6c7a1907d09739f959c6297"><code>ae50d9b</code></a> Update protobuf version</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/8260126500f073894c38b2211d383442eb7e58d5"><code>8260126</code></a> Update protobuf version</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/c741c4660443da46bfaf6c96fd1f01e743f97b56"><code>c741c46</code></a> Resovled issue in the .pb.cc files</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/eef276412ec417e2f0563c1c51d59a968cb2a6db"><code>eef2764</code></a> Resolved an issue where NO_DESTROY and CONSTINIT were in incorrect order</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/0040102e6f001724194d9c4c6bcd5effcec52bf1"><code>0040102</code></a> Updated collect_all_artifacts.sh for Ubuntu Xenial</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/26cb6a7a6d7973657f09fc44b201287c046da62e"><code>26cb6a7</code></a> Delete root-owned files in Kokoro builds</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/1e924efa90b476d23157426ad1eb17301bc4df41"><code>1e924ef</code></a> Update port_def.inc</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/9a80cf12254dec1af833d9fb78a80673dce45dc4"><code>9a80cf1</code></a> Update coded_stream.h</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/a97c4f4f2c9e5ffce0db787268414eb141194c62"><code>a97c4f4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8276">#8276</a> from haberman/php-warning</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/44cd75d2153fab614480517e40ee4c10cb153716"><code>44cd75d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8282">#8282</a> from haberman/changelog</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.5.1...v3.15.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobuf&package-manager=pip&previous-version=3.5.1&new-version=3.15.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-02-11 02:48:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1899" class=".btn">#1899</a>
            </td>
            <td>
                <b>
                    [feature] #1195: Close a websocket connection cleanly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

* Now `torii` checks for WebSocket `Close` messages on `/events` path and gracefully handles them.
* Also added test for it.
* As a bonus I refactored some error types from `eyre::Report` to custom Error enums. I thought, that it will help me, but it doesn't. I can reset it, if everybody else think it wasn't necessary

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Resolves #1195 

I was working only with that `handle_subscription()` method, cause it's mentioned in the issue. I don't know if issue appears somewhere else

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Closing WebSocket requires waiting for response. `torii` wasn't doing it, so clients had to interrupt connection.
Now this works as it shoud be.


<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Any suggestions about additional tests will be helpful. May be it should be tested with js-client, as it was mentioned in #1195

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

See `torii/tests.rs`

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-02-10 20:37:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1895" class=".btn">#1895</a>
            </td>
            <td>
                <b>
                    [refactor] #1892: remove `type Diff` in Execute
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                Signed-off-by: Marin Veršić <marin.versic101@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

I think this is just adds unnecessary complexity to codebase because even single Events are converted to `Vec` when executing instruction. I don't think we'll ever execute instructions except through the `Instruction` enum or that we need the ability to convert instructions into events

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-02-09 19:20:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1894" class=".btn">#1894</a>
            </td>
            <td>
                <b>
                    [feature]  #1877: produce events when executing wasm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Marin Veršić <marin.versic101@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

1. add event generation to wasm instruction execution
2. add integration test to verify events are generated
3. move `client/tests/integration_test` -> `client/tests/integration`

Submodules are a little bit special when inside `tests` directory. In particular, every `.rs` file inside `tests/` will be compiled as a separate crate. Is there a reason why all integration tests are inside `integration` directory and meticulously included in `tests/integration/mod.rs`? If not explicitly included these tests could be skipped, but on the other hand I think they get compiled as one crate instead of many?

### Issue

closes  #1877

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-02-09 18:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1886" class=".btn">#1886</a>
            </td>
            <td>
                <b>
                    [feature] #1606: Add ipfs link to domain logo in Domain structure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Add new field into Domain structure. Field represents IPFS link into Domain logo.
Add `IpfsPath` structure to superficially validate path

I haven't find good IPFS paths specifications, so I was inspiring these realisations:
1. [ipfs crate](https://docs.rs/ipfs/latest/src/ipfs/path.rs.html#42-75)
2. [cid crate](https://docs.rs/cid/0.5.1/src/cid/cid.rs.html#196-224)

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Resolves #1606 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now domains can have logo

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

IPFS paths isn't fully validated. Full validation requires hash decoding and possible requesting IPFS system to check, if image really exists.

Checkout #1885 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

See `client/integration_tests/add_domain.rs`

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->


<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 08:09:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1880" class=".btn">#1880</a>
            </td>
            <td>
                <b>
                    [documentation]: Add arjentix into codeowners file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Add myself to the codeowners file

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

I'm gonna receive notificaitons from this repo

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-02-07 17:56:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1879" class=".btn">#1879</a>
            </td>
            <td>
                <b>
                    [feature] #1767: Wasm limit memory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Linear memory can be limited with `StoreLimits` via `store.limiter` and therefore, importing memory from host wasn't required and would only increase complexity of writing smartcontract for the user

### Issue

closes #1767 

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

As of Wasmtime(0.33.0) the `Trap` returned is that of fuel consumed. I opened an issue with `Wasmtime` to fix that

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-02-07 16:41:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1878" class=".btn">#1878</a>
            </td>
            <td>
                <b>
                    [fix] #0000: Make implicitly ignored doc-test explicitly ignored. Fix…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                … typo.

Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements --


### Description of the Change

HotFix for ignored dockets becoming un-ignored on `stable-x86-darwin` toolchain. Fixed typo in aforementioned test.

### Issue

Closes #0000 (hot fix)

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Working test.

### Possible Drawbacks

none. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 15:32:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1876" class=".btn">#1876</a>
            </td>
            <td>
                <b>
                    Add in-repo documentation about GH Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds feature `skip_testing` to skip testing in jobs. This optional buildspec argument adds '-DTESTING=OFF' to cmake configuration step, disables step 'ctest' in build jobs in workflow.

`/build all skip_testing` is now default buildspec for manual workflow_dispatch.
Testers would want `/build ubuntu debug release gcc-9 normal skip_testing` to produce 2 configurations without burrow and ursa.


> ### To make workflow_dispatch (manual run from web UI or CLI)  work it must be merged to main branch. 
> ### Consider cherry-picking it to `develop` also

Signed-off-by: kuvaldini <ivan@kuvaldini.pro>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 13:19:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1874" class=".btn">#1874</a>
            </td>
            <td>
                <b>
                    [feature] #1619: Introduce event-based triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

Add `TriggerSet` and carry trigger recommendations through the lifecycle of a block. 

`TriggerSet` is stored in WSV. 

### Issue

Closes #1619
Closes #1859
Related to #1771 


### Benefits

Event triggers

### Possible Drawbacks

Prototype implementation, so both UX and reliability are untested. 

Event processing is quadratic.

Opens #1889 
Opens #1890
Opens #1891
Opens #1892 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 05:17:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1873" class=".btn">#1873</a>
            </td>
            <td>
                <b>
                    [fix] #1872: Wasm no multiline retval
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

Closes ##1872

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-02-07 00:13:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1871" class=".btn">#1871</a>
            </td>
            <td>
                <b>
                    Docs: Additions to 1.4 docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …eck endpoint, information about iroha-swarm tool

Signed-off-by: Sara G <lira.lemur@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Due to some git-related issues, this PR combines several PRs that would've conflicted or were not available anymore (fully my fault):
https://github.com/hyperledger/iroha/pull/1870 (yet unapproved) - Healthcheck Endpoint
https://github.com/hyperledger/iroha/pull/1741 (approved) - iroha-swarm added to docs
https://github.com/hyperledger/iroha/pull/1778 (approved) - build-fix
https://github.com/hyperledger/iroha/pull/1829 (approved) - RocksDB and Postgres comparison
https://github.com/hyperledger/iroha/pull/1850 (not fully approved) - good migration practice 

### Issue

Closes #1840
Closes #1834

### Benefits

More docs

### Possible Drawbacks

Sorry for combining these changes together


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-06 19:18:54 +0000 UTC
    </div>
</div>

