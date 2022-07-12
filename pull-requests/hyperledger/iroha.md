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
                PR <a href="https://github.com/hyperledger/iroha/pull/2472" class=".btn">#2472</a>
            </td>
            <td>
                <b>
                    [feature] #2338: Add `cargo-all-features` instrumentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
- Bumped all versions to RC6
- Removed redundant examples. 
- Fixed all feature combinations to compile and have no warnings.
- Added metadata to exclude redundant checks of different feature sets (double coverage)
- Evaluated performance versus `cargo hack` (orders of magnitude faster). 

### Issue

Closes #2338 
<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Better feature consistency

### Possible Drawbacks

None

### Usage Examples or Tests *[optional]*

![image](https://user-images.githubusercontent.com/15856657/178465001-5cff3d49-0b60-40fa-ab6d-1ec3cbab5579.png)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 10:00:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2471" class=".btn">#2471</a>
            </td>
            <td>
                <b>
                    [feature] #1769: Optimize pub/sub messaging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

WIP.

- Establish all the possible channels at the components initialization
- Remove the broker

### Issue

- Closes #1769

### Benefits

- No broker access

### Possible Drawbacks

- Readability, if the boilerplate were pushed into macros

### Usage Examples or Tests

- 4082d4d1 implies the current implementation is not properly working
- f8e4dc0d is a blueprint -- not working due to lack of implementations

### Alternate Designs

The broker stores a receiver of 1:n channel on the publish declaration and clones on the subscription request:

```rust
use tokio::sync::watch::Receiver;

pub struct Broker {
    receivers: Arc<DashSet<Receiver<Box<dyn Msg>>>>,
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 09:24:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2470" class=".btn">#2470</a>
            </td>
            <td>
                <b>
                    [feature] #2467: Add account grant subcommand into iroha_client_cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">CLI</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

* Added `grant` subcommand for `account` command

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2467


### Benefits

Now users can grant permissions using `iroha_client_cli`

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

* Not a drawback of this PR, but still no support for roles
* We might need to introduce server response cheking in `Client::submit_transaction()` so that user can see if something has failed on the server-side
* I've mentioned that the documentation for `iroha_client_cli` tells about possibility to pass empty line for key when registering new account. This does not work now

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

1. Run docker compose:

``` bash
docker compose up
```

2. Open new terminal window and go to `configs/client_cli`

3. Run this commands:

```bash
cargo run --bin iroha_client_cli -- domain register --id looking_glass
cargo run --bin iroha_client_cli -- account register --id="mad_hatter@looking_glass" --key="ed01207233bfc89dcbd68c19fde6ce6158225298ec1131b6a130d1aeb454c1ab5183c0"
cargo run --bin iroha_client_cli -- asset register --id tea#looking_glass --value-type Quantity
```

4. Then create file `premission_token.json` and paste the following:

```json
{
    "name": "can_transfer_user_assets",
    "params": {
        "asset_id": {
            "Id": {
                "AssetId": {
                    "definition_id": {
                        "name": "tea",
                        "domain_id": {
                            "name": "looking_glass"
                        }
                    },
                    "account_id": {
                        "name": "mad_hatter",
                        "domain_id": {
                            "name": "looking_glass"
                        }
                    }
                }
            }
        }
    }
}
```

5. Open `config.json` in `configs/client_cli` directory and replace `alice` with `mad_hatter` and `wonderland` with `looking_glass`. This is needed because `alice` can't grant permissions to assets of another domain (I think so; I didn't checked if it's the real reason why it's not working without it)

6. Run the final command:

```bash
cargo run --bin iroha_client_cli -- account grant --id "mad_hatter@looking_glass" --permission permission_token.json
```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 20:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2469" class=".btn">#2469</a>
            </td>
            <td>
                <b>
                    [documentation]: Update test flakyness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Contents

Updated test flakyness. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 17:53:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2464" class=".btn">#2464</a>
            </td>
            <td>
                <b>
                    [ci]: Bump versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
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
        Created At 2022-07-11 07:49:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2463" class=".btn">#2463</a>
            </td>
            <td>
                <b>
                    [ci]: Bump versions
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
        Created At 2022-07-11 07:49:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2459" class=".btn">#2459</a>
            </td>
            <td>
                <b>
                    [documentation] hyperledger#2446 adds a spoiler to issue templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: 6r1d <vic.6r1d@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Adds a spoiler to issue templates, like in #2456.

### Issue

Fixes #2446

### Benefits

* Adds a spoiler with highlight as a default value, potentially improving readability
* Asks user to format logs if formatting is broken for some reason
* Hints a code highlight is needed for Rust MWE

### Possible Drawbacks

None

### Usage Examples or Tests

Creating an example issue in [this fork](https://github.com/6r1d/iroha/issues/new/choose) can show the current form.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 14:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2453" class=".btn">#2453</a>
            </td>
            <td>
                <b>
                    [feature] #2098: Block header queries
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

Added queries for block headers.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#2098 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 12:21:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2452" class=".btn">#2452</a>
            </td>
            <td>
                <b>
                    [fix] #2416: Fix lints on macOS arm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ales Tsurko <ales.tsurko@gmail.com>

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
A cross-platform wrapper for `BlockValue` added to encapsulate platform dependent code. On macOS with arm architecture `Value::Block` inner is now boxed. 

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Closes #2416 

### Benefits

<!-- What benefits will be realized by the code change? -->
No more linter errors on M1.

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
As it's now a smart pointer, it requires dereferencing, when the inner value is needed.

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
        Created At 2022-07-07 10:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2448" class=".btn">#2448</a>
            </td>
            <td>
                <b>
                    [documentation] #2446: improve issue templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change

This PR adds detailed forms to fill into the issues. To see the issue form, open [this page](https://github.com/6r1d/iroha/issues/new/choose).

### Issue

This PR closes #2446 and covers all the items in it.

### Benefits

* Contributors sending the bug requests will fill the form with all the details that are needed for quicker debugging.
* The supported branches of Iroha are immediately visible.
* Contributors also see who to tag, so the issue gets resolved faster.
* People who have questions will immediately see Discord and Telegram community links.

### Possible Drawbacks

~~I have several questions I'll be marking as resolved here~~.
**UPD**: these questions were resolved.

- [x] I am not sure where to redirect people who have an SDK problem. In addition to that, it is possible to add a link to SDK in `/issues/new/choose`. This detail needs to be considered before the merge.
- [x] The [Discord server link](https://discord.gg/hyperledger) with `#iroha` channel shows a Telegram bridge and little activity. Is it the current actual Discord for Iroha?
- [x] The tags are auto-filled and need a change; I have not seen a `stable` tag, so both types of issues are tagged the same way, making it confusing.
- [x] This PR still has `blank_issues_enabled` as `true` for now. I think this will need a bit of a discussion: should we have blank issues in addition to the "bug" issues for questions, not related to bugs or future planning?
- [x] I am not sure if [this](https://hyperledger.github.io/iroha-2-docs/guide/configure/peer-configuration.html#logger) is the correct documentation link for JSON logs. While all the details match, is it the correct doc to refer to?

### Alternate Designs

At a later date, there may be an internal command to collect most of the current Iroha environment data: LibC version, OS info, etc. I am not sure if this can be done reliably all the time, so I am thinking of implementing this at a later date.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 05:31:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2447" class=".btn">#2447</a>
            </td>
            <td>
                <b>
                    [feature] #2454: Add a build script to the parity-scale-decoder tool
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

Add a build script that automatically updates sample binaries from sources in the parity-scale-decoder. This feature also fixes the broken test from #2418. 

### Issue

Resolves #2454 

### Benefits

Automatically updates sample binaries from sources.

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
        Created At 2022-07-06 17:21:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2445" class=".btn">#2445</a>
            </td>
            <td>
                <b>
                    [fix] #1480: Shut down on panic
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
Currently, when panic occurs, only the corresponding thread shuts down. But we need the whole program to shut down if a panic appeared on any thread. A panic hook is provided, which uses [`tokio::sync::Notify`](https://docs.rs/tokio/1.19.2/tokio/sync/struct.Notify.html) to gracefully shut down the program.

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Fixes #1480 

### Benefits

<!-- What benefits will be realized by the code change? -->

The program will shut down gracefully if a panic occurs on any thread.

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
As we use globals (i.e. panic hook), it can affect tests in some cases. But the test environment should be close or same as the production one. Following contributors should have it in mind.

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

[A cargo config](https://doc.rust-lang.org/book/ch09-01-unrecoverable-errors-with-panic.html) or `std::process::exit` can be used instead, but that could leave garbage.

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 13:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2436" class=".btn">#2436</a>
            </td>
            <td>
                <b>
                    [refactor] #2369: Refactor permission validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
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

* Type returned by `IsAllowed` changed from `Result` to `ValidatorVerdict`
* `ValidatorVerdict` allows validators to skip checking if operation is unsuported or has no meaning for them
* Added `Judge` trait returning `Result`. Judge usually gather validators together to produce result based on verdicts from validators
* Removed `IsAllowedBoxed`. To be able to parse permissions from genesis we should introduce an enum`JudgeBoxed` in future. That's should be anough to deserialize.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2369 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* More readable error message
* More meaningfull validators system

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

* Very detailed error message. Maybe we should use `Display` instead of `Debug` for it

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 22:46:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2435" class=".btn">#2435</a>
            </td>
            <td>
                <b>
                    [fix] #2422: Hide private keys in configuration endpoint response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">macros</span>
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

- Add configuration-related to `data_model` to be able to share configuration;
- Fix `GetConfiguration` endpoint to return sharable configuration without private keys;
- Add proc macro to derive conversation between inner and sharable config. 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closses #2422.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

- No sensitive information are leaked;
- Opens possibility to share configuration between peers through Query (#1966);

### Possible Drawbacks

- Duplication configuration structs.
- Add dependency `iroha_data_model` to `telemetry` and `logger` crates.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Alternate Designs

Simpler solution would be to mask or hide private keys during serialization but this would affect generated reference configuration.
Add it still won't be possible to send config through queries.

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
        Created At 2022-07-05 14:23:52 +0000 UTC
    </div>
</div>

