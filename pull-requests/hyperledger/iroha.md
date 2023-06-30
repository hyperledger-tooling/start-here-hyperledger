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
                PR <a href="https://github.com/hyperledger/iroha/pull/3663" class=".btn">#3663</a>
            </td>
            <td>
                <b>
                    [feature] #3309: Bumps `wasmtime` version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

1. Replaces error lifting from `Trap` with `wasmtime::Error` that is `anyhow::Error` actually.
2. Replaces all codec errors with structured errors.
3. Replaces `eyre` with `wasmtime::Error` in structured errors related to executing smart-contracts.

### Linked issue

Closes #3309 

### Benefits

Upgrades `wasmtime` to the latest version.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
- [ ] Fix FFI troubles

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
        Created At 2023-06-30 16:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3662" class=".btn">#3662</a>
            </td>
            <td>
                <b>
                    [refactor]: reject incorrect config topology early
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
        Created At 2023-06-30 13:04:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3661" class=".btn">#3661</a>
            </td>
            <td>
                <b>
                    [feature] #3236: Cache `iroha_wasm_builder` output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Optimization</span>
            </td>
            <td>
                ## Description

Now you can configure `iroha_wasm_builder` output dir in a three ways (in order of priority):

1. Explicitly use `out_dir()` method
2. Set `IROHA_WASM_BUILDER_OUT_DIR` env var
3. Do nothing if you are in a build-script. Directory will be inherited from `OUT_DIR` env var which is set by `cargo`

By default `target` directory of running crate will be used.

Other than that optimization *caching* is also implemented.
This is done by comparing `sha256` hashes of non-omptimized wasm-files. If hash before and after build are equal, then non-omptimized file wasn't changed, which means that optimized wasm file should also stay unchanged and we don't have to spent time on running `wasm-opt`.

Also `build()` will fail now if it's being called on workspace. I think, it was an error that we didn't have that before. It's an error because we run `build()` only to get `Output` from it, where `Output` is a binary encoded WASM file, which we can't choose if we build workspace.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3236 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Cached wasm binaries allows us not to rebuild them everytime from scratch. I.e. cached validator builds now take much less time. Same for tests which sumbit wasm.

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
        Created At 2023-06-29 14:13:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3659" class=".btn">#3659</a>
            </td>
            <td>
                <b>
                    [fix] #3543: Increment quantity change, not total
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

Closes #3543


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 12:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3655" class=".btn">#3655</a>
            </td>
            <td>
                <b>
                    [ci]: Update rust toolchain in the Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
Update rustup toolchain iroha2 `Dockerfile`.

### Linked issue
[Failed CI after updating Dockerfile.build](https://github.com/hyperledger/iroha/actions/runs/5388372729).

### Benefits
Should help to fix `registry` jon in `I2::Dev::Publish` workflow.

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
        Created At 2023-06-27 12:43:36 +0000 UTC
    </div>
</div>

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

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up
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

