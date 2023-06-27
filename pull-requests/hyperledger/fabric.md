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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4292" class=".btn">#4292</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: isolate common subcomponents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I274d8883add91fac08da5202199d1bac53e99adb

#### Type of change

- New feature

#### Description
- Isolate subcomponents from the CFT Deliverer that can be used in the BFT Deliverer
- A skeleton of the BFT Deliverer (no censurship monitor, no tests)

#### Related issues
#4293 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 16:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4291" class=".btn">#4291</a>
            </td>
            <td>
                <b>
                    update of fabric-config version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- update

#### Description

update fabric-config version in go.mod

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 08:33:14 +0000 UTC
    </div>
</div>

