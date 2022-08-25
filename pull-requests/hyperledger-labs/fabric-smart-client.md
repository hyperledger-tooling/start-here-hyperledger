---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    Remove need for GOPATH to be set
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If GOPATH is set and fabric-smart-client is a subdir in that GOPATH then it must still follow the pattern
src/github.com/hyperledger-labs/fabric-smart-client

GOPATH can be set and not contain fabric-smart-client (means the go module cache can be stored elsewhere)

GOPATH not being set will default to $HOME/go and above rules apply

It still requires to be checked out as fabric-smart-client still though, see TODO

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 07:17:52 +0000 UTC
    </div>
</div>

