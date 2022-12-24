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
                PR <a href="https://github.com/hyperledger/solang/pull/1115" class=".btn">#1115</a>
            </td>
            <td>
                <b>
                    Arrays indexes must be dereferenced when needed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When we index an array, we have a reference to an element of that array. If the result of an indexation is used to index another array, we must dereference it first, because indexes must be integers.

This PR fixes https://github.com/xermicus/fuzzy-sol/issues/132
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-23 18:49:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1114" class=".btn">#1114</a>
            </td>
            <td>
                <b>
                    The type of a storage offset should be that of the target's storage pointer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calculating the storage offset for a struct, the type of the corresponding addition should not be the struct member type, but instead the type of a storage offset.

This fixes https://github.com/xermicus/fuzzy-sol/issues/115 and https://github.com/xermicus/fuzzy-sol/issues/111
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-23 17:00:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1113" class=".btn">#1113</a>
            </td>
            <td>
                <b>
                    `Expression::CheckingTrunc` should be recursed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes https://github.com/xermicus/fuzzy-sol/issues/143.

I have found two problems:
1. `Expression::CheckingTrunc` should be part of `impl recurse for Expression`. 
2. `impl recurse for CallArgs` should recurse the expression instead of calling the function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-23 14:03:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1112" class=".btn">#1112</a>
            </td>
            <td>
                <b>
                    Fix storage array deref bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes the function `Type::is_storage_bytes()` to account for fixed size bytes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-23 11:46:01 +0000 UTC
    </div>
</div>

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
                The Solana tests sometimes fail with timeouts, maybe this will work.

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

