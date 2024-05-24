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
                PR <a href="https://github.com/hyperledger/solang/pull/1645" class=".btn">#1645</a>
            </td>
            <td>
                <b>
                    Soroban counter.sol example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to make Solang support a simple counter.sol example on Soroban, where a storage variable is instatiated, modified and retrieved. 

- [x] Support Soroban storage function calls `put_contract_data`, `get_contract_data` and `has_contract_data`
- [x] Implement a wrapper `init` for `storage_initializer` 
- [x] Implement wrappers for public functions
- [x] Insert decoding/encoding instructions into the wrapper functions 
- [x] Soroban doesn't have function return codes. This needs to be handled all over emit
- [ ] Add integration tests and MockVm tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-18 15:29:40 +0000 UTC
    </div>
</div>

