---
layout: default
title: perun-node
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-node
---

# perun-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Fix adjudicator event handling logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->
- In case of non-collaborative close, the concluded event is handled by
  the go-perun framework by making a new subscription for the event, in
  separate from the one used by watcher. Hence this event need not be
  handled by perun-node.
  Update the HandleAdjudicator function to ignore this event.

- In case of collaborative close, the register event is not received.
  Update the HandleAdjudicator function to ignore the event.

- Tests to check if channel close notifications are received properly
  already exist in "Test_Channel_Close".

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
Improvement
<!-- Implementation Task -->

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Closes #198.

#### Testing
<!-- Tell us how you have tested the changes. -->

Existing tests already check for the updated logic for handling adjudicator events.

It has been passing, because the additional scenarios that was handled before never occurred and hence were not causing any problem.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 12:22:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    Use new error type channel close notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->

- Settling a channel is handled in "HandleAdjudicator" function, when
registered / concluded events are received.
    
- Any error occuring during channel settle is passed to the user via
channel channel close notification. These errors can be related to
on-chain calls.
    
- Hence update this error to perun.APIError type to ensure user receives
proper error information in the same way as the other errors.
    
- Also, update cli and tui apps to handle this error.

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
Implementation Task

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Relates to #132.

#### Testing
<!-- Tell us how you have tested the changes. -->

`Test_channel_Close` is updated to tests if channel close notifications are received properly.

The update tests also check if watcher returns properly when a channel is closed.
Hence the `Test_HandleWatcherReturned` is now obselete and it is removed.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [ ] Name is added to the NOTICE file, if it is not present already.
- [ ] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 12:16:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Refactor test helper newMockPCh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->

- Currently, the test helper method sets up the response for "State"
method, which returns the same response on multiple calls.
    
- In some tests that are to be added, it is required to set this method
such that different responses are returned on consequent calls.
    
- Hence, modify the test helper to not set the response for State


##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
Implementation Task

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Relates to #132.

#### Testing
<!-- Tell us how you have tested the changes. -->

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 12:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Refactor by merging client & session pkg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->

- Functionality of client package is closely related to initialization
  of a session. This can also seen in duplication of many test cases in
  integration tests on client.NewEthereumPaymentClient & session.New.

- In implementing named errors (#132), a lot of errors in session init
  will have to be detected in NewEthereumPaymentClient function.

- Hence, to remove the duplication of test cases and for simpler error
  handling, these two packages are combined.

- Also some of the types defined in perun.go for tying these two
  packages together are also moved inside of session package

.##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
Implementation Task

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Relates to #132.

#### Testing
<!-- Tell us how you have tested the changes. -->

As a part of the refactor the tests in client package and session package have been combined.
Coverage should be the same and all existing tests should pass.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 08:29:24 +0000 UTC
    </div>
</div>

