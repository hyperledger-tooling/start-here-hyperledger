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
                PR <a href="https://github.com/hyperledger/iroha/pull/3711" class=".btn">#3711</a>
            </td>
            <td>
                <b>
                    [ci] #3654: Add Dockerfiles to build iroha2 on GNU libc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
Add `Dockerfile.build.glibc` and `Dockerfile.glibc` files to build `iroha2-ci` and `iroha2` images on GNU libc library and without `musl`.

### Linked issue
#3654 

### Benefits
1. To have a `iroha2` CI on GNU libc and without `musl`.
2. To reduce the sizes of `iroha2-ci` and `iroha2` final images.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 14:26:54 +0000 UTC
    </div>
</div>

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

