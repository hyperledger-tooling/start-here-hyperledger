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
                PR <a href="https://github.com/hyperledger/iroha/pull/2074" class=".btn">#2074</a>
            </td>
            <td>
                <b>
                    Iroha v1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Contains all features and fixes for v1.5
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 12:09:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2071" class=".btn">#2071</a>
            </td>
            <td>
                <b>
                    DOPS-1722: CI for iroha2-longevity-load-rs
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

Signed-off-by: Vasilii Zyabkin <vzyabkin@soramitsu.co.jp>

### Description of the Change
Add action to trigger the CI workflow for `iroha2-longevity-load-rs` in order to build and push its image:release to docker registry.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Currently we don't have CI for `iroha2-longevity-load-rs` at all.
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
It should be automatically triggers to run iroha2-longevity-load-rs CI from other repository at the successful ending of iroha2 release deploy workflow job.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Some possibility for issue with token permissions since it's required to use third-party creds.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*
https://github.com/soramitsu/iroha2-longevity-load-rs/actions
<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 07:47:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2070" class=".btn">#2070</a>
            </td>
            <td>
                <b>
                    DOPS-1722: CI for iroha2-longevity-load-rs
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

Signed-off-by: Vasilii Zyabkin [vzyabkin@soramitsu.co.jp](mailto:vzyabkin@soramitsu.co.jp)

### Description of the Change
Add action to trigger the CI workflow for `iroha2-longevity-load-rs` in order to build and push its image to docker registry.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Currently we don't have CI for `iroha2-longevity-load-rs` at all.
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
It should be automatically triggers to run `iroha2-longevity-load-rs` CI from other repository at the successful ending of `iroha2-dev` deploy workflow job.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Some possibility for issue with token permissions since it's required to use third-party creds.
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
        Created At 2022-04-07 07:42:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2069" class=".btn">#2069</a>
            </td>
            <td>
                <b>
                    Docs: Fix Docs Build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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

Fixed broken requirement

### Issue

Jinja2 and MarkupSafe had an issue. Now they are friends again :) 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Building docs

### Possible Drawbacks

None

### Usage Examples or Tests *[optional]*

Tested on RTD on test acc - all works. 

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

[skip ci] (in case it works)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 22:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2065" class=".btn">#2065</a>
            </td>
            <td>
                <b>
                    Feature/rdb burrow storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
RocksDB storage implementation for Burrow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 14:29:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2063" class=".btn">#2063</a>
            </td>
            <td>
                <b>
                    [feature] #0000: Add pagination to schema. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

### Description of the Change



### Issue

Relevant to #1998 

### Benefits

Queries can now be paginated. 

### Possible Drawbacks

None

### Usage Examples or Tests 

```rust 
#![allow(clippy::restriction)]

use std::thread;

use iroha_client::client::asset;
use iroha_data_model::prelude::*;
use test_network::{Peer as TestPeer, *};

use super::Configuration;

#[test]
fn client_add_asset_quantity_to_existing_asset_should_increase_asset_amount() {
    let (_rt, _peer, mut iroha_client) = <TestPeer>::start_test_with_runtime();
    wait_for_genesis_committed(&vec![iroha_client.clone()], 0);
    let pipeline_time = Configuration::pipeline_time();

    let register: Vec<Instruction> = ('a'..'z')
        .map(|c| c.to_string())
        .map(|name| AssetDefinitionId::new(&name, "wonderland").expect("Valid"))
        .map(AssetDefinition::new_quantity)
        .map(IdentifiableBox::from)
        .map(RegisterBox::new)
        .map(Instruction::Register)
        .collect();
    iroha_client
        .submit_all(register)
        .expect("Failed to prepare state.");

    thread::sleep(pipeline_time);
    //When

    let vec = iroha_client
        .request_with_pagination(
            asset::all_definitions(),
            Pagination {
                start: Some(5),
                limit: Some(5),
            },
        )
        .expect("Failed to get assets");
    assert_eq!(vec.len(), 5);
}
```



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 08:43:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2057" class=".btn">#2057</a>
            </td>
            <td>
                <b>
                    [refactor]: Remove unnecessary `&mut` from the API.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

### Description of the Change

Remove unnecessary `&mut` references from the client. 

### Issue

HotFix

### Benefits

Fewer Mutexes needed

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 12:17:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2054" class=".btn">#2054</a>
            </td>
            <td>
                <b>
                    [fix] #1917: Added easy_from_str_impl macro for use with AssetValueType
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

Created a variadic declarative macro that implements FromStr for C like enums.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#1917 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Future FromStr implementations for C like enums can be a lot smaller codesize.

### Possible Drawbacks

May be harder to read and understand for some.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 11:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2051" class=".btn">#2051</a>
            </td>
            <td>
                <b>
                    [feature] #2040: Add integration test with transaction execution limit
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

- Added new permission validator that checks for `Transfer` execution count and sets some limit per time period. I.e. it's possible to limit someone to **10** `Transfer` transactions per day
- Added test which demostrates it. Also there are additional comments so that someone from Orillion project could read this, cause this test is needed for their use-cases

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2040 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

One more permission validator and one more integration test

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

- I'm not sure if I used permission validators system on the right way
- Should this new validator participate in `default_permissions()`?

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 00:24:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2049" class=".btn">#2049</a>
            </td>
            <td>
                <b>
                    [feature] #2048: Add toolchain file
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

Added toolchain file setting up rustc to version 1.57

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2048 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now project can be build without additional steps like `rustup override`

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Not a drawback, but at first I thought that will be a way to set different toolchains for different tools.
Unfortunatly we still have to use `cargo +<toolchain> ...` for `clippy` and `fmt`.

This situation looks a bit like `clippy` problem with multiple sub-crates, so that we have to use `cargo lints`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 17:44:31 +0000 UTC
    </div>
</div>

