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
                PR <a href="https://github.com/hyperledger/iroha/pull/2625" class=".btn">#2625</a>
            </td>
            <td>
                <b>
                    [feature] #2491: Enum support in FFi
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

Add support for converting data-carrying enums to and from FFI types. FFI equivalents for enums are not opaque, rather they are structs generated with FFI representation. Take the following enum as an example:

```rs
#[derive(IntoFfi, TryFromReprC)]
pub enum Enumeration {
    A(u32),
    B(PublicKey),
    C,
}
```

for `IntoFfi` will generate:

```rs
impl IntoFfi for Enumeration {
    type Target = __iroha_ffi__ReprCEnumerationIntoFfiTarget;
    
    fn into_ffi(self) -> Self::Target {
        ///
    }
}

unsafe impl ReprC for __iroha_ffi__ReprCEnumerationIntoFfiTarget {}

#[repr(C)]
#[derive(Clone, Copy)]
pub struct __iroha_ffi__ReprCEnumerationIntoFfiTarget {
    tag: u8,
    payload: __iroha_ffi__ReprCEnumerationIntoFfiTargetPayload,
}

#[repr(C)]
union __iroha_ffi__ReprCEnumerationIntoFfiTargetPayload {
    A: <u32 as IntoFfi>::Target,
    B: <PublicKey as IntoFfi>::Target,
}
```

for `TryFromReprC` will generate:

```rs
impl<'itm> TryFromReprC<'itm> for Enumeration {
    type Source = __iroha_ffi__ReprCEnumerationTryFromReprCSource<'itm>;
    type Store = (<u32 as TryFromReprC<'itm>>::Source, <PublicKey as TryFromReprC<'itm>>::Source);

    unsafe fn try_from_repr_c(source: Self::Source, store: &'itm mut Self::Store) -> Result<Self> {
        ///
    }
}

unsafe impl ReprC for __iroha_ffi__ReprCEnumerationIntoFfiSource {}

#[repr(C)]
#[derive(Clone, Copy)]
pub struct __iroha_ffi__ReprCEnumerationTryFromReprCSource<'itm> {
    tag: u8,
    payload: __iroha_ffi__ReprCEnumerationTryFromReprCSourcePayload<'itm>,
}

#[repr(C)]
#[derive(Clone, Copy)]
union __iroha_ffi__ReprCEnumerationTryFromReprCSourcePayload<'itm> {
    A: <u32 as TryFromReprC<'itm>>::Source,
    B: <PublicKey as TryFromReprC<'itm>>::Source,
}
```

### Issue

Closes #2622

### Benefits

Data-carrying enums can be used in FFI functions

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
        Created At 2022-08-15 18:53:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2618" class=".btn">#2618</a>
            </td>
            <td>
                <b>
                    [fix] #2560: Added back in block_sync and peer disconnecting.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sam H. Smith <sam.henning.smith@protonmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 13:14:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2613" class=".btn">#2613</a>
            </td>
            <td>
                <b>
                    [ci]: Updates an expected error in ui_fail tests
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

This error appeared after switching from 1.61 to 1.62 because error messages are a mismatch.

### Issue

None

### Benefits

Fixes [this problem](https://github.com/hyperledger/iroha/runs/7793931336?check_suite_focus=true#step:7:1296)

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
        Created At 2022-08-12 08:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2610" class=".btn">#2610</a>
            </td>
            <td>
                <b>
                    [ci]: Fix `iroha2:build` image build
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
Add build-args corresponding tags values for workflows.

### Issue
The step of `iroha2:build` image building can not identify TAG value in `Dockerfile.base` ARG pointer,

### Benefits

Make CI step of `iroha2:base` image build workable.

### Possible Drawbacks

Should be none.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 13:07:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2603" class=".btn">#2603</a>
            </td>
            <td>
                <b>
                    [documentation] #2544: Tutorial doctests 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span><span class="chip">Tests</span>
            </td>
            <td>
                Signed-off-by: 6r1d <vic.6r1d@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Adds example that mirrors tutorial examples, so that changes in the API can be propagated by directly taking them from GitHub. 

### Issue

Addresses #2544 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Direct connection to tutorial

### Possible Drawbacks

More code to test

### Usage Examples or Tests *[optional]*

```bash
cargo run --example tutorial
```

### Alternate Designs *[optional]*

As test

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 20:02:55 +0000 UTC
    </div>
</div>

