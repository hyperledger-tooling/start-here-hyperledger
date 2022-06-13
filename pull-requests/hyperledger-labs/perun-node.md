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
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    Avoiding  invalid cross-device link at generate
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

Moving files between devices on file system leads to  invalid
cross-device link by using os.Rename. Therefore another way to move
files is used, which avoids this error.
Additional library is added, which implements this feature.

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
resolves #238 
#### Testing
<!-- Tell us how you have tested the changes. -->
Tested on machine with two different hard drives, one for / inlcuding /tmp, where the tmp files are generated.
Other harddrive contains perun node.
##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. Mount an additional harddrive, which is different from /tmp
2. Checkout perun-node to new harddrive and execute make
3.  Run ./perunnode generate

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x ] Name is added to the NOTICE file, if it is not present already.
- [x ] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 08:36:04 +0000 UTC
    </div>
</div>

