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
                PR <a href="https://github.com/hyperledger/solang/pull/1008" class=".btn">#1008</a>
            </td>
            <td>
                <b>
                    Emit events using Borsh encoding for Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the new scheme for events emission on Solana. It follows Anchor strategy for events.

[According to Anchor source code](https://github.com/coral-xyz/anchor/blob/0c70d183ef9187cef576749e4fee8f443e4dbc34/lang/attribute/event/src/lib.rs#L86-L88), `indexed` fields are emitted as data. In addition, all fields are encoded using borsh encoding, and [the result is passed directly](https://github.com/coral-xyz/anchor/blob/0c70d183ef9187cef576749e4fee8f443e4dbc34/lang/attribute/event/src/lib.rs#L77-L84) to `sol_log_data`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 14:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1006" class=".btn">#1006</a>
            </td>
            <td>
                <b>
                    Substrate constructor overloading names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since in `ink!` constructors also have names. This is another precondition for making #989 happen.

As discussed in our daily: We could easily extend this for solana as well. Additionally we will probably want to have a way for instantiating contracts using various constructors, which is impossible using solidity syntax.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 13:31:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    Fix overflow detection tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Numbers that overflow the input type was generated, causing some overflow detection tests to fail
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 21:24:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1002" class=".btn">#1002</a>
            </td>
            <td>
                <b>
                    Solana NFT example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates a Solidity contract to manage NFTs on Solana. It is an example to show Solang functionality during Solana's Singapore Hacker House. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 20:16:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    Improve vscode extension documentation
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
        Created At 2022-09-02 13:11:33 +0000 UTC
    </div>
</div>

