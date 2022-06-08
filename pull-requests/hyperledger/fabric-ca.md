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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.2.

Update FVT tests to use sha256 since Go 1.18 does not accept certs signed with sha1.

Build gendoc utility from a commit of Fabric main branch that supports Go 1.18. gendoc is used in 'make docs' for metrics doc generation. This change also updates the metrics doc to use the latest formatting from Fabric.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 18:30:01 +0000 UTC
    </div>
</div>

