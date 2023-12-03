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
                PR <a href="https://github.com/hyperledger/solang/pull/1604" class=".btn">#1604</a>
            </td>
            <td>
                <b>
                    No version of Solidity supports octal numbers
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
        Created At 2023-11-30 09:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1603" class=".btn">#1603</a>
            </td>
            <td>
                <b>
                    Fix rust clippies and evm balance length
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
        Created At 2023-11-28 09:28:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1602" class=".btn">#1602</a>
            </td>
            <td>
                <b>
                    Add Soroban target foundations.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a follow up to this  PR: #1138 and #1129 , both of which discuss adding Soroban as a target for Solang.
The PR addresses three main points:
1- Soroban contracts have no dispatcher (a single point of entry). Therefore, externally callable functions in the contract should preserve their original name (if possible).
2- Soroban functions do not have their outputs as pointers in the inputs. Instead, they return the value at the end of execution.
3-Linking Soroban WASM contracts is pretty much similar to Polkadot's WASM, but with the following minor differences:
a- public functions are exported.
b- host functions (of course)

The next steps for this PR would be: (to be followed in another PRs)
1- Implement host function invocations. (The VM interface)
2- Implement XDR encoding and decoding.
3- Add Integration tests, and complete the mock VM implementation in soroban_tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-26 19:01:34 +0000 UTC
    </div>
</div>

