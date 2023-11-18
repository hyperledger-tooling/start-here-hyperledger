---
layout: default
title: fabric-contract-api-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-contract-api-go
---

# fabric-contract-api-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-contract-api-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    Allow schema types with the same name from different packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the short type name was used as a schema key. This meant that types of the same name from different packages would overwrite each other in the map of schema type definitions, causing unexpected serialization errors. Now the fully qualified (package + type) name is used so that entries for types with the same name from different packages are unique.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 12:02:33 +0000 UTC
    </div>
</div>

