---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Feature/general indy resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Builds upon #80 

- Adds a VDR API with a general DID resolver. Network configuration can be taken from a Github Repo or a local folder structure
- Initial support for multiple ledgers and DID resolution with indy-vdr-proxy

The VDR API uses Async/Await and is therefore not suited for FFI, but I'll look into it.

I think it would help to create a `did-indy` branch to have smaller PRs at some point :) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 16:32:52 +0000 UTC
    </div>
</div>

