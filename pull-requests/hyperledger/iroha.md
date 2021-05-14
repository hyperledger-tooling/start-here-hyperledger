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
                PR <a href="https://github.com/hyperledger/iroha/pull/1016" class=".btn">#1016</a>
            </td>
            <td>
                <b>
                    Telemetry futures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                https://jira.hyperledger.org/browse/IR-1096
https://jira.hyperledger.org/browse/IR-1097

### Description of the Change

Pr adds telemetry for futures, macro for wrapping them and tools for analyzing data:
- Number of polls
- Their time

### Benefits

It will help to see outliers and blocking async functions (which are not desired at all) and opens opportunities for analysis in ci.

### Possible Drawbacks 

Slower runtime and more used memory/

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 14:57:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1013" class=".btn">#1013</a>
            </td>
            <td>
                <b>
                    Feature/rdb commands executor
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
Adds rocksdb command executor.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 19:23:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1012" class=".btn">#1012</a>
            </td>
            <td>
                <b>
                    FlatFile: close file before rename
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrei Lebedev <lebdron@gmail.com>

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

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 14:10:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1011" class=".btn">#1011</a>
            </td>
            <td>
                <b>
                    Feature/proposal creation timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Replace round delay with proposal creation timeout
- Send batches to current and next rounds
- Decouple Yac and OnDemandOrdering from rxcpp
- Asynchronous proposal request
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 13:27:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1010" class=".btn">#1010</a>
            </td>
            <td>
                <b>
                    Spawn blocking CPU intensive tasks in separate threads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Egor Ivkov <e.o.ivkov@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Spawn blocking CPU intensive tasks in separate threads, where it is impossible yeild control manually to executor, to give other tasks chance to run.

Also adds several corrections in tests, they were initially mistakenly rewritten, so this PR reverts these things.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits
Should reduce the possibility of starvation in async tasks.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 
Code complexity increases.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Jira Issue
https://jira.hyperledger.org/browse/IR-1094

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 10:24:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1009" class=".btn">#1009</a>
            </td>
            <td>
                <b>
                    Use unique_port and cargo-lints from crates.io
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Egor Ivkov <e.o.ivkov@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Use unique_port and cargo-lints from crates.io instead of github links to master branch. This can be done as we finally published the first version of these crates.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits
Standard versioning.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 
None found.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 12:57:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1008" class=".btn">#1008</a>
            </td>
            <td>
                <b>
                    Add simple actor framework
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                https://jira.hyperledger.org/browse/IR-1092
https://jira.hyperledger.org/browse/IR-1093
Signed-off-by: i1i1 <vanyarybin1@live.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

This commit adds actor framework message broker for actors.

### Benefits

Using actor framework can benefit architecture by clearing relationships between actors a lot.

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

Look at doc tests and tests

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 15:29:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1007" class=".btn">#1007</a>
            </td>
            <td>
                <b>
                    Add nice panic and error reporters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                https://jira.hyperledger.org/browse/IR-1019
Signed-off-by: i1i1 <vanyarybin1@live.ru>

### Description of the Change

Add panic handler with stacktrace and error reporting. Add error reporter for `iroha_error::Error`. Now it can be nicely formatted  everywhere if needed.

### Benefits

More context where needed on errors.

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-08 13:16:29 +0000 UTC
    </div>
</div>

