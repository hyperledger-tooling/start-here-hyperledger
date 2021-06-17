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
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    Move contract validation from node to session init
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

- Contracts are validated during node initialization using a read-only
  blockchain backend. Validated addresses are then stored in a registry
  and passed on to the session.

- Since valid contract addresses are provided by the node, use the
  addresses without validation in session init. Also, remove the tests
  related to invalid contracts for OpenSession and updates its doc
  comments to remove InvalidContracts Error.

- Remove the option for user to provide the addresses in session config.
  Also, remove the contract addresses from session config template in
  testdata.


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

Resolves #106.
#### Testing
<!-- Tell us how you have tested the changes. -->
Added tests for contract validation in node init. Tested `perunnodetui` and perunnodecli`.

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
        Created At 2021-06-16 11:46:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    Add read-only chain backend to validate contracts
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
- For validating contracts during node initialization, a read-only chain
  backend is needed, because node does not have credentials to
  initialize a full chain backend.

- Add a ROChainBackend interface that specifies only methods for
  validating the contracts.

-  Implement a constructor for ROChainBackend, where the transactor is
   set to nil. This is safe to use because only validation methods are
   exposed via this interface and those methods do not use the
   transactor.

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

Relates to #106.

#### Testing
<!-- Tell us how you have tested the changes. -->

Tests are added for validating contracts using read-only backend.

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
        Created At 2021-06-16 11:41:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    Remove hard-coded secondary settle, register
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

- Hard coded secondary logic for settle and register transactions were
  implemented in go-perun, since they were not working as expected.

- But in go-perun/issues/8, it was concluded to add this feature later,
  when there is a concrete use case.

- Now, it is removed, because the hard-coded sleep:
  - Does not save any cost, as we work on testnet.
  - Doubles the test execution time for session package.

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

Closes #204.

#### Testing
<!-- Tell us how you have tested the changes. -->

Test execution time for session package becomes half compared to previous test run.

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
        Created At 2021-06-16 07:00:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    Improve API Error impl & document errors in API
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
- The implementation is improved to
  - Store the underlying error, so that error stack can be retreived.
  - Implement formatter interface, so that error stack is retreived from
    the underlying error and printed when using the "%+v" verb in printf
    style funcs.
  - For most errors (except for failed pre-condition), generate error
    messages within the error constructors. So that redundant definition
    of error messags is removed.

- Add tests for all error constructors, perun pkg has 100% coverage now.

- Move error assertions functions to perun-node/peruntest, as most of
  them are used in perun_test both session_test packages.

- Document the named errors returned by each of the API.

- Also, use upper case 'O' in timedOut in all the places.



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

Resolves #132.

#### Testing
<!-- Tell us how you have tested the changes. -->

Tests have been added in perun package for error constructors. This package now has 100% coverage.

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
        Created At 2021-06-15 20:34:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    Add missing named errors in OpenSession
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

- Add invalid contracts error in blockchain package to detect type of
  contract.

For OpenSession API:

- Used InvalidConfig error (for each parameter), InvalidContractsError.

- Updated the proto buff definitions and grpc bindings to handle the
  newly added errors.

- Removed the parsing of PartAddrs from config and the tests related
  to it as partsAddrs are not used now.


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

Tests for newly added named errors have been added.

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
        Created At 2021-06-15 11:08:30 +0000 UTC
    </div>
</div>

