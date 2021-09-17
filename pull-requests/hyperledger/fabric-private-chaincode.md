---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/631" class=".btn">#631</a>
            </td>
            <td>
                <b>
                    Updated helloworld readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed an old path reference in the helloworld tutorial.

Signed-off-by: Riccardo Zappoli <42180293+ricc-zappoli@users.noreply.github.com>

<!--  Thanks for sending a pull request!  Here are some tips for you:

1. If this is your first time, please read our code of conduct and contributor guidelines: 
     https://github.com/hyperledger/fabric-private-chaincode/blob/main/CONTRIBUTING.md
     https://github.com/hyperledger/fabric-private-chaincode/blob/main/CODE_OF_CONDUCT.md
   In particular pay attention to the git workflows
      https://docs.google.com/document/d/1sR7YV3pSYN3NEFiW-2fUqtpsJeJrpC0EWUVtEm0Blcg/edit#heading=h.kwcug3pkefak
2. Fill out below sections.
3. Label the PR with the label of any component this PR touches.
4. ALso don't forget to sign your comments before submitting. 
   Github will complain if there is no DCO but it's easier if we don't have to hunt you down to fix that :-)

-->

**What this PR does / why we need it**:
This PR replaces `/examples/helloworld/` by `/samples/chaincode/helloworld/`in the helloworld tutorial readme file.

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Fixes #630 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 11:08:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    Fixed the version of fabric-ccenv to 2.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: ikegawa-koshi <koshi.ikegawa.mf@hitachi.com>

**What this PR does / why we need it**:

I found a bug in the current main branch and v1.0-rc2 that causes FPC to fail to build (Issue #628).
As a result of discussions with the community, it was found that it was caused by differences in the version of fabric-ccenv.
This PR solves the issue of Issue #628 by setting the version of fabric-ccenv to v2.3.0.

**Which issue(s) this PR fixes**:

Fixes #628

**Special notes for your reviewer**:

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 11:53:00 +0000 UTC
    </div>
</div>

