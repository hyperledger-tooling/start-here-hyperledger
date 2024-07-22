---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    fix tessera for ARM64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are no official images for Tessera that can run in ARM64 so we need to use the `--platform` flag to emulate them using the `AMD64` images

It also fixed startup problems with dependency from Quorum to Tessera
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 11:14:13 +0000 UTC
    </div>
</div>

