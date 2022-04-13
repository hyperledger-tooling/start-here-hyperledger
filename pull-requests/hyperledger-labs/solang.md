---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/740" class=".btn">#740</a>
            </td>
            <td>
                <b>
                    Calling internal function type broken on solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This has been broken for some time, clearly it was missing a test case.

Fixes issue #733.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 09:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    Shift on integer struct member causes panic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The syntax `self._x >> 112` causes a panic because retrieving the bit
width of a referene to an integer is broken.

Fixes issue #732.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 09:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/738" class=".btn">#738</a>
            </td>
            <td>
                <b>
                    Sema test for casting destructure values is broken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When the left hand side of a destructure statements is a structure member or array element, the test incorrectly assumed the value was not assignable.
    
Fixes issue #734.
    

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 09:06:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/737" class=".btn">#737</a>
            </td>
            <td>
                <b>
                    Update the development progress in README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm updating our README.md with our latest development progresses. 🥳
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 17:38:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    More info for overload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix https://github.com/hyperledger-labs/solang/issues/707

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 15:22:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/735" class=".btn">#735</a>
            </td>
            <td>
                <b>
                    Update links to discord to the correct channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The links to discord chat is to the discord server, but we can do better
than that and link to the correct channel on the server.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 14:41:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/734" class=".btn">#734</a>
            </td>
            <td>
                <b>
                    chore: typo fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 14:16:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/730" class=".btn">#730</a>
            </td>
            <td>
                <b>
                    struct member expressions are not written to graphviz dot file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The handling was incorrect and no nodes were generated.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 13:18:08 +0000 UTC
    </div>
</div>

