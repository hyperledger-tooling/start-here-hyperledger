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
                PR <a href="https://github.com/hyperledger/iroha/pull/3291" class=".btn">#3291</a>
            </td>
            <td>
                <b>
                    [ci]: Use pull_request_target trigger for I2::Dev::Publish workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
1. Change `I2::Dev::Publish` workflow trigger from `pull_request` to `pull_request_target`.
2. Remove unnecessary workflow permissions.

### Issue
`permissions: pull-requests: read` probably won't help to share the secret. `write` permission for PR will not work according to the GH Actions documentation. `on: workflow_run` trigger could be used, but this trigger only works on the default branch, which iroha2-dev is not. And if we put it in the default `main` branch, then the context is read from there.

### Benefits
Make "workflow to check that the docker containers are properly buildable" to be working.

### Possible Drawbacks
`pull_request_target` trigger is not so safe and base-repository permissions limited. It allows to have much more permissions for forks. But we have the policy about outside collaborators PRs limitation, so this should mitigate the potential risks of using this workflow trigger.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 09:51:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3290" class=".btn">#3290</a>
            </td>
            <td>
                <b>
                    [refactor] #3232: Share workspace metadata
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

* replace `anyhow` with `eyre`
* use workspace package inheritance

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

Closes #3285 #3232

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
        Created At 2023-03-08 10:51:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3288" class=".btn">#3288</a>
            </td>
            <td>
                <b>
                    [ci]: Add Jenkinsfile for i2-PR-image k8s deployment generator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
Add `Jenkinsfile` to connect iroha2 CI `iroha2:pr` building with this image Kubernetes deployment from Soramitsu private Jenkins library.

### Issue
Sometimes we need to have an opportunity to deploy iroha2 image from Pull Request branch before merging to the base branch to confirm that it's workable.


### Benefits
For the particular PRs we will able to deploy this PR-image on the fly and quickly test it if it works as expected.

### Usage
1. It will work only if the PR comes from branch inside `hyperledger/iroha` repository. Work with PRs from forks is impossible.
2. To run this job trigger, you should add `experimental_environment` label to your PR.

### Possible Drawbacks
Actually nothing from GH Actions iroha2 CI process. Only outside PR-deployment Jenkins job could not work.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 18:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3287" class=".btn">#3287</a>
            </td>
            <td>
                <b>
                    [refactor] #3226: Extract `iroha_wasm_validator` crate from `iroha_wasm`
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

- Updated version of `iroha_wasm`
- Created `iroha_derive_primitives`
- Created `iroha_wasm_validator`

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes:

- #3226 
- #3285 
- #3286
- #3292 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Code which is useful only for *Validators* will not be compiled for other things like *Triggers* and *Smart contracts*

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Can't see any

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 12:20:49 +0000 UTC
    </div>
</div>

