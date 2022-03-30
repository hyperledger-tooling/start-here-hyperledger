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
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    Feature/python wrapper with multiple ledger support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added python wrapper for multi-ledger did resolution

Exposes three simple ways to set up a resolver:

1. Provide a list of namespaces, genesis files will be retrieved from did indy networks repo
2. Local did indy networks compatible folder structure
3. Autopilot: Library will try to fetch genesis files from did indy networks repo when a DID with an unknown namespace is encountered.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 14:19:11 +0000 UTC
    </div>
</div>

