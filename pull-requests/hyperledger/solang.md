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
                PR <a href="https://github.com/hyperledger/solang/pull/1059" class=".btn">#1059</a>
            </td>
            <td>
                <b>
                    Fix clippy warnings for rust 1.65.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rust 1.65.0 will be released tomorrow
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 10:07:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1058" class=".btn">#1058</a>
            </td>
            <td>
                <b>
                    Update @solana/solidity version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the `@solana/solidity.js` library version in order to make integration tests pass again.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 20:38:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1057" class=".btn">#1057</a>
            </td>
            <td>
                <b>
                    Add check for SPDX headers
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
        Created At 2022-10-31 10:40:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1055" class=".btn">#1055</a>
            </td>
            <td>
                <b>
                    Add Serialize [derive] using serde crate.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Hi there, 
I would like to add some derive `Serialize, Deserialize` over most of the objects. 
This will permit us to get the **AST** in **JSON** and then help us interface with **JSON** tools already created.
Thanks! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-29 14:05:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1053" class=".btn">#1053</a>
            </td>
            <td>
                <b>
                    🚀 Use Borsh encoding everywhere on Solana ⚓
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                This PR includes many changes in order to enable Borsh encoding everywhere on Solana. Here is a list of all of them:

1. Borsh encoding is used whenever we need to encode or decode things on Solana.
2. There is now a single interface for AbiEncoding that is used by both Borsh and Scale codecs.
3. CFG expressions the encoder normally utilizes are now wired up in constant folding and strength reduce to optimize the output.
4. All Solana runtime tests now use `BorshToken` for arguments and returns instead of `ethabi::Token`.
5. Integration tests and Anchor tests underwent many changes to accommodate the new encoding scheme.
6. `ethabiencoder.rs` has been deleted.
7. Borsh encoding now saves to a variable all basic types that are read from buffer. This made the code less optimal, but solved the problem with `Expression::ReturnData`. A fix has been suggested int #1054.


Integration tests are failing because the Typescript library needs [this PR](https://github.com/solana-labs/solana-solidity.js/pull/44) merged in order to work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-27 14:01:38 +0000 UTC
    </div>
</div>

