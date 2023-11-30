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
                PR <a href="https://github.com/hyperledger/iroha/pull/4108" class=".btn">#4108</a>
            </td>
            <td>
                <b>
                    [BACKPORT]: replace test_env.sh with test_env.py in CI
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
        Created At 2023-11-30 08:29:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4107" class=".btn">#4107</a>
            </td>
            <td>
                <b>
                    [fix] #4106: Fix trigger atomicity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Fix trigger atomicity by cloning wsv.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4106<!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 07:48:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4103" class=".btn">#4103</a>
            </td>
            <td>
                <b>
                    [chore]: #4102 Update issue templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR changes the issue templates for Iroha.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 06:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4100" class=".btn">#4100</a>
            </td>
            <td>
                <b>
                    [fix] #4030, #4063, #4064, #4079: re-architect logger and dynamic configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">config-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

_todo_

### Linked issue

Closes #4030 #4063 #4064 #4079

### Benefits

_todo_

### Checklist

_todo_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 04:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4098" class=".btn">#4098</a>
            </td>
            <td>
                <b>
                    [fix] #4097: Fix warp noise in logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- `warp::trace::request()` was attached twice for some endpoints, which lead to noise in logs
- logging error inside queue push was redundant because error should be handled on caller site

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4097 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Less noise in logs.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2023-11-29 07:22:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4096" class=".btn">#4096</a>
            </td>
            <td>
                <b>
                    [fix] #4090 #3858: Fix having to pass IROHA_SKIP_WASM_CHECKS env variable with true
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
Change the checking parts in build.rs files to check if the env is passed during the build. this should only build the WASM builder if the code snippet will be used and in our case it will not be because the env variable is not passed. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 16:36:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4095" class=".btn">#4095</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #0000: Fix trigger atomicity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

If trigger failed during execution all of it's changes will be reverted.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Intended behavior for trigger execution. 

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2023-11-28 14:43:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4089" class=".btn">#4089</a>
            </td>
            <td>
                <b>
                    [feature] #3941: Remove expressions
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

The main idea was to move all expressions into executor. After a discussion with @mversic we decided not to implement any of them inside `default_executor`, but to have an example executor to show PoC.

- All expressions were removed
- `#[model]` together with `ffi` have become useless for data_model because in future clients should link against executor_data_model. So I partly removed them. This might need future investigation

I wii squash all my commits before merge.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3941 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Much less code
- No stillborn expression system inside data_model and core
- Types for ISI now can't contain unsupported parameters

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Follow up tasks

- Reconsider ffi for data_model
- Make block content opaque
- Write example executor with expressions or even DSL

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
        Created At 2023-11-27 23:11:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4088" class=".btn">#4088</a>
            </td>
            <td>
                <b>
                    [fix] #4084: NumericValue suffix is mandatory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Previously suffix for `Fixed` was optional which led to confusion in cases like `{"value": "100"}` which was parsed as `Fixed` nor `String` or integer type. 

After introduced changes `_fx` is required. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4084 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Less confusion when desalinizing.  

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2023-11-27 13:52:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4081" class=".btn">#4081</a>
            </td>
            <td>
                <b>
                    [refactor] #4080: Export data model through iroha_client
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

Closes #4080

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
        Created At 2023-11-24 12:48:48 +0000 UTC
    </div>
</div>

