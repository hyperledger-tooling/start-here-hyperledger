---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6210" class=".btn">#6210</a>
            </td>
            <td>
                <b>
                    Don't disconnect if insufficient peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For 3 types of infractions, don't actively disconnect
* timeout
* useless response
* IO exception (common from DeFramer)

And, don't do any outbound disconnects if EthPeers count is below maxPeers

With these changes, while below maxPeers, the only disconnects that happen with established peers are those found by removing peers if the connection becomes disconnected. This still happens quite frequently.

TODO - test this PR out on a mainnet node
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 03:11:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6209" class=".btn">#6209</a>
            </td>
            <td>
                <b>
                    worldstate refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

for verkle, I’m starting a refactor. In simple terms, many classes can distinguish whether they’re in ‘bonsai’ or ‘forest’ mode, so a generic interface doesn’t offer much value, except for some minor and synchronization parts.
So, I’ve developed a ’WorldstatestorageCoordinator class. This will have a storage strategy, which could be either ‘bonsai’ or ‘forest’. This coordinator is needed when we’re unsure about the storage mode we use, and it helps for the routing process. when we’re sure about the storage mode, we directly use the appropriate strategy.
This approach reduces the number of generic interfaces, eliminating locations that are not applicable to modes like ‘forest’ or other not clean things like that.
Will be better when we will have to add some custom method or field for verkle

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 10:14:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6207" class=".btn">#6207</a>
            </td>
            <td>
                <b>
                    moved some logs to trace level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span><span class="chip">logging</span><span class="chip">ux</span>
            </td>
            <td>
                * move "Requesting x headers" etc to trace level logging
* use peer.shortNodeId rather than logging the whole peer record
* move "Wrote initial crypto handshake message" to trace
* also a couple of frequently logged tx pool logs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 02:20:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6206" class=".btn">#6206</a>
            </td>
            <td>
                <b>
                    Fix log index in transaction receipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Assign log index to transaction receipt according to position in block instead of in transaction.

## Fixed Issue(s)
fixes #6204 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 15:30:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6205" class=".btn">#6205</a>
            </td>
            <td>
                <b>
                    fix collision issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

The idea of this PR is to revert some modification that was made to pass tests  https://github.com/hyperledger/besu/pull/5686.

Therefore, I decided to revert some modification on this PR by fixing the problem differently. Indeed, the idea of the collision test that does not pass is to selfdestruct a contract and recreate it afterwards. Instead of modifying the logic of the accumulator and listing all the storage leaves to be deleted during the selfdestruct, which seems to lead to edge cases, I prefer to let BonsaiWorldstate handle it as before and just load the storage with EMPTY_TRIE_HASH if we detect that it has been cleared before pushing the new slots after recreation. Indeed, the clearing of the storage that is done at the beginning of calculateRootHash removes the storage but does not change the storage root of the contract. Therefore, we falsely believe that the storage is not empty.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 13:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6202" class=".btn">#6202</a>
            </td>
            <td>
                <b>
                    New cli options to limit rewards return by eth_feeHistory 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
On Goerli: 

##  Test 1

  - api-priority-fee-limiting-enabled=true
  - api-priority-fee-lower-bound-coefficient=120
  - api-priority-fee-upper-bound-coefficient=150
  - min-priority-fee=1

```
eth.feeHistory("0x1", "0x9a6b98", [0,10,20,30,40,50,60,70,80,90,100])
{
  baseFeePerGas: ["0xa", "0xa"],
  gasUsedRatio: [0.17461906666666666],
  oldestBlock: "0x9a6b98",
  reward: [["0x1", "0x1", "0x1", "0x1", "0x1", "0x1", "0x1", "0x1", "0x1", "0x1", "0x1"]]
}

```

##  Test 2

  - api-priority-fee-limiting-enabled=true
  - api-priority-fee-lower-bound-coefficient=15000
  - api-priority-fee-upper-bound-coefficient=150000000000
  - min-priority-fee=1


```
> eth.feeHistory("0x1", "0x9a6b98", [0,10,20,30,40,50,60,70,80,90,100])
{
  baseFeePerGas: ["0xa", "0xa"],
  gasUsedRatio: [0.17461906666666666],
  oldestBlock: "0x9a6b98",
  reward: [["0x96", "0x96", "0x96", "0x96", "0x3b9aca00", "0x3b9aca00", "0x3b9aca00", "0x3b9aca00", "0x59682f00", "0x59682f00", "0x59682f00"]]
}
```

##  Test 3

  - api-priority-fee-limiting-enabled=true
  - api-priority-fee-lower-bound-coefficient=0
  - api-priority-fee-upper-bound-coefficient=9999999999999999
  - min-priority-fee=1

```
eth.feeHistory("0x1", "0x9a6b98", [0,10,20,30,40,50,60,70,80,90,100])

{
  baseFeePerGas: ["0xa", "0xa"],
  gasUsedRatio: [0.17461906666666666],
  oldestBlock: "0x9a6b98",
  reward: [["0x2", "0x2", "0x2", "0x5", "0x3b9aca00", "0x3b9aca00", "0x3b9aca00", "0x3b9aca00", "0x59682f00", "0x721646a2", "0x2ba7def2ff6"]]
}
```



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 06:32:33 +0000 UTC
    </div>
</div>

