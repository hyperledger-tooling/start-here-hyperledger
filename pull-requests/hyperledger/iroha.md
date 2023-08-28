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
                PR <a href="https://github.com/hyperledger/iroha/pull/3841" class=".btn">#3841</a>
            </td>
            <td>
                <b>
                    [refactor] #3833, #2373: Split off Kagami
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Outline:

- **Refactor Kagami**
  - Remove `kagami validator`
  - Remove `kagami swarm`
  - Refactor `kagami genesis` according to the [comment](https://github.com/hyperledger/iroha/issues/3833#issuecomment-1693023658)
- **Introduce `iroha_swarm`**: according to the [comment](https://github.com/hyperledger/iroha/issues/2373#issuecomment-1690971061)
- **Introduce `iroha_wasm_builder_cli`**: a CLI around `iroha_wasm_builder`. It replaces `kagami validator` in the following way:
  ```bash
  # before
  kagami validator > validator.wasm
  
  # after
  iroha_wasm_builder_cli check ./default_validator
  iroha_wasm_builder_cli build ./default_validator --optimize --format > validator.wasm
  ```
- **Update CI scripts** which used the previous commands

### Linked issue

Closes #3833, #2373

### Benefits

- Kagami is now a portable and lightweight tool. There is no issue with mentioning it in the documentation.
- Swarm is now simpler, without redundant functionality. Easy to enhance in the future.
- A general tool for building smartcontracts. Easy to enhance in the future. More reliable than `kagami validator` thanks to spinners.


### Checklist

- [ ] Investigate the logic behind the `format` option in `iroha_wasm_builder::Builder`, maybe open an issue to refactor it.
- [x] Self-review
- [ ] Add README to `iroha_swarm`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 05:20:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3840" class=".btn">#3840</a>
            </td>
            <td>
                <b>
                    Add new protobuf parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
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
        Created At 2023-08-27 21:57:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3837" class=".btn">#3837</a>
            </td>
            <td>
                <b>
                    [refactor] #3574: make all numeric values serialize as string literals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This changes how numbers in expressions are serialized in json. 

`{"U32":  42}` -> `"42_u32"`
`{"U64":  42}` -> `"42_u64"`
`{"U128":  "42"}` -> `"42_u128"`
`42.0` -> `"42.0_fx"`

As a side-effect, this prohibits the usage of json number literals and, as such, no longer requires using serde_json's `arbitrary_precision` feature to deserialize 128-bit numbers.

This also removes some of the `#[serde(flatten)]`s from ISIs, as integers are no longer serialized as maps and can't be flattened.

This breaks the user-facing interface (AFAIK, only in `genesis.json`. Or is `client-cli` affected too?)

### Linked issue

Closes #3574 

### Benefits

- similar handing of all bit sizes, all numbers are quoted


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 09:30:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3835" class=".btn">#3835</a>
            </td>
            <td>
                <b>
                    [RFC]: on-chain scripting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 16:29:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3832" class=".btn">#3832</a>
            </td>
            <td>
                <b>
                    [feature] #3812 adding registerbox to DSL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Getting started on a syntax for `RegisterBox` to replace writing `RegisterBox::new(Domain::new("neverland".parse()?))` with `expr!(register "neverland")`, currently there's no way to describe objects which aren't domains. It also makes sense to separate the name detection logic from the DSL.

### Benefits

There's a consistent grammar across different kinds of resources like domains, assets, accounts which can be inferred when creating objects within the DSL. For instance, all assets will be `asset#domain`.

https://hyperledger.github.io/iroha-2-docs/guide/blockchain/naming.html

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] syntax for `register`
- [x] Domains
- [ ] Assets
- [ ] AssetDefinitions
- [ ] Accounts
- [ ] Moving detection code into separate crate
- [ ] CI checks

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 06:42:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3831" class=".btn">#3831</a>
            </td>
            <td>
                <b>
                    [fix] #3059: Simplify kura lock file code
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

Closes #3059  <!-- Replace with an actual number,  -->

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
        Created At 2023-08-21 18:29:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3830" class=".btn">#3830</a>
            </td>
            <td>
                <b>
                    [refactor] #3814: Update `iroha_ffi_derive` to use syn 2.0 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Separate parsing & (some) validation of attributes and codegen using `darling`, by storing this information into a strongly typed struct (`FfiTypeInput` and alike).

To facilitate this, add  parsers for `derive(FfiType)`, `getset` crate and built-in `repr` and `derive` attributes and tests for them.

One unfortunate concern is that now `ffi_derive` has stopped supporting unions completely, due to a limitation of `darling`. I don't think they are _that_ useful though, especially in context of a high level API iroha provides

### Linked issue

Closes #3814 

### Benefits

Cleaner code, better macro errors

### Checklist

- [x] Rebase (need less commits and proper messages)
- ~~[ ] Move utility classes to a common place (`iroha-derive-primitives`, probably)~~ not a good idea until `iroha-derive-primitives` is syn2-only
- [x] Make codegen for `ffi!`, `#[ffi_import]` and `#[ffi_export]` `emit!` errors rather than `bail!`ing
- [x] Clean up stray commented out code
- [x] Fix lints
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 15:07:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3827" class=".btn">#3827</a>
            </td>
            <td>
                <b>
                    [refactor] #3674: Elide `.cloned()` in `data_model/src/block.rs`
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
Get rid of unnecessary `iter::cloned()` call.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3674. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2023-08-21 08:00:41 +0000 UTC
    </div>
</div>

