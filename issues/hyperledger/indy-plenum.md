---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/indy-plenum/issues/1507" class=".btn">1507</a>
            </td>
            <td>
                <b>
                    Replace dependency on Indy SDK with Indy VDR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">help wanted</span>
            </td>
            <td>
                [Indy-VDR](https://github.com/hyperledger/indy-vdr) is receiving more development than [Indy-SDK](https://github.com/hyperledger/indy-sdk), so we should replace calls to libindy with calls to indy-vdr.

Steps:
* Update unit tests.
* Update integration tests.
* Update package dependencies.

Notes:
* [Related issue in Indy Node](https://github.com/hyperledger/indy-node/issues/1644).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-01-29 22:55:12 +0000 UTC
    </div>
</div>

