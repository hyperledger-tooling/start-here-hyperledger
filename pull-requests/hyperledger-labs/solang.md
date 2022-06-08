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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/863" class=".btn">#863</a>
            </td>
            <td>
                <b>
                    Fix right side of the Loc of ContractDefinition
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
        Created At 2022-06-08 17:47:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/862" class=".btn">#862</a>
            </td>
            <td>
                <b>
                    Move to latest solana-rbpf crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This crate is used for solana tests. The version used before this commit has an security issue:

Solana solana_rbpf before 0.2.29 has an addition integer overflow via invalid ELF program headers. elf.rs has a panic via a malformed eBPF program.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 09:01:37 +0000 UTC
    </div>
</div>

