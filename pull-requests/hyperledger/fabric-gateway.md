---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/678" class=".btn">#678</a>
            </td>
            <td>
                <b>
                    Use FABRIC_CFG_PATH in fabric-tools container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Scenario test scripts used hard-coded paths to reference Fabric configuration files within the fabric-tools Docker container. This made the tests sensitive to changes of the configuration file location between Fabric releases. The container defines a FABRIC_CFG_PATH environment variable that points to the correct location so scripts now use this instead of hard-coded paths.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 21:27:08 +0000 UTC
    </div>
</div>

