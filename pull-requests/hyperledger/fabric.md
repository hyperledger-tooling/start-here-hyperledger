---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3000" class=".btn">#3000</a>
            </td>
            <td>
                <b>
                    Move to better IsAbs Implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #2998 

Signed-off-by: D <d_kelsey@uk.ibm.com>


- Bug fix

#### Description

path.IsAbs is a poor implementation in Go, filepath.IsAbs looks to be much better 
and addresses the problem where a windows absolute path is not recognised


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 08:42:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2999" class=".btn">#2999</a>
            </td>
            <td>
                <b>
                    Retry logic for evaluate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify the evaluate method to retry processing of a transaction proposal on another peer in the case of an error.

resolves #2913 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 15:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2997" class=".btn">#2997</a>
            </td>
            <td>
                <b>
                    Protobuf and etcd upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Update protobuf and etcd to their latest versions.

#### Additional details

This is a reprisal of the work on updating protobuf by #2185

#### Related issues

FAB-18363


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 15:57:35 +0000 UTC
    </div>
</div>

