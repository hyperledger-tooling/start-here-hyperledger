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
                PR <a href="https://github.com/hyperledger/fabric/pull/3646" class=".btn">#3646</a>
            </td>
            <td>
                <b>
                    Improves image size for better readability
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

Removes the height of the image *getting_started_image2.png* to improve the readability.

#### Additional details

![Screenshot from 2022-09-23 15-29-37](https://user-images.githubusercontent.com/7544858/192047532-181550e3-cd31-4e31-a0b9-5f156b66e7fb.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 19:59:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3643" class=".btn">#3643</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove solo from integration tests (1)
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

Remove solo from integration tests (part 1)

#### Related issues

Issue: #3514 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 13:32:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3642" class=".btn">#3642</a>
            </td>
            <td>
                <b>
                    verify leadership transfer status before waiting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description
The thread which was waiting on the notifyc channel was not notified as the other thread well passed the execution before the channel gets established/initialized. Its a race condition between these 2 threads lead to the test case failure. Added additional check to check the status before waiting for notification from other go routine.

#### Related issues
#3629 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 19:02:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3641" class=".btn">#3641</a>
            </td>
            <td>
                <b>
                    Ordrer v3: stop using solo in orderer/common/server unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I00846aa130d5b9fb486ace5f84898a0b0affddf5

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Stop using solo in orderer/common/server unit tests

#### Related issues

Issue: #3514 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 12:01:56 +0000 UTC
    </div>
</div>

