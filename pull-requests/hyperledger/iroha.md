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
                PR <a href="https://github.com/hyperledger/iroha/pull/3775" class=".btn">#3775</a>
            </td>
            <td>
                <b>
                    [feature] #3641: Human-readable permission token payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

**Scale** codec for Permission Token Payloads was replaced with **JSON**.

That's the most congruent way to fix the problem of readability. Permission tokens aren't used frequently and their main purpose is to be transparent for users. So their payload should be always readable.

Also did refactor a bit.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3641  <!-- Replace with an actual number,  -->

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
        Created At 2023-08-01 20:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3772" class=".btn">#3772</a>
            </td>
            <td>
                <b>
                    [feature] #3276: Add `Log` isi 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

`Log` is was edded to make debugging of isi only triggers easier.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3276  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Debugging should be easier.

### Drawbacks

We add new isi which will need to be maintained.

### How to test 

1. Submit `Log` isi to iroha through `cat log_isi.json | ./iroha_client_cli json`

```json
[
  {"Log": {"LogLevel":"ERROR","msg":{"String":"Cool error"}}}
]
```

2. Grep iroha message for this log message
3. Check that it have appropriate log level

### Migrate WASM to use `Log` isi instead of `log` function

After discussion with @mversic and @Arjentix it was decided not to make this migration because `Log` isi approach face multiple issues in `WASM` context: 

1. We lose `Span`s.
4. Not every WASM entrypoint is allowed to execute instructions at all.
5. Since every instruction is executed by validator we can't distinguish whatever this isi came from smart-contract or validator itself.  

Unless this problems will be solved migration is not desirable.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] Move log `Level` into data model
- [x] Implement `Log` isi 

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
        Created At 2023-08-01 03:22:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3770" class=".btn">#3770</a>
            </td>
            <td>
                <b>
                    [refactor] #3752: Replace `MockValidator` with `Initial`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

- Removed `MockValidator` and its usage with `#[cfg(test)]`
- `Validator` is now an enum with `Initial` variant set by default
- This `Initial` variant will perform no permission checking, just operation execution

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3752 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

No divergence between real and test code

### Question

Should we allow genesis without Validator then?

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
        Created At 2023-07-31 16:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3769" class=".btn">#3769</a>
            </td>
            <td>
                <b>
                    [tests]: Iroha2 dev client cli tests fixing
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
        Created At 2023-07-31 16:15:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3760" class=".btn">#3760</a>
            </td>
            <td>
                <b>
                    [fix] #3758: Individual crates build without errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Due to `#[model]` some struct fields was private for `client` crate.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3758 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Builds correctly.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] Checked that individual crates build correctly (except `kagami` will be fixed by #3748)

### How to test

1. Cd into crate folders
2. Run `cargo build --tests --examples`

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
        Created At 2023-07-28 10:11:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3759" class=".btn">#3759</a>
            </td>
            <td>
                <b>
                    [refactor]: update `iroha_schema_derive` to use syn 2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Also parse attributes with `darling` and handle errors with `manyhow`

## Description

This is continuation of work started in #3727, touching on `iroha_schema_derive`.

There was an unused API in `TypeId` derive: `#[type_id(bound = "...")]`, I removed support for it for now.

### Benefits

Same as before: less code, better error messages.

### Checklist

- [x] update the `iroha_schema_derive` crate
- [x] add more ui tests covering all the API

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 09:41:20 +0000 UTC
    </div>
</div>

