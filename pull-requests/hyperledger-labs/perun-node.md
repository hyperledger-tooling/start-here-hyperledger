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

