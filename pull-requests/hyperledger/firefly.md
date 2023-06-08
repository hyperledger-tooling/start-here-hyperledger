---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1338" class=".btn">#1338</a>
            </td>
            <td>
                <b>
                    v1.2: Backport fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of the following fixes:

https://github.com/hyperledger/firefly/pull/1249
https://github.com/hyperledger/firefly/pull/1275
https://github.com/hyperledger/firefly/pull/1313
https://github.com/hyperledger/firefly/pull/1316
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 18:14:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1337" class=".btn">#1337</a>
            </td>
            <td>
                <b>
                    Fix coverage drop in aggregator
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
        Created At 2023-06-07 16:38:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1336" class=".btn">#1336</a>
            </td>
            <td>
                <b>
                    Surface message rejection reason to API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposal to add a "reject_reason" to messages (ie to database and API), which will be populated with the error text whenever a message is rejected. Previously this reason would only be logged, so the hope is that this assists in debugging when a message is rejected for an unexpected reason.

Note that this does slightly reduce the performance of inserting rejected messages, because we must insert them one-by-one instead of in one large update (but I think the net benefit of having the extra info far outweighs the cost, since this is a non-happy path anyway).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 15:40:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1335" class=".btn">#1335</a>
            </td>
            <td>
                <b>
                    Update idempotency.md to fix sentence
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
        Created At 2023-06-07 09:53:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1334" class=".btn">#1334</a>
            </td>
            <td>
                <b>
                    Move idempotency key architecture docs into main docs site
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
        Created At 2023-06-07 01:44:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1333" class=".btn">#1333</a>
            </td>
            <td>
                <b>
                    fix: multiple named tuple result from contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                Fixes EVM queries for:

### Functions with multiple return values

```solidity
function myFunction() public view returns (uint256, uint256) 
```

Result of JSON will become:

```js
{
  "output": "12345",
  "output1": "12345" // prior to this PR, this value was missing
}
```

### Functions with  named return values

```solidity
function myFunction() public view returns (myvalue uint256) 
```

```js
{
  "myvalue": "12345" // prior to this PR, this value was missing (empty object returned)
}
```

### Functions with multiple named return values

```solidity
function myFunction() public view returns (my1 uint256, my2 uint256, my3 uint256) 
```

```js
{
  "my1": "12345", // all these values were missing (empty object returned)
  "my2": "12345",
  "my3": "12345" 
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 14:38:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1332" class=".btn">#1332</a>
            </td>
            <td>
                <b>
                    Add fftokens docs on /deactivatepool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New API added to fftokens API spec by these PRs:

https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/136
https://github.com/hyperledger/firefly-tokens-erc1155/pull/125
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 14:21:38 +0000 UTC
    </div>
</div>

