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
                PR <a href="https://github.com/hyperledger/iroha/pull/2235" class=".btn">#2235</a>
            </td>
            <td>
                <b>
                    [feature] #1413: Add API version endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ilia Churin <churin.ilya@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Added a new endpoint that gives back the current API version as a JSON string. 
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Resolves #1413.
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
As we're about to introduce versioning, this will allow end users to check if their client and our API versions match.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Set to grab the version from the genesis block, so the endpoint should be usable at all times when a minimal network is up. `ChainIterator` in `wsv`'s `blocks()` method was mentioning possible deadlock, but it should be safe in this case in all I can tell.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests
Added some documentation describing the change in `api_spec.md`.
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
        Created At 2022-05-19 11:03:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2234" class=".btn">#2234</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update Iroha Client and Iroha CLI Client documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Updates readmes for:

- Iroha Client: https://github.com/outoftardis/iroha/tree/doc-client/client#iroha-client
- Iroha CLI Client: https://github.com/outoftardis/iroha/tree/doc-client/client_cli#iroha-cli-client

### Issue

Partially addresses #2193 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 09:52:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2230" class=".btn">#2230</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update benchmarks documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Updated readme in `client/benches/tps`: https://github.com/outoftardis/iroha/tree/doc-tps-bench/client/benches/tps#benchmarks-transactions-per-second-tps

### Issue

Partially addresses #2193 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 07:45:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2229" class=".btn">#2229</a>
            </td>
            <td>
                <b>
                    [refactor]: Move `TriggerSet` to `data_model`
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

Initially it suppose to close #1889 but in the middle of work it was decided to wait until we get dynamic wasm linking. Dynamic linking is important, cause it will remove `no_std` limitations from `data_model` and `TriggerSet` is not compatible with `no_std`.
So this PR contains only `TriggerSet` moving to `data_model`. It should be useful for the future.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

None

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* `TriggerSet` now is stored there it should be
* Errors produced by `TriggerSet` make more sense

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 15:54:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2224" class=".btn">#2224</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update Parity Scale Decoder Tool documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Updated README for Parity Scale Decoder Tool: https://github.com/outoftardis/iroha/tree/doc-psd/tools/parity_scale_decoder#parity-scale-decoder-tool

### Issue

Partially addresses #2193 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 07:23:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2223" class=".btn">#2223</a>
            </td>
            <td>
                <b>
                    [ci] #2222: Split tests by whether it involves coverage or not
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
- Split tests into 3 jobs
  - `checks`
    - script checks
    - Wasm build check
  - `tests_with_coverage`
    - unit tests #2222
    - integration tests (in a broad sense; crate/tests/) except for client/tests/integration/
  - `integration_tests` #1683
    - integration tests (in a narrow sense; client/tests/integration/)
- Move from `grcov` to `cargo-llvm-cov`
- Include UI tests to coverage profiling #2148

### Issue
- Closes #1683
- Closes #2148
- Closes #2222

### Benefits
- Revival of coverage
- Visible coverage failure
- Accuracy of cover rate by #1683 #2148
- CI optimization by #2222

### Possible Drawbacks
- Appearance of 10% or more regression in coverage due to the strict new standard
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 16:54:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2221" class=".btn">#2221</a>
            </td>
            <td>
                <b>
                    Merge commit
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
        Created At 2022-05-17 13:26:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2220" class=".btn">#2220</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update Kagami documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                ### Description of the Change

Update the readme for Kagami: https://github.com/outoftardis/iroha/tree/doc-kagami/tools/kagami

### Issue

Partially addresses #2193 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 12:27:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2219" class=".btn">#2219</a>
            </td>
            <td>
                <b>
                    [documentation] #2192: Review contributing guidelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Update the structure and wording of the CONTRIBUTING guide

https://github.com/outoftardis/iroha/blob/doc-contributing-review/CONTRIBUTING.md

### Issue

Addresses #2192 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 08:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2218" class=".btn">#2218</a>
            </td>
            <td>
                <b>
                    Minor fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.6</span>
            </td>
            <td>
                ### Description of the Change
1. No cache synchronization on round switch
2. Send/Recv packets size become 128 Mb.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 07:30:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2217" class=".btn">#2217</a>
            </td>
            <td>
                <b>
                    [fix] #2215: Make nightly optional for building Iroha.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                April release<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

See #2216 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 06:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2216" class=".btn">#2216</a>
            </td>
            <td>
                <b>
                    [fix] #2215: Make nightly-2022-04-20 optional for `cargo build`
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

Removed the requirement for having the `nightly-2022-04-20` installed with the right components for building Iroha. The client test with the WASM smartcontract is now only ran if the `+nightly` toolchain was used to run cargo. 

### Issue

Closes #2215
Opens #2225 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Easier to compile for users. 

### Possible Drawbacks

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 13:21:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2214" class=".btn">#2214</a>
            </td>
            <td>
                <b>
                    [feature] #2125: Add query for `FindAssetDefinitionById`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Fixes #2125 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 12:11:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2213" class=".btn">#2213</a>
            </td>
            <td>
                <b>
                    [feature] #2056: Add a derive proc macro crate for AssetValueType enum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ilia Churin <churin.ilya@gmail.com>

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
Added a crate with a proc macro to `data_model` that allows automatically deriving `FromStr` impls for any enums exhaustively. 

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->
Resolves #2056.
<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
`FromStr` derived automatically for all variants instead of having to list them manually as was done with a declarative macro.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Doubtful if this new dependency should be placed into `data_model` or in the `macro` crate and then re-exported. Opted for the former.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-15 05:25:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2211" class=".btn">#2211</a>
            </td>
            <td>
                <b>
                    [feature] #2161: generate FFI functions for `data_model`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                <!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

You can find a description here: #1973 

This PR introduces an `ffi` crate which holds a macro `ffi_bindgen`. This macro when attached to the impl block generates the equivalent `ffi` out of the methods listed in the impl block. The macro can also be attached to the structure definition where it integrates with `getset` to make `ffi` fn equivalents of the getters/setters produced by the `getset`.

#### Note:
1. All FFI functions return `FfiResult` return code. The idea is that the returned code can be used to query the error
2. Considering the previous points, all FFI functions take, as a last argument, a mutable pointer where the return value of the corresponding method is stored (the so called out-pointer pattern)

#### Limitations:
1. mutable references are not supported for input arguments, except for the self argument, i.e. handle

### Issue

Closes #2161 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

```rs
#[derive(Getters)]
#[getset(get = "pub")]
struct Struct {
    elem: u32,
    #[getset(skip)]
    elems: Vec<u32>,
}

#[ffi_bindgen]
impl Struct {
    pub fn new(elem: u32) -> Self {
        Self {elem, elems: vec![]}
    }
    pub fn get_elems(&self) -> impl ExactSizeIterator<&u32> {
        self.elems.iter()
    }
}

fn main() {
    let s = struct_new(42);
    let elems = MaybeUninit::<*const *const u32>::uninit();
    let elems_len = MaybeUninit::<usize>::uninit();
    if FfiResult::Ok != unsafe {struct_elems(&s, elems.as_mut_ptr(), elems_len.as_mut_ptr())} {
        // TODO: Handle error
    }
    let elems_len = unsafe {elems_len.assume_init()};
    let elems = unsafe {elems.assume_init()};
}
```

### Alternate Designs *[optional]*

List out ffi functions manually. This is tedious and highly error prone because we're operating in the `unsafe` space

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 17:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2210" class=".btn">#2210</a>
            </td>
            <td>
                <b>
                    [feature] #2103: support querying for blocks and transactions
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

Added `FindAllBlocks` and `FindAllTransactions` queries as described in #2103 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

No way to query for e.g. block explorer to query for older blocks

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Support querying for list of all blocks and transactions

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

As implemented in this PR, FindAllBlocks query introduces a block representation in `iroha_data_schema` parallel to one already present in `iroha_core`.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, ### Possible Drawbacksexplicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 15:34:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2209" class=".btn">#2209</a>
            </td>
            <td>
                <b>
                    I2 dco
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
        Created At 2022-05-13 08:58:35 +0000 UTC
    </div>
</div>

