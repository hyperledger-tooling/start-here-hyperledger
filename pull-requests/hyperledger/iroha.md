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
                PR <a href="https://github.com/hyperledger/iroha/pull/2374" class=".btn">#2374</a>
            </td>
            <td>
                <b>
                    [feature] #2053: Add tests to the asset-related queries in private blockchain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">2.0.0-pre-rc.5-lts</span>
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

Add tests to the asset-related queries in private blockchain. 

### Issue

Partially resolves #2053 .

### Benefits

New tests.

### Possible Drawbacks

None.

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 22:33:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2372" class=".btn">#2372</a>
            </td>
            <td>
                <b>
                    Docs: iroha-swarm Description + Deploy docs Fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sara <lira.lemur@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Added description to iroha-swarm and fixed some issues with Deploy part of the docs

### Issue

Request by @kuvadldini

### Benefits

Better docs. 

### Possible Drawbacks
None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 00:52:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2371" class=".btn">#2371</a>
            </td>
            <td>
                <b>
                    [fix] #2081: Fix role granting bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">2.0.0-pre-rc.5-lts</span>
            </td>
            <td>
                ### Bug description

Our `IsGrantAllowed` validators was checking only for *permissions* and not for *roles* granting. This validators return `Err` if got something unexpected. That's why SDK-developers test was failing.

Our integration tests was using `AllowAll` for instruction validation by default. That's why test introduced in #2312 haven't fully covered real world scenario.

### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

* Fixed bug with granting role. Before that it was only possible to gran permissions
* Default instructions validator for integration tests was replaced with `default_permissions()`. This will reduce the gap between our integration tests and SKD-developers tests
* `Role` registration process was unified with other things registration such as `Domain` and `Account`
* Add more `const` to some functions

### Issue

* Closes #2081 
* Opens #2368
* Opens #2369
* Opens #2370

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* Closed bug request
* Now it's possible to grant roles with `default_permissions()`, not only permissions
* More consistency with SDK-developers test

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Now tests by default are sensitive for instructions and signer (`alice@wonderland` right now). I.e. it's illegal now to mint roses, because noone can mint assets that was registered by another account.
This can be bypassed by setting custom validators. Example:

```rust
let (_rt, _peer, mut test_client) = <PeerBuilder>::new()
    .with_instruction_validator(AllowAll)
    .start_with_runtime();
```

But be carefull, because this is not how `Iroha 2` works by default. This may introduce inconsistency between our and SDK-developers tests.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-18 15:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2367" class=".btn">#2367</a>
            </td>
            <td>
                <b>
                    [ci] #1658: Add documentation check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Sorry for omitting the PR template here, but the change is very little and clear. It just adds  documentation check (using `cargo doc`) to CI.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 21:55:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2366" class=".btn">#2366</a>
            </td>
            <td>
                <b>
                    Fix/single send state creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Minor optimization
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 15:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2365" class=".btn">#2365</a>
            </td>
            <td>
                <b>
                    [refactor] #1985: Reduce size of `Name` struct
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

- Add `ConstString`: immutable, inlinable string, which uses `union` internally to store boxed and inlined variants in the same space;
- Replace `String` with `ConstString` in `Name` struct.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #1985.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

All structs that uses `Name` take up less space.
We win at least one machine word for every instance of `Name` and up to 23 byte for strings 15 bytes long on 64-bit architecture, also strings shorter than 15 bytes are stored on the stack, which avoids allocation.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

`ConstString` uses `unsafe` code, which increases the risk of bugs and vulnerabilities.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

```
cargo test --package iroha_data_primitives --lib -- conststr::tests --nocapture
```

### Alternate Designs

It possible to use enum instead of union to avoid `unsafe`, but it take 24 bytes instead of 16, [see](https://play.rust-lang.org/?version=stable&mode=debug&edition=2021&gist=a28c4bfc22d99f5808638dcc82c46553).

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
        Created At 2022-06-16 15:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2364" class=".btn">#2364</a>
            </td>
            <td>
                <b>
                    Feature/single pointer cache ref
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Minor refactoring to remove mutex overhead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 10:02:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2363" class=".btn">#2363</a>
            </td>
            <td>
                <b>
                    [fix] #2137: Prepare tests for multiprocess context
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

This is a draft for now. I need to clean up everything and document the code. Also, I suggest extending [the fork of `unique_port`](https://github.com/soramitsu/iroha2-unique_port) with my changes, instead of copy-pasting it here to extend it.

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
        Created At 2022-06-15 22:18:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2359" class=".btn">#2359</a>
            </td>
            <td>
                <b>
                    [fix] #2358: Add release with debug profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Sam H. Smith <sam.henning.smith@protonmail.com>

### Description of the Change
Adds a profile in the workspace Cargo.toml.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
#2358 
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
        Created At 2022-06-14 09:03:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2357" class=".btn">#2357</a>
            </td>
            <td>
                <b>
                    Feature/proposal batches
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Safe implementation of batched proposals processing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 06:18:52 +0000 UTC
    </div>
</div>

