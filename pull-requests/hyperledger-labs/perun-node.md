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

