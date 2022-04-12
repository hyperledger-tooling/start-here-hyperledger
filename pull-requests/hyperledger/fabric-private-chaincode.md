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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    Go upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Current build fails to an incompatibility of one of our go tools.

This PR upgrade to go 1.17.5, which is currently also used by Fabric. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 14:26:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/670" class=".btn">#670</a>
            </td>
            <td>
                <b>
                    Fix shim.go link in readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: munapower <mmunaro@hotmail.com>

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
Fixes a link in readme documentation of go support preview that instead of taking you to shim.go returns a 404 error.
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 13:57:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/669" class=".btn">#669</a>
            </td>
            <td>
                <b>
                    Fix get_*_partial_state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                **What this PR does / why we need it**:

When we call a `get_*_partial_state`, we fetch the data outside the enclave and wrap the entire result in a json message with the format [`key=value,...]`. Inside the enclave, we translate this json to `std::map<string, string>` and return it to the chaincode.

With non-public data, the values are encrypted and base64 encoded. That is, the json to map translation works as expected. However, for public data, where we handle arbitrary data, it seems that a value which contains a json string, will corrupt the json message and cannot be transformed into the map.

To fix this problem we do the following:
When creating the json message outside the enclave, we just take the value and encode it with base64 no matter if it is encrypted or not. After the translation into `std::map`, we just decode the value again. In case of encrypted values, we encode/decode twice and thereby increase payload size.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>

Thanks @lebdron for spotting this bug! The full discussion about this error can be found on [discord](https://discord.com/channels/905194001349627914/943059293765267497/962989270329602078).

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


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 15:05:56 +0000 UTC
    </div>
</div>

