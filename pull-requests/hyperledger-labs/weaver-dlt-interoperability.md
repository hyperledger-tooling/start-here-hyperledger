---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    chaincode changes to support ECDLP lock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses the below:
- Reorganize the interop-cc, base-class and base-class-contract pertaining to locking mechanism
- Add the code to support ECDLP lock along with HashLock
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 17:29:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    returning the correct number of args
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Krishnasuri Narayanam <knaraya3@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 11:49:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    using generic lockInfo and claimInfo structs in interop-cc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Krishnasuri Narayanam <knaraya3@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 11:36:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    Adding support for Corda-Network2 data transfer.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added certs for network2 in Corda network, and modified `Corda_Relay.toml` config file.
2. Modified the way Certs are added in Corda network, so that its no longer hard coded and is configurable without need to re-deploy network.
3. Added commands like `configure-create-all`, `configure-all`, `configure-data`, and `configure-network`, which works similar to fabric-cli commands, except that `configure-all <list of networks separated by comma>` to add all these networks' credentials in Corda-network.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 09:36:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    fabric-cli link fix in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sannish <sannish1@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 10:15:15 +0000 UTC
    </div>
</div>

