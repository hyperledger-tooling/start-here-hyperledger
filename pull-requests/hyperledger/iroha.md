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
                PR <a href="https://github.com/hyperledger/iroha/pull/2389" class=".btn">#2389</a>
            </td>
            <td>
                <b>
                    #2008: Interning of common objects
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
Tried adding internment inside `new()` methods of `data_model/src/account.rs` and `data_model/src/asset.rs`. Also added a new example to the `client` crate that would supposedly showcase interning better, with two domains having 500_000 accounts each. For note, the traces given in the last section were produced on a slightly smaller example of 300_000 accounts each.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->
Work in progress towards #2008.
<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
The only positive thing that I was able to track is a very slightly reduced number of calls to allocation functions, down from 1.22 billion to about 1.18 billion. The distribution of allocation sizes also changed slightly, with the internment case seeing an increase in mid-sized allocations (9 to 64 bytes), and a decrease in allocations <= 8B or within 65-256B range.

A smaller feature worthy of attention is that the memory consumed graph in the internment case has a small dip around 6 minute mark (probably connected to the fact that the two domains are created first, and only then they are populated with accounts), whereas no internment case just grows linearly from the start until both of them peak off around 1h40m and plunge (I suppose this marks hash verification stage).
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
The actual performance seems to have degraded a bit, with a heap memory overhead max increased by about 4 Mb, from ~85 to 89 Mb.

It could also easily be the case that I'm just doing it wrong. The `internment` crate returns a `&'static T`, and as `Id` methods require ownership (otherwise I believe the refactoring would take up too many of the codebase, introducing lifetimes and drastically increasing complexity), there is inadvertent cloning involved even when the object is present in the intern, which definitely takes its toll. I couldn't come up with any strategy to circumvent that, so feedback would be appreciated.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests
The below traces were produced for use with [heaptrack](https://github.com/KDE/heaptrack), which gives flamegraphs to diagnose allocations or memory usage and provides a few other helpful visualizations compared to valgrind's massif. However, I've struggled with making actionable conclusions out of the differences produced between the cases. The links will die in 24 hours, so I'll update them after that should need arise.

Trace of `two_domains_million_accounts_tx.rs` with internment: [link](https://wormhole.app/lPAl1#B7wit4sFt_o7q06CT6zj1Q)
Same example, but without: [link](https://wormhole.app/ApZoO#X6iqIXJBk6sjO-b5Jp61LQ)
<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs
Another crate allowing internment of any structures is [hashconsing](https://docs.rs/hashconsing/latest/hashconsing/index.html). It makes use of a lazy static `RWLock`-wrapped `HashSet` or `HashMap`, with the consigned terms each put into `Arc`. The `internment` crate also has other options for the strategy, such as arena or arc internment. Neither of those were tested properly yet.
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
        Created At 2022-06-23 07:56:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2387" class=".btn">#2387</a>
            </td>
            <td>
                <b>
                    Feature/db cache multi layer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Multilayer DB cache.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 13:59:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2383" class=".btn">#2383</a>
            </td>
            <td>
                <b>
                    [feature] #2053: Add tests to all remaining queries in private blockchain
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

Add tests to all remaining queries in the private blockchain module. Finally closes the #2053 issue.

### Issue

Resolves #2053 

### Benefits

More tests, more coverage.

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
        Created At 2022-06-21 22:44:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2382" class=".btn">#2382</a>
            </td>
            <td>
                <b>
                    [feature] #1827: Parametrize hashes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                TBD

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
        Created At 2022-06-21 21:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2378" class=".btn">#2378</a>
            </td>
            <td>
                <b>
                    [feature] #2127: Add sanity check to ensure that all data decoded by `parity_scale_codec` is consumed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Security</span>
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

* Added `decode_all_versioned()` that works like  [`decode_all()`](https://docs.rs/parity-scale-codec/2.3.1/parity_scale_codec/trait.DecodeAll.html#tymethod.decode_all) from `parity_scale_codec`
* `decode_all()` and `decode_all_versioned()` were used in some places where `decode()` and `decode_versioned()` were used before. It wasn't replaced in all places, cause we have to do it only on high decoding level (i.e. receiving message from client, reading *kura* block and etc.)
* To not to introduce new errors for *SDK*-developres all usage of `_all*`-functions mentioned above check for error, print warning and call for not-`all` analogue

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2127

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* Checked that Iroha peers and client communicate without extra bytes in messages
* *SDK*-developers will get warning message if they send extra-bytes. In future we can return error

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

* In the future there can be another place there decoding will be done. If someone will forget to use `_all*` version of function then it's only possible to track it on review. No code checks we can done with this approach
* I may missed some places where `decode()` (or `decode_versioned()`) should be replaced with `decode_all()` (or `decode_all_versioned()`)

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

I've inserted `panic!` in `decode_all_versioned()` impl in `impl_decode_versioned()` and in other places where just `parity_scale_codec::decode()` was used. After that I've ran our tests. Nothing has failed. Seems like our internal communication works fine 

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs

At first I was trying to implement my own procedural *derive* macro so that `decode` implementation would check if all bytes were consumed. I was thinking that it's better to make this check permanent and undependent from external usage. So that there will be no way to make a mistake in the future.
But another problem occurred: it only works for high level structures. If some structure can be decoded by it's own and at the same time as a part of another strucutre -- this approach fails. So I decided not no use this macro and find another way. That's why there is `2` in my branch name.

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
        Created At 2022-06-20 20:42:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2377" class=".btn">#2377</a>
            </td>
            <td>
                <b>
                    Develop
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
Fix PR check issues
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Pull request https://github.com/hyperledger/iroha/pull/2372 was stuck
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
        Created At 2022-06-20 16:59:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2375" class=".btn">#2375</a>
            </td>
            <td>
                <b>
                    Fix status checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: safinsaf <safinsaft@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Removed path-ignore for both iroha1 workflows, as some checks are obligatory in branch protection rules

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Pull request https://github.com/hyperledger/iroha/pull/2372 was stuck  

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
        Created At 2022-06-20 09:35:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2374" class=".btn">#2374</a>
            </td>
            <td>
                <b>
                    [feature] #2053: Add tests to the asset-related queries in private blockchain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">2.0.0-pre-rc.5-lts</span>
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

Add tests to the asset-related queries in private blockchain. 

### Issue

Partially resolves #2053 .

### Benefits

New tests.

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
        Created At 2022-06-19 22:33:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2372" class=".btn">#2372</a>
            </td>
            <td>
                <b>
                    Docs: iroha-swarm Description + Deploy docs Fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sara <lira.lemur@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Added description to iroha-swarm and fixed some issues with Deploy part of the docs

### Issue

Request by @kuvadldini

### Benefits

Better docs. 

### Possible Drawbacks
None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 00:52:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2371" class=".btn">#2371</a>
            </td>
            <td>
                <b>
                    [fix] #2081: Fix role granting bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">2.0.0-pre-rc.5-lts</span>
            </td>
            <td>
                ### Bug description

Our `IsGrantAllowed` validators was checking only for *permissions* and not for *roles* granting. This validators return `Err` if got something unexpected. That's why SDK-developers test was failing.

Our integration tests was using `AllowAll` for instruction validation by default. That's why test introduced in #2312 haven't fully covered real world scenario.

### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

* Fixed bug with granting role. Before that it was only possible to grant permissions
* Default instructions validator for integration tests was replaced with `default_permissions()`. This will reduce the gap between our integration tests and SDK-developers tests
* `Role` registration process was unified with other things registration such as `Domain` and `Account`
* Add more `const` to some functions

### Issue

* Closes #2081 
* Opens and closes #2381
* Opens #2368
* Opens #2369
* Opens #2370

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* Closed bug request
* Now it's possible to grant roles with `default_permissions()`, not only permissions
* More consistency with SDK-developers test

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Now tests by default are sensitive for instructions and signer (`alice@wonderland` right now). I.e. it's illegal now to mint roses, because noone can mint assets that was registered by another account.
This can be bypassed by setting custom validators. Example:

```rust
let (_rt, _peer, mut test_client) = <PeerBuilder>::new()
    .with_instruction_validator(AllowAll)
    .start_with_runtime();
```

But be carefull, because this is not how `Iroha 2` works by default. This may introduce inconsistency between our and SDK-developers tests.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-18 15:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2367" class=".btn">#2367</a>
            </td>
            <td>
                <b>
                    [ci] #1658: Add documentation check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Sorry for omitting the PR template here, but the change is very little and clear. It just adds  documentation check (using `cargo doc`) to CI.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 21:55:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2366" class=".btn">#2366</a>
            </td>
            <td>
                <b>
                    Fix/single send state creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Minor optimization
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 15:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2365" class=".btn">#2365</a>
            </td>
            <td>
                <b>
                    [refactor] #1985: Reduce size of `Name` struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Optimization</span><span class="chip">Unsafe</span>
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

- Add `ConstString`: immutable, inlinable string, which uses `union` internally to store boxed and inlined variants in the same space;
- Replace `String` with `ConstString` in `Name` struct.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #1985.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

All structs that uses `Name` take up less space.
We win at least one machine word for every instance of `Name` and up to 23 byte for strings 15 bytes long on 64-bit architecture, also strings shorter than 15 bytes are stored on the stack, which avoids allocation.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

`ConstString` uses `unsafe` code, which increases the risk of bugs and vulnerabilities.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

Run unit tests:
```
cargo test --package iroha_data_primitives --lib -- conststr::tests --nocapture
```

Run unit tests with miri to find leaks and UB:
```
cargo +nightly-2022-04-20 miri test --package iroha_data_primitives --lib -- conststr::tests --nocapture
```

### Alternate Designs

It possible to use enum instead of union to avoid `unsafe`, but it take 24 bytes instead of 16, [see](https://play.rust-lang.org/?version=stable&mode=debug&edition=2021&gist=a28c4bfc22d99f5808638dcc82c46553).

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 15:36:20 +0000 UTC
    </div>
</div>

