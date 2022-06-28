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
                PR <a href="https://github.com/hyperledger/iroha/pull/2403" class=".btn">#2403</a>
            </td>
            <td>
                <b>
                    [feature] #2000: Disallow empty names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                This PR disallows to use empty strings for `iroha_data_model::Name`. Thus, it forbids empty `AccountId`, `DomainId` etc. In case of `Name`'s initialization from an empty string, an error is raised. For discussion see the linked issue (#2000).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 12:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2401" class=".btn">#2401</a>
            </td>
            <td>
                <b>
                    [fix] #1649: remove `spawn` from `do_send`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
Deadlock described in #1649 is no longer reproducible. Tested under load for about an hour, periodically restarting and re-regestering peers.

### Issue

Closes #1649 

### Benefits

Performance

### Possible Drawbacks

None (if deadlock really is gone)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 11:29:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2397" class=".btn">#2397</a>
            </td>
            <td>
                <b>
                    [fix] #2376: Simplified Kura, no async, two files
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

Removes most of the async from kura. Revamps the way blocks are stored on filesystem to a two file design. All communication *into* kura is composed of simple function calls.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#2376 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

The code and design  are a lot better. They will allow easier development.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 17:27:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2394" class=".btn">#2394</a>
            </td>
            <td>
                <b>
                    [ci] #2393: Bump the version of the Docker base image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
Version bump, which fixes the build failure. This is a stopgap until #2278 is merged

### Issue
- Closes #2393

### Benefits
- Docker can build

### Possible Drawbacks
- None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 12:53:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2390" class=".btn">#2390</a>
            </td>
            <td>
                <b>
                    [feature] #2360: Make `genesis.json` optional again
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
Pretty much wrapping `GenesisConfiguration` from `cli` crate into an `Option` to allow peer startup without a `genesis.json` if they're not submitting genesis.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Resolves #2360 .
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
More flexibility with deployment.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Slightly wordier initialization of all the related structs, as we have to wrap in `Some`.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

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
        Created At 2022-06-23 14:01:59 +0000 UTC
    </div>
</div>

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

