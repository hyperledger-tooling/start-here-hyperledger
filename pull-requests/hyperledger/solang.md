---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1111" class=".btn">#1111</a>
            </td>
            <td>
                <b>
                    Increase timeout on Solana integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These regularly fail with timeouts, maybe this will work.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 09:27:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1110" class=".btn">#1110</a>
            </td>
            <td>
                <b>
                    Fix assignment chains
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix assigning to both a storage variable and non-storage in assignment chain.

Fixes https://github.com/xermicus/fuzzy-sol/issues/142

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 13:27:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1109" class=".btn">#1109</a>
            </td>
            <td>
                <b>
                    super should not consider parents without a body
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the parent is an interface, don't use a function from that for super, as it is uncallable and will generate bogus code.

Fixes: https://github.com/xermicus/fuzzy-sol/issues/128

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 12:53:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1108" class=".btn">#1108</a>
            </td>
            <td>
                <b>
                    Fix handling of new int[](count <<= 1)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also improves handling of any garbage passed as a size.

Fixes https://github.com/xermicus/fuzzy-sol/issues/146

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 10:55:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1107" class=".btn">#1107</a>
            </td>
            <td>
                <b>
                    Give nice diagnostics when old style call arguments are used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                	C c = (new C).value(1).gas(2)(1, 2, 3);

Fixes https://github.com/xermicus/fuzzy-sol/issues/141

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 18:37:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1105" class=".btn">#1105</a>
            </td>
            <td>
                <b>
                    Make instruction data compatible with anchor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span><span class="chip">breaking</span>
            </td>
            <td>
                *Solana* breaking change.For constructors, a function selector is now required.
    
Remove the following from the instruction data:
  - Sender
  - Destination
  - Value
  - Seeds
  - Contract hash

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 17:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1104" class=".btn">#1104</a>
            </td>
            <td>
                <b>
                    Generate Anchor IDL from Solidity contracts ⚓
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                This PR generates Anchor ⚓ IDL files for Solidity contracts. There are unit tests for the functions that construct the `struct IDL`. All Solana runtime tests have been updated to leverage Anchor IDL instead of Ethereum ABI.

The final json file is not generated when we compile a Solidity contract to avoid confusing users with files that are not yet useful for them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 21:11:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1103" class=".btn">#1103</a>
            </td>
            <td>
                <b>
                    Ensure no data is returned when a function has no return values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 15:47:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1102" class=".btn">#1102</a>
            </td>
            <td>
                <b>
                    Fix rust 1.66 clippy warnings and run crate doc tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 09:45:24 +0000 UTC
    </div>
</div>

