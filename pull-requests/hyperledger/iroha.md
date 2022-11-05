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
                PR <a href="https://github.com/hyperledger/iroha/pull/2935" class=".btn">#2935</a>
            </td>
            <td>
                <b>
                    Added more descriptive Readme file.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Documentation</span><span class="chip">1.5</span>
            </td>
            <td>
                Describe how Hyperledger Iroha C++ library works. Provide examples. Show how to install and use current version of library.
Show how to run examples with transactions, batch and commands.

Benefits:
End user will know what is library responsible for and how to use it properly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-05 12:36:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2934" class=".btn">#2934</a>
            </td>
            <td>
                <b>
                    [ci]: Switсh dev tests to Equinix self-hosted runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
1. Substitute default GitHub Actions runners with the `self-hosted` demand persistent instances _[s(1-4)-dev-iroha2-iroha-tech]_ with the following characteristics:
- CPU: 1 x Intel(R) Xeon(R) E-2278G
- RAM: 32 Gb
- Drive: 2 x 500 Gb
- OS: Ubuntu 22.04 LTS

For the following CI test jobs into `I2::Dev::Tests` workflow:
- check
- with_coverage
- integration
- unstable

2. Update links to `load-rs` CI.

### Issue
1. A long and heavy jobs from iroha2 CI take too much time on the default GitHub Actions runners.
2. Wrong configuration to call `load-rs` image compiltation.

### Benefits
1. Increase the speed, effectiveness and reliability of the heavy parts of iroha2 CI.
2. Fix `load-rs` CI trigger.

### Possible Drawbacks
1. Using a `self-hosted` runners, especially demand instanes, for PR trigger workflows for open repositories is not a good practice: theoretically someone could execute malicious and undesirable code from his fork as PR's code. This requires being attentive and careful.
3. According to GitHub Actions setting, `self-hosted` runner can execute only one job from single workflow per unit of time. We added four instances for now, that means they can execute for jobs in the same time. May be we can try to this `self-hosted` runners to job that builds `iroha2-dev` image as well. Perhaps we can several instances more if it will be useful in the future.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 19:51:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2930" class=".btn">#2930</a>
            </td>
            <td>
                <b>
                    [refactor]: move parametrization into traits and remove FFI IR types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Marin Veršić <marin.versic101@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

* simplified conversion process

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* less code
* easier to understand

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
        Created At 2022-11-03 06:29:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2929" class=".btn">#2929</a>
            </td>
            <td>
                <b>
                    [feature] #2905: Extend arithmetic operations to support `AssetValue` 
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

Extend arithmetic operations to support `AssetValue`  instead of only `u32`.

### Issue

Closes #2905.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Arithmetic instructions support more types.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None.

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
        Created At 2022-11-01 14:28:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2928" class=".btn">#2928</a>
            </td>
            <td>
                <b>
                    [feature] #2899, #2508: Add multi-instructions and wasm subcommands into 'client_cli'
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

Merge changes from #2898 and #2918 into LTS.

### Issue

Close #2899 and #2508

### Benefits

Add a couple of subcommands into the LTS branch.

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-01 14:02:00 +0000 UTC
    </div>
</div>

