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
                    [ci]/Update Dockerfiles & Codecov reports reuse & Concurrency
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
1. We need to update iroha2 ci process in order to improve it, make faster and get rid of some bottlenecks.
2. Codecov coverage reports takes so much time, so we have to try to reuse the same reports in the case if repository state is the same.
3. Pushing a new commits into branch doesn't stop previously running workflows and jobs,

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2423" class=".btn">#2423</a>
            </td>
            <td>
                <b>
                    [release]: 2.0.0-pre-rc.6-lts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Long-term supported release 

checklist: 
- [x] all CI checks pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 06:18:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2421" class=".btn">#2421</a>
            </td>
            <td>
                <b>
                    [fix] #2420: Fix "Permission already exists" bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
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

- `PermissonToken` now derives `PartialOrd` and `Ord`. Manual implementation that was using only token name used to cause collision and is the reason of the bug
- `PartialOrd` and `Ord` were derived for many other structs that `PermissionToken` depends on
- Added test to check this bug

### One more *dangerous* bug was found and fixed with the same changes

While fixing this bug I have also found another bug which this PR also fixes.
`PermissionToken` collision used to make it possible to i.e. have a permission to modify only one asset, but the same permission was enough to modify any other asset.
The test I introduced checks that too.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

- Closes #2420 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

- Permission collision bug fixed
- One more test

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 16:53:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2418" class=".btn">#2418</a>
            </td>
            <td>
                <b>
                    [feature] #1889: Add domain-scoped triggers (#2302)
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

The PR adds domain-scoped triggers that interact with entities within the same domain.

- [x] Add API
- [ ] Add restrictions to interaction with entities
- [x] Add docs, create an issue about `FindTriggersByDomainId` and a PR to `iroha2-docs`
- [ ] Add new `encode` command to the `parity_scale_decoder` 

### Issue

Resolves #1889 and #2302

### Benefits

Allows to create domain-scoped triggers.

### Possible Drawbacks

Seems none.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 07:45:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2417" class=".btn">#2417</a>
            </td>
            <td>
                <b>
                    [refactor] #2307: Make `events_sender` in `WorldStateView` non-optional
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

- Change `events_sender` in `WorldStateView` from `Option<EventsSender>` to `EventsSender`: this change is possible because previously `WorldStateView::with_events` was called single time during `Iroha` initialization just after `WorldStateView::from_configuration`. 
- Add `events_sender` parameter to `WorldStateView::from_configuration` constructor. 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2307.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Avoid overhead of checking if `events_sender` is `Some` with every call to `produce_event`.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

In `WorldStateView::new` fake `events_sender` is created, but since `new` called only in tests it should be fine.

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
        Created At 2022-06-30 07:25:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2415" class=".btn">#2415</a>
            </td>
            <td>
                <b>
                    [feature] #2395: Add panic if genesis cannot be applied
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

Raise panic if genesis contains invalid transactions.

Changes:

- Add function `validate_every` to `TransactionValidator` to validate slice of transactions;
- Add genesis transactions validity check to the `Iroha` constructor;
- Add test `scripts/tests/panic_on_invalid_jenesis.sh` to check that panic indeed invoked;
- Add test to `iroha2-pr` pipeline.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2395.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Early detection of problems associated with genesis.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

All instructions in genesis must be valid, impossible to have `FailBox` instruction for example.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

```
bash -c './scripts/tests/panic_on_invalid_genesis.sh' 
```
<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs

Correct type checking would make possible to detects invalid transactions during deserialization.

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
        Created At 2022-06-29 14:40:04 +0000 UTC
    </div>
</div>

