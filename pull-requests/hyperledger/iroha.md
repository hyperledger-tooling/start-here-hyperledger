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
                PR <a href="https://github.com/hyperledger/iroha/pull/3064" class=".btn">#3064</a>
            </td>
            <td>
                <b>
                    [fix] #1170: Implement cloning-wsv-style soft-fork handling.
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
        Created At 2023-01-17 18:47:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3062" class=".btn">#3062</a>
            </td>
            <td>
                <b>
                    [feature] #2794: Reject Fieldless enums with explicit discriminants in FFI
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

Derive macro `FfiType` now rejects fieldless enums with explicit discriminants.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2794.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Less space to make errors.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 13:51:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3060" class=".btn">#3060</a>
            </td>
            <td>
                <b>
                    [refactor]: simplify sumeragi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

I believe you will find it much more easier to understand now
I also left some comments in the code

The hanging issue still persists:
1. `Failed to push into queue err=InBlockchain` is observed:
```
2023-01-12T22:42:41.821378Z  WARN request{method=POST path=/transaction version=HTTP/1.1 remote.addr=127.0.0.1:54960}: iroha::torii::routing: Failed to push into queue tx_hash=d543e665272d74fd5f6733d1ca01869c78ac8633e7b5a49c36b563fb6baa51b9 err=InBlockchain
2023-01-12T22:42:41.821378Z  WARN request{method=POST path=/transaction version=HTTP/1.1 remote.addr=127.0.0.1:54955}: iroha::torii::routing: Failed to push into queue tx_hash=5b042f8b52a4d9cc1fca8f57d237cb8c5ff8f92aa58333f61314eb859dc5ae37 err=InBlockchain
2023-01-12T22:42:41.821378Z  WARN request{method=POST path=/transaction version=HTTP/1.1 remote.addr=127.0.0.1:54966}: iroha::torii::routing: Failed to push into queue tx_hash=5a272b4b5f92ad980bb23a7632672ebcf1ba076ca56cd7b967cbd88b182d90f7 err=InBlockchain
2023-01-12T22:42:41.821423Z  WARN request{method=POST path=/transaction version=HTTP/1.1 remote.addr=127.0.0.1:54960}: warp::filters::trace: unable to serve request (client error) status=400 error=None
2023-01-12T22:42:41.821423Z  WARN request{method=POST path=/transaction version=HTTP/1.1 remote.addr=127.0.0.1:54955}: warp::filters::trace: unable to serve request (client error) status=400 error=None
2023-01-12T22:42:41.821456Z  WARN request{method=POST path=/transaction version=HTTP/1.1 remote.addr=127.0.0.1:54966}: warp::filters::trace: unable to serve request (client error) status=400 error=None
2
```
2. And is followed by endless view changes where view change index increases:
```
2023-01-12T21:55:55.603155Z  WARN run: iroha_core::sumeragi::main_loop: Block not committed in due time, requesting view change... role=ObservingPeer
2023-01-12T21:55:55.607356Z  WARN run: iroha_core::sumeragi::main_loop: Block not committed in due time, requesting view change... role=ProxyTail
2023-01-12T21:55:55.610777Z  WARN run: iroha_core::sumeragi::main_loop: Block not committed in due time, requesting view change... role=Leader
2023-01-12T21:55:55.615403Z  WARN run: iroha_core::sumeragi::main_loop: Block not committed in due time, requesting view change... role=ValidatingPeer
2023-01-12T21:55:55.617158Z ERROR run: iroha_core::sumeragi::main_loop: No consensus, updating view change ... current_view_change_index=4
2023-01-12T21:55:55.618910Z ERROR run: iroha_core::sumeragi::main_loop: No consensus, updating view change ... current_view_change_index=4
2023-01-12T21:55:55.622082Z ERROR run: iroha_core::sumeragi::main_loop: No consensus, updating view change ... current_view_change_index=4
2023-01-12T21:55:55.625818Z ERROR run: iroha_core::sumeragi::main_loop: No consensus, updating view change ... current_view_change_index=4
2
```

This might also mean that there are no new incoming transactions

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
        Created At 2023-01-12 22:02:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3058" class=".btn">#3058</a>
            </td>
            <td>
                <b>
                    [ci]: Adding five more self-hosted runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Signed-off-by: BAStos525 <jungle.vas@yandex.ru>

### Description of the Change
1. Add four more self-hosted runners for `I2::Dev::Tests` workflow.
2. Add a new self-hosted runner for `I2::Dev::Publish` workflow.
3. Make `load-rs` job inside `I2::Dev::Publish` workflow conditional.

### Issue
1. We can not run a two `I2::Dev::Tests` workflows in parallel on self-hosted runners (increase their amount from 4 to 8 for four tests jobs).
2. A `dockerhub` job  inside `I2::Dev::Publish` workflow takes a lot of time.
3. `I2::Dev::Publish` workflow fails if `load-rs` job was failed or `load-rs` job doesn't run.

### Benefits

1. Now a two`I2::Dev::Tests` workflows could be run in parallel.
2. Increase `dockerhub` job  inside `I2::Dev::Publish` speed.
3. Do not failI `2::Dev::Publish` workflow if `load-rs` job was fails.

### Possible Drawbacks

None.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 11:25:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3057" class=".btn">#3057</a>
            </td>
            <td>
                <b>
                    doc: correct typos in `readme.md`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: typos

Signed-off-by: omahs <73983677+omahs@users.noreply.github.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 09:51:46 +0000 UTC
    </div>
</div>

