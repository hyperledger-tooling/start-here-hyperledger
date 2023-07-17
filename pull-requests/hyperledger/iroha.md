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
                PR <a href="https://github.com/hyperledger/iroha/pull/3710" class=".btn">#3710</a>
            </td>
            <td>
                <b>
                    [feature] #3688: Implement basic arithmetic as proc macro
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Implement skeleton DSL crate. Arithmetic and boolean logic handled as a procedural macro. Uses `data_model::expression`. 

### Linked issue

Closes #3688 

### Benefits

DSL for expressions.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
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
        Created At 2023-07-17 07:44:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3708" class=".btn">#3708</a>
            </td>
            <td>
                <b>
                    [refactor] #3289: Use workspace inheritance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR extracts all common dependencies (2 usages or more) into a workspace level, so that it is easier to update them in lockstep.

Also, all iroha crates besides except inner `_derive` crates are also specified at workspace level.

### Issues

There are two places where I couldn't unify the dependencies:

1. `tokio-tungstenite` of versions 0.16 and 0.17 is used
https://github.com/hyperledger/iroha/blob/39504a5a8029080e0a7fe93b0f06a74710dba347/client/Cargo.toml#L44-L43

2. `clap` v3 and v4 is used:
https://github.com/hyperledger/iroha/blob/39504a5a8029080e0a7fe93b0f06a74710dba347/client_cli/Cargo.toml#L31-L30

I haven't tried too hard, but it seems that it would require some code changes to update these places. 

### Linked issue

Closes #3289 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 14:18:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3707" class=".btn">#3707</a>
            </td>
            <td>
                <b>
                    [feature] #3692: Validator migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

- Removed `permission_tokens()` entrypoint
- Created `migrate()` entrypoint
- Implemented migration on validators side
- Updated `entrypoint` macro
- Added new Runtime for migration including imports to (un-)register permission tokens
- Permission tokens update is now the responsibillity of validators
- Added test to check that failed migration makes no side effects

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3692 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Possibility to write any custom logic to perform migration from one validator to another

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2023-07-13 12:29:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3706" class=".btn">#3706</a>
            </td>
            <td>
                <b>
                    [ci]: Trigger iroha2 PR-build only for PR-generator case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

1. Add the trigger to build iroha2 PR-image from INTERNAL repository `hyperledger/iroha` branch if it's a PR-generator case.

## Requirements
1. INTERNAL branch should start from `iroha2-pr-deploy/`
2. PR should has `experimental_environment` label

### Benefits

Check if iroha2 PR-image is properly buildable when it's necessary.


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
        Created At 2023-07-12 17:20:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3703" class=".btn">#3703</a>
            </td>
            <td>
                <b>
                    [fix] #3613: Do not tolerate invalid signatures on transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Fail deserializing/decoding transactions with invalid signatures 

Closes #3613 

## Unsolved questions

1. There are other places where the "retain valid signatures" logic is used: https://github.com/hyperledger/iroha/blob/c0a59c002b822a9dbca9bba376651d0e7457547a/core/src/sumeragi/network_topology.rs#L233 and https://github.com/hyperledger/iroha/blob/c0a59c002b822a9dbca9bba376651d0e7457547a/core/src/sumeragi/main_loop.rs#L1042 Maybe the logic in these places should be changed too? Or would it break some assumptions?

2. Error handling here is a bit funky. It returns an ad-hoc `&'static str` as an error type, potentially losing some context. It _could_ make sense to defined another error type just for this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 14:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3701" class=".btn">#3701</a>
            </td>
            <td>
                <b>
                    Kura init mode, wsv serialization basics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR is not done. But I want to get feedback on the strategy taken for serializing the WSV. If you think I should do something differently or that I've missed something please tell me.

### Linked issue

Closes #1915 

### Benefits

Fast init and boot for peers after power outage. 

### Checklist

- [ ] Draft PR released
- [ ] Strategy analysed
- [ ] Weakpoints discovered
- [ ] Weakpoints addressed
- [ ] Regular PR
- [ ] Tests (via Pytest)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 07:50:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3699" class=".btn">#3699</a>
            </td>
            <td>
                <b>
                    [ci]: Remove i2 PR-build trigger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                [ci]: Remove i2 PR-build & Update rust nightly toolchain

## Description
1. Remove PR-trigger from `I2::Dev::Publish` workflow. It doesn't make sense it is always executed in base branch context. `pull_request` trigger makes sense only if PR is coming from internal repo PR branch. But it fails while PR from fork. Increasing workflow permission doesn't help as well. Instead of this, to check if PR-image is buildable, we can try PR-generator feature soon with the whole k8s CI/CD process when it's really necessary. Or to invent an another approach like keeping Actions secrets in an external place.

### Linked issue
[Failed Actions](https://github.com/hyperledger/iroha/actions/runs/5517090208)

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 11:35:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3698" class=".btn">#3698</a>
            </td>
            <td>
                <b>
                    [refactor] #3374: Unify error's doc-comments and Display impl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Use `displaydoc` instead of `derive_more`'s `Display` derive or `thiserror`'s `error` attribute.

This unifies error's doc-comments and `Display` implementation, as they are often repeated/convey the same information.

Sometimes `#[ignore_extra_doc_attributes]` is used. In this case only the first line of the doc-comment is used for the `Display`, leaving the others only for documentation

### Linked issue

Closes #3374

### Checklist

- [x] `iroha_promitives`
- [x] `iroha_data_model`
- [x] `iroha_p2p`
- [x] `iroha_config`
- [x] `iroha_client`
- [x] `iroha_core`
- [x] `iroha`
- [x] make sure all tests pass


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 08:38:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3694" class=".btn">#3694</a>
            </td>
            <td>
                <b>
                    [bump]: Rust toolchain and CI container to `nightly-2023-06-25`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Caution, make sure all CI checks pass before merging. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 13:32:24 +0000 UTC
    </div>
</div>

