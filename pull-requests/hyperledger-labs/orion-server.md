---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    Provenance disable switch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">provenance</span>
            </td>
            <td>
                Add a config option in the local config to disable the provenance store.
    
- When disabled:
  - The provenance store is not initialized and is set to nil.
  - In the commit path, no data is committed to the provenance store.
  - Provenance queries return 503 Service Unavailable, with a text message that informs that this server has the provenance disabled in it.
- Provenance can be enabled on one server but disabled on another.
- Restarting a server with provenance switched from on to off will leave the provenance store intact, but no more data will be committed to it.
- Restarting a server with provenance switched from off to on is not supported  and will result in an error.
    
Some ledger queries that previously depended on the provenance store are now decoupled from the provenance store and continue to be served.


Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-17 08:38:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    fix remove node test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: tohar-ayash <toharayash1@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 14:04:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/434" class=".btn">#434</a>
            </td>
            <td>
                <b>
                    change server test port
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: tohar-ayash <toharayash1@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 12:07:44 +0000 UTC
    </div>
</div>

