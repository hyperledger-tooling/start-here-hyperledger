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
                PR <a href="https://github.com/hyperledger/iroha/pull/2929" class=".btn">#2929</a>
            </td>
            <td>
                <b>
                    [feature] #2905: Extend arithmetic operations to support `AssetValue` 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Extend arithmetic operations to support `AssetValue`  instead of only `u32`.

### Issue

Closes #2905.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Arithmetic instructions support more types.

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
        Created At 2022-11-01 14:28:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2928" class=".btn">#2928</a>
            </td>
            <td>
                <b>
                    [feature] #2899, #2508: Add multi-instructions and wasm subcommands into 'client_cli'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Merge changes from #2898 and #2918 into LTS.

### Issue

Close #2899 and #2508

### Benefits

Add a couple of subcommands into the LTS branch.

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-01 14:02:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2924" class=".btn">#2924</a>
            </td>
            <td>
                <b>
                    [fix] #2923: Return `FindError` when `AssetDefinition` does not exist
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

Skip validation if `AssetDefinitionId` doesn't exist.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2923.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Proper error message.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

No.

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
        Created At 2022-10-28 14:01:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2918" class=".btn">#2918</a>
            </td>
            <td>
                <b>
                    [feature] #2899: Add multi-instructions subcommand into `client_cli`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

More details about the suggestion you can find [here.](https://github.com/hyperledger/iroha/issues/2899)

I spent some time trying to reuse `GenesisTransaction`s format (`configs/peer/genesis.json`) but it's a bad way cause demand depends on `iroha_core` and a lot of boilerplate code being converted. But I noticed that we can just use `Serialize/Deserialize` which already implemented for `Instruction`s and use those traits to represent instructions as JSON. As a result, I got a way to make a more convenient and simple implementation of this command.

### Issue

Closes #2899 

### Benefits

Submit multiple instructions using one command

### Possible Drawbacks

None

### Usage Examples or Tests

Save these instructions into a file:
```json
[
    {
        "Register": {
            "Identifiable": {
                "NewDomain": {
                    "id": "neverland",
                    "logo": null,
                    "metadata": {}
                }
            }
        }
    },
    {
        "Register": {
            "Identifiable": {
                "NewAccount": {
                    "id": "steve@neverland",
                    "signatories": [
                        "ed0120cc25624d62896d3a0bfd8940f928dc2abf27cc57cefeb442aa96d9081aae58a1"
                    ],
                    "metadata": {}
                }
            }
        }
    },
    {
        "Register": {
            "Identifiable": {
                "NewAssetDefinition": {
                    "id": "sapporo#neverland",
                    "value_type": "Quantity",
                    "mintable": "Infinitely",
                    "metadata": {}
                }
            }
        }
    },
    {
        "Mint": {
            "object": {
                "U32": 1010
            },
            "destination_id": {
                "Id": {
                    "AssetId": "sapporo##steve@neverland"
                }
            }
        }
    }
]
```

And then pass to `client_cli` like this:
```
cat ./test.json | ./iroha_client_cli json
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-27 08:05:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2917" class=".btn">#2917</a>
            </td>
            <td>
                <b>
                    [feature] #2163: Add trait to handle log-and-ignore pattern
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">UI</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

The log-and-ignore pattern is all too common in our code base. I've added a trait that makes it much easier to enforce "best practices" for such errors. Specifically, errors now need to be explicitly ignored using an `expect`-like `ignored` function. 

For most errors their kind determines the severity. So instead of writing 
```rust
if let Err(e) = some_fallible_operation() {
    warn!(%e, "Some erorr occurred")
}
```

We write 
```rust
some_fallible_operation()
	.logged()
	.ignored("If `some_fallible_operation` failed, you probably have something wrong with your ports");
```
Less code, more information, the message in the `ignored` doubles as a comment for why we aren't handling the error. 

Additionally the code generated here will make use of the fact that `eyre::Report`'s `core::fmt::Debug` implementation prints the traceback, so as to print the entire traceback in the logs for the **debug** build, while reducing the verbosity in the **release** build. 



### Issue

#2163 

### Benefits

Less boilerplate, more diagnostic information when you need it. 

### Possible Drawbacks

For all errors handled this way, the `error` span is attached to the implementation for this error type and not the call-site where the error "first" occurred. 

Resolution pending 
https://discord.com/channels/500028886025895936/627649734592561152/1034897182333091850

### Alternate Designs *[optional]*

A (postfix) macro based solution could do just as well. 

A prefix macro with a mini-syntax could resolve the issue of spans, but be more cumbersome to use. 

An attribute-like macro is also possible with the following syntax:
```rust 
#[log_on_err]
fn function_calling_fallible(… ) -> … {
	some_fallible_operation().logged().ignored("Helpful message");
	another_fallible_op()
		.map(do_something)
		.map_err(do_something_else)
		.logged!() // Expands in-place. 
		.map_err(one_last_time)
		.ignored("With this error"); 
	for e in results {
		e.is_err().break() now; // `.break()` returns `ControlFlow::Break` which then gets applied by the `now` keyword
	} // functions as `if let Err(e)` break. 
	result.if_error().short_circuit()
}
```
which corrects the span information and adds functionality and posprocesses the methods via keywords, but complicates the system and removes the flexibility of the trait implementation using the full-fat type level information. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-26 19:21:44 +0000 UTC
    </div>
</div>

