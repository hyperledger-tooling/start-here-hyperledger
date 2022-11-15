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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/867" class=".btn">#867</a>
            </td>
            <td>
                <b>
                    Feature/no zure - DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **DO NOT MERGE** 

Ports the remainder of the fabric-samples tests to GHA.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 02:52:38 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/852" class=".btn">#852</a>
            </td>
            <td>
                <b>
                    Moves the Full Stack Asset Transfer Development Guide to fabric-samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a step towards migrating the Hyperledgendary [Full Stack Asset Transfer](https://github.com/hyperledgendary/full-stack-asset-transfer-guide) Guide to fabric-samples.

This content was developed (and tested by fire!) as part of an interactive workshop at the HL Global Forum in 2022 in Dublin.  

The material covers: 
- Interactive and step-level debugging with CCaaS and microfab
- Interactive exercises and guidelines for building Gateway Client (Fabric > 2.4) based applications
- Interactive exercises and guides for deploying _cloud native_ Fabric networks and applications to local, hybrid, and public cloud.

The PR is generally a "pick up and move" from Hyperledgendary to the fabric-samples repo.   Some minor tweaks related to `$PWD` have been made to the READMEs and guides.

This PR includes some minor updates necessary to run the Kubernetes operator, Fabric network, and chaincode on an M1 / Mac running with the QEMU emulation.  (More work / testing in this area is necessary for the "local build" on the M1 for chaincode images running with the k8s builder.)

The last submission to the full-stack guide at the time of this import was at [commit fb554befdbbeff9e69159b54fce0b811603f29c7](https://github.com/hyperledgendary/full-stack-asset-transfer-guide/commit/fb554befdbbeff9e69159b54fce0b811603f29c7) on the remote repo ([PR #158](https://github.com/hyperledgendary/full-stack-asset-transfer-guide/pull/158).)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 21:52:49 +0000 UTC
    </div>
</div>

