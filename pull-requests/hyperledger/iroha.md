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
                PR <a href="https://github.com/hyperledger/iroha/pull/1940" class=".btn">#1940</a>
            </td>
            <td>
                <b>
                    [fix] #1939: Proper features for `iroha_config_derive`.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Fixed improper feature flags. 

### Issue

Closes #1939 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Pass QA tests. 


### Possible Drawbacks

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 08:18:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1938" class=".btn">#1938</a>
            </td>
            <td>
                <b>
                    [ci]: fix failing tests.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description of change

Fixed failing CI pipelines in the `iroha2-dev` to `iroha2` merge pipeline. 

## Issue
None

## Benefits

Working CI pipeline

## Possible drawbacks 

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 07:10:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1937" class=".btn">#1937</a>
            </td>
            <td>
                <b>
                    RC2 Release PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                # Preview Release Candidate 2

## Overview of changes

- Migration to the actor framework
- Permission validation
- Triggers
- Telemetry: `status` endpoint and Prometheus `metrics` endpoint. 
- Multiple refactors. 
- …

The changelog can be found [here](https://github.com/hyperledger/iroha/pull/1937/files#diff-2c623f3c6a917be56c59d43279244996836262cb1e12d9d0786c9c49eef6b43c)

## Release checklist
- [ ] The crates have been version bumped.
- [ ] Iroha successfully passes all CI checks
- [ ] Iroha passed all QA tests
- [ ] Iroha lasted for five days at the longevity stand
- [ ] Standard benchmarks are ran and the results are recorded in the repository
- [ ] Iroha documentation and tutorial are up to date. 
- [ ] SDKs compiled successfully using the schema from latest branch (Hash: 9a149eecb00485f71fd23179dd16a73815d739b2)
  - [ ] Java
  - [ ] JavaScript
  - [ ] Swift
- [ ] All SDK tests pass
  - [ ] Java
  - [ ] JavaScript
  - [ ] Swift
- [ ] (Optional) SDKs implemented the main features added in the current release


## Comments 

This is the first timed release and the first merge into `iroha2` since July 2020. It includes changes made before and since RC1, and is the latest version of Iroha to be used. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 10:47:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1936" class=".btn">#1936</a>
            </td>
            <td>
                <b>
                    Testing workflow | should not be merged
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
Should not be merged, for testing purposes only 
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
        Created At 2022-02-27 23:58:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1935" class=".btn">#1935</a>
            </td>
            <td>
                <b>
                    Docs: Additions to 1.4 docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …eck endpoint, information about iroha-swarm tool

Signed-off-by: Sara G <lira.lemur@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Due to some git-related issues, this PR combines several PRs that would've conflicted or were not available anymore (fully my fault):
https://github.com/hyperledger/iroha/pull/1870 (yet unapproved) - Healthcheck Endpoint
https://github.com/hyperledger/iroha/pull/1741 (approved) - iroha-swarm added to docs
https://github.com/hyperledger/iroha/pull/1778 (approved) - build-fix
https://github.com/hyperledger/iroha/pull/1829 (approved) - RocksDB and Postgres comparison
https://github.com/hyperledger/iroha/pull/1850 (not fully approved) - good migration practice 

### Issue

Closes #1840
Closes #1834

### Benefits

More docs

### Possible Drawbacks

Sorry for combining these changes together


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 08:18:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1932" class=".btn">#1932</a>
            </td>
            <td>
                <b>
                    [ci] #1726: Re-introduce API tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>

### Description of the Change

Added a workflow that: 
1. Runs tests that used to be run by `test-docker`, checking for API compatibility between `iroha` and `iroha_client_cli`. 
2. Runs a benchmark. 
3. Runs an Iroha-java API-compatibility test.

This workflow triggers only when creating a release pull-request:  merging from `iroha2-dev` into `iroha2` (the "main" branch). 

### Issue
Closes #1726 

### Benefits

This is much-requested functionality that will help other SDK developers. 

### Possible Drawbacks
None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 07:53:45 +0000 UTC
    </div>
</div>

