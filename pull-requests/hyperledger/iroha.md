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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2517" class=".btn">#2517</a>
            </td>
            <td>
                <b>
                    [refactor] #2052: make permission token ids registrable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Artemii Gerasimovich <gerasimovich@soramitsu.co.jp>

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

### Issue

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
        Created At 2022-07-21 21:51:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2516" class=".btn">#2516</a>
            </td>
            <td>
                <b>
                    [feature] #1891: Validate trigger execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ales Tsurko <ales.tsurko@gmail.com>

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

Validation for trigger execution is added. Now triggers are allowed to be executed only by the register and technical accounts.

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Closes #1891 

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
        Created At 2022-07-21 21:36:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2515" class=".btn">#2515</a>
            </td>
            <td>
                <b>
                    [fix] #2501: Fixes the order of assets in queries with pagination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Vladimir Pesterev <pesterev@pm.me>

### Description of the Change

Replaces the lexicographical order of assets with a timestamp-based order in `AssetsMap`.

For example:

Before: `1 (1658432537)`, `10 (1658432546)`, `2 (1658432538)`, `3 (1658432539)`, `4 (1658432540)`, `5 (1658432541)`, `6 (1658432542)`, `7 (1658432543)`, `8 (1658432544)`, `9 (1658432545)`.

Now: `1 (1658432537)`, `2 (1658432538)`, `3 (1658432539)`, `4 (1658432540)`, `5 (1658432541)`, `6 (1658432542)`, `7 (1658432543)`, `8 (1658432544)`, `9 (1658432545)`, `10 (1658432546)`.

Where `N` is Id and `T` is an insertion timestamp in `N (T)` format.

### Issue

Resolves #2501 

### Benefits

Order now depends on insertion timestamp.

### Possible Drawbacks

The queries that retrieve an asset will execute a bit slower because `O(log n)` (current implementation) and `O (log n + log n)` (twice b-tree lookup) (impl in this PR).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 19:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2505" class=".btn">#2505</a>
            </td>
            <td>
                <b>
                    [feature] #2073: Prefer ConstString over String
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Optimization</span>
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

Replaces `String` with `ConstString` for types stored in the blockchain. It also encapsulates `iroha_data_primitives` into a shared crate.

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Closes #2073 

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
        Created At 2022-07-18 19:19:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2503" class=".btn">#2503</a>
            </td>
            <td>
                <b>
                    [refactor] #2253: Add `Registrable` trait to `data_model`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Introduce `Registrable` trait to create unified interface for building objects.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2253.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Unified interface.

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
        Created At 2022-07-18 13:33:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2500" class=".btn">#2500</a>
            </td>
            <td>
                <b>
                    [documentation] #2499: Fix client_cli error messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                <!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

A tiny correction for the error messages, which seem to be copied previously; the error message ''Failed to get all **accounts**" was used for:

```rust
.request(client::domain::all())
```

and 

```rust
.request(client::asset::all())
```

### Issue

I can open one if needed, but this is nothing more than a typo.

### Benefits

Error messages being displayed will be corrected.

### Possible Drawbacks

None

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
        Created At 2022-07-18 10:06:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2497" class=".btn">#2497</a>
            </td>
            <td>
                <b>
                    [refactor]: impl `HasOrigin` instead of `Identifiable` for the data events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

The minimum change to [remove `Identifiable` implementation from events](https://github.com/hyperledger/iroha/pull/2476#issuecomment-1184107169)

### Issue

- Relates to #2476

### Benefits

- Less complexity to derive `Identifiable`
- Rationality that an event should not be identified by its origin

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 05:55:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2495" class=".btn">#2495</a>
            </td>
            <td>
                <b>
                    [fix] #2492: Fixes not all triggers being executed that match an event (lts)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Vladimir Pesterev <pesterev@pm.me>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

It adds a test that reproduces [this bug](https://github.com/hyperledger/iroha/issues/2492) and also changes that fix it. Also [see](https://github.com/hyperledger/iroha/pull/2493) these changes to `iroha2-dev` branch.

### Issue

Fixes #2493 

### Benefits

Adds changes from #2493 directly into the LTS branch.

### Possible Drawbacks

None

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-16 22:20:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2494" class=".btn">#2494</a>
            </td>
            <td>
                <b>
                    Update documentation: AddPeer with syncing_node option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span><span class="chip">Documentation</span>
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
In Iroha 1.4 SyncingNode option was added. So I've updated documentation:
![obraz](https://user-images.githubusercontent.com/15332594/179312734-8031a766-90b3-433d-aff4-4e7865dd7d58.png)
The update is using `commands.rst` instead of copy-paste.

I've also changed indentations in `queries.rst` - once it was 2 spaces, other time 4 spaces - I've unified into 4 spaces everywhere.


<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Updated documentation

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Time for review:D.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*
`make html` according the instruction and comparing with eyes:D.

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
        Created At 2022-07-15 21:27:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2493" class=".btn">#2493</a>
            </td>
            <td>
                <b>
                    [fix] #2492: Fixes not all triggers being executed that match an event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Vladimir Pesterev <pesterev@pm.me>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

I've added a test that reproduces [this bug](https://github.com/hyperledger/iroha/issues/2492) and also changes that fix it. Also [see](https://github.com/hyperledger/iroha/pull/2495) these changes to `iroha2-lts` branch.

### Issue
Fixes #2492 

### Benefits
Fixes triggers execution

### Possible Drawbacks
None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 19:27:40 +0000 UTC
    </div>
</div>

