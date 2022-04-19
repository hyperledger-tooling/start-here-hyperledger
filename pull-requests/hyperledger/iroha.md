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
                PR <a href="https://github.com/hyperledger/iroha/pull/2117" class=".btn">#2117</a>
            </td>
            <td>
                <b>
                    [refactor] #1256: redesign http workflow, expose internal client api
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

Resolves https://github.com/hyperledger/iroha/issues/1256 (partially)

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

- The big part of client is not refactored to new design.
- `Headers` are still `HashMap<String, String>`, which can be optimized in scope of `RequestBuilder` trate.
- Response handlers expect `Response` structure from the `http` crate. It may be unefficient if custom http implementation returns some other response and user has to transform it first. Maybe it is better to replace `Response` with some trait.

### Usage Examples or Tests

For example, making async queries could be done like this:

```rust
use iroha_client::{Client, http::{RequestBuilder, Method, Headers}};
use iroha_data_model::prelude::{FindAllAccounts, Account};
use std::borrow::Borrow;
use eyre::Result;

struct MyClient(SomeAsyncClient);

// Implementing request building
impl RequestBuilder for MyClient {
    fn build<U, P, K, V>(
        method: Method,
        url: U,
        body: Vec<u8>,
        query_params: P,
        headers: Headers,
    ) -> Result<Self>
    where
        U: AsRef<str>,
        P: IntoIterator,
        P::Item: Borrow<(K, V)>,
        K: AsRef<str>,
        V: ToString,
    {
        let builder = _; // build your underlying client

        Ok(Self(builder))
    }
}

// making query asynchronously!
async fn make_some_query(client: &Client) -> Result<Vec<Account>> {
  let (req, resp_handler): (MyClient, _) = client.prepare_query_request(FindAllAccounts::new(), _ /* some pagination*/)?;
  let resp = req.0.send().await?; // depends on the client itself
  resp_handler.handle(resp.into())
}
```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs

<!-- Explain what other alternates were considered and why the proposed version was selected -->

Other implementations, like implementing the whole HTTP-cycle within the client, require an injection of the exact http-client or passing a callback inside of it. But an implementation may be both blocking and async. In this case, client should expose both symmetric APIs - blocking and async, for each endpoint. It requires a more complex solution than mine one. Also it can bring some limits to the library if it exposes async (Future-based) APIs, but not necessary. 

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 08:55:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2115" class=".btn">#2115</a>
            </td>
            <td>
                <b>
                    [schema] #2114: Sorted collections support in schemas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span>
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

* define stable schema type names
* introduce sorted collections to schemas

Considering that we make abundant use of digital signatures, serialized formats of our internal structures must have a defined ordering, e.g. `BTreeMap` must be represented as a sorted vector of tuples. While it may be possible that there will be `BTreeMap`s that won't be part of a structure that is signed(and require a defined ordering of tuples), I find it to be quite unlikely and don't think it worth to support such exception.

### Issue

Closes #2114 

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2022-04-17 14:25:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2110" class=".btn">#2110</a>
            </td>
            <td>
                <b>
                    [refactor] #2109: Make `integration::events::pipeline` test stable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
Refactored.

### Issue
- Closes #2109

### Benefits
- Stable test result
- Shorter CI time

### Possible Drawbacks
None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-16 11:48:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2107" class=".btn">#2107</a>
            </td>
            <td>
                <b>
                    [feature] #2108: Add pagination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: BAStos525 <66615487+BAStos525@users.noreply.github.com><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Add pagination support for SDKs. 

### Issue

Closes #2108 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Pagination added to queries, so that SDKs have access to the Pagination struct. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 09:50:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2104" class=".btn">#2104</a>
            </td>
            <td>
                <b>
                    [fix] #1640: Generate `genesis.json` and consolidate generation into one tool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span><span class="chip">Refactor</span>
            </td>
            <td>
                ### Description of the Change

Can now use `iroha_docs` binary to generate sample `genesis.json`

### Issue
Closes #1640 
Relates to #1992


<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Can now generate and check if the `genesis.json` needs updating. 

### Possible Drawbacks

None

### Usage Examples or Tests *[optional]*

```
cargo run --bin iroha_docs -- --genesis > /tmp/genesis.json && diff /tmp/genesis.json  configs/peer/genesis.json
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 13:27:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2095" class=".btn">#2095</a>
            </td>
            <td>
                <b>
                    [fix] #2005: Fix `Client::listen_for_events()` not closing WebSocket stream
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

* Fix `Client::listen_for_events()` not closing WebSocket stream
* Fix `torii` doing only part of WebSocket handshake

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2005

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now event streaming satisfies WebSocket protocol

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 12:38:14 +0000 UTC
    </div>
</div>

