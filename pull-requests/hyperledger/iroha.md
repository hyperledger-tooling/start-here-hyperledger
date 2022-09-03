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
                PR <a href="https://github.com/hyperledger/iroha/pull/2693" class=".btn">#2693</a>
            </td>
            <td>
                <b>
                    [refactor] #2650: Add `ThreadHandle` to shutdown iroha submodules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

- Add `ThreadHandler` struct to shutdown iroha submodules threads on `Iroha` shutdown (RAII).
- Rewrite `Kura` block writing loop: on shutdown `Kura` writes remaining blocks and then exits.
- Add temporary directory to `Peer` struct to delete directory after `Iroha` (and thus `Kura` thread).  

### Issue

Closes #2650.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Unified mechanism for stopping iroha submodules threads.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Alternate Designs

Possibly better name for `ThreadHandler` :)

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
        Created At 2022-09-02 15:01:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2692" class=".btn">#2692</a>
            </td>
            <td>
                <b>
                    [ci]: Add step to upload iroha2 stable image to Soramitsu registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Signed-off-by: BAStos525 [jungle.vas@yandex.ru](mailto:jungle.vas@yandex.ru) 


### Description of the Change
1. Add the step to `I2::Release::Publish` workflow to upload `stable` and `lts` iroha2 images to Soramitsu Harbor private registry.

### Issue
@Mingela asked to add this feature after incident with testnet due to overwritten image on DockerHub.

### Benefits

To have an opportunity to keep `stable` and `lts` images of iroha2 in the reliable private registry as well.

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 14:49:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2687" class=".btn">#2687</a>
            </td>
            <td>
                <b>
                    [feature] #2677: WASM base64 (de-)serialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">Yellow</span>
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

* Added *base64* (de-)serialization for `WasmSmartContract` structure
* Checkouted `iroha_client` build-script from #2641 
* Created test

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2677 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Possibility to use normally-looking WASM code in genesis. This allows us:

* Submitting smartcontracts inside genesis transactions to achieve complex logic
* Submitting WASM-triggers in genesis
* Submitting WASM-validators in genesis (after merge of #2641)

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Breaks existing API, but it wasn't used by anyone, I believe

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

1. Comment the **line 312** (the one with `ignore`) in `client/tests/integration/triggers/by_call_trigger.rs`
2. Run the following:
    ```bash
    cargo +nightly-2022-08-15 test --package iroha_client --test mod -- integration::triggers::by_call_trigger::trigger_in_genesis_using_base64 --exact --nocapture
    ```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 13:14:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2683" class=".btn">#2683</a>
            </td>
            <td>
                <b>
                    [fix] #0: Remove `/iroha/rust-toolchain.toml` from the builder image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

- Cherry-pick of 1d4a9499 from #2680

### Issue

- Docker fails to build

### Benefits

- Fix

### Possible Drawbacks

- None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 08:50:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2682" class=".btn">#2682</a>
            </td>
            <td>
                <b>
                    [fix] #2678: Fix tests abort on Kura force shutdown.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Sam H. Smith <sam.henning.smith@protonmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Stop a kura panic from aborting the tests.

### Issue

Partial fix for #2678 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 07:30:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2680" class=".btn">#2680</a>
            </td>
            <td>
                <b>
                    [ci]: Fix after #2662, #2663 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                <!-- [ci]: Fix after #2662, #2663 -->
### Description of the Change

1. Publish `iroha2-base` and `iroha2` images in sequence
2. Trigger `trybuild` tests on release PRs instead of on dev PRs
3. Remove `/iroha/rust-toolchain.toml` from the builder image

### Issue

1. https://github.com/hyperledger/iroha/pull/2662#discussion_r959346170
2. https://github.com/hyperledger/iroha/pull/2663#discussion_r959424599
3. https://github.com/hyperledger/iroha/pull/2663#discussion_r959480886

### Benefits

- Fix

### Possible Drawbacks

- None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 14:47:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2673" class=".btn">#2673</a>
            </td>
            <td>
                <b>
                    [feature] #2672: Add `ipv4Addr` variant and predicates.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Add `ipv4Addr` variant to `Value`, and predicates to filter on ranges of `Ipv4Addr`s. 
### Issue

Closes #2672

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

One step closer to #1786 

### Possible Drawbacks

More complexity

### Usage Examples or Tests *[optional]*

See `predicate.rs`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 06:35:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2670" class=".btn">#2670</a>
            </td>
            <td>
                <b>
                    [fix] #2667: Refactor &Option<T> to Option<&T>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Jonathan Plasse <13716151+JonathanPlasse@users.noreply.github.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Replace `&Option<T>` by `Option<&T>` as described in  #2667
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
        Created At 2022-08-29 20:34:52 +0000 UTC
    </div>
</div>

