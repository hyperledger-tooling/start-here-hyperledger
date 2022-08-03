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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Merge main into go-support-preview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR get the go-support-preview up-to-date with main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 16:37:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Fix path to SGX hardware
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

An error occurred when performing a FPC build in the go-support-preview branch on a DCsv2 instance of Microsoft Azure.
I fixed it because the way the path to the SGX hardware in `integration/go_chaincode/utils/utils.go` was written was not an absolute path.


**Which issue(s) this PR fixes**:

None

**Special notes for your reviewer**:

None

Signed-off-by: ikegawa-koshi <koshi.ikegawa.mf@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 07:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Alternative simulation support for non-sgx platforms
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

This PR introduces an alternative simulation support for non-sgx platforms, such as Mac M1. 
To make this work, both, the FPC chaincode and ercc can be compiled using pure go and without any SGX dependency, which allows playing with your FPC chaincode while developing on your non-sgx host. 

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
        Created At 2022-07-29 19:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/681" class=".btn">#681</a>
            </td>
            <td>
                <b>
                    Upgrade ego
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR upgrades ego to v1.0.0. With the new ego bundle command, which
packages the signed enclave binary with the ego runtime, there is no
need for the dedicated `fpc-ccenv-go` image anymore as we can just use
`fpc-ccenv` with the bundled chaincode.

- Upgrade to ego v1.0.0
- Remove fpc-ccenv-go
- Upgrade `go.mod` to go 1.17
- Fix staticcheck issues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 16:05:17 +0000 UTC
    </div>
</div>

