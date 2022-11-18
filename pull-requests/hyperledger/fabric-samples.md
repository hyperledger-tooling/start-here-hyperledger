---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/871" class=".btn">#871</a>
            </td>
            <td>
                <b>
                    add condition during delete self recipient key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is an issue during transfer token to the current implementation.
If a sender tries to sent all of his/her token to a receiver then the issue happen.

Conditions :
Sender need to send all of his/her token to the receiver 
Sender should not have any self Recipient Key for that token.

Error during endorsement : 
{
  status: 500,
  message: 'failed to delete the state of : DEL_STATE failed: transaction ID: dd10c301c30e4849c0d236ee778710e97a5576955726c87d1f16ed17ffc9cce0: invalid key. Empty string is not supported as a key by couchdb',
  payload: <Buffer >
}
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 07:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/870" class=".btn">#870</a>
            </td>
            <td>
                <b>
                    Run Full Stack Asset Transfer Guide tests on GHA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR runs the full stack asset transfer scenario tests on GitHub Actions.

🐢🐢🐢 

🐇🐇🐇🐇🐇🐇🐇🐇🐇 


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 17:26:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/869" class=".btn">#869</a>
            </td>
            <td>
                <b>
                    Move the remaining sample tests from Azure to GHA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moves the remaining fabric-samples tests from Azure to GHA.

The Azure pipeline is still responsible for publishing the rest-sample image to ghcr.io.  

We need to do a little work around establishing consistent revision semantics to the samples repo before porting the image distribution to GHA.  Included in this push should be the generation of sample chaincode images suitable for running with CCaaS and/or k8s-builder.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 15:03:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/866" class=".btn">#866</a>
            </td>
            <td>
                <b>
                    Move Kube Test Network tests from Azure -> GHA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR ports the Kubernetes Test Network tests from Azure to GHA.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-14 21:43:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    Remove commercial paper and fabcar tests from Azure pipelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR : 

- Removes the commercial paper and fabcar samples from the Azure test suites.

- Does a little bit of refactoring to create a custom `test-network-setup` action which can be used by multiple test network workflows. 

- Tests the addition of gradle, npm, and golang caches to help reduce the overall test runtimes. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-14 17:29:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/862" class=".btn">#862</a>
            </td>
            <td>
                <b>
                    Move lint and test-network-basic tests from Azure to GHA - READY FOR MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR ports the _glacial_ Linter and Test Network Basic tests from Azure to GHA: 

- Test Network Basic - Go
- Test Network Basic - Java
- Test Network Basic - Javascript
- Test Network Basic - Typescript

In addition, the scripts have been updated to run each test case in a different chaincode scope / ledger, re-using a single Fabric network across all tests in the suite.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 18:12:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/861" class=".btn">#861</a>
            </td>
            <td>
                <b>
                    Add FSAT appdev E2E test - READY FOR MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR runs the Full Stack Application Guide "app-dev" test suite as a GitHub Action on `pull_request` to main. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 15:57:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/860" class=".btn">#860</a>
            </td>
            <td>
                <b>
                    Only run GHA on PRs targeting the mainline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR reduces the frequency of running "hello-GHA" pipelines to target only mainline PRs. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 14:35:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/859" class=".btn">#859</a>
            </td>
            <td>
                <b>
                    Activate GHA on fabric-samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR launches a no-op / hello-world action to enable GitHub Actions on the samples repository.

Until this workflow is triggered (once) on the repo, GHA will refuse to run on PRs targeting main.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 13:04:08 +0000 UTC
    </div>
</div>

