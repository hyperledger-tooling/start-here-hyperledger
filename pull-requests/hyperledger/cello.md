---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/343" class=".btn">#343</a>
            </td>
            <td>
                <b>
                    Fix peer cmd 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix peer cmd, so we can use `peer channel` cmd in api-engine container.  There are some changes in this pr. 
* Refactor the configtx generation by using a template file. 
* The admin permission check errors were caused by `MSP ID` mismatched, the configtx defined the MSP as `Org1OrdererMSP`, but `orderer.yaml` and `core.yaml` defined different ones. 
* Add some environment variables when creating nodes. 
* Create a docker network to connect node containers, api-engine container and agent container for development purposes. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 18:04:07 +0000 UTC
    </div>
</div>

