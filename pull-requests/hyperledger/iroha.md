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
                PR <a href="https://github.com/hyperledger/iroha/pull/2557" class=".btn">#2557</a>
            </td>
            <td>
                <b>
                    [feature] #2536: FFI client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Marin Veršić <marin.versic101@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

* introduce `client` feature for FFI crate
* introduce additional `ffi!` macro
* rename `TryFromFfi` -> `TryFromReprC`
* make `ffi` crate `no_std`
* two disjoint feature flags `ffi_api` and `ffi`
* refactor of FFI crate - reduce duplicated code
* closes #2536 

# NOTE
To make the change manageable, this PR only introduces the `client` flag. The flag does not expand to completely valid code yet and is commented out. This is expected to be completed with #2231 . I'm trying to get this merged so that @Erigara and I don't step on each other's toes anymore

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 18:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2556" class=".btn">#2556</a>
            </td>
            <td>
                <b>
                    [fix] #2465: Reimplement sumeragi node as singlethreaded state machine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sam H. Smith <sam.henning.smith@protonmail.com>

### Description of the Change

Sumeragi now runs on it's own thread and is a relatively simple statemachine. To the eye it might seem more complicated because it is laid out flat. But that is to make explicit everything that is done. The final form of the code is not this. But it is a very malleable intermediate stage. Which is why it's going on the staging branch.

#### What you want to pay attention to is `run_sumeragi_main_loop` in `fault.rs`

### Issue

#2465
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

It's actually very possible to debug this implementation as opposed to the previous version.

### Possible Drawbacks
None
### Usage Examples or Tests *[optional]*
The best way to get an understanding for the code is to run
`cargo test integration::unstable_network::unstable_network_4_peers_1_fault -- --nocapture`.
I have left in prints to stdout that should help you follow the execution.
### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 17:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2552" class=".btn">#2552</a>
            </td>
            <td>
                <b>
                    [ci] #2461: Reverse docker login ver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Signed-off-by: BAStos525 <jungle.vas@yandex.ru>


### Description of the Change

1. Revert to `docker/login-action@v1`
2. Remove `Rename lcov report file` step in `upload_coverage` job

### Issue
`deploy` and `upload_coverage` jobs doesn't work in `I2::Dev::Deploy` workflow.

- Resolves partially #2461

### Benefits
Hopefully to resolve the current `I2::Dev::Deploy` workflow failing.

### Possible Drawbacks
`I2::Dev::Deploy` might still to be failed.

### Usage Examples or Tests *[optional]*
1. [Upload coverage](https://codecov.io/gh/BAStos525/soramitsu-iroha/commit/630c2877f6abaf8e2642686b6b8539ce814307e4/build)
2. [Uploaded iroha2 image from fork's runner](https://hub.docker.com/layers/iroha2/bastos525/iroha2/dev/images/sha256-593958d9ed760bfe864b7ee62a4a2c5a99bdb1c11e27316195a0eaacb4d384b2?context=explore)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 10:33:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2550" class=".btn">#2550</a>
            </td>
            <td>
                <b>
                    [fix] #2551: Remove the version specification of `archlinux:base-devel`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

Remove the version specification from the base image of `iroha2:base`

### Issue

- Closes #2551

### Benefits

`iroha2:base` can be built

### Possible Drawbacks

Different images can be built at the same commit
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 16:25:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2546" class=".btn">#2546</a>
            </td>
            <td>
                <b>
                    Iroha 1 | Fix print error in docker push stage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
1. Fix print error in docker push stage
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
jq fail on push stage
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 10:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2538" class=".btn">#2538</a>
            </td>
            <td>
                <b>
                    [feature] #2490: Implement ffi_export for freestanding functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

Make `ffi::derive::export::gen_ffi_fn` working with freestanding functions, so `ffi_export` macro could be used for such functions.

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->
Closes #2490 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 21:46:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2535" class=".btn">#2535</a>
            </td>
            <td>
                <b>
                    [refactor] #2419: Remove explicit `drop`s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                Signed-off-by: Shanin Roman <shanin1000@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Remove explicit `drop` call through the codebase. 
There were 2 use cases for `drop`:
- Ignore `Result` and pass `clippy` linting: replaced with `let _result = some_func_call(...)`. IMO ideally we should handle errors not ignoring them;
- Actually free some resource: replaced with proper scope.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2419.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

No code smell constructions.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 12:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2523" class=".btn">#2523</a>
            </td>
            <td>
                <b>
                    [refactor] #2468: Remove debug supertrait from permission validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Security</span>
            </td>
            <td>
                
<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

* Removed as much output-like supertraits from validators as possible
* `Debug` was replaced with `Display`
* `Display` implemented for permissions validators
* `Display` was also implemented for instructions, queries and expressions

This gives us much more readable error output when something is wrong with permissions. See examples below.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2468
* Impls #2334. Why it was already closed I have no idea

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* Better permission error messages
* More things can be `Display`ed now
* No more `Debug` supertrait for validators

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Can't see any

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Examples

#### Example 1

<details>

**iroha2-dev**:

```
Action not permitted: Validator CheckNested { validator: JudgeAsValidator { judge: NoDenies { validators: [IsGrantAllowedAsValidator { is_grant_allowed: GrantMyAssetAccess }, IsGrantAllowedAsValidator { is_grant_allowed: GrantRegisteredByMeAccess }, IsGrantAllowedAsValidator { is_grant_allowed: GrantRegisteredByMeAccess }, IsGrantAllowedAsValidator { is_grant_allowed: GrantMyAssetAccess }, IsGrantAllowedAsValidator { is_grant_allowed: GrantRegisteredByMeAccess }, IsGrantAllowedAsValidator { is_grant_allowed: GrantMyAssetAccessRemove }, IsGrantAllowedAsValidator { is_grant_allowed: GrantMyAssetAccessSet }, IsGrantAllowedAsValidator { is_grant_allowed: GrantMyMetadataAccessSet }, IsGrantAllowedAsValidator { is_grant_allowed: GrantMyMetadataAccessRemove }, IsGrantAllowedAsValidator { is_grant_allowed: GrantMyAssetDefinitionSet }, IsGrantAllowedAsValidator { is_grant_allowed: GrantMyAssetDefinitionRemove }] } } } denied operation Grant(GrantBox { object: EvaluatesTo { expression: Raw(PermissionToken(PermissionToken { name: "can_set_key_value_in_asset_definition", params: {"asset_definition_id": Id(AssetDefinitionId(DefinitionId { name: "rose", domain_id: Id { name: "wonderland" } }))} })), _value_type: PhantomData }, destination_id: EvaluatesTo { expression: Raw(Id(AccountId(Id { name: "alice", domain_id: Id { name: "wonderland" } }))), _value_type: PhantomData } }): Validator IsGrantAllowedAsValidator { is_grant_allowed: GrantMyAssetDefinitionSet } denied operation Grant(GrantBox { object: EvaluatesTo { expression: Raw(PermissionToken(PermissionToken { name: "can_set_key_value_in_asset_definition", params: {"asset_definition_id": Id(AssetDefinitionId(DefinitionId { name: "rose", domain_id: Id { name: "wonderland" } }))} })), _value_type: PhantomData }, destination_id: EvaluatesTo { expression: Raw(Id(AccountId(Id { name: "alice", domain_id: Id { name: "wonderland" } }))), _value_type: PhantomData } }): Cannot grant access for assets registered by another account.
```

**this branch**:

```
Action not permitted: Validator ``Grant validator` with nested checking` denied the operation `GRANT `can_set_key_value_in_asset_definition` TO `alice@wonderland`` by `mouse@wonderland`: Validator `Allow to grant `can_set_key_value_in_asset_definition` permission token if `the signer is the asset creator`` denied the operation: Cannot grant access for assets registered by another account.
```

</details>

#### Example 2

<details>

**iroha2-dev**:

```
Action not permitted: Validator CheckNested { validator: Or { first: AccountSetOnlyForSignerAccount, second: HasTokenAsValidator { has_token: SetGrantedByAccountOwner }, _phantom_operation: PhantomData } } denied operation SetKeyValue(SetKeyValueBox { object_id: EvaluatesTo { expression: Raw(Id(AccountId(Id { name: "mouse", domain_id: Id { name: "wonderland" } }))), _value_type: PhantomData }, key: EvaluatesTo { expression: Raw(Name("key")), _value_type: PhantomData }, value: EvaluatesTo { expression: Raw(String("value")), _value_type: PhantomData } }): Nor first validator AccountSetOnlyForSignerAccount succeed: Cannot set values to the account store of another account., nor second validator HasTokenAsValidator { has_token: SetGrantedByAccountOwner } succeed: Account does not have the needed permission token: PermissionToken { name: "can_set_key_value_in_user_metadata", params: {"account_id": Id(AccountId(Id { name: "mouse", domain_id: Id { name: "wonderland" } }))} }.
```

**this branch**:

```
Action not permitted: Validator ```Allow to set account metadata keys only for signer` or `Allow if signer has the corresponding `can_set_key_value_in_user_metadata` permission token`` with nested checking` denied the operation `SET `key` = `value` IN `mouse@wonderland`` by `alice@wonderland`: Nor first validator `Allow to set account metadata keys only for signer` succeed: Cannot set values to the account store of another account, nor second validator `Allow if signer has the corresponding `can_set_key_value_in_user_metadata` permission token` succeed: Account does not have the needed permission token: PermissionToken { name: "can_set_key_value_in_user_metadata", params: {"account_id": Id(AccountId(Id { name: "mouse", domain_id: Id { name: "wonderland" } }))} }
```

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 17:09:13 +0000 UTC
    </div>
</div>

