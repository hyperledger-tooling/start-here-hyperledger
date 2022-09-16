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
                PR <a href="https://github.com/hyperledger/iroha/pull/2755" class=".btn">#2755</a>
            </td>
            <td>
                <b>
                    Feature/dops 1957/reduce ci runs
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
        Created At 2022-09-16 08:19:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2752" class=".btn">#2752</a>
            </td>
            <td>
                <b>
                    [ci]: Fix iroha2:dev-nightly image build
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
Add default git context execution to `build-push-action` Action.

### Issue
`iroha2:nightly` image could not be compiled due to the same error as `iroha2:dev` image had with the same workflow configuration.

### Benefits
Allow to build and publish `iroha2-nightly` image.

### Possible Drawbacks
None.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 18:57:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2749" class=".btn">#2749</a>
            </td>
            <td>
                <b>
                    Fix/gRPC drop stream bugfix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.5</span>
            </td>
            <td>
                ### Description of the Change
1. Remove timeout of gRPC deadline for stream.
2. Fixed logout crash.
3. Add reestablish YAC stream if previous send was failed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 07:27:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2743" class=".btn">#2743</a>
            </td>
            <td>
                <b>
                    [ci] #2732: Add a conditions to update iroha2-base images and add PR labels
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
1. Modify iroha2 CI in order to enable conditional step of `iroha2-base` image build if its `Dockerfile.base` has been changed.
2. Get back `I2::Dev::Label` workflow since we are able to apply the same approach as for `base-image` build.
3. Remove necessaries iroha2-dev-pr-label-config.yml` and `iroha2-dev-pr-label-api.yml` workflows files.

### Issue
Since `tj-actions/changed-files` and `dorny/paths-filter` Actions doesn't work within `hyperledger/iroha` repository, this is another one possible solution to resolve #2732.

### Benefits
1. Refactoring of iroha2 CI.
2. Reduce the amount of workflows files.

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 17:24:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2740" class=".btn">#2740</a>
            </td>
            <td>
                <b>
                    [ci]: Fix `buildx` error with `docker/build-push-action`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                <!-- [ci]: Fix `buildx` error with `docker/build-push-action` -->
### Description of the Change

- Apply [the diff](https://github.com/s8sato/iroha/commit/aade1ee304301c89d883926b41c33553025a110b) between [a reproduction](https://github.com/s8sato/iroha/actions/runs/3044140289/jobs/4904192521) and [a fix](https://github.com/s8sato/iroha/actions/runs/3044430691/jobs/4904811102) on my fork

### Issue

- https://github.com/hyperledger/iroha/actions/runs/3042899274/jobs/4902058622

### Benefits

- Publish `iroha2:<tag>` images

### Possible Drawbacks

- None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 11:20:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2739" class=".btn">#2739</a>
            </td>
            <td>
                <b>
                    Develop to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Iroha v1.6.0-hotfix-1

1. TransferAsset hotfix.
2. Check allowed symbols in cache before any transaction.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 05:42:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2736" class=".btn">#2736</a>
            </td>
            <td>
                <b>
                    [ci]: Version bump to RC.8
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
        Created At 2022-09-12 18:53:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2735" class=".btn">#2735</a>
            </td>
            <td>
                <b>
                    [fix] #2734: Remove logger config from client config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">UI</span>
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

- Removed logger config from Client config

#### Why remove?

AFAIK Rust libraries are [disallowed](https://crates.io/crates/log#usage) to activate logs by themself. Binaries should enable it. And user should decide if he want to run with logs and with which level of logs.

You can try to create a binary, import `iroha_client` and use something like [`env_logger`](https://crates.io/crates/env_logger) to enable logs. Then run your binary with `RUST_LOG=debug` env var. This will enable logs.

We don't have a lot of logs inside our `iroha_client` crate so that you won't see much of them, especially if you are not doing something. But in you can experiment with some methods or insert your logs in `iroha_client` crate manually to see, that it works.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

- Closes #2734

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

- No more useless config

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None

### LTS update?

I don't think, that this is an important fix. I just remove what does not work. I don't think we need a PR into `iroha2-lts`, but if you insist, I can do that
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 18:45:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2733" class=".btn">#2733</a>
            </td>
            <td>
                <b>
                    [ci]: First-aids for non-functioning `tj-actions/changed-files`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                <!-- [ci]: First-aids for non-functioning `tj-actions/changed-files` -->
### Description of the Change

1. Remove `if` condition to update `iroha2-base` images
2. Separate `I2::Dev::Label` jobs into workflows

### Issue

- Resolves https://github.com/hyperledger/iroha/pull/2680#issuecomment-1243492824

### Benefits

1. Publish images
2. The auto-labels works

### Possible Drawbacks

There should be a better way. This is just a stopgap for this release. Could you take over @BAStos525 ?
- Opens #2732

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 13:46:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2731" class=".btn">#2731</a>
            </td>
            <td>
                <b>
                    Fix/unkai unexpected symbol check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Handling of unexpected symbol in domain name.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 10:33:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2729" class=".btn">#2729</a>
            </td>
            <td>
                <b>
                    Merge main into develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Merge main into develop.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 07:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2728" class=".btn">#2728</a>
            </td>
            <td>
                <b>
                    [fix] #2703: Fix orillion dev env bugs (lts)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">LTS</span>
            </td>
            <td>
                ### Description

See details in #2724  -- dev-version of this commit

### Issue

* Closes #2703

### Tests

Tested manually. Using `Docker` to test locally and *Orillion dev environment* to test on remotely
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-11 23:27:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2724" class=".btn">#2724</a>
            </td>
            <td>
                <b>
                    [fix] #2703: Fix orillion dev env bugs (dev)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">Dev defect</span>
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

- Add TLS support for websockets
- Fix closing WebSocket bug

See also #2728   -- lts version of this PR

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2703 
* Opens #2725
* Opens #2726 
* Opens #2727

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Two bugs fixed and no more annoying `ERROR` log in Iroha saying about wrong web-socket closing

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

I had to remove timeout in client when listening to events. To bring it back properly we need more work to be done 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-11 22:50:26 +0000 UTC
    </div>
</div>

