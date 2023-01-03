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
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Update CA integration test to use localho.st DNS domain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #90 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-02 12:58:48 +0000 UTC
    </div>
</div>

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

