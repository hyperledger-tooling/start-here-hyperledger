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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3879" class=".btn">#3879</a>
            </td>
            <td>
                <b>
                    [documentation] #3878: Add the documentation-related Iroha configurat…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Original issue: https://github.com/hyperledger/iroha/issues/3878

We're actively using the "[Code snippets](https://hyperledger.github.io/iroha-2-docs/documenting/snippets.html)" feature, and I'm trying to have more.
While doing https://github.com/hyperledger/iroha-2-docs/pull/394, I want to reach some granularity.

I can either have `Cargo.toml` for the "[Client setup](https://hyperledger.github.io/iroha-2-docs/guide/rust.html#_1-iroha-2-client-setup)" section of the [Rust tutorial](https://hyperledger.github.io/iroha-2-docs/guide/rust.html) here or add it to the snippets directory in Iroha 2 documentation. It has less chance of remaining unnoticed for a long time if it belongs to the main repo, at least in my opinion.

Collecting a list of doc-related configurations that depend on the release in the main repo seems OK to me, but someone may disagree.

Please comment here.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 16:57:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3876" class=".btn">#3876</a>
            </td>
            <td>
                <b>
                    [refactor] #3875: Fix authentication/authorization docstring
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

Closes #3875

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

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
        Created At 2023-09-07 13:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3873" class=".btn">#3873</a>
            </td>
            <td>
                <b>
                    [feature] #1915: Implement Fast kura init mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Implement `fast` kura init mode.
Which can skip loading blocks from disk and thus bootstrap startup time. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #1915 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Improve startup time.


### Downsides

Take additional space for storing hashes on disk (32 bytes per hash) time/memory tradeoff.

`fast` init mode should be used with caution because it can detect some mutations in hashes file. 

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### How to test

1. Run iroha with `strict` kura init mode
2. Create couple of blocks
3. Check that `storage/blocks.hashes` is created
4. Shutdown iroha peer
5. Switch to `fast` kura init mode in the configuration
6. Start peer again
7. Check that peer is running correctly
8. Shutdown iroha peer ones more
9. Make backup of `storage/blocks.hashes` (`storage/blocks.hahses.old`)
10. Remove some data from data from `storage/blocks.hashes` or whole file entirely
11. Start peer
12. Check that kura failed to load in `fast` mode and failed back to STRICT mode (grep for “Hashes file is broken”)
13. Check that peer is running correctly
14. Check that `storage/blocks.hashes` is restored (`storage/blocks.hashes` == `storage/blocks.hashes.old`)
15. Check that peer is running correctly

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
        Created At 2023-09-07 07:40:53 +0000 UTC
    </div>
</div>

