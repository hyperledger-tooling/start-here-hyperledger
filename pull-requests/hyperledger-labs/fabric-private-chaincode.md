---
layout: default
title: fabric-private-chaincode
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-private-chaincode
---

# fabric-private-chaincode

You can clone this repo on <span class="fs-3">[GitHub](https://github.com/hyperledger-labs/fabric-private-chaincode){: .btn .mr-4 }</span>


<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#572](https://api.github.com/repos/hyperledger-labs/fabric-private-chaincode/pulls/572)
            </td>
            <td>
                <b>
                    Make fabric patch optional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update readme and remove statements telling the reader to patch fabric
- Remove fabric patch from default build path; patch targets are still available for custom use;
- Docker dev image still checkouts fabric repo
- By default fabric binaries are fetched into `fabric/_internal` and set in `config.mk`

Signed-off-by: Marcus brandenburger <bur@zurich.ibm.com>

<!--  Thanks for sending a pull request!  Here are some tips for you:

1. If this is your first time, please read our code of conduct and contributor guidelines: 
     https://github.com/hyperledger-labs/fabric-private-chaincode/blob/main/CONTRIBUTING.md
     https://github.com/hyperledger-labs/fabric-private-chaincode/blob/main/CODE_OF_CONDUCT.md
   In particular pay attention to the git workflows
      https://docs.google.com/document/d/1sR7YV3pSYN3NEFiW-2fUqtpsJeJrpC0EWUVtEm0Blcg/edit#heading=h.kwcug3pkefak
2. Fill out below sections.
3. Label the PR with the label of any component this PR touches.
4. ALso don't forget to sign your comments before submitting. 
   Github will complain if there is no DCO but it's easier if we don't have to hunt you down to fix that :-)

-->

**What this PR does / why we need it**:

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Fixes #

**Special notes for your reviewer**:

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:
<!--
  If no, you can delete this section
  If yes, describe what changes and/or what breaks ..
-->
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 14:20:02 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#571](https://api.github.com/repos/hyperledger-labs/fabric-private-chaincode/pulls/571)
            </td>
            <td>
                <b>
                    Remove some make dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                enhancement{: .label-grey }
            </td>
            <td>
                - Remove docker build from default build path (Full docker build is still done by CI)
- Remove build-dep on test and linter to give the developer the freedom to just do the stuff they want (make all, or just make, still performs make build test)

Signed-off-by: Marcus brandenburger <bur@zurich.ibm.com>

<!--  Thanks for sending a pull request!  Here are some tips for you:

1. If this is your first time, please read our code of conduct and contributor guidelines: 
     https://github.com/hyperledger-labs/fabric-private-chaincode/blob/main/CONTRIBUTING.md
     https://github.com/hyperledger-labs/fabric-private-chaincode/blob/main/CODE_OF_CONDUCT.md
   In particular pay attention to the git workflows
      https://docs.google.com/document/d/1sR7YV3pSYN3NEFiW-2fUqtpsJeJrpC0EWUVtEm0Blcg/edit#heading=h.kwcug3pkefak
2. Fill out below sections.
3. Label the PR with the label of any component this PR touches.
4. ALso don't forget to sign your comments before submitting. 
   Github will complain if there is no DCO but it's easier if we don't have to hunt you down to fix that :-)

-->

**What this PR does / why we need it**:

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Fixes #

**Special notes for your reviewer**:

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:
<!--
  If no, you can delete this section
  If yes, describe what changes and/or what breaks ..
-->
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 13:31:00 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#570](https://api.github.com/repos/hyperledger-labs/fabric-private-chaincode/pulls/570)
            </td>
            <td>
                <b>
                    Samples reorg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                comp/examples{: .label-grey }
            </td>
            <td>
                <!--  Thanks for sending a pull request!  Here are some tips for you:

1. If this is your first time, please read our code of conduct and contributor guidelines: 
     https://github.com/hyperledger-labs/fabric-private-chaincode/blob/main/CONTRIBUTING.md
     https://github.com/hyperledger-labs/fabric-private-chaincode/blob/main/CODE_OF_CONDUCT.md
   In particular pay attention to the git workflows
      https://docs.google.com/document/d/1sR7YV3pSYN3NEFiW-2fUqtpsJeJrpC0EWUVtEm0Blcg/edit#heading=h.kwcug3pkefak
2. Fill out below sections.
3. Label the PR with the label of any component this PR touches.
4. ALso don't forget to sign your comments before submitting. 
   Github will complain if there is no DCO but it's easier if we don't have to hunt you down to fix that :-)

-->

**What this PR does / why we need it**:

This PR implements the changes as discussed in #555. We introduce `/samples` as a central place to locate all samples, including chaincodes, clients SDK, and deployments. 

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Fixes #555 

**Special notes for your reviewer**:

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:
<!--
  If no, you can delete this section
  If yes, describe what changes and/or what breaks ..
-->
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 11:17:00 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#569](https://api.github.com/repos/hyperledger-labs/fabric-private-chaincode/pulls/569)
            </td>
            <td>
                <b>
                    Remove unused docker build dependencies (cc builder & peer)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the cc_builder and peer from the docker build (but maintains the docker files as they might be useful in the future), thereby speeding up both local and CI build. 

Signed-off-by: Bruno Vavala <bruno.vavala@intel.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 00:09:18 +0000 UTC
    </div>
</div>

