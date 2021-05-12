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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    Fix nested mappings in Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Uniswap v2 has the following mapping which fails to compile.

	mapping(address => mapping(address => uint)) public allowance;

Fix this and other nested mappings.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 23:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    Implement block.timestamp for Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 16:08:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    Implement this for Solana
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
        Created At 2021-05-09 12:00:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    functions ripemd160(), sha256(), and keccak256() for Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ripemd160 has its own implementation, and sha256 uses a syscall. The
keccak256() function relies on sol_keccak256() syscall which is not
available yet.

See https://github.com/solana-labs/solana/pull/16498

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-08 10:57:56 +0000 UTC
    </div>
</div>

