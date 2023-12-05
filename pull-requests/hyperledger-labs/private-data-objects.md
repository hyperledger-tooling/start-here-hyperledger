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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    Improve debugging of failed tests during github workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several fixes/improvements:
* debug logging is now available in the docker/docker compose tests
* when logging is enabled, unit tests will now generate output, respects environment variables
* github commits can add '[debug]' to turn on debug build/logging during runs
* fix sgx ssl abort when running actions on non-intel processors (skip the CPU check in SIM mode)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 16:02:14 +0000 UTC
    </div>
</div>

