---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/404" class=".btn">#404</a>
            </td>
            <td>
                <b>
                    Use fabric-lib-go for bccsp, metrics, flogging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following packages are being moved from fabric to fabric-lib-go so that they can be shared across fabric and fabric-ca:

- github.com/hyperledger/fabric/bccsp
- github.com/hyperledger/fabric/common/flogging
- github.com/hyperledger/fabric/common/metrics

This commit updates fabric-ca to use the common code in fabric-lib-go.

The fabric-ca dependency on fabric is no longer needed. That's good!

Also ran goimports to clean up imports.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 22:47:41 +0000 UTC
    </div>
</div>

