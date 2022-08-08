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
                PR <a href="https://github.com/hyperledger/iroha/pull/2593" class=".btn">#2593</a>
            </td>
            <td>
                <b>
                    [documentation]: Fix incorrect doc comment in permission validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 11:03:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2591" class=".btn">#2591</a>
            </td>
            <td>
                <b>
                    [feature] #2158: Update `parity_scale_codec`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Add changelog

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 09:28:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2590" class=".btn">#2590</a>
            </td>
            <td>
                <b>
                    [feature] #2511: Restrict FFI types on wasm (WIP)
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

- Add `wasm` feature to `iroha_ffi` crate;
- Add `PrimitiveRepr` trait to substitute unsupported types with supported ones;
- Refactor `Vec`  transfer through ff-boundry.  

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2511.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Protect from various errors (when user can pass u32 where u8 supposed to be).

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

More complex implementation.

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
        Created At 2022-08-03 15:03:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2583" class=".btn">#2583</a>
            </td>
            <td>
                <b>
                    [refactor] #2118: WIP: `Default` config
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

- [x] A new trait `Combine` in `iroha_config_base::proxy` and its corresponding error
- [x] Refactor `iroha_config_base::derive` crate into modules
- [x] `Proxy` derive macro
- [ ] Deeper refactor of `Configurable` trait to make it more readable
- [ ] Make `Proxy` completely conform to `Configurable` and implement all its methods
- [x] Placeholder trait `DocsDefault` to make `kagami` work for the time being 

All of these changes won't probably go into a final real PR (quite likely nothing in its current form besides the crate refactor), so instead this draft may serve as a ground for comments that can become guidelines for my future work. Moreover, the code doesn't even compile at the time of writing due to the unfinished point 5 from the list above.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

Was part of work towards #2118, but in a discussion with @appetrosyan it was decided to make it an epic and split it into more smaller ones to make the progress more trackable. Will update this part after most of them are created.

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Ideally, the end result should not only allow flexible loading of configuration, but also give informative messages/suggestions in case of failure. E.g. if no keys were provided, suggest a command to generate them (or have a flag for generation on the fly). Moreover, it wouldn't hurt if at start Iroha logs explicitly, which parts of configs are loaded as default values due to them not being provided. 
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Current design of `Configurable` trait suffers from interface multiplicity, that is, it serves two functions at once which should eventually be decoupled: things pertaining to configuration loading and initialization, and all the things related to querying it or modifying parameters at runtime.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


### Alternate Designs
Not necessarily alternate designs, but a few things mentioned in previous discussion:
* To save space, some of the values in config proxies could be stored as `ConstStr`.
* Typechecking in procedural macros. This is more of a general issue relating to all our macro work. Instead of trying to naively check some AST node ident against a string, it would make sense to have a small function that's part of the macro expansion doing this job.
* Despite all of the fields in `ConfigProxy` being wrapped in `Option` to signify the possibility of them being uninitialized, there are some fields which have to be initialized eventually, and those that don't and can instead rely on the default value. This distinction could be marked by having a separate struct for the non-defaultable option fields.

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
        Created At 2022-08-02 15:36:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2582" class=".btn">#2582</a>
            </td>
            <td>
                <b>
                    [refactor] #2001: `EvaluatesTo` static type checking
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Security</span>
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

#### EvaluatesTo (#2001)

* `Into EvaluatesTo<V>` conversion now has stricter bounds which provides static type checking
* For some cases there is no possibility to make a compile-time check (i.e. `Where`, `ContextValue` expressions and all queries) so we need a way to explicitly construct `EvaluatesTo<V>` omitting the type checking. That's why I've created `EvaluatedTo::<V>::new_unchecked()`
* Since all expressions and queries return `impl TryFrom<Value>` it's always safe to construct `EvaluatesTo<Value>`. That's why there is `EvaluatesTo::<Value>::new_evaluates_to_value()`
* Added ui test which ensures that there is no way to implicitly construct `EvaluatesTo` from uncompatible type

While doing that I've found a bug in `Queue` and fixed it. See next section.

#### Tx signature condition checking bug (#2580)

* Added `MustUse` type wrapper to `primitives`
* `MustUse` used for a checking function
* Added test which ensures that you get `unused_must_use` warning will be generated if `MustUse` type is unused
* Fixed actual bug

### Issue

* Closes #2001 
* Closes #2580 

After succesfull review I'll squash my commits into two -- one per resolved issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

#### EvaluatesTo (#2001)

* Now it's easier to write correct tests
* Found the important bug

#### Tx signature condition checking bug (#2580)

* Added helpful `MustUse` wrapper type
* Important bug fixed

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Harder to construct `EvaluatesTo` from types which require runtime check

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

You can run existing test, because a bunch of them where updated.

Also there are two new tests with `trybuild`:

#### `EvaluatesTo`

```bash
cargo test --package iroha_data_model --test ui -- ui --exact --nocapture 
```

#### `MustUse`

```bash
cargo test --package iroha_primitives --test ui -- ui --exact --nocapture
```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs

@appetrosyan suggested to add `ok_or(err)` function to `MustUse` which should work something like this:

```rust
impl MustUse<bool> {
    pub fn ok_or<E>(err: E) -> Result<(), E> {
        if self.0 {
            Ok(())
        } else {
            Err(E)
        }
    }
}
```

But I have next the thoughts:

1. It's not that usable as it may look
2. [`std ok_or`](https://doc.rust-lang.org/std/option/enum.Option.html#method.ok_or) does not force you to return `()` as `Ok`
3. It does not follow the *Unix rule* and *Single-responsibility rule*

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
        Created At 2022-08-02 15:33:28 +0000 UTC
    </div>
</div>

