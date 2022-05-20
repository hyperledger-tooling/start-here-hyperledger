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
                PR <a href="https://github.com/hyperledger/besu/pull/3840" class=".btn">#3840</a>
            </td>
            <td>
                <b>
                    don't wrap and re-throw, pollutes logs and causing exception is handl…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ed correctly

Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 20:03:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3839" class=".btn">#3839</a>
            </td>
            <td>
                <b>
                    Fix: getMixHashOrPrevRandao to return the value present in the block header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …he block header

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 16:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3837" class=".btn">#3837</a>
            </td>
            <td>
                <b>
                    Fcu verify payload attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adds payload attributes checks to EngineForkchoiceUpdated and returns INVALID_PAYLOAD_ATTRIBUTES error if any of them should be invalid.

## Fixed Issue(s)
"fixes #3836 "

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-15 22:19:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3835" class=".btn">#3835</a>
            </td>
            <td>
                <b>
                    Ref tests 10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                
## PR description
Upgrade reference Tests to 10.3

10.3 revision of reference tests has notable changes

* Nonce can be up to 2^64-1, with some opcode and validity interactions 
  specced in eip-2681
* Wei fields can be up to 2^256, tests check for rollover
* VM Tests were removed
* Legacy Tests were removed

Includes changes from PR #3747 
 
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-14 07:28:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3834" class=".btn">#3834</a>
            </td>
            <td>
                <b>
                    3619 unify rpc ports
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

- Introduces new JsonRPCService that handles both http and websockets
- Removes websocket specific configs
- renames WebSocketRequestHandler to WebSocketMessageHandler to be more in line with websocket semantics.

## Fixed Issue(s)

fixes #3619 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 16:07:51 +0000 UTC
    </div>
</div>

