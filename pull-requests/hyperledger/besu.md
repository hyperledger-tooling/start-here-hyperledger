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
                PR <a href="https://github.com/hyperledger/besu/pull/3510" class=".btn">#3510</a>
            </td>
            <td>
                <b>
                    Refactor trace api methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Refactor trace api methods to pave way for 
https://github.com/hyperledger/besu/pull/3459
https://github.com/hyperledger/besu/pull/3477
https://github.com/hyperledger/besu/pull/3468

Two abstract classes for code reuse and minimise the amount of merge conflict needed fixing

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 04:21:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3508" class=".btn">#3508</a>
            </td>
            <td>
                <b>
                    3465 jwt auth
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
If merge and jwt auth is enabled, starts the Engine API (both websockets and http) requiring JWT auth as described in Kiln2 spec.

Extracts an AuthenticationService interface and provides a Default (legacy) implementation alongside an Engine specific implementation. Either may be used from HTTP or Websocket stacks.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3465 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 22:27:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3505" class=".btn">#3505</a>
            </td>
            <td>
                <b>
                    [Issue 3115] Support mining beneficiary transitions
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
Add the ability to transition the `miningbeneficiary` for *bft (ibft2, qbft) consensus mechanisms. 

Example genesis file with `miningbeneficiary` transitions:
```
{
  "config": {
    "chainId": 999,
    "byzantiumBlock": 0,
    "ibft2": {
      "blockperiodseconds": 1,
      "epochlength": 30000,
      "requesttimeoutseconds": 5,
      "blockreward": "5000000000000000000",
      "miningbeneficiary": "0x0000000000000000000000000000000000000001"
    }
  },
  "transitions": {
    "ibft2": [
        {
            "block": 10000, 
            "miningbeneficiary": "",
        },
        {
            "block": 20000, 
            "miningbeneficiary": "0x0000000000000000000000000000000000000002",
        }
    ]
  }
  ...
}
```
The `miningbeneficiary` will only be updated if there is a "miningbeneficiary" key in the `transitions.ibft2` array element.  Setting the `miningbeneficiary` to an empty value will clear out any override so that block rewards go to the miner rather than a global override address.  

Other changes:
* Keep the miningbeneficiary as an `Address` rather than a `String` in `BftConfigOptions` and make the conversion from `String` to `Address` strict (i.e. all 20 address bytes are required "0x01" is not valid). 
* Fix `ThreadBesuNodeRunner` so that it respects a node's genesis config.


## Fixed Issue(s)
Fixes #3115

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 17:05:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3503" class=".btn">#3503</a>
            </td>
            <td>
                <b>
                    Add GitHub action to verify gradle-wrapper.jar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Checks that the gradle wrapper jar is from an official release since a maliciously modified jar added as part of a gradle upgrade would be a significant security risk but is hard to verify from the code diff.  This checks the jar comes from an Official Gradle release.

See https://github.com/gradle/wrapper-validation-action for more details.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 04:42:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3502" class=".btn">#3502</a>
            </td>
            <td>
                <b>
                    Update ef bootnodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Updates ef bootnode addresses
Geth PR: https://github.com/ethereum/go-ethereum/pull/24432

## Fixed Issue(s)
fixes #3488 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 02:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3501" class=".btn">#3501</a>
            </td>
            <td>
                <b>
                    Bugfix/terminal block check
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
Ensure besu correctly checks for latest ancestor before checking if a block descends from terminal.  

Also, forkchoiceUpdated calls for finalized blocks which besu does not have should start or append to a backward sync.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3500

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 23:32:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3499" class=".btn">#3499</a>
            </td>
            <td>
                <b>
                    Improve contract validation errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

For each contract validation error return a relevant error instead of
the incorrect "INSUFFICIENT_GAS" error.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 17:02:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3497" class=".btn">#3497</a>
            </td>
            <td>
                <b>
                    Prepare for release 22.1.2 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Prepare for release 22.1.2

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 00:44:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3496" class=".btn">#3496</a>
            </td>
            <td>
                <b>
                    Release 22.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Release 22.1.1

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 18:55:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3495" class=".btn">#3495</a>
            </td>
            <td>
                <b>
                    Rename field random to prevRandao
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

Renames the field `random` in ExecutionPayloadV1, PayloadAttributesV1 and the block header to `prevRandao` to be Kiln spec v2 compatible.

## PR description

## Fixed Issue(s)
fixes #3490

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 14:04:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3494" class=".btn">#3494</a>
            </td>
            <td>
                <b>
                    [MINOR] remove orion refs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Removed some orion references

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 02:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3493" class=".btn">#3493</a>
            </td>
            <td>
                <b>
                    3378 ws engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

## PR description
Implements the engine API via websockets.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #3378 

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 01:32:18 +0000 UTC
    </div>
</div>

