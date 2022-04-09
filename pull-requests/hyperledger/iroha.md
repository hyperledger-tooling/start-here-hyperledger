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
                PR <a href="https://github.com/hyperledger/iroha/pull/2079" class=".btn">#2079</a>
            </td>
            <td>
                <b>
                    [feature] #2003: Introduce Parity Scale Decoder tool
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

* Added new derive-macro `DumpDecoded` and corresponding trait
* New derive is used on pretty all `data_model` types. Exceptions: those, which don't implement `Debug + Decode`, and generics
* Added `tools/parity_scale_decoder`
* Added some binary samples for testing and demo

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2003 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* With this tool we can debug incompatibility issues
* Useful for SDK developers

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

That's the tricky part... Here I use 3 different procedurals macros and 2 of them should be executed in order. Rust have no guarantees for that and that's the problem. See [here](https://stackoverflow.com/questions/52910783/is-it-possible-to-store-state-within-rusts-procedural-macros) for details. Right now it works on my machine and I think it should be fine for others too.

Order:

1. Derive macro. Used in `data_model` multiple times. Generates implementation and adds type name at the global vector
2. `generate_dump_decoded_map!()`. Used in `data_model` once. Takes names from global vector and creates global Map with `Type Name -> dump_decoded() ptr` reflection
3. `get_dump_decoded_map!()`. Used in `parity_scale_decoder`. Just a getter for global map from step 2.

This approach allows not to hardcode every type by hand inside `parity_scale_decoder`... At least while it's working. **If sometime we will have a trouble with it, we can rewrite it using the less (or more?) elegant way, see the last section.**

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

See README.md

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs

#### Hardcode types-map by hand
Pros:
  * Safe
  * Clear what types are presented
 
Cons:
  * Inflexible
  * A lot of code

#### Use `include!(data_model)`

Just an idea. Not even sure it's possible

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

### Another thing to note

We should be care when choosing #1983 implementation so that it don't rely on macro exectuion order as this one
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 22:59:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2077" class=".btn">#2077</a>
            </td>
            <td>
                <b>
                    [refactor] #1982: encapsulate access to `iroha_crypto` structures
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
        Created At 2022-04-08 17:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2076" class=".btn">#2076</a>
            </td>
            <td>
                <b>
                    [fix] #1623: Create a RawGenesisBlockBuilder
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

Created a builder struct to ease the assembling of genesis blocks for used in tests and by a web tool.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#1623

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Many of the tests can be made more efficient using this instead of client code to register accounts et cetera.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

It is possible to create invalid genesis blocks using the builder as validation would slow it down and add complexity.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 14:37:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2075" class=".btn">#2075</a>
            </td>
            <td>
                <b>
                    Iroha v1.5 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Contains all features and fixes for iroha v1.5
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 12:40:10 +0000 UTC
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

