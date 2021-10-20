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
                PR <a href="https://github.com/hyperledger/besu/pull/2931" class=".btn">#2931</a>
            </td>
            <td>
                <b>
                    GoQuorum static flag reset missing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes 2 spots where the static flag was not being reset to the default value.
More permanent refactor is happening here - https://github.com/hyperledger/besu/pull/2805

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 04:21:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2930" class=".btn">#2930</a>
            </td>
            <td>
                <b>
                    fix difficulty gauge metric in stratumserver, add simple test coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
fix a divide by zero issue in stratum server difficulty metrics gauge.

These resources are useful to understand the calculation:
* https://eth.wiki/en/concepts/ethash/ethash#Mining
* https://github.com/hyperledger/besu/blob/main/ethereum/blockcreation/src/main/java/org/hyperledger/besu/ethereum/blockcreation/PoWBlockCreator.java#L89-L92

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2921 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 20:24:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2929" class=".btn">#2929</a>
            </td>
            <td>
                <b>
                    corrects typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Corrects typo in method name.

## Changelog

- [X ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 19:44:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2928" class=".btn">#2928</a>
            </td>
            <td>
                <b>
                    Upgrade OpenJDK used by CircleCI to version 11.0.12 [#2927]
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
Upgrade OpenJDK used by CircleCI to version 11.0.12

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2927
## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 13:53:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2926" class=".btn">#2926</a>
            </td>
            <td>
                <b>
                    [#2925] Update JDK 11 to latest version in Besu Docker images 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                AdoptOpenJDK project is now deprecated.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Replace AdoptOpenJDK base image for Java 11, with the updated base image provided by Eclipse Temurin.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2925

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 12:43:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2924" class=".btn">#2924</a>
            </td>
            <td>
                <b>
                    Simplify clock in ValidatorContractTest
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
        Created At 2021-10-19 05:56:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2923" class=".btn">#2923</a>
            </td>
            <td>
                <b>
                    QBFT Contract based validators Acceptance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">consensus</span>
            </td>
            <td>
                ## PR description
Add Acceptance test for QBFT contract based validators [#2620]

Signed-off-by: Usman Saleem <usman@usmans.info>

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 03:12:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2922" class=".btn">#2922</a>
            </td>
            <td>
                <b>
                    [MINOR] Typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed some typos

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 01:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2919" class=".btn">#2919</a>
            </td>
            <td>
                <b>
                    propagate the changelog and next version from RC3 release to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

propagate changelog and version from RC3 branch to main

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 16:29:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2918" class=".btn">#2918</a>
            </td>
            <td>
                <b>
                    [#2454] Set gas fees to zero when simulating a transaction without enforcing balance checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                Before, when the `strict` was set to `false`, we set the sender balance to the maximum allowed, but this had
side effects in smart contracts that use `msg.sender.balance`.

With this change, setting `strict` field to `false` in the `eth_call` call, forces gas fees to be set to zero,
so the execution of the transaction is not constrained to the balance of the sender.

There are limitations on what can be simulated with `strict: false`:

- The sender cannot send a value higher than its balance.
- Be aware that `gasPrice` and `baseFee` are set to zero, when simulating smart contract calls.

Removing these limitations requires some effort to add a simulation mode to the way transaction are processed,
that do not seem to be worth, since an user could always use an account with enough balance on a test network,
to simulate the call.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#2454 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 13:57:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2917" class=".btn">#2917</a>
            </td>
            <td>
                <b>
                    EVM Speed Improvements for MSTORE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR Description

More EVM Speed Improvements aimed at improving MSTORE times.
* Move Memory from raw bytes to byte array
* Add calls for 32 byte MSB aligned writes
* Remove `incrementProgramCounter` and move data into OperationResult

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 00:19:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2916" class=".btn">#2916</a>
            </td>
            <td>
                <b>
                    2705 - logging unused request fields during serialization for JsonCallParameter class
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

- used the @JsonAnySetter marker annotation to catch unused request fields and log their values and class type for JsonCallParameter.java domain class.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fix for #2705 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-17 17:45:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2911" class=".btn">#2911</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.10.0-RC4-SNAPSHOT
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
        Created At 2021-10-15 17:44:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2910" class=".btn">#2910</a>
            </td>
            <td>
                <b>
                    Release 21.10.0-RC3
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
        Created At 2021-10-15 17:13:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2909" class=".btn">#2909</a>
            </td>
            <td>
                <b>
                    Added log for validator selection mode transition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Add a log message when validator selection mode changes between blocks
- Notification logic implemented on `QbftTransitionNotifier`
- Check happens upon creation of a new `QbftBlockHeighManager` in the corresponding factory. That means that we notify before the transition actually happens, to help diagnose any issues with the transition that is about to happen (e.g. wrong address for the validator contract).

Example messages:
```
Transitioning validator selection mode from blockheader to contract (address: 0x0000000000000000000000000000000000008888)

Transitioning validator selection mode from contract (address: 0x0000000000000000000000000000000000008888) to blockheader

Transitioning validator selection mode from contract (address: 0x0000000000000000000000000000000000008888) to contract (address: 0x0000000000000000000000000000000000007777)
```

## Fixed Issue(s)
fixes #2784

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 01:53:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2908" class=".btn">#2908</a>
            </td>
            <td>
                <b>
                    Always copy create code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Always copy the create code. Since it is memory bytes it is subject to
re-writing by the caller and all data would otherwise have to be treated
 as mutable.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>


## Fixed Issue(s)
#2899

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 17:04:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2904" class=".btn">#2904</a>
            </td>
            <td>
                <b>
                    Add trace_filter API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR adds the trace_filter API. This API returns traces matching given filter

    fromBlock:  trace will start at this block (optional) .
    toBlock:race will stop at this block (optional) .
    fromAddress: only traces with this senders  (optional) .
    toAddress: only traces with this destination addresses  (optional) .
    after: the offset 
    count:  maximum number of traces to return

#### Request
```json
{
    "jsonrpc": "2.0",
    "method": "trace_filter",
    "params": [
      {
        "fromBlock": "0x1",
        "toBlock": "0x21",
        "after": 2,
        "count": 2,
        "fromAddress": [
          "0xfe3b557e8fb62b89f4916b721be55ceb828dbd73"
        ]
      }
    ],
    "id": 415
  }
```


#### Response
```json
{
    "jsonrpc": "2.0",
    "result": [
      {
        "action": {
          "callType": "call",
          "from": "0xfe3b557e8fb62b89f4916b721be55ceb828dbd73",
          "gas": "0xffad82",
          "input": "0x0000000000000000000000000000000000000999",
          "to": "0x0020000000000000000000000000000000000000",
          "value": "0x0"
        },
        "blockHash": "0xcd5d9c7acdcbd3fb4b24a39e05a38e32235751bb0c9e4f1aa16dc598a2c2a9e4",
        "blockNumber": 6,
        "result": {
          "gasUsed": "0x7536",
          "output": "0x"
        },
        "subtraces": 1,
        "traceAddress": [],
        "transactionHash": "0x91eeabc671e2dd2b1c8ddebb46ba59e8cb3e7d189f80bcc868a9787728c6e59e",
        "transactionPosition": 0,
        "type": "call"
      },
      {
        "action": {
          "callType": "call",
          "from": "0xfe3b557e8fb62b89f4916b721be55ceb828dbd73",
          "gas": "0xffad52",
          "input": "0xf000000000000000000000000000000000000000000000000000000000000001",
          "to": "0x0030000000000000000000000000000000000000",
          "value": "0x0"
        },
        "blockHash": "0xeed85fe57db751442c826cfe4fdf43b10a5c2bc8b6fd3a8ccced48eb3fb35885",
        "blockNumber": 7,
        "result": {
          "gasUsed": "0x1b",
          "output": "0xf000000000000000000000000000000000000000000000000000000000000002"
        },
        "subtraces": 0,
        "traceAddress": [],
        "transactionHash": "0x47f4d445ea1812cb1ddd3464ab23d2bfc6ed408a8a9db1c497f94e8e06e85286",
        "transactionPosition": 0,
        "type": "call"
      }
    ],
    "id": 415
  }
```

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 09:11:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2903" class=".btn">#2903</a>
            </td>
            <td>
                <b>
                    fix some flakey onchain privacy tests (ConsenSys/protocol-misc#419)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ConsenSys/protocol-misc#419 lists a number of onchain privacy acceptance tests that are flakey. 

All these tests fail because of a timeout while checking that a privacy group has been created on all the member nodes.

This PR changes the timeout from the default 10s to 20s

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 05:09:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2902" class=".btn">#2902</a>
            </td>
            <td>
                <b>
                    Bft block period transition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">consensus</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Allow the Bft block period to be changed using a transition. This allows the block period to be changed in either IBFT2 or QBFT.

Example configuration for ibft2 to change the block period to 4 seconds at block 1240 would be:
```
"transitions": {
	"ibft2": [
		{
			"block": 1240,
			"blockperiodseconds": 4
		}
	]
}
```		

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 04:06:15 +0000 UTC
    </div>
</div>

