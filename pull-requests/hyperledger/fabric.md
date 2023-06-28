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
                PR <a href="https://github.com/hyperledger/fabric/pull/4301" class=".btn">#4301</a>
            </td>
            <td>
                <b>
                    remove kafka from documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

update documentation regarding the removal of Kafka

#### Related issues

issue #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 15:05:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4299" class=".btn">#4299</a>
            </td>
            <td>
                <b>
                    Create CITATION.cff
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Please create a CITATION.cff file so researchers can cite this repo. Thank you.

#### Additional details


#### Related issues






            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 14:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4298" class=".btn">#4298</a>
            </td>
            <td>
                <b>
                    update Fabric to include fabric-config latest commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- dependency update


#### Description

update fabric-config version to include the latest commit

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:08:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4297" class=".btn">#4297</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: Stop deliver service correctly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Change-Id: Icd1725913e3be913b3628b3f37e252c8e13a0461

#### Type of change
- Bug fix

#### Description

After the delivery service StopDeliveryForChannel is called, it should be possible to call StartDeliveryForChannel  again.
After the delivery service Stop is called, it should not be possible to call <Start/Stop>DeliveryForChannel  again.

This was introduced by #4260

#### Related issues

#4261 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 16:18:16 +0000 UTC
    </div>
</div>

