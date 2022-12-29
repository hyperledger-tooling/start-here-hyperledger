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
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    fix: occasional gosec failure to get version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                gosec install script will auto get latest version(for example:https://github.com/bestchains/fabric-operator/actions/runs/3799271745/jobs/6461638960#step:5:7).  Not only is it unnecessary to get latest version, but this request is easily rejected by github, resulting in a `null` version (for example https://github.com/bestchains/fabric-operator/actions/runs/3799115622/jobs/6461341294#step:5:7) and installation failure.

Signed-off-by: Abirdcfly <fp544037857@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-29 08:09:30 +0000 UTC
    </div>
</div>

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

