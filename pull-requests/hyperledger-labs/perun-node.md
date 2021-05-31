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
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Upgrade Go and golangci-linter used in CI
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

- Upgrading in preparation to the upcoming release.
    
- In golangci-lint, two deprecated linters are removed and replaced with alternatives.
    
- Fix warnings thrown after linter upgrade.

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

Closes #189.

#### Testing
<!-- Tell us how you have tested the changes. -->

CI pipeline should pass after the upgrade.

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
        Created At 2021-05-31 14:49:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    Upgrade go-perun version to c6caccb6d2b4
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

- This update includes fix for contructor for FundingTimeoutError.
    
- It also includes changes to the format in which data is stored in
      leveldb during persistence. So testdata is also updated.
    

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

Relates #189.

#### Testing
<!-- Tell us how you have tested the changes. -->

All existing tests in the CI pipeline should pass.

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
        Created At 2021-05-31 14:46:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    Add periodic redraw in perunnodetui
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
- Previously, screens of TUI app are refreshed only on mouse event or
  keyboard event. Now enable periodic redraw for every "n" secs.

- Also, refactor the signature of eventloop function to make it shorter
  after adding a new argument.

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

#### Testing
<!-- Tell us how you have tested the changes. -->

perunnodetui component does not have unit tests. When running the app, all data should be automatically updated in real time, even the app is not focused. Visibly, the change in time (in the top right corner) can be observed.

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
        Created At 2021-05-31 12:30:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/187" class=".btn">#187</a>
            </td>
            <td>
                <b>
                    Revise the readme for perunnode TUI
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
- Fix a mistake and revise few sentences.
- 
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

#### Testing
<!-- Tell us how you have tested the changes. -->

No code changes.

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
        Created At 2021-05-31 12:28:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    Add readme for perunnodetui
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

- Containes a brief tutorial on how to use the tui client.

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

No modifications in code.

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
        Created At 2021-05-28 10:06:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    Add example for using payment API as integ test
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

    
- This example will be used in tutorial for using perun-node as a  library.


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

The example is itself implemented as a test in `app/payment` package: `Test_Integ_PaymentAPI`.

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
        Created At 2021-05-28 07:52:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Add a Text Based UI client for perun-node.
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

- This is an additional client implementation beside of perunnodecli.
    
- It provides a more graphical way to try out the perun-node.

A how to documentation is to be added.

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

The client needs to be tested manually. 

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
        Created At 2021-05-28 06:21:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Preparation for TUI client
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

Add function to get a logger instance without any fields. This will be used in Text Based UI client that is coming up.

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
        Created At 2021-05-28 06:19:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    Remove V2 tag for new APIErr,remove old err types
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

    
    
    - All APIs have been updated to use the newly defined error type.
    
    - So remove the V2 tag for it and delete all refs to the older error
      types and related funcs.
    
  
    


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

  Closes #132.
#### Testing
<!-- Tell us how you have tested the changes. -->

No new tests. Existing tests should pass.

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
        Created At 2021-05-28 06:16:32 +0000 UTC
    </div>
</div>

