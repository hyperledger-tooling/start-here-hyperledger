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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1331" class=".btn">#1331</a>
            </td>
            <td>
                <b>
                    Process batch of events from Blockchain connector, in a single DB TX
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                One of the outstanding observations from the performance testing in V1.2 was that we are performing a DB commit for each Blockchain event.

These are sequential on the single logical delivery thread from the blockchain connector (which currently is server-wide, although that should itself become namespace-wide).

This PR proposes that instead we update all the internal callback interfaces, to propagate the batch of events that come in over the wire from the connector, through to the event processor.

This means a few things handled in this PR:
1. Handling a batch that contains events of multiple types -  Batch Pin, Network Action, or custom Blockchain Event Listener
2. Handling a batch that needs different events dispatching to different namespaces
3. Continuing to handle old events that didn't come with a namespace at all (these are dispatched to all registered namespaces)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 05:48:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1330" class=".btn">#1330</a>
            </td>
            <td>
                <b>
                    feat: TLS Configs for Webhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sitting in draft as there is some more extend testing that needs to be done but this is the general idea I was going for. 

Have tested it e2e with a local server secured with mTLS and it works.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 16:37:51 +0000 UTC
    </div>
</div>

