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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/587" class=".btn">#587</a>
            </td>
            <td>
                <b>
                    data provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Bruno Vavala <bruno.vavala@intel.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 15:54:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    Enable stress tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This enables the stress test suite to be executed with the integration test.
The stress test was introduced with #584 but we missed to add it the integration test pipeline.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>

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
        Created At 2021-05-21 07:39:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/585" class=".btn">#585</a>
            </td>
            <td>
                <b>
                    Add hybrid request encryption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This introduces a hybrid encryption scheme for fpc requests. Before FPC
requests were encrypted using the chaincode encryption key using
RSA-based encryption. This had the limitation that the maximum payload
size was restricted to ~200bytes. They new scheme uses symmetric
encryption to encrypt the actual request and uses the chaincode
encryption key to encrypt the key used to encrypt the FPC request. The
encrypted request key is added to the request protos. Unit test for go
cryto package and support for mock_ecc were added.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>

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
        Created At 2021-05-19 00:41:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    Add hybrid request encryption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">com/client-sdk</span><span class="chip">comp/shim</span><span class="chip">urgent</span>
            </td>
            <td>
                This introduces a hybrid encryption scheme for fpc requests. Before FPC
requests were encrypted using the chaincode encryption key using
RSA-based encryption. This had the limitation that the maximum payload
size was restricted to ~200bytes. They new scheme uses symmetric
encryption to encrypt the actual request and uses the chaincode
encryption key to encrypt the key used to encrypt the FPC request. The
encrypted request key is added to the request protos. Unit test for go
cryto package and support for mock_ecc were added.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>

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
        Created At 2021-05-18 14:32:57 +0000 UTC
    </div>
</div>

