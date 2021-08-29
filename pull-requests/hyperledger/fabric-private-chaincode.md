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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/622" class=".btn">#622</a>
            </td>
            <td>
                <b>
                    Fixing Codecov reporting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">Test</span>
            </td>
            <td>
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

- Fixes broken reporting to codecov
- Enables go test coverage

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->

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
        Created At 2021-08-26 12:26:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    Separate the FPC go SDK from the Fabric Client SDK Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>

**What this PR does / why we need it**:

This commit introduces the following:
- a core package containing a fabric-sdk independent lifecycle and contract client
- a refactored resmgmt and gateway that instantiate the core package primitives using the fabric go-sdk

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 07:49:36 +0000 UTC
    </div>
</div>

