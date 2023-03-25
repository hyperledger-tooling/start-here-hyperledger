---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    New approach to docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                First... there are lots of extra commits in here. Many are necessary for this to work (e.g. separating service unit tests from client tests). There will be a number of PRs to cover these changes.

Check $(PDO_SOURCE_ROOT)/docker-new for different way of building the docker files based on pushing scripts into the images rather than building them along the way. This should make it easier to remove the proxy complexity, start persistent services, and split execution across multiple hosts.

Tests are now run in a separate client image. See the docker compose configuration file for tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 20:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/418" class=".btn">#418</a>
            </td>
            <td>
                <b>
                    a series of small fixes for random issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * make service host configurable with site.psh. this should make client configuration a little easier
* export PDO_SOURCE_ROOT through common-config.sh; we document this but don't set it consistently
* allow scripts to pick a site.psh file; another change to make it easier for clients to use multiple services
* remove several unused targets from the CCF makefile
* move the python package requirements out of the makefile into a (more standard) requirements file
* remove the unused auctiontest configuration file from the client tree
* check the return value for eservice database operations & improve the error message
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 15:25:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    Remove the Sawtooth ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes support for Sawtooth in PDO.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 06:38:37 +0000 UTC
    </div>
</div>

