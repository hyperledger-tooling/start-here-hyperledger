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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    Release commit for v1.5.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add release notes for v1.5.9.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 02:52:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    Use fabric-lib-go v1.1.0 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transition from the fabric-lib-go temporary branch to the actual release v1.1.0.

This is the release that includes the common
bccsp, metrics, and flogging packages that
are shared across fabric and fabric-ca.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 14:43:26 +0000 UTC
    </div>
</div>

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

