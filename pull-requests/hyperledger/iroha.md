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
                PR <a href="https://github.com/hyperledger/iroha/pull/4096" class=".btn">#4096</a>
            </td>
            <td>
                <b>
                    [fix] #4090: Fix having to pass IROHA_SKIP_WASM_CHECKS env variable with true
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
Change the checking parts in build.rs files to check if the env is passed during the build. this should only build the WASM builder if the code snippet will used and in our case it will not be because the env variable is not passed. 

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4076" class=".btn">#4076</a>
            </td>
            <td>
                <b>
                    [fix] #4063: update configuration endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I've implemented the changes according to the linked issue:

- Remove documentation retrieval from the API
- Normalize DTO structure with the configuration file

### Linked issue

Closes #4063 

### Benefits

A little step closer to implementing the Configuration RFC (#2585).

### Checklist

- [x] I've written unit tests for the code changes
- [x] Self-review
- [x] Open corresponding PR updating the docs
  - https://github.com/hyperledger/iroha-2-docs/pull/435
- [x] Write an integration test
- [x] Remove redundant `Result<bool>`
- [ ] Use `PATCH` instead of `POST`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 06:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4073" class=".btn">#4073</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4065: Prevent pub key spoofing in p2p
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport for recently merged #4069

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 11:59:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4071" class=".btn">#4071</a>
            </td>
            <td>
                <b>
                    [fix] #4070: Enable `tls-rustls-native-roots` `iroha_client` feature by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Deploying behind an HTTPS proxy seems like a common occurrence, so we should have some TLS implementation by default.

Rustls brings less problems with linking under musl, so use it

### Linked issue

Closes #4070

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Make a sane choice so that the user does not have to. If they don't like the choice, they can disable the default features and make their own.

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 10:51:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4069" class=".btn">#4069</a>
            </td>
            <td>
                <b>
                    [fix] #4065: Prevent pub key spoofing in p2p
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">Security</span>
            </td>
            <td>
                ## Description

Instead of sending just pub key it's now required to send pub key + signature of shared session key to prove ownership of this public key in order to prevent spoofing.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4065 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Security bug resolved.

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
        Created At 2023-11-22 08:37:56 +0000 UTC
    </div>
</div>

