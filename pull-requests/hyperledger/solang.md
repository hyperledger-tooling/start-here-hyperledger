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
                PR <a href="https://github.com/hyperledger/solang/pull/1211" class=".btn">#1211</a>
            </td>
            <td>
                <b>
                    Refactor scale decoder into codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Decoding for `abi.decode` is now done in codegen. Like with the encoder, most of the code can be shared with the borsh decoder.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-04 21:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1210" class=".btn">#1210</a>
            </td>
            <td>
                <b>
                    Remove unnecessary files from solang crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These files bloat the crate file without any function. The list of files can be seen with `cargo package --list`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1209" class=".btn">#1209</a>
            </td>
            <td>
                <b>
                    Bump solang-parser version for crate publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note we don't want to include the entire solc source tree in the crate, so exclude all the testdata.

New version is required for `forge fmt`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 14:00:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1208" class=".btn">#1208</a>
            </td>
            <td>
                <b>
                    Simplify switch in constant folding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I was checking if `fn block_edges` could be pre-calculated during CFG generation, for we call it six times (one more after we collect all Solana accounts). The only problem would be constant folding, which simplifies branches. While I was checking that, I realized we could simplify switches before trying to remove `fn block_edges`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 23:04:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1207" class=".btn">#1207</a>
            </td>
            <td>
                <b>
                    Update LLVM installation steps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The CMAKE command must indicate we are not building zstd. 

PS: The indentation is now fixed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 22:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1206" class=".btn">#1206</a>
            </td>
            <td>
                <b>
                    Fix flipper.sol example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR moves `example/flipper.sol` to the substrate examples folder and fixes the references in the docs. It also updates the README example with the correct contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 22:28:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1204" class=".btn">#1204</a>
            </td>
            <td>
                <b>
                    Add Hyperledgers' suggestions for inclusivity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The DCI  tool is marked `continue-on-error` for now, due to https://github.com/petermetz/gh-action-dci-lint/issues/2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 11:20:08 +0000 UTC
    </div>
</div>

