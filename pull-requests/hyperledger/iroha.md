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
                PR <a href="https://github.com/hyperledger/iroha/pull/3930" class=".btn">#3930</a>
            </td>
            <td>
                <b>
                    [refactor]: Rename ISI from *Box to *Expr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

1. This was a complete misnomer because `Box` suffix if for enums used to group objects for serialization purpose
2. This is an interlude into another PR where I will introduce proper `Box`ed instructions which will not contain expressions inside them, i.e. they will be evaluated instructions
3. I'm only doing this rename in separate PR first so that changes are not overwhelming to review

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
        Created At 2023-09-27 15:23:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3925" class=".btn">#3925</a>
            </td>
            <td>
                <b>
                    [refactor]: Replace Registered with Identifiable in ISI bounds
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
        Created At 2023-09-26 06:58:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3923" class=".btn">#3923</a>
            </td>
            <td>
                <b>
                    [feature]: parse filter as JSON5 in `iroha_client_cli`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

There is inconsistency of what `iroha_client_cli` accepts:

- JSON5 input for `iroha_client_cli json` command
- JSON input for filters, e.g.
  ```bash
  iroha_client_cli domains list filter '{"Identifiable": {"Is": "wonderland"}}'
  ```

This chore PR adds support for JSON5 for filters:

```bash
iroha_client_cli domains list filter '{Identifiable: {Is: "wonderland"}}'
```


### Context

It makes examples of `iroha_client_cli` usage _a little_ more clear and consistent.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 06:10:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3920" class=".btn">#3920</a>
            </td>
            <td>
                <b>
                     [refactor] #3874: Removes `IsAssetDefinitionOwnerQuery`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Removed all instances of `IsAssetDefinitionOwner` except for some:

**In `wasm/validator/src/permission.rs` and `/default.rs**

With the function

```rust
fn is_asset_definition_owner(
        asset_definition_id: &AssetDefinitionId,
        authority: &AccountId,
    ) -> Result<bool> {
        IsAssetDefinitionOwner::new(asset_definition_id.clone(), authority.clone()).execute()
    }
```

I am unsure what to replace this result with. I have tried replacing it with `FindAssetDefinitionById` (since this is said to do the exact same thing as is asset definition owner in #3874) but this creates build errors. Should I delete everything that uses the `is_asset_definition_owner` function as well?



### Linked issue

Remove `IsAssetDefinitionOwnerQuery`

This query was introduced only for the purposes of validator. Since #3442 we can use `FindAssetDefinitionById` to do the exact same thing.

Closes #3442<!-- Replace with an actual number,  -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 10:33:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3917" class=".btn">#3917</a>
            </td>
            <td>
                <b>
                    [refactor]: Move roles in `WSV`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Move accounts' roles into `wsv`.

This PR takes alternate design from #3681 since it might be preferable to operate on roles as first class citizens (e.g. have specific queries, isi, ...). 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3681 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Move effective range quires over all assets, roles.

Cloning account is less expensive.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 06:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3916" class=".btn">#3916</a>
            </td>
            <td>
                <b>
                    [refactor] #3895: move `commit_topology` into block payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3895

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
        Created At 2023-09-25 06:49:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3915" class=".btn">#3915</a>
            </td>
            <td>
                <b>
                    [refactor] #3911: Migrate `iroha_futures_derive` to syn 2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Update `iroha_futures_derive` to use syn 2.0

Would be nice to be able to use the `Emitter` type from #3897, will update the PR when it will be merged

Also, a drive-by fix to silence the "unused" lints in some other feature combinations

### Linked issue

Closes #3911 

### Checklist

- [x] make CI pass
- [x] use `Emitter` once #3882 is merged


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 12:03:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3914" class=".btn">#3914</a>
            </td>
            <td>
                <b>
                    [fix] #1232: Introduce startup time benchmark
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

You can now run `scripts/test_env.py setup -b`

If you want times for release mode you must copy the release binary to `target/debug/iroha`

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
        Created At 2023-09-22 12:01:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3913" class=".btn">#3913</a>
            </td>
            <td>
                <b>
                    [refactor] #3886: Remove 'Versioned' prefix from versioned containers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I think this makes a better API.
Would you agree?

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3886

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
        Created At 2023-09-22 12:00:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3912" class=".btn">#3912</a>
            </td>
            <td>
                <b>
                    [fix] #3905: Fix apply_blocks and validate_blocks benchmark
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Benchmarks now measure what they suppose to measure.
Fix memory issue inside wasm validator.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3905, #3906 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Fixed benchmarks.

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
        Created At 2023-09-22 11:48:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3908" class=".btn">#3908</a>
            </td>
            <td>
                <b>
                    [fix]: `mkdir -r` with store path, not lock path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

TBH, I am lazy to prepare a proper reproduction of the bug. In my case, Iroha repeatedly failed to start, complaining about existence of the lock file all the time. After all, it turned out that `./storage/kura.lock`, created by Iroha, **is a directory, not a file**.

This PR makes variables naming clearer, and passes actual block-store path into `mkdir -r`, not the path of the lockfile. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 08:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3907" class=".btn">#3907</a>
            </td>
            <td>
                <b>
                    [documentation]: Remove the develop-iroha-module guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Closes https://github.com/hyperledger/iroha-2-docs/issues/203
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 08:01:49 +0000 UTC
    </div>
</div>

