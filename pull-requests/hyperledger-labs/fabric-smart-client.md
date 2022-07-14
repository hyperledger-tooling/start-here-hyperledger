---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Add NWO support for existing fabric bins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 08:44:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Enable race tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 10:39:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Upgrade to CodeQL v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 12:21:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/310" class=".btn">#310</a>
            </td>
            <td>
                <b>
                    view-sdk: enhancements 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces utility functions needed to address https://github.com/hyperledger-labs/fabric-token-sdk/issues/283 

Enhancements:
- add ability to retrive responder from the registry
- additional logging

Bug fix:
- fabric-sdk: update orderers list when apply config blocks after a restart

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 05:45:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/309" class=".btn">#309</a>
            </td>
            <td>
                <b>
                    Rework github actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Merge integration tests workflows in a single flow
- The new test workflow first runs our `checks` target, if successful, the integration tests and unit tests are started in parallel using the github actions matrix features. Running the checks first gives as a fast fail without wasting github action resources on long unit/integration tests.
- The job matrix features helps to configure a job with different configurations. That is, we don't need to create a workflow file per integration test we would like to run in parallel.
- Docker images are only pulled for integration tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 14:40:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/308" class=".btn">#308</a>
            </td>
            <td>
                <b>
                    Refactor nwo docker support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR changes the use of docker in the NWO. The NWO uses docker to launch some components, such as Orion, Weaver, Monitoring. This refactoring has two goals: 
First, remove the use of docker (use of docker client) during platform `init` function and move the corresponding logic to `postRun`. This allows a docker-free use of the fsccli artifactgen. 
Second, reduce redundant and cluttered code. Docker related code is now located in a `docker.go` file per platform. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 14:14:59 +0000 UTC
    </div>
</div>

