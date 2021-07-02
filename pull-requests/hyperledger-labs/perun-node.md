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
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    WIP : Add ERC20 support (completed). Approach 3 for fixing a bug in go-perun (WIP)
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

Demo for fixing the error in PR #213. Using two assets in a single channel.

In the mentioned PR, `Test_Integ_Role` in `api/grpc` package is failing due to tx nonce mismatch when using ERC20 asset is the the channel. See the test output [here](https://app.circleci.com/pipelines/github/hyperledger-labs/perun-node/667/workflows/8ced469d-f41a-45e1-b329-665818578a03/jobs/1424/steps?invite=true#step-109-2699)

This is because two tx's are required for funding ERC20 asset. Both tx's have same nonce. This issues has been discussed in [go-perun#62](https://github.com/hyperledger-labs/go-perun/issues/62).

In #214, a fix was suggested, but it has some limitations. The limitation is demonstrated in this PR.

It is done here instead of go-perun repo because, this error occurs only in case of `ganache-cli` and go-perun project currently uses only a simulated backend for testing.

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
<!-- Implementation Task -->
DEMO

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

#### Testing
<!-- Tell us how you have tested the changes. -->

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
        Created At 2021-07-02 06:38:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    WIP : Add ERC20 support (completed). Approach 1 for fixing a bug in go-perun (WIP)
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

Demo for fixing the error in PR #213.

In the mentioned PR, `Test_Integ_Role` in `api/grpc` package is failing due to tx nonce mismatch when using ERC20 asset is the the channel. See the test output [here](https://app.circleci.com/pipelines/github/hyperledger-labs/perun-node/667/workflows/8ced469d-f41a-45e1-b329-665818578a03/jobs/1424/steps?invite=true#step-109-2699)

This is because two tx's are required for funding ERC20 asset. Both tx's have same nonce. This issues has been discussed in [go-perun#62](https://github.com/hyperledger-labs/go-perun/issues/62).

A fix is demonstrated in this PR by using `go-perun` as a vendored library. It is done here instead of go-perun repo because, this error occurs only in case of `ganache-cli` and go-perun project currently uses only a simulated backend for testing.

In this PR, implemented approach 1 described in the issue (manually increasing the nonce after first TX).  However, this solution has limitations that it does not work when two assets are used in the same channel (See #215) for more info on this.

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
<!-- Implementation Task -->
DEMO

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

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
        Created At 2021-07-02 06:32:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/213" class=".btn">#213</a>
            </td>
            <td>
                <b>
                    Add erc20 support
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

Add support for using ERC20 tokens.

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

#### Testing
<!-- Tell us how you have tested the changes. -->

Tests are added for the new features. For testing use of ERC20 tokens, tests are added in `api/grpc` package.

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
        Created At 2021-07-02 06:09:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/212" class=".btn">#212</a>
            </td>
            <td>
                <b>
                    194 add deploy register api
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

Add APIs for deploying asset ERC20 contracts and for registering currencies.
Made some refactors to enable better testing of these functionalities.

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
an issue before submitting a pull request.

Resolves #194.

#### Testing
<!-- Tell us how you have tested the changes. -->

Tests have been added for the newly added APIs.
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
        Created At 2021-07-01 06:29:56 +0000 UTC
    </div>
</div>

