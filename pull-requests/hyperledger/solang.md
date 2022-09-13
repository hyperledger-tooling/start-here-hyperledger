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
                PR <a href="https://github.com/hyperledger/solang/pull/1012" class=".btn">#1012</a>
            </td>
            <td>
                <b>
                    Add semantic information to CFG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should help @salaheldinsoliman implement overflow detection for constants in the CFG. It adds information about the origin of each instruction to the CFG. Each instruction is now classified either as from Solidity, Yul or Codegen.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 21:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1011" class=".btn">#1011</a>
            </td>
            <td>
                <b>
                    Fix function calls via contract name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Disallow direct access to functions (and constants) except for base contracts. This is not valid in `solc` but was allowed in solang.

Fixes #1007 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 12:16:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1010" class=".btn">#1010</a>
            </td>
            <td>
                <b>
                    constant arthimeteic overflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Check for constant arthimetic overflow during semantic analysis.
Signed-off-by: salaheldinsoliman <salaheldin_sameh@aucegypt.edu>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 21:11:31 +0000 UTC
    </div>
</div>

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

