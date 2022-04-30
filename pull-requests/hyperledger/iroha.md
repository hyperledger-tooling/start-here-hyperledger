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
                PR <a href="https://github.com/hyperledger/iroha/pull/2169" class=".btn">#2169</a>
            </td>
            <td>
                <b>
                    [feature] #2163: Detailed logging.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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
Adds  a new trait `LoggedError`, that allows quickly logging errors when they occur. 

### Issue

Addresses #2163 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

More logging information

### Possible Drawbacks

Performance regression possible. 

### Usage Examples or Tests *[optional]*

TODO

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 10:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2168" class=".btn">#2168</a>
            </td>
            <td>
                <b>
                    [ci]: Fix deploy pipeline.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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

Added missing dependencies to the `Dockerfile`

### Issue

None



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 10:10:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2166" class=".btn">#2166</a>
            </td>
            <td>
                <b>
                    [ci] #2153: Fix #2154
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
- Add a step to add `llvm-tools-preview` component

### Issue
- Closes #2153
- Opens #2165

### Benefits
- Enables the coverage by fixing [the error](https://github.com/hyperledger/iroha/runs/6213237858?check_suite_focus=true#step:6:8) that #2154 did not resolve

### Possible Drawbacks
- CI cost by the duplicated step which [should have been done in the container](https://github.com/hyperledger/iroha/blob/7e338a5c762f7e0e25b79937e6215c10ae53b290/Dockerfile.ci#L51), which could be cut off
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 06:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2164" class=".btn">#2164</a>
            </td>
            <td>
                <b>
                    [feature] #2161: generate FFI functions for `data_model`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Marin Veršić <marin.versic101@gmail.com><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

You can find a description here: #1973 
#### Limitations:
1. mutable references are not supported for input arguments, except for the self argument, i.e. handle

There is a possibility `iroha_data_model_derive` will have to be made into a crate accessible by `iroha_crypto` as well

#### TODO:
* conversions in the FFI function body
* tests - most of all compile tests

### Issue

Closes #2161 

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
        Created At 2022-04-28 16:16:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2162" class=".btn">#2162</a>
            </td>
            <td>
                <b>
                    [documentation] #1991: Add readme to Kura inspector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

Add readme for Kura Inspector

### Issue

Resolves #1991
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 13:55:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2160" class=".btn">#2160</a>
            </td>
            <td>
                <b>
                    [feature] #2105: handle query errors in client
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

- `QueryResponseHandler` emits typed error, which can be either a certain error with decoded `QueryError` or some indeterminate `eyre` error
- Add some unit tests
- Add one integration test

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Resolves #2105 

### Benefits

<!-- What benefits will be realized by the code change? -->

Client users will be able to handle query errors more precisely. Improves DX/UX. 

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

None

<!-- ### Usage Examples or Tests *[optional]* -->

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

<!-- ### Alternate Designs *[optional]* -->

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
        Created At 2022-04-28 09:46:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2157" class=".btn">#2157</a>
            </td>
            <td>
                <b>
                    [feature] #1889: Domain scoped triggers
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

I'm not sure if I have understood the issue completely. As I understand *domain-scoped triggers* are just triggers with filter watching for specified domain and not trying to match events from other domains. So I decided to just improve existing system for domain-associated events and filters.

`TriggerSet` now works faster with domain-associated events.
In module description there is a proposal to make `TriggerSet` to be something like tree or hash-table (see `core/src/triggers.rs`). As I can see it should have some *nodes* to be hardcoded as structure field to provide strong-typing. My change is something like that.

Now `TriggerSet` can be represented like this:
```
                      triggers
                      /      \
            data-triggers     others
               /        \
domain-associated      non-domain-associated
```

So it's closer to a tree than before, but it's not ideal for now

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #1889

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now domain-associated triggers won't check every event, and will check only ones that happened in the related domain. That should be a huge performence improvement for blockchains with a lot of domains.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

I've found a bug with our `log` macro from `iroha_logger`. In fact it's just an alias for `instrument` macro from `tracing` crate. It just goes to a deadlock or infinite recursion or something. The problem occurs in the newest packages too. I used `cargo expand` to debug this, but it's a deep rabit-hole with no end.

I've found a way to avoid this problem, but it requires to clone every trigger before executing it. This can be really painful for big triggers i.e. with WASM blobs. You can see details in `WorldStateView::apply()`.
Another way to avoid this bug would be just removing `log` macro from every `Execute` implementor in `smartcontracts/isi/mod.rs`

Also maybe I should try to create minimal reproducible example of this bug and create a new issue in `tracing` repo. But this will require some work to do.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Alternate Designs

Let me know if it's not what supposed to be a *Domain-scoped trigger* or the design doesn't fit well for it

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
        Created At 2022-04-27 22:03:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2156" class=".btn">#2156</a>
            </td>
            <td>
                <b>
                    [feature]: #1572: Specialized permission tokens
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

Created concrete types for `PermissionToken`s predefined in `public_blockchain` to enable client interaction with `public_blockchain` be less stringly-typed.
Added cli util to list the new concrete token types. 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Resolves #1572 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Less stringly-typed `public_blockchain`.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None?
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 13:40:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2155" class=".btn">#2155</a>
            </td>
            <td>
                <b>
                    Fix GHA security issue
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
Change all checkouts from REFs to HASHes
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
https://gist.github.com/ryjones/b64ac4eb5123d114323851bc8ef64480
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
        Created At 2022-04-27 09:20:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2154" class=".btn">#2154</a>
            </td>
            <td>
                <b>
                    [ci] #2153: Fix coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
1. Resolve the toolchain differences around `llvm-tools-preview`

2. ~~Move the coverage tool from [`grcov`](https://github.com/mozilla/grcov#example-how-to-generate-source-based-coverage-for-a-rust-project) to [`cargo-llvm-cov`](https://github.com/taiki-e/cargo-llvm-cov#cargo-llvm-cov) ?~~

### Issue
- Closes #2153

### Benefits
1. Fix the CI failure

### Possible Drawbacks
2. ~~Not sure how long `cargo-llvm-cov` will be maintained~~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 07:51:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2147" class=".btn">#2147</a>
            </td>
            <td>
                <b>
                    [refactor] #2144: redesign client's http workflow, expose internal api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
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

Currently client is built on top of blocking synchronous HTTP client, which is not very flexible for different use cases.

To make it more flexible, I've split some of the APIs into 2 parts:

1. Preparing transaction/query/other HTTP request in terms of pure data
2. Handle related HTTP response for this request

I've **moved the part of actual doing** the request out of this. By the way, current main function are still using the default http implementation, but these parts are moved out from it.

It is done with a new trait - `RequestBuilder`. I've added several functions to the `Client`:

- `prepare_query_request(query, pagination)`, that returns a tuple with a provided `RequestBuilder` and a special response handler.
- `prepare_transaction_request(tx)`, same as for queries, but also returns a hash of a transaction.
- `prepare_status_request()`, same as above, but simpler.

There are also 3 new structs - `QueryResponseHandler`, `TransactionResponseHandler` and `StatusResponseHandler`. All of them encapsulates the logic of handling an HTTP-response in a correct way.

I haven't touched WebSocket-based logic and some other complex utilities that rely on default HTTP client yet. Anyway it should be refactored as well.

Also I've refactored the http internal module itself.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Resolves #2144 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

- Possibility to use `iroha_client` with custom HTTP transport, even async. **Only for queries, transactions and status for now.**
- Usage of `trait RequestBuilder` allows to build requests in an efficient way. It would be less efficient if build it via callbacks or by returning the exact request structure.
- Client is still responsible to handle http response
- You don't need to import anything to handle response, and currently "responders" are a zero-cost abstraction
- Existing client API hasn't been changed, but has been extended.

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

- `Headers` are still `HashMap<String, String>`, which can be optimized in scope of `RequestBuilder` trate.
- Response handlers expect `Response` structure from the `http` crate. It may be unefficient if custom http implementation returns some other response and user has to transform it first. Maybe it is better to replace `Response` with some trait.

### Usage Examples or Tests

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

Existing client methods now uses the same API, but with default HTTP client. See how they now work.

<!-- ### Alternate Designs -->

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
        Created At 2022-04-25 18:28:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2146" class=".btn">#2146</a>
            </td>
            <td>
                <b>
                    [refactor] #2145: refactor client's `WebSocket` side, extract pure data logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
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

The idea is the same as in #2147, but now it is about WebSocket side.

Iroha Events API and Blocks Stream API are built on top of the same WebSocket flow:

1. Open a WS connection
2. Client sends some "subscription" message
3. Server responses with some "accepted" message
4. Client waiting for some events and responses to them with some "accepted" message, not same as for p.3

In this PR I've normalized this flow with a few traits. They are binded to each. Their relationship aims to provide API that targets these goals:

- don't have `dyn`s, but clear abstraction
- prevent "invariant violation" by scoping flow stages in separate traits
- be functional and data-oriented

Also, I've refactored `trait RequestBuilder`. Now it forces to call `.body()` fn anyway to get the output of the builder. It is how `RequestBuilder` from `http` crate works. With this design, its impls became clearer.

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Resolves #2145 

### Benefits

<!-- What benefits will be realized by the code change? -->

With this change, it is possible to use Events API with any WebSocket client, async or not.

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

I don't like naming of `WebSocketFlowXXX` traits.

### Usage Examples or Tests

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

See how now Events API is implemented. Note that all data-related logic is incapsulated within flow-structs, and all transportation logic is moved away from it.

<!-- ### Alternate Designs *[optional]* -->

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
        Created At 2022-04-25 18:26:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2140" class=".btn">#2140</a>
            </td>
            <td>
                <b>
                    [fix] #1737: Blockchain by reference instead of cloning.
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
Replace dashmap with spinlock based mutex in order to support referencing into the block chain.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#1737 and #1974
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Easier to debug deadlocks due to them being a lot less subtle.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
We might have slower performance due to locking but so far I haven't measured any significant change.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-23 14:00:13 +0000 UTC
    </div>
</div>

