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
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Refactor test helper to explicitly pass config
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

- Currently, session.NewChForTet function sets the response timeout
  internally. Hence this value is not known to calling funcs in test.

- Refactor the func to take response timeout as an additional parameter.
  Because, the value is reaquired in tests for upcoming changes (#132).

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

Relates to #132.

#### Testing
<!-- Tell us how you have tested the changes. -->

No functional changes. All existing tests should pass.


#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-16 17:33:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Fix occasional failure in session.Test_Integ_Role
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

- The test case  Session_Close_NoForce_Error and
  OpenCh_Sub_Unsub_ChProposal_Respond_Accept in the mentioned test
  failed occasionally because of mismatch in channel IDs.

- Cause: Assumption (made in the tests) that GetChsInfo returns the
  channels in the order in which they were created is not always true.
  Because, GetChsInfo previously ranged over a map, in which case the
  elements are returned in random order during each iteration.

- Fix: Update the implementation of session, so that GetChsInfo returns
  the channels in the order in which they were created. Add a test case
  to document this behavior.

- Now, the assumption made in the test will always hold true (added a test case for this).

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

Bug Fix
<!-- Improvement -->
<!-- Implementation Task -->

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Fixes #179

#### Testing
<!-- Tell us how you have tested the changes. -->

Role integration test will be consistent. Will always pass (if implementation is correct) or always fail.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->


1. Run the newly added test that ensures channels Info returned by `GetChsInfo` is always in the same order - order in which the channels were created.

```
# In session directory
go test -run Test_ProposeCh_GetChsInfo/Test_ProposeCh_GetChsInfo
```
2. Start ganache-cli node in a different terminal

```
ganache-cli -b 1 --account="0x1fedd636dbc7e8d41a0622a2040b86fea8842cef9d4aa4c582aad00465b7acff,100000000000000000000" --account="0xb0309c60b4622d3071fad3e16c2ce4d0b1e7758316c187754f4dd0cfb44ceb33,100000000000000000000"
``` 

3. Run the role integration test in session package (previously failing test).
```
# In session directory
go test -cover -p 1 -count=1 -tags=integration  -v -run Role 
```

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 13:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Update test output format in circle ci config
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
- Previous output format (short-verbose aka testname) does not print
  sufficient info when a test is struck and eventual times out.

- Hence changing the format to standard-versbose. In this format,
  anything written by the program to stdout is also printed.

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

Closes #177 

#### Testing
<!-- Tell us how you have tested the changes. -->

This changes the output format for test in CI pipeline. The console window (in circle ci) for running the tests should now print all the log messages from the program. Also any test failure should also be printed as soon as it occurs.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 08:42:20 +0000 UTC
    </div>
</div>

