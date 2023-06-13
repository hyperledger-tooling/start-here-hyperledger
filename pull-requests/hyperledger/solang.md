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
                PR <a href="https://github.com/hyperledger/solang/pull/1364" class=".btn">#1364</a>
            </td>
            <td>
                <b>
                    Fix codegen tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make the failing case less brittle
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 18:00:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1363" class=".btn">#1363</a>
            </td>
            <td>
                <b>
                    Update Address and Hash types to ink ABI v4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This slipped through integration tests because the frontends remain backwards compatibility. I added a test that would have caught it (based of it, more can be added in the future).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 08:33:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1362" class=".btn">#1362</a>
            </td>
            <td>
                <b>
                    Implement `is_contract` builtin 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1333
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-12 09:49:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1360" class=".btn">#1360</a>
            </td>
            <td>
                <b>
                    Tornado cash on Substrate  :rocket: 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding [tornado cash](https://github.com/tornadocash/tornado-core) as a Substrate integration test.

- The tornado contracts contain minor mechanical changes to compile fine on Substrate. Side note: During the process I discovered a couple of bugs (all fixed in previous PRs); ideally we add many more real world state of the art dApps as integration test.
- For simplicity reasons, the ZK-SNARK setup is just the same as the ETH Tornado on mainnet uses. Because the withdraw key is quite large (600K line json file) I decided to add it as a sub module.
- For compatible proof generation, I factored out the relevant parts from the [tornado CLI](https://github.com/tornadocash/tornado-cli). The tornado CLI code is very tightly coupled to ETH and related chains, no chance to re-use it directly. 
- `circomlib` provides the MiMC sponge hash function as EVM bytecode only, so I implemented them directly in the node as chain extension. I found and tested a Solidity version, but it was so horribly gas-inefficient that merkle tree heights > 4 led to exceeding the transaction refTime limit (tornado uses a merkle tree of height 20). It uses the `u256` type heavily so I don't expect it to be particularly efficient, but it shouldn't be that bad; should be investigated further.
- Addition, multiplication and pairing operations on the `bn128` curve are precompiles on EVM. To make live easy I basically just converted the moonbeam precompiles into a chain extension on our substrate CI node.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 18:44:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1358" class=".btn">#1358</a>
            </td>
            <td>
                <b>
                    Substrate: Add an integration test for chain extensions
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
        Created At 2023-06-06 20:19:09 +0000 UTC
    </div>
</div>

