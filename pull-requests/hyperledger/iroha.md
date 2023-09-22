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

Would be nice to be able to use the `Emitter` type from #3882, will update the PR when it will be merged

Also, a drive-by fix to silence the "unused" lints in some other feature combinations

### Linked issue

Closes #3911 

### Checklist

- [ ] use `Emitter` once #3882 is merged


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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3904" class=".btn">#3904</a>
            </td>
            <td>
                <b>
                    [ci] #3622: Use cargo manifest lints instead of unmaintained cargo-lints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                __TL;DR__: use `cargo clippy -Zlints --workspace --benches --tests --examples --all-features` instead of `cargo lints`. Also you can permanently enable the `-Zlints` for your IDE by putting the following into `.cargo/config.toml`:

```toml
[unstable]
lints = true
```

# Description

Since the implementation of rust-lang/rfcs#3389, it is now possible to specify workspace-level lints for rustc and clippy. This PR updates the cargo configuration and CI to use this new feature instead of cargo-lints.

Note that it was only stabilized in `nightly-2023-09-10`. Using it with out current toolchain requires either a -Zlints flag or a modification to `.cargo/config.toml`:

```toml
[unstable]
lints = true
```

Also note that unlike the original suggestion in #3622, this doesn't make the lints crate-level, but merely replaces a clunky unmaintained tool with a standard solution for configuring lints.

In particular, this PR:
- Removes old lints.toml configuration files for cargo-lints
- Adds [lint] tables to Cargo.toml of the root and wasm workspaces. The lints are duplicated between the two
- Replaces `cargo lints clippy` invocations with `cargo clippy -Zlints` in CI scripts
- Silences/fixes some new lints that popped up due to differences in how between `cargo lints` and workspaces
- Does a drive-by fix to iroha_genesis: it now too shares cargo metadata as do other crates

### Checklist

- [x] Make sure it passes CI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-20 12:27:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3903" class=".btn">#3903</a>
            </td>
            <td>
                <b>
                    [fix] #3899: Fix topology mismatch bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- Fixed trusted peer deserialization. `HashSet` was replaced by `Vec`
- Some minor refactoring

However I don't quite understand this change fixes the main problem. I was testing with `test_env.py` which runs the same binary multiple times, so hashing should stay the same.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3899<!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- No more `TopologyMismatch` error on network startup

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
        Created At 2023-09-20 11:15:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3902" class=".btn">#3902</a>
            </td>
            <td>
                <b>
                    [ci] #3825: Clean default runner free space
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
Some CI jobs have a lack of space problem on the default GitHub runners.

### Linked issue
#3825 

### Benefits
This possible fix might help to free up approximate 10G disk size.

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
        Created At 2023-09-20 10:42:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3897" class=".btn">#3897</a>
            </td>
            <td>
                <b>
                    [refactor] #3822, #3737, #2437: Refactor iroha_data_model_derive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Introduces various improvements to `iroha_data_model_derive`:
- updated to use syn 2.0
- add tests (where possible, see [1])
- use darling derives and traits to parse macro inputs
- add support for `Self` type in serde partially tagged enums (#3737)
- address problems in `derive(Filter)` outlined in #2437

[1] I am a bit unhappy with the testing of `derive(Filter)`, but it seems so intertwined with all the parts of `iroha_data_model` that it's really hard to test. Additionally, testing the generated `Filter` impl requires the `transparent_api` feature

### Linked issue

Closes #3882, #3737, #2437

### Checklist

- [x] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 14:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3896" class=".btn">#3896</a>
            </td>
            <td>
                <b>
                    [refactor] #3856: Proc macro for default validator boilerplate
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
Now the different flavors of validators can be generated with less repetition.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3856. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Less non-obvious boilerplate when defining custom validators.
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2023-09-18 10:35:04 +0000 UTC
    </div>
</div>

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

