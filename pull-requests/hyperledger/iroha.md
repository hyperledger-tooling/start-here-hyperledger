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
                PR <a href="https://github.com/hyperledger/iroha/pull/2095" class=".btn">#2095</a>
            </td>
            <td>
                <b>
                    [fix] #2005: Fix `Client::listen_for_events()` not closing WebSocket stream
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

* Fix `Client::listen_for_events()` not closing WebSocket stream
* Fix `torii` doing only part of WebSocket handshake

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2005

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now event streaming satisfies WebSocket protocol

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 12:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2082" class=".btn">#2082</a>
            </td>
            <td>
                <b>
                    [skip ci] Retire inactive maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Last activity:
2019/07/24 06:25:12 issue_comment.update bakhtin
2018/12/11 14:07:33 issue_comment.update grimadas
2019/12/25 14:09:13 repository_vulnerability_alert.resolve igor-egorov
2019/01/16 12:36:58 issue_comment.update l4l
2018/09/25 11:34:38 issue_comment.update laSinteZ
2018/02/16 15:38:38 issue_comment.update luckychess
2018/07/19 16:06:05 issue_comment.destroy muratovv
2019/02/20 10:16:17 issue_comment.update neewy
2018/12/21 14:47:14 issue_comment.destroy nickaleks
2018/05/03 04:59:54 issue_comment.update Solonets
2018/07/10 13:27:31 issue_comment.update stinger112
2018/06/29 18:16:18 issue_comment.update tyvision
2018/03/20 14:42:37 issue_comment.update victordrobny
2018/03/27 10:07:33 issue_comment.update x3medima17
2017/06/28 05:35:19 org.oauth_app_access_requested yannoban

Signed-off-by: Ry Jones <ry@linux.com>

### Description of the Change

Retire inactive maintainers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 21:46:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2080" class=".btn">#2080</a>
            </td>
            <td>
                <b>
                    [feature] #2003: Introduce Parity Scale Decoder tool (stable implementation)
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

## Caution!!!

This is the alternative implementation of #2079 . Only one of them should be accepted in the end

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Added the same tool as in #2079 but with alternative design and implementation. Every type is hardoced now.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2003 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits over #2079 

* Should work everywhere and forever
* Much less code
* Supported types are predictable

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

* Every new type should be added mannualy in this tool source code

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 14:54:23 +0000 UTC
    </div>
</div>

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

