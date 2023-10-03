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

