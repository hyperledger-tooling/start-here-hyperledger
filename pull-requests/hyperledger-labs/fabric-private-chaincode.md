---
layout: default
title: fabric-private-chaincode
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-private-chaincode/pull/573" class=".btn">#573</a>
            </td>
            <td>
                <b>
                    Fix test-network setting and README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">comp/examples</span><span class="chip">documentation</span>
            </td>
            <td>
                I fixed the problem that test-network deployment could not be executed due to the path being changed.
Additionally, I fixed the content of the README.

Signed-off-by: ikegawa-koshi <koshi.ikegawa.mf@hitachi.com>

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
        Created At 2021-04-27 15:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-private-chaincode/pull/572" class=".btn">#572</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-private-chaincode/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Remove some make dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                - Move docker build from default `build` to `all` target
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-private-chaincode/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Samples reorg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">comp/examples</span>
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

