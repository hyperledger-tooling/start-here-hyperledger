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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    Step 2 to improve sample test-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
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
This improves the test-network sample to show how to change from echo chain code to helloworld chain code.
**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Fixes #605 

**Special notes for your reviewer**:

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:
<!--
  If no, you can delete this section
  If yes, describe what changes and/or what breaks ..
-->
```
This changes the Test-network sample Readme adding a section to explain how to change the chain code and test it afterwards. It also fixes how the path to the chain code was defined.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 23:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    WIP Unittest for ECC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Test</span>
            </td>
            <td>
                **What this PR does / why we need it**:
Adding missing unit tests for ECC. This PR includes some refactoring ECC for better testing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 08:07:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Introduce staticchecks and spellchecking for go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                **What this PR does / why we need it**:

This PR introduces more tools to enhance code quality to our build pipeline.
In particular, we add [staticcheck](https://staticcheck.io/) and spellchecking to our golinter script and fix all detected issues, including dead code, removing dependencies of deprecated code, unchecked vars, and spelling issues.

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Closes #403 

**Special notes for your reviewer**:

Note that there exists a commit for adding the new tool and another commit that fixes the detected issues. I suggest review commit by commit.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 12:21:45 +0000 UTC
    </div>
</div>

