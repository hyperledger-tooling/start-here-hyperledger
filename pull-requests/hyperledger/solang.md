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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1357" class=".btn">#1357</a>
            </td>
            <td>
                <b>
                    Use custom substrate CI image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use [a custom node](https://github.com/hyperledger/solang-substrate-ci) for the integration tests. This tests contains chain extension which I'll add integration tests for in a followup PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 17:51:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1356" class=".btn">#1356</a>
            </td>
            <td>
                <b>
                    Improve unused variable elimination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following code causes an invalid memory access:

```solidity
function foo() public pure returns (bytes memory) {
    bytes b1 = hex"41";
    bytes b2 = hex"42";
 
   b2.push(0x41);
   return b1;
}

```

That happens because the unused variable elimination removes the declaration `bytes b2`, but maintains the `push`. This PR improves the elimination algorithms so much so that it removes the unnecessary pushes and pops if there is no actual read to the array in the function. It also takes care not to discard such operations when arrays are pointers to either storage or memory.

In addition, the error message for unused function parameter has been updated to `function parameter 'my_parameter' is unused`. When the parameter is a vector and has a push but no read, writing that it is `never read` is not the proper warning.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 21:17:15 +0000 UTC
    </div>
</div>

