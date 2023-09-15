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
                PR <a href="https://github.com/hyperledger/iroha/pull/3894" class=".btn">#3894</a>
            </td>
            <td>
                <b>
                    [ci] #3849: Fix stable/lts configs pushing job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
In `I2::Release::Publish`, add third-party Action step to commit and push the changes by `sorabot` user PAT to the protected branch

### Linked issue
#3849 

### Benefits

This Action should help to solve the problem of pushing changes to the `iroha2-dev` protected branch. However, it's an experiment and might not work due we are not able to use `sorabot` bot-user on forks.

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
        Created At 2023-09-15 16:49:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3893" class=".btn">#3893</a>
            </td>
            <td>
                <b>
                    [feature] #3891: Implement `Retrieve` isi internally
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- Added `Retrieve` isi
- Added `Output` associated type for `Instruction` trait, because now instructions can return something other than just `()`
- Refactored validators to support these new output types
- Fixed error types in `iroha_wasm_codec`
- `ValidationFail::InternalError` is now more descriptive, because it's filled with debug formated error now

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3891 <!-- Replace with an actual number,  -->

### Follow-up task

- #3892

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

- Users can send `Retrieve` instruction
- Validator infrastructure is now more flexible with different verdict types

### Downsides

- Validator infrastructure becomed a bit more complicated

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
        Created At 2023-09-15 13:20:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3884" class=".btn">#3884</a>
            </td>
            <td>
                <b>
                    [feature] #3355: Standardize block API
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

* replaced `VersionedCommittedBlock` with `VersionedSignedBlock`
* improved block lifecycle and state transitions
* introduced `BlockBuilder`
* introduced `ProofBuilder`

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3355 #3424 #3295 #2767

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
        Created At 2023-09-13 07:36:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3881" class=".btn">#3881</a>
            </td>
            <td>
                <b>
                    [refactor] #3880 : Make `prepare_query_request` public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description
Making the ```prepare_query_request``` public to make ```RC19``` comapatible with blockchain explorer.

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue
Closes #3880 
<!-- Duplicate the main issue and add additional issues closed by this PR. -->

### Benefits

Currently, the blockchain explorer backend requires various methods that were in Iroha version 2.0.0-pre-rc.16 but are not present / structured changed in Iroha version 2.0.0-pre-rc.19.
This patch will be addressing commits related to it.
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
        Created At 2023-09-11 07:10:13 +0000 UTC
    </div>
</div>

