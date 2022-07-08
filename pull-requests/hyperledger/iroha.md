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
                PR <a href="https://github.com/hyperledger/iroha/pull/2453" class=".btn">#2453</a>
            </td>
            <td>
                <b>
                    [feature] #2098: Block header queries
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

Added queries for block headers.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#2098 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 12:21:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2452" class=".btn">#2452</a>
            </td>
            <td>
                <b>
                    [fix] #2416: Fix lints on macOS arm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ales Tsurko <ales.tsurko@gmail.com>

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
A cross-platform wrapper for `BlockValue` added to encapsulate platform dependent code. On macOS with arm architecture `Value::Block` inner is now boxed. 

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Closes #2416 

### Benefits

<!-- What benefits will be realized by the code change? -->
No more linter errors on M1.

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
As it's now a smart pointer, it requires dereferencing, when the inner value is needed.

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
        Created At 2022-07-07 10:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2448" class=".btn">#2448</a>
            </td>
            <td>
                <b>
                    [documentation] #2446: improve issue templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change

This PR adds detailed forms to fill into the issues. To see the issue form, open [this page](https://github.com/6r1d/iroha/issues/new/choose).

### Issue

This PR closes #2446 and covers all the items in it.

### Benefits

* Contributors sending the bug requests will fill the form with all the details that are needed for quicker debugging.
* The supported branches of Iroha are immediately visible.
* Contributors also see who to tag, so the issue gets resolved faster.
* People who have questions will immediately see Discord and Telegram community links.

### Possible Drawbacks

~~I have several questions I'll be marking as resolved here~~.
**UPD**: these questions were resolved.

- [x] I am not sure where to redirect people who have an SDK problem. In addition to that, it is possible to add a link to SDK in `/issues/new/choose`. This detail needs to be considered before the merge.
- [x] The [Discord server link](https://discord.gg/hyperledger) with `#iroha` channel shows a Telegram bridge and little activity. Is it the current actual Discord for Iroha?
- [x] The tags are auto-filled and need a change; I have not seen a `stable` tag, so both types of issues are tagged the same way, making it confusing.
- [x] This PR still has `blank_issues_enabled` as `true` for now. I think this will need a bit of a discussion: should we have blank issues in addition to the "bug" issues for questions, not related to bugs or future planning?
- [x] I am not sure if [this](https://hyperledger.github.io/iroha-2-docs/guide/configure/peer-configuration.html#logger) is the correct documentation link for JSON logs. While all the details match, is it the correct doc to refer to?

### Alternate Designs

At a later date, there may be an internal command to collect most of the current Iroha environment data: LibC version, OS info, etc. I am not sure if this can be done reliably all the time, so I am thinking of implementing this at a later date.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 05:31:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2447" class=".btn">#2447</a>
            </td>
            <td>
                <b>
                    [feature] #2454: Add a build script to the parity-scale-decoder tool
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

Add a build script that automatically updates sample binaries from sources in the parity-scale-decoder. This feature also fixes the broken test from #2418. 

### Issue

Resolves #2454 

### Benefits

Automatically updates sample binaries from sources.

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
        Created At 2022-07-06 17:21:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2445" class=".btn">#2445</a>
            </td>
            <td>
                <b>
                    [fix] #1480: Shut down on panic
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
Currently, when panic occurs, only the corresponding thread shuts down. But we need the whole program to shut down if a panic appeared on any thread. A panic hook is provided, which uses [`tokio::sync::Notify`](https://docs.rs/tokio/1.19.2/tokio/sync/struct.Notify.html) to gracefully shut down the program.

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

Fixes #1480 

### Benefits

<!-- What benefits will be realized by the code change? -->

The program will shut down gracefully if a panic occurs on any thread.

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
As we use globals (i.e. panic hook), it can affect tests in some cases. But the test environment should be close or same as the production one. Following contributors should have it in mind.

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

[A cargo config](https://doc.rust-lang.org/book/ch09-01-unrecoverable-errors-with-panic.html) or `std::process::exit` can be used instead, but that could leave garbage.

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 13:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2436" class=".btn">#2436</a>
            </td>
            <td>
                <b>
                    [refactor] #2369: Refactor permission validators
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

* Type returned by `IsAllowed` changed from `Result` to `ValidatorVerdict`
* `ValidatorVerdict` allows validators to skip checking if operation is unsuported or has no meaning for them
* Added `Judge` trait returning `Result`. Judge usually gather validators together to produce result based on verdicts from validators
* Removed `IsAllowedBoxed`. To be able to parse permissions from genesis we should introduce an enum`JudgeBoxed` in future. That's should be anough to deserialize.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2369 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* More readable error message
* More meaningfull validators system

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

* Very detailed error message. Maybe we should use `Display` instead of `Debug` for it

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 22:46:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2435" class=".btn">#2435</a>
            </td>
            <td>
                <b>
                    [fix] #2422: Hide private keys in configuration endpoint response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">macros</span>
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

- Add configuration-related to `data_model` to be able to share configuration;
- Fix `GetConfiguration` endpoint to return sharable configuration without private keys;
- Add proc macro to derive conversation between inner and sharable config. 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closses #2422.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

- No sensitive information are leaked;
- Opens possibility to share configuration between peers through Query (#1966);

### Possible Drawbacks

- Duplication configuration structs.
- Add dependency `iroha_data_model` to `telemetry` and `logger` crates.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Alternate Designs

Simpler solution would be to mask or hide private keys during serialization but this would affect generated reference configuration.
Add it still won't be possible to send config through queries.

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
        Created At 2022-07-05 14:23:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2433" class=".btn">#2433</a>
            </td>
            <td>
                <b>
                    [ci]: Update Dockerfiles & Codecov reports reuse & Concurrency
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

Signed-off-by: Vasilii Zyabkin [vzyabkin@soramitsu.co.jp](mailto:vzyabkin@soramitsu.co.jp)

### Description of the Change
1. Update iroha2 Dockerfiles for ci and switch to musl architecture for building processes.
2. Update workflows for new Dockerfiles.
3. Update jobs for codecov coverage reports generation.
4. Add concurrency feature to stop previous running merged & PR workflows after pushing a new commit.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
1. [x] We need to update iroha2 ci process in order to improve it, make faster and get rid of some bottlenecks.
2. [ ] Codecov coverage reports takes so much time, so we have to try to reuse the same reports in the case if repository state is the same.
3. [x] Pushing a new commits into branch doesn't stop previously running workflows and jobs,

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
1. Reduce the size of images, switch to alpine and Arch base images, increase the speed of building process.
2. Implement the process of iroha-2 CI the reuse of codecov reports for the same state of the repository for which GH Actions workflow is running.
3. Add `concurrency` Actions feature to stop previous running outdated workflows.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Some possibility of failing compilation on any building stages is possible.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 15:44:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2431" class=".btn">#2431</a>
            </td>
            <td>
                <b>
                    [feature] #2061: Derive macro for filters
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
To avoid having to update `Filter` structs manually each time `Events` are changed or vice versa, which is error-prone and tedious, have a derive procedural macro to do that instead, and also automatically generate `...Filter` structs, `...EventFilter` enums and their `impl Filter` methods.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Closes #2061.
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
* Greatly simplifies the `data_model/src/events/data/filters.rs` file, leaving only common types and `EntityFilter` there.
* Removes the need for unit testing on event fields exhaustiveness.
* Makes a step toward domain-oriented hierarchy of the data model instead of the functional one, which is what was agreed upon in discussion of its structure.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
The macro is dependent on the conventions that have been adopted in our codebase so far, such as events being enums and having only tuple fields with one member, the latter being either some `Id` or `Event`. Thus it might become very brittle should any of those assumptions change.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests
Codegen can be checked by putting the `data_model/.../events.rs` file into crate's `tests` folder and running `cargo expand --test events` on it (after fixing some imports).
<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs
The current design was selected upon comparison with the approach where filters would still be generated in the `filters.rs` file where they resided before. This option would require bringing the `Event` enum into scope somehow, and I found no other option besides reading the AST of the whole `events.rs` file, which would be *very* ugly. As @appetrosyan proposed, there could be some crates that would help with this, but in the end the current solution is cleaner, simpler and makes a lot of sense structurally.

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
        Created At 2022-07-04 12:53:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2428" class=".btn">#2428</a>
            </td>
            <td>
                <b>
                    [feature] #2228: Add Unauthorized variant to smartcontracts query error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                Closes #2228

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Added `iroha_core::smartcontracts::query::Error::Unauthorized` to better mirror semantics of unauthorized request (i.e. without an account in this case). Also, in case of querying without an account, **HTTP 401 UNAUTHORIZED** status is returned.

### Issue

Previously, in case of query without an account `FindError::Account` returned. And the corresponding **HTTP 404 NOT_FOUND** status code returned. That appeared to be semantically incorrect.

### Benefits

Now `POST /query` in case of request without an account returns `Error::Unauthorized` and **HTTP 401 UNAUTHORIZED** status code.

### Alternate Designs *[optional]*

At first glance, this can be moved to `Error::Permission` and the `Unauthorized` variant could be added to `DenialReason`, but it doesn't share semantics with **HTTP 401 UNAUTHORIZED** (it's **HTTP 403 FORBIDDEN** instead, [which is different](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/403)).
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
        Created At 2022-07-01 16:12:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2427" class=".btn">#2427</a>
            </td>
            <td>
                <b>
                    [ci] #2309: Re-enable doc tests in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
- b92a5858 Add doc tests to `tests_with_coverage` job
- f956b134, 4320aecd Fix doc tests
- 8bb2a4a8..c5646d3 Add tests with `--no-default-features` mainly for `no_std`

### Issue
- Closes #2309

### Benefits
1. CI can test the examples in the documentation, which have not been tested since #2223
2. CI can test the codebase with no default features, which has not been tested before

### Possible Drawbacks
1. Takes more CI time
2. Consumes 2 more runners
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 09:20:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2424" class=".btn">#2424</a>
            </td>
            <td>
                <b>
                    [ci]: Fix docker build
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

- Remove cargo chef
- Add workflow for LTS release
- Add `cargo deny` configuration

### Issue

Closes #2345 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 06:30:32 +0000 UTC
    </div>
</div>

