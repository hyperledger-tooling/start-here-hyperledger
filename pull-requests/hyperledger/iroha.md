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
                PR <a href="https://github.com/hyperledger/iroha/pull/3652" class=".btn">#3652</a>
            </td>
            <td>
                <b>
                    [fix] #3352: Split up control flow and data messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Create a second incomming packet queue inside sumeragi.

Closes #3352


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 16:42:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3650" class=".btn">#3650</a>
            </td>
            <td>
                <b>
                    [ci]: Update rustup toolchain & add musl-x86_64 component
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Add rustup toolchain `nightly-2023-06-25`.
2. Add [musl-x86_64](https://aur.archlinux.org/packages/musl-x86_64) Arch package. Probably should help to fix ` error occurred: Failed to find tool. Is `musl-g++` installed?` error.

### Linked issue
[Broken iroha2-dev compilation](https://github.com/hyperledger/iroha/actions/runs/5346333962/jobs/9693207108).

### Benefits
Should help to fix `registry` job in `I2::Dev::Publish` workflow.

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
        Created At 2023-06-26 10:00:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3646" class=".btn">#3646</a>
            </td>
            <td>
                <b>
                    [fix] #3042: Fix bad request message.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Turns out this issue is kind of already fixed. I've just simply corrected the error message to exactly match the *expected* section of the issue.

### Linked issue #3042


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-24 17:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3645" class=".btn">#3645</a>
            </td>
            <td>
                <b>
                    [fix] #3516: make FindTrigger queries return original WASM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Retain original WASM blobs in `TriggerSet`
Substitute internal representation for original when querying for Triggers

### Linked issue

Closes #3516 

### Benefits

No more leaking internal representation
`FindTrigger` queries return actually useful WASM

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
        Created At 2023-06-24 11:19:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3643" class=".btn">#3643</a>
            </td>
            <td>
                <b>
                    [fix] #3195: Also panic when receiving rejected genesis.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Simple fix for attached issue but needs to be confirmed by QA.

Closes #3195

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 12:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3638" class=".btn">#3638</a>
            </td>
            <td>
                <b>
                    [ci]: Iroha2 pr-generator test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">experimental_environment</span>
            </td>
            <td>
                Just test, please skip.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 17:34:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3636" class=".btn">#3636</a>
            </td>
            <td>
                <b>
                    [fix] #3627: Transaction atomicity through cloning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Apply transaction on cloned wsv and replace original one in case of successful execution. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Partially closes #3627 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Transaction execution within block is atomic.

### Drawbacks

Cloning `wsv` will be costly in case of large wsv.

However on the current benchmarks i don't see significant differences.

We should explore time/space tradeoffs for improved solution.
Consider implementation of transaction rollbacks.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up

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
        Created At 2023-06-22 15:16:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3635" class=".btn">#3635</a>
            </td>
            <td>
                <b>
                    [feature] #3628: Implement `iroha_wasm_builder` optimization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Optimization</span>
            </td>
            <td>
                ## Description

Implemented WASM size optimization using `wasm-opt`.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3628 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

~**36.5%** wasm size reduction

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
        Created At 2023-06-21 19:16:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3634" class=".btn">#3634</a>
            </td>
            <td>
                <b>
                    [refactor] #3615: Preserve wsv after validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2023-06-21 11:02:18 +0000 UTC
    </div>
</div>

