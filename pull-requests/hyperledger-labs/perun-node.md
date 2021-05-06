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
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    Refactor tests to use assertion helpers
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

- Assertion helper functions for tests in session package was added when
  updating OpenCh method to use new error type.

- Use those helper functions in tests for methods that were previously
  updated to use the new error type.

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

Should be merged only after #172, #173, #175, #150.

#### Testing
<!-- Tell us how you have tested the changes. -->

Does not modify any functionality. All existing tests should pass.

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
        Created At 2021-05-06 09:21:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    Fix bug in unknown internal error
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

- Previously the error category was wrongly defined as Client Error.
  Change this to Internal Error.

- Remove the use of "unknown internal error" in AddPeerID, GetSessionV2
  and GetChV2. Because errors in each of these APIs must be one of the
  named errors and cannot be an "unknown internal error".

- Though the constructor is not used anywhere except in tests, it is
  still retained, as it will be required later (when updating other APIs
  such as OpenCh to use the new error type.


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

Closes #174.

Should be merged only after #172, #173.

#### Testing
<!-- Tell us how you have tested the changes. -->

The fix is not covered by tests, as the function is not used anywhere and will only be used later.
The function is retained for the reasons described in the description.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. View line 117 in `errorsV2.go`. 


#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 09:02:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    132 update error codes
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
Update error codes for the new error type

- Removed  "Insufficient balance for tx" and "Insufficient balance for
deposit". These errors cannot be identified in the framework and will
be treated as "Tx timed out" error.
    
- Reorganized the error codes after removing these errors.
    
- Renamed "chain node not reachable" to "cannot connect to chain" as it
represents error connecting to chain during node/session init.
    
- Renamed "chain node disconnected" to "chain not reachable" as it
represents a error reaching to an already connected chain node.
      
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

Should be merged ony after #172.

#### Testing
<!-- Tell us how you have tested the changes. -->

Updated error codes should be consistent with the ones defined in [updated issue description](https://github.com/hyperledger-labs/perun-node/issues/132#issuecomment-744280220). Also the below tests should pass.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. Test the correct mapping of error codes in go-perun to the error codes in gRPC adapter for user API.
```
go test -count=1 ./api/grpc -run Test_ErrorCode
```

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 07:28:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    Update go-perun dependency to 0fe85e7
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
- This version contains named errors (chainNotReachable, txTimedOut and
  peerRejectedItem). These are needed in upcoming changes related to
  named error described issue #132.

Additionally, in the updated version of go-perun

- Dependencies have been updated to later versions.

- HandleUpdate callback has an additional parameter - "current state".
  This change removes the necessity to store the "current state" in the
  "channel struct" in session package. Hence, session package is updated
  to use the variable passed in callback; and remove the "currState"
  field from "channel struct".
  
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

All existing tests should pass.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. Run ganache-cli in one terminal.
```
ganache-cli -b 1 --account="0x1fedd636dbc7e8d41a0622a2040b86fea8842cef9d4aa4c582aad00465b7acff,100000000000000000000" --account="0xb0309c60b4622d3071fad3e16c2ce4d0b1e7758316c187754f4dd0cfb44ceb33,100000000000000000000"
```
2.  Run all the tests (including integration).
```
go test -cover -p 1 -count=1 -tags=integration ./...
```

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 07:16:52 +0000 UTC
    </div>
</div>

