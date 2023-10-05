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
                PR <a href="https://github.com/hyperledger/iroha/pull/3958" class=".btn">#3958</a>
            </td>
            <td>
                <b>
                    Lazy query for wasm
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
        Created At 2023-10-04 23:12:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3957" class=".btn">#3957</a>
            </td>
            <td>
                <b>
                    [fix] #3995: Fix wasm cache directory permission bug in docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Wasm cache directory is being created in the Dockerfile and all required permissions are being granted to the user.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3955 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Working Iroha stable image

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
        Created At 2023-10-04 21:21:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3956" class=".btn">#3956</a>
            </td>
            <td>
                <b>
                    [refactor] #3950: Merge API and Telemetry endpoints into a single server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR merges the Telemetry endpoint into the main API endpoint

### Linked issue

Closes #3950

### Benefits

Less complexity, no more threading multiple port numbers to configuration

### Checklist

- [ ] check that the endpoints actually work (I don't think they are covered by any tests?)
- [ ] make ci pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 15:58:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3949" class=".btn">#3949</a>
            </td>
            <td>
                <b>
                    [refactor]: move expression len out of public API into core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

let's not pollute public API with internal stuff

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
        Created At 2023-10-03 08:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3946" class=".btn">#3946</a>
            </td>
            <td>
                <b>
                    [documentation] #3945: Update MAINTAINERS.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Before merging, please comment on Aleksandr's role, because he's more of an advisor at this point.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 05:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3944" class=".btn">#3944</a>
            </td>
            <td>
                <b>
                    [refactor]: Include smart contract code into the workspace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

* renamed `wasm` crate to `smart_contract` (`wasm` is just one of potentially many VMs)
* included `smart_contract` crate in the workspace

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

we no longer have a split in the workspace.

### Downsides

writer of the smart contract now must explicitly include allocator

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
        Created At 2023-10-02 14:45:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3940" class=".btn">#3940</a>
            </td>
            <td>
                <b>
                    [refactor] #3640: place permission tokens in a separate module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

* moved all tokens to a separate module 
I'll still explore the way of how to make them in a separate crate
* optimized permission execution

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3640 

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
        Created At 2023-10-02 06:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3938" class=".btn">#3938</a>
            </td>
            <td>
                <b>
                    [fix] #3939: Fix the usage of `Span::join`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Actually, `Span::join` doesn't work on stable at all (and returns `None`), so care should be taken to have a fallback

This means that on stable we will have error spans that are slightly incorrect

Closes #3939


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 06:01:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3935" class=".btn">#3935</a>
            </td>
            <td>
                <b>
                    [refactor] #3934: Migrate `iroha_wasm_derive` and `iroha_validator_derive` to syn 2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Use syn 2.0, manyhow and darling to enhance the error messages

### Linked issue

Closes #3934 

### Checklist

- [ ] make sure the CI passes
- [ ] add tests?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 14:36:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3933" class=".btn">#3933</a>
            </td>
            <td>
                <b>
                    [fix] #3928: Make failing the wasm tests actually fail the CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Add a new `iroha_wasm_test_runner` tool. It mostly duplicates the `webassembly-test-runner`, but actually returns a non-zero exit code if there are any test failures. As an added bonus 

This tool is expected to be installed on the developer's system with `cargo install`. It's not going to change often, so I don't think there's a risk of it going out-of-sync with the state of the repo.

Also fix the `evaluate_expression` test, which was never passing before due to a typo.

### Linked issue

Closes #3928 

### Benefits

- Actually makes the CI check that the wasm test

### Alternatives

An alternative would be to continue to use the upstream test runner when/if https://github.com/matklad/webassembly-test/pull/1 gets merged, but I wouldn't bet on it.

### Checklist

- [x] make sure CI passes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 07:46:53 +0000 UTC
    </div>
</div>

