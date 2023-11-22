---
layout: default
title: aries-framework-kotlin
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-kotlin
---

# aries-framework-kotlin <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-kotlin){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-kotlin/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Added handling of server side problem reports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Problem reports from the cloud agent were not handled by the wallet.

This PR adds handling of problem reports so that they can be received and processed by the application layer.

Tested against `aca-py`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 10:10:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-kotlin/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    Fix crash during pickup if network is turned off
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the current implementation, if the network is turned off, pickup of messages causes an application crash.

This PR fixes this by silently ignoring crashes during a pickup (as pickup will be retried at the polling frequency specified).

Also, there was no exception handling during the establishment of a connection (in the `WalletMainActivity`), this has been fixed too.

@conanoc / @DrumRobot request you to review this and merge. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 07:47:42 +0000 UTC
    </div>
</div>

