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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/461" class=".btn">#461</a>
            </td>
            <td>
                <b>
                    Small PR to address missing content for docker builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Three things in this PR:

- add lsof to the list of packages, we use it for ccf to detect duplicate instances but it is not installed by default in the CCF docker image
- add settings of no_proxy, NO_PROXY to the start_services tools script. The settings were used in the service tests but not when running persistent services
- make ccf ping_test.py a useful debugging tool; removed a lot of dependencies so the tool can be used stand alone and from someplace other than the ccf installation; that is, you should be able to test liveness (and certificate validity) for a ledger running
anywhere
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 20:55:21 +0000 UTC
    </div>
</div>

