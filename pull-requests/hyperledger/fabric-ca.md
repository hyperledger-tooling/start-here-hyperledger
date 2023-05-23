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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Update operations_guide.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                FIX: CA Admin identities for org1, org2 must be properly registered as admin

#### Type of change

- Documentation update

#### Description

Following the documentation I got error on [create-and-join-channel](https://hyperledger-fabric-ca.readthedocs.io/en/latest/operations_guide.html#create-and-join-channel) part, getting the following error:
```
Error: got unexpected status: BAD_REQUEST -- error validating channel creation transaction for new channel 'mychannel', could not successfully apply update to template configuration: error authorizing update: error validating DeltaSet: policy for [Group]  /Channel/Application not satisfied: implicit policy evaluation failed - 0 sub-policies were satisfied, but this policy requires 1 of the 'Admins' sub-policies to be satisfied
```
I looked up orderer log to find out that OU being `user` is causing the problem not meeting the policy. I suggest the documentation to use `admin` OU for CA identities of org1 and org2.

#### Additional details

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 01:51:57 +0000 UTC
    </div>
</div>

