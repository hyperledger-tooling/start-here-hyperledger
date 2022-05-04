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
                PR <a href="https://github.com/hyperledger/iroha/pull/2174" class=".btn">#2174</a>
            </td>
            <td>
                <b>
                    [ci]: Version bump all of the crates.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

### Description of the Change
Version bump

### Issue
None

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Version bump

### Possible Drawbacks

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 06:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2173" class=".btn">#2173</a>
            </td>
            <td>
                <b>
                    [feature] #2004: Forbid `isize` and `usize` from becoming `IntoSchema`.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

### Description of the Change

Add a unit test that fails when `usize`/`isize` are `Encode`/`Decode`/`IntoSchema`

### Issue

Closes #2004 

### Benefits

Impossible to add structures which utilise `usize`, `isize` inside the schema, and thus cause UB in decoding if the pointer size on the host machine is smaller than the encoded integer.

### Possible Drawbacks
None

### Usage Examples or Tests *[optional]*


```
cargo test -p iroha_schema --test architecture-dependent
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 18:49:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2172" class=".btn">#2172</a>
            </td>
            <td>
                <b>
                    April release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Overview of changes
- Kagami (consolidating generators)
- Key-pairs validated on construction
- Client has low-level API exposed 
- Benchmarks
- Various FFI-friendly changes. 
- Pagination
- Parity scale decoder
- Non-mintable assets
- Websocket fixes. 
- `RawGenesisBlockBuilder` API. 


The changelog shall be generated soon. 

## Release checklist
- [ ] The crates have been version bumped.
- [ ] Iroha successfully passes all CI checks
- [ ] Iroha passed all QA tests
- [ ] Iroha lasted for five days at the longevity stand
- [ ] Standard benchmarks are ran and the results are recorded in the repository
- [ ] Iroha documentation and tutorial are up to date. 
- [ ] SDKs compiled successfully using the schema from latest branch (Hash: [94f75ba2465da8bc4b602c3be892a68f0c030ecc](https://github.com/hyperledger/iroha/commit/94f75ba2465da8bc4b602c3be892a68f0c030ecc))
  - [ ] Java
  - [ ] JavaScript
  - [ ] Swift (N/A)
- [ ] All SDK tests pass
  - [ ] Java
  - [ ] JavaScript
  - [ ] Swift (N/A)
- [ ] (Optional) SDKs implemented the main features added in the current release (N/A)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 07:54:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2171" class=".btn">#2171</a>
            </td>
            <td>
                <b>
                    [documentation]: Add Ekaterina to the list of codeowners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Add Ekaterina (the tech writer for the project) to the list of codeowners
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 07:42:05 +0000 UTC
    </div>
</div>

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

This PR introduces an `ffi` crate which holds a macro `ffi_bindgen`. This macro when attached to the impl block generates the equivalent `ffi` out of the methods listed in the impl block. The macro can also be attached to the structure definition where it integrates with `getset` to make `ffi` fn equivalents of the getters/setters produced by the `getset`.

#### Note:
1. All FFI functions return `FfiResult` return code. The idea is that the returned code can be used to query the error
2. Considering the previous points, all FFI functions take, as a last argument, a mutable pointer where the return value of the corresponding method is stored (the so called out-pointer pattern)

#### Limitations:
1. mutable references are not supported for input arguments, except for the self argument, i.e. handle

#### WIP:
* `getset` integration
* tests

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

