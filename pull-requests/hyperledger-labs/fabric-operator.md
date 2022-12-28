---
layout: default
title: fabric-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operator
---

# fabric-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    fix: the clusterole name associated with clusterrolebinding is incorrect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: 0xff-dev <stevenshuang521@gmail.com>

There are some problems here.
1. ServiceAccount is missing the namespace field. kustomize cannot normally replace the namespace of serviceAccount in clusterrolebinding.
2. role_binding.yaml ClusterRoleName isn't right.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-27 06:48:27 +0000 UTC
    </div>
</div>

