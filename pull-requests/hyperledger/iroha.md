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
                PR <a href="https://github.com/hyperledger/iroha/pull/2115" class=".btn">#2115</a>
            </td>
            <td>
                <b>
                    [schema] #2114: Sorted collections support in schemas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span>
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

* define stable schema type names
* introduce sorted collections to schemas

Considering that we make abundant use of digital signatures, serialized formats of our internal structures must have a defined ordering, e.g. `BTreeMap` must be represented as a sorted vector of tuples. While it may be possible that there will be `BTreeMap`s that won't be part of a structure that is signed(and require a defined ordering of tuples), I find it to be quite unlikely and don't think it worth to support such exception.

### Issue

Closes #2114 

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2022-04-17 14:25:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2110" class=".btn">#2110</a>
            </td>
            <td>
                <b>
                    [refactor] #2109: Make `integration::events::pipeline` test stable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
Refactored.

### Issue
- Closes #2109

### Benefits
- Stable test result
- Shorter CI time

### Possible Drawbacks
None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-16 11:48:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2107" class=".btn">#2107</a>
            </td>
            <td>
                <b>
                    [feature] #2108: Add pagination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: BAStos525 <66615487+BAStos525@users.noreply.github.com><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Add pagination support for SDKs. 

### Issue

Closes #2108 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Pagination added to queries, so that SDKs have access to the Pagination struct. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 09:50:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2104" class=".btn">#2104</a>
            </td>
            <td>
                <b>
                    [fix] #1640: Generate `genesis.json` and consolidate generation into one tool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span><span class="chip">Refactor</span>
            </td>
            <td>
                ### Description of the Change

Can now use `iroha_docs` binary to generate sample `genesis.json`

### Issue
Closes #1640 
Relates to #1992


<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Can now generate and check if the `genesis.json` needs updating. 

### Possible Drawbacks

None

### Usage Examples or Tests *[optional]*

```
cargo run --bin iroha_docs -- --genesis > /tmp/genesis.json && diff /tmp/genesis.json  configs/peer/genesis.json
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 13:27:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2095" class=".btn">#2095</a>
            </td>
            <td>
                <b>
                    [fix] #2005: Fix `Client::listen_for_events()` not closing WebSocket stream
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

* Fix `Client::listen_for_events()` not closing WebSocket stream
* Fix `torii` doing only part of WebSocket handshake

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2005

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now event streaming satisfies WebSocket protocol

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 12:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2082" class=".btn">#2082</a>
            </td>
            <td>
                <b>
                    [skip ci] Retire inactive maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Last activity:
2019/07/24 06:25:12 issue_comment.update bakhtin
2018/12/11 14:07:33 issue_comment.update grimadas
2019/12/25 14:09:13 repository_vulnerability_alert.resolve igor-egorov
2019/01/16 12:36:58 issue_comment.update l4l
2018/09/25 11:34:38 issue_comment.update laSinteZ
2018/02/16 15:38:38 issue_comment.update luckychess
2018/07/19 16:06:05 issue_comment.destroy muratovv
2019/02/20 10:16:17 issue_comment.update neewy
2018/12/21 14:47:14 issue_comment.destroy nickaleks
2018/05/03 04:59:54 issue_comment.update Solonets
2018/07/10 13:27:31 issue_comment.update stinger112
2018/06/29 18:16:18 issue_comment.update tyvision
2018/03/20 14:42:37 issue_comment.update victordrobny
2018/03/27 10:07:33 issue_comment.update x3medima17
2017/06/28 05:35:19 org.oauth_app_access_requested yannoban

Signed-off-by: Ry Jones <ry@linux.com>

### Description of the Change

Retire inactive maintainers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 21:46:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2080" class=".btn">#2080</a>
            </td>
            <td>
                <b>
                    [feature] #2003: Introduce Parity Scale Decoder tool (stable implementation)
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

## Caution!!!

This is the alternative implementation of #2079 . Only one of them should be accepted in the end

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Added the same tool as in #2079 but with alternative design and implementation. Every type is hardoced now.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2003 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits over #2079 

* Should work everywhere and forever
* Much less code
* Supported types are predictable

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

* Every new type should be added mannualy in this tool source code

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 14:54:23 +0000 UTC
    </div>
</div>

