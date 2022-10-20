---
layout: default
title: minifabric
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minifabric
---

# minifabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minifabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    Fix for deploynode not properly waiting for each node to deploy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Humphrey <ryanhumphrey777@gmail.com>
Previously, the wait task would hang for 90 secs until timeout for every node deployment because it could not find the  namespace. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 21:27:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Added testing for deployoperator and deploynodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds github action that deploys kubernetes cluster and tests the new deployoperator and deploynodes operations
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 00:49:10 +0000 UTC
    </div>
</div>

