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
                PR <a href="https://github.com/hyperledger/solang/pull/993" class=".btn">#993</a>
            </td>
            <td>
                <b>
                    Remove references to hyperledger-labs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solang has moved into incubation, so now the repo can be found at
https://github.com/hyperledger/solang

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 20:28:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/990" class=".btn">#990</a>
            </td>
            <td>
                <b>
                    WIP: test: initial subxt test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                alternative tests using subxt, currently using raw selector until the ABI are compatible where we can just use contract-transcode.
test cases are semantically derived from the original substrate integration tests using polkadot.js.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-28 05:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/989" class=".btn">#989</a>
            </td>
            <td>
                <b>
                    WIP: Feature ink metadata for substrate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                attempt to generate ink compatible metadata using ink_metadata::InkProject
currently relies on unmerged branched of scale-info, ink_metadata.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 07:35:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/988" class=".btn">#988</a>
            </td>
            <td>
                <b>
                    Multiplication overflow detection for integer width > 64 bits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: salaheldinsoliman <salaheldin_sameh@aucegypt.edu>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 03:15:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/987" class=".btn">#987</a>
            </td>
            <td>
                <b>
                    Create 'writeString' and 'writeBytes'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates `writeStringData` and `writeBytesData` functions that write only the contents of strings and bytes arrays into a buffer. They are useful for using bincode when creating a library for System Instructions on Solana.

For arrays (strings and bytes included) bincode encodes lengths in `u64`, so borsh encoding cannot be used for this case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 19:31:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/985" class=".btn">#985</a>
            </td>
            <td>
                <b>
                    Generate solidity interface from Anchor IDL files so that anchor contracts can be called
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
        Created At 2022-08-23 18:59:45 +0000 UTC
    </div>
</div>

