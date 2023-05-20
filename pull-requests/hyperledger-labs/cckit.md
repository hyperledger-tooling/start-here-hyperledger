---
layout: default
title: cckit
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/cckit
---

# cckit <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/cckit){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cckit/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Expose additional protojson marshal options. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is in relation to issue #31 and storing the state a json objects. This exposes two additional options for json serialization and enables them by default for the json sterilization. The first option has it encode the enums as an int instead of a string. This will reduce the size of the objects stored in the ledger. The second option is to enable it to encode default values when translating the proto to json. This will ensure that the objects in the CouchDB will have the expected shape so that rich queries can be ran on the world state db for objects that have default values. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 18:53:54 +0000 UTC
    </div>
</div>

