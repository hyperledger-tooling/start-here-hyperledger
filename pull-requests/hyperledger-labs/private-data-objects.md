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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    Implements a new set of docker scripts
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
        Created At 2023-03-17 22:46:56 +0000 UTC
    </div>
</div>

