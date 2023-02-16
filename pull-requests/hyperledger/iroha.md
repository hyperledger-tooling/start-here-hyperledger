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
                PR <a href="https://github.com/hyperledger/iroha/pull/3159" class=".btn">#3159</a>
            </td>
            <td>
                <b>
                    [ci] #2577, #2606: Make CI independent from 7272721/i2-ci & Push i2-d…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
1. Create a workflow to build and push `iroha2-ci:nightly-<>` image.
2. In `I2::Dev::Publish` substitute `on pull_request` trigger by `on workflow_run` trigger that allows to share Actions Secrets to push dev images before base branch merging.
3. Update some Actions versions.

### Issue
1. #2577  
2. #2606 

### Benefits
1. Covers #2577 issue.
2. Covers #2606 issue.

### Possible Drawbacks
We have to build and push `iroha2-ci:nightly-<>` image before to apply changes to `container: image` value. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 10:46:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3156" class=".btn">#3156</a>
            </td>
            <td>
                <b>
                    [fix] #3155: Fix panic-hook for tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">Tests</span><span class="chip">high-priority</span>
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

See #3155 for bug details.

To fix it I used [thread-local-panic-hook](https://crates.io/crates/thread-local-panic-hook) crate. It's not popular at all, but it solves our problem.

So when `test-network` feature is enabled I set thread local panic hook instead of basic panic hook (process local).

Also I removed useless invocation of previously set hook.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

- #3155 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Panic in one test won't cause Iroha shutdowns in another tests.

<!-- What benefits will be realized by the code change? -->

### Drawbacks

When `test-network` feature is activated all sub-threads (e.g. Sumeragi thread) won't have specified panic-hook. Instead they will have a default one.

I and @appetrosyan decided that this this acceptable because of this:

- Sumeragi and etc. are designed to not panic because of client actions
- It works normally right now
- There will be no new integration tests in future. They will be rewritten in Python
- After rewriting tests this change will be rollbacked

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

Don't know how to prove that it fixes the problem. But it works for me in #3106 .

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs

There is an idea how to fix this problem with sub-threads but it doesn't worth implementation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 11:48:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3149" class=".btn">#3149</a>
            </td>
            <td>
                <b>
                    [fix] #3141: Manually implement `IntoSchema` for `Hash`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
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

Manually implement `IntoSchema` for `Hash`, to correctly serialize data on SDK side.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #3141.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Work on SDK side.

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
        Created At 2023-02-14 08:47:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3148" class=".btn">#3148</a>
            </td>
            <td>
                <b>
                    Fix in iroha-cpp library + added example of few transactions (HL branch -> develop)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">1.x</span><span class="chip">CLI</span><span class="chip">1.5</span><span class="chip">queries</span>
            </td>
            <td>
                Signed-off-by: Grzegorz Bazior <g.bazior@yodiss.pl>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
I noticed that in examples queries were not working - after some time of investigation I noticed that `counter` must be greated than 0, but default  value is 0. So I changed into 1. Also I added another example file with error checking (it was my first time with GRPC in C++ so there can be errors)

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Good example for somebody who wants to start developing Iroha 1 with iroha-cpp-lib + fix
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
I don't know what `counter` is:D.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*
```
make irohalib_domainassetcreation_example
```
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
        Created At 2023-02-14 07:46:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3142" class=".btn">#3142</a>
            </td>
            <td>
                <b>
                    [ci]: Upload i2-dev image tag to Soramitsu Harbor
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
Enable `iroha2-dev` image uploading  to Soramitsu images registry.

### Issue
Some time ago we did the same thing for `stable&lts` tags: #3049. Now we have a need to upload the `dev` tag as well. 

### Benefits

We will have the opportunity to test the freshest iroha2 features like #3120 within k8s deployment and do not encounter pulling limitation on DockerHub.

### Possible Drawbacks
None.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 20:31:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3140" class=".btn">#3140</a>
            </td>
            <td>
                <b>
                    [documentation]: Generate CHANGELOG for pre-rc.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

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
        Created At 2023-02-10 09:24:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3138" class=".btn">#3138</a>
            </td>
            <td>
                <b>
                    [refactor]: Remove `iroha_client` dependency on `iroha_core`
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

- `ISI` and `Query` errors are moved into `iroha_data_model`
- `AcceptedTransaction` moved into `iroha_data_model`
- `*Block` structures moved into `iroha_data_model`
- Dependency of `iroha_client` on `iroha_core` is removed (only `dev-dependency` now)
 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Resolves #3128.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

More clear design.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

A bit more code due to introduction on `Ext` traits.

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
        Created At 2023-02-10 08:14:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3134" class=".btn">#3134</a>
            </td>
            <td>
                <b>
                    Iroha v2.0.0-pre-rc.13 release PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Release checklist

- [x] All crates have been bumped to the correct versions
- [x] Changelog generated @outoftardis 
- [ ] Java SDK updated @arndey 
- [ ] Java SDK tests pass @arndey 
- [ ] shell tests pass @appetrosyan 
- [ ] Flakyness check @appetrosyan 
- [ ] Benchmarks on distributed system matching internal project deployment @astrokov7 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 18:57:36 +0000 UTC
    </div>
</div>

