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
                PR <a href="https://github.com/hyperledger/iroha/pull/2644" class=".btn">#2644</a>
            </td>
            <td>
                <b>
                    [feature] #2628: Add support for `repr(transparent)` in FFI
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

- Before transparent structs cross ffi as opaque pointers, now conversion to ffi delegated to inner field;
- Remove special handling of `fn(T) -> T` because this case was created under assumption that every struct passed as opaque pointer (implementation use `read/write/is_null` methods) which not hold in general for transparent and non-opaque structs.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2628.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Reduce number of indirections.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Case `fn(T) -> T` now uses 2 allocations instead of 1 and a bit less convenient to write.

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
        Created At 2022-08-23 08:46:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2641" class=".btn">#2641</a>
            </td>
            <td>
                <b>
                    [feature] #2596: Wasm validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Security</span><span class="chip">Yellow</span>
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

* Added `Validator` and related things to the *data_model*
* Added `Chain` of validators to the `World`. With that we can check operations using runtime validators.
* Added instructions to modify this chain. Such as `Register<Validator>` and `Unregister<Validator>`
* Added entrypoint macro for validators
* Added suppor of validators into `wasm.rs` module
* Added test with sample validator

There are also **a lot** of **TODO** in this PR. This **TODO**s are the questions to the reviewers and my suggestions for a future.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2596 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* Runtime validators

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

There are two main drawbacks (which are mentioned in the code too):

1. Malicious validator probably can break Iroha peer because right now Iroha believes that *validator* provides valid memory with `Verdict` sruct inside. If not, then UB. 
2. I really don't know why, but I can't prevent memory leak with this returned `Verdict`. Then I'm trying to deallocate it on Iroha side I get: `pointer being freed was not allocated` error. See `wasm.rs` and `wasm/derive/src/validator.rs` for details.

I think this 2 problems can be fixed with one shot. We should limit `Verdict` struct size (I mean denial reason string should be limited e.g. 256 bytes). Then we can allocate memory on Iroha side and provide it to the validator.
Remember that right now we need to allocate not just `size_of::<Verdict>()` but unpredictable number of bytes, because we use `parity_scale_codec::Encode` which encodes string with denial reason as well, and that string can have any size.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

Comment `ignore` attribute on `deny_new_validators()` test.

Then run:

```bash
cargo +nightly-2022-08-15 test --package iroha_client --test mod -- integration::permissions::runtime_validators::deny_new_validators --exact --nocapture
```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-20 16:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2639" class=".btn">#2639</a>
            </td>
            <td>
                <b>
                    [feature] #2586, #2616: `Builder` and `LoadFromEnv` for proxy structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ilia Churin <churin.ilya@gmail.com>

-------

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Proxy structs in the `Combine` derive macro now also derive `LoadFromEnv`, as well
as have their `Builder` implementation fixed.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Resolves #2586 and #2616.
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Getting closer to the aims of the corresponding epic.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Implementations still untested. Though they typecheck, thorough foolproofing
is a matter of future work.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

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
        Created At 2022-08-20 07:11:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2636" class=".btn">#2636</a>
            </td>
            <td>
                <b>
                    [fix] #2561: Reintroduce viewchanges to consensus.
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

Viewchanges are reintroduced without transaction receipts. This method does diverge slightly from the whitepaper, but I think it is warrented as no malicious node would ever send you a proof of the fact that they are censoring you. And in the common case on a real world network, most nodes have transactions to test against the leader, so if a block is not created they can all very quickly coordinate a view change because they will all be suspicious of the leader.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#2561 
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
This version is simpler, faster, and more robust.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
In this implementation we do not track who to blame for a failed round. This can be added though.
The test for time triggers fails on my machine, I don't know why though. Probably has to do with this implementation producing blocks at a different pace.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*
I've enabled trace level logging on the tests. Use the following to observe execution and build an understanding. 
```
cargo test integration::unstable_network::unstable_network_4_peers_1_fault -- --nocapture | grep sumeragi
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 15:37:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2634" class=".btn">#2634</a>
            </td>
            <td>
                <b>
                    [feature] #2611: Derive `TryFromReprC` and `IntoFfi` for generic opaque structs
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

Derive `TryFromReprC` and `IntoFfi` for generic opaque structs.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Resolves #2611.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Make possible to define ffi functions with generic struct parametrized with concrete type as argument or return value.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None. 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

```
cargo test --package iroha_ffi --test generics -- return_generic --exact --nocapture
```

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 05:30:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2633" class=".btn">#2633</a>
            </td>
            <td>
                <b>
                    [refactor]: Use context in IntoFfi
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
        Created At 2022-08-17 15:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2631" class=".btn">#2631</a>
            </td>
            <td>
                <b>
                    [fix] #2623: fix doctest for VariantCount
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Artemii Gerasimovich <gerasimovich@soramitsu.co.jp>

### Description of the Change

Fix doctest for `VariantCount` derive macro.

### Issue

#2623 


### Benefits

Doctest passes

### Possible Drawbacks

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 22:02:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2630" class=".btn">#2630</a>
            </td>
            <td>
                <b>
                    [fix] #2457: Forcibly shut down kura in tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Artemii Gerasimovich <gerasimovich@soramitsu.co.jp>

### Description of the Change

So I’ve been debugging #2457, and the problem there is as follows:

When we start a peer for tests, we [create](https://github.com/hyperledger/iroha/blob/a2b373d7fb21dc24f27cf83bf1c8cb9a6b187b98/core/test_network/src/lib.rs#L673) a [TempDir](https://docs.rs/tempfile/latest/tempfile/struct.TempDir.html) for kura storage. It is then [held](https://github.com/hyperledger/iroha/blob/a2b373d7fb21dc24f27cf83bf1c8cb9a6b187b98/core/test_network/src/lib.rs#L502) until the peer is dropped to prevent its deletion. But kura thread receiving new blocks actually [lives on its own](https://github.com/hyperledger/iroha/blob/a2b373d7fb21dc24f27cf83bf1c8cb9a6b187b98/core/src/kura.rs#L77) and periodically [checks](https://github.com/hyperledger/iroha/blob/a2b373d7fb21dc24f27cf83bf1c8cb9a6b187b98/core/src/kura.rs#L182) if all other references to kura have been dropped and then returns. 

What happens is essentially a race condition, where after a test is finished, peer is dropped, dropping the tempdir, but kura is in process of writing a new block, so it's working directory is pulled from underneath it. This causes kura thread to panic, which wasn't a problem on its own, but is now caught by panic handler and leads to failure.

This PR is my shot of solving it by providing an ability to forcibly shut kura down and doing just that while dropping a test peer.

### Issue

#2457

### Benefits

Kura doesn't panic in tests.

### Possible Drawbacks

Not a particularly elegant solution.

### Alternate Designs

We can't hold tempdir for long enough, since there's no scope that's guaranteed to exceed kura threads lifetime.

We also can't provide a method to just _wait_ for kura to shut down without forcing it to with how it's currently implemented, since kura shuts down only when all strong references to it are dropped, and there is one in the same task that holds the tempdir.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 21:42:43 +0000 UTC
    </div>
</div>

