---
layout: default
title: fabric-ansible-collection
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-ansible-collection
---

# fabric-ansible-collection <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-ansible-collection){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Add metadata update for CA, peer, ordering nodes
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
        Created At 2024-04-06 22:09:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Correction for Ordering Service Node Action plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Completed corrections for the Ordering Node Actions module
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 12:34:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    remove unsupported flags for init chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The original code leads to an error when init_required is true:

```
Failed to init legacy chaincode on peer:  Error: unknown flag: --endorsement-plugin
```

See also: https://hyperledger-fabric.readthedocs.io/en/release-2.5/commands/peerchaincode.html#peer-chaincode-invoke
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 07:52:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    strip the 'v' prefix that newer fabric binaries print as their versio…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …n, to prevent LooseVersion comparison breakage
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 10:09:00 +0000 UTC
    </div>
</div>

