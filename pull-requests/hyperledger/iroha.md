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
                <span class="chip">iroha2</span>
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

