---
layout: default
title: aries-framework-swift
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-swift
---

# aries-framework-swift <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-swift){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Fix crash when there are multiple attributes to prove
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #44

Swift collections are not thread-safe, so we need a lock when updating them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 07:25:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Support build on XCode 14
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix #48

XCode 14 requires the minimum deployment target to be ios11. Added a post-install script to adjust deployment targets following [this tip](https://github.com/CocoaPods/CocoaPods/issues/9884#issuecomment-908835911)

The drawback of this approach is that users of this framework have to add the same script to their Podfile.
Changing the podspec files of all the dependent pods by cloning them to our repo would be a very challenging task.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 06:41:55 +0000 UTC
    </div>
</div>

