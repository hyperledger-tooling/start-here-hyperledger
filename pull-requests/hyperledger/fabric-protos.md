---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Fix missing node module content
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The generated content was not shared between jobs in the GitHub actions workflow

These changes keep the whole node build and publish in a single job since uploading/downloading generated artifacts between jobs is time consuming

The new structure also means that the Java build can run independently

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 10:31:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    Update node publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make module public and tag with latest

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 14:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Publish node module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix main ci workflow and add workflow to publish the node bindings

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 16:54:02 +0000 UTC
    </div>
</div>

