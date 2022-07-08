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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    fabric-sdk: use orderers set in the config block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, the FSC node uses only the orderers defined
in the configuration file. But, orderers can change
with a configuration update.
Thefore, this PR let the fabric-sdk to use the orderers
defined in the configuration block.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 07:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    Run goimports over the code base
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
        Created At 2022-07-04 17:04:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    Move tools deps into tools folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Rename tools.go to deps.go to better reflect the nature of these
  "indirect" dependencies
- Introduce tools/tools.go as a single place to collect all our tools we
  are using for building and testing. This structure allows us to keep
  these tool deps out our project go.mod file
- Replace golint with staticchecks.
- Enhance makefile structure

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 12:55:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Pin Fabric 2.2 LTS
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
        Created At 2022-07-04 09:21:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    orion db
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-02 08:03:53 +0000 UTC
    </div>
</div>

