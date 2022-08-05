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
                    [documentation]: Changelog for pre-rc.7
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2576" class=".btn">#2576</a>
            </td>
            <td>
                <b>
                    [ci] #2461: Improve iroha2 CI
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

1. Move `iroha2:base` image build to the separate workflow and publish it on Dockerhub in order to make it reusable.
2. Distribute `iroha2:base` and `iroha2:build` images usage among branches.
3. Update references of `building load-rs script` jobs to the [iroha2-longevity-load-rs repository](https://github.com/soramitsu/iroha2-longevity-load-rs.git).
4. Switch to `actions/checkout@v3` where it hasn't been done so far.
5. Add step to trigger workflow of `Cargo.toml` dependencies updating.

### Issue
1. This PR resolves the major part of #2461 issue.
2. It also resolves [this issue](https://github.com/soramitsu/iroha2-longevity-load-rs/issues/18) partially.

### Benefits
1. Make iroha2 CI faster and more effective.
2. Make `iroha2-ci:<tag>` and `iroha2:build-<tag>` images be available for calling from other branches.
3. Follow to the last versions of third-party actions.
6. Update workflows calling for `longevity-load-rs` repo.

### Possible Drawbacks
1. A fresh feature: CI might be failed on any of `release` workflows or deploying `iroha2-ci` image.
2. It will not work until the corresponding `Dockerfile.base` and `Dockerfile.base` will be added to `iroha2` and `iroha2-lts` branches.
3. This [note](https://github.com/hyperledger/iroha/issues/2461#issuecomment-1184150212) hasn't still resolved (@s8sato @appetrosyan). [Original link to issue](https://github.com/hyperledger/iroha/pull/2433#discussion_r919960840).
4. `hyperledger/iroha2-ci` image doesn't compatible to be used for any of iroha2 tests workflows and jobs instead of `7272721/i2-ci:latest`. I spent some time to adopt it but it was unsuccessful due to a bunch of possible reasons. So, It is not the time for that yet.
5. Firstly we should merge [this PR](https://github.com/soramitsu/iroha2-longevity-load-rs/pull/23).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 15:56:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2575" class=".btn">#2575</a>
            </td>
            <td>
                <b>
                    [feature] #2553: Add sorting to asset queries
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

I've added sorting parameter into asset ISI queries. [More about here](https://github.com/hyperledger/iroha/issues/2553).

- [x] Minimal representation of this feature.
- [x] Implement for all queries.
- [ ] More tests.

### Issue

Resolves #2553 

### Benefits

Allows to sort asset queries

### Possible Drawbacks

None.

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 12:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2570" class=".btn">#2570</a>
            </td>
            <td>
                <b>
                    Bump mistune from 2.0.1 to 2.0.3 in /docs/source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mistune](https://github.com/lepture/mistune) from 2.0.1 to 2.0.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/lepture/mistune/releases">mistune's releases</a>.</em></p>
<blockquote>
<h2>Version 2.0.2</h2>
<p>Fix <code>escape_url </code> via <a href="https://github-redirect.dependabot.com/lepture/mistune/pull/295">lepture/mistune#295</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/lepture/mistune/blob/master/docs/changes.rst">mistune's changelog</a>.</em></p>
<blockquote>
<h2>Changelog</h2>
<p>Here is the full history of mistune v2.</p>
<p>Version 2.0.4</p>
<pre><code>
Released on Jul 15, 2022
<ul>
<li>Fix <code>url</code> plugin in <code>&amp;lt;a&amp;gt;</code> tag</li>
<li>Fix <code>*</code> formatting</li>
</ul>
<p>Version 2.0.3
</code></pre></p>
<p>Released on Jun 27, 2022</p>
<ul>
<li>Fix <code>table</code> plugin</li>
<li>Security fix for CVE-2022-34749</li>
</ul>
<p>Version 2.0.2</p>
<pre><code>
Released on Jan 14, 2022
<p>Fix <code>escape_url</code></p>
<p>Version 2.0.1
</code></pre></p>
<p>Released on Dec 30, 2021</p>
<p>XSS fix for image link syntax.</p>
<p>Version 2.0.0</p>
<pre><code>
Released on Dec 5, 2021
<p>This is the first non-alpha release of mistune v2.</p>
<p>Version 2.0.0rc1
</code></pre></p>
<p>Released on Feb 16, 2021</p>
<p>Version 2.0.0a6</p>
<pre><code>
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lepture/mistune/commit/3f422f1e84edae0f39756c45be453ecde534b755"><code>3f422f1</code></a> Version bump 2.0.3</li>
<li><a href="https://github.com/lepture/mistune/commit/a6d43215132fe4f3d93f8d7e90ba83b16a0838b2"><code>a6d4321</code></a> Fix asteris emphasis regex CVE-2022-34749</li>
<li><a href="https://github.com/lepture/mistune/commit/5638e460459cb59ceb20e4ce4716c802d4d73c53"><code>5638e46</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/lepture/mistune/issues/307">#307</a> from jieter/patch-1</li>
<li><a href="https://github.com/lepture/mistune/commit/0eba47196a81453bafe1f2492748a87475063dff"><code>0eba471</code></a> Fix typo in guide.rst</li>
<li><a href="https://github.com/lepture/mistune/commit/61e9337884e20f9f8fdc0b7788d319afdd259729"><code>61e9337</code></a> Fix table plugin</li>
<li><a href="https://github.com/lepture/mistune/commit/76dec68c4514c2612ef9263b49c6ec7f4d77bd14"><code>76dec68</code></a> Add documentation for renderer heading when TOC enabled</li>
<li><a href="https://github.com/lepture/mistune/commit/799cd118cc5e664b72e98410ce1b68645f1a38c0"><code>799cd11</code></a> Version bump 2.0.2</li>
<li><a href="https://github.com/lepture/mistune/commit/babb0cfa57a983ead615286a2b7c8f6885c46721"><code>babb0cf</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/lepture/mistune/issues/295">#295</a> from dairiki/bug.escape_url</li>
<li><a href="https://github.com/lepture/mistune/commit/fc2cd53d7698e432ab5b250ffac53458263a49e2"><code>fc2cd53</code></a> Make mistune.util.escape_url less aggressive</li>
<li>See full diff in <a href="https://github.com/lepture/mistune/compare/v2.0.1...v2.0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mistune&package-manager=pip&previous-version=2.0.1&new-version=2.0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 23:45:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2569" class=".btn">#2569</a>
            </td>
            <td>
                <b>
                    [feature] #2407: Parametrise triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
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

* Added event storing in `trigger::Set`
* `WorldStateView` now passes event from `trigger::Set` to `wasm::Runtime`
* `wasm::Runtime` was a little bit refactored and got a new function `execute_trigger()`
* Added `trigger_entrypoint` macro to `iroha_wasm` which accepts function with `event` parameter
* `mint_nft_for_every_user_smartcontract` was updated to use `trigger_entrypoint`

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2407
* After merging this PR we should discuss possibility to make event strongly typed

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* Now smartcontract writers can handle an event, that triggered thier smartcontract execution

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Events are not strong-typed. A top-level enum `Event` is used for now, which is not very handy.
I have some ideas, how to fix ths, but it needs further disscussion

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests 

1. Comment line **173** (`#[ignore = "Only on nightly"]`) in `client/tests/integration/triggers/time_triggers.rs`
2. Run
    ```bash
    cargo +nightly-2022-04-20 test --package iroha_client --test mod --integration::triggers::time_trigger::mint_nft_for_every_user_every_1_sec --exact --nocapture
    ```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 14:28:52 +0000 UTC
    </div>
</div>

