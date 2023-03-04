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
                PR <a href="https://github.com/hyperledger/besu/pull/5157" class=".btn">#5157</a>
            </td>
            <td>
                <b>
                    Burn-in candidate #1 of 23.1.1 
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
Candidate 1 for 23.1.1 burn-in.  This candidate is without the bonsai refactor from #5123 


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5156" class=".btn">#5156</a>
            </td>
            <td>
                <b>
                    update changelog in main to reflect current releases
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
Update changelog in main to reflect releases for 23.1.0 and 23.1.1-RC1

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5155" class=".btn">#5155</a>
            </td>
            <td>
                <b>
                    Merge main into 23.1.x release branch to prep for 23.1.1 release
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
prep 23.1.x release branch for alternate burn-in candidate by merging main into release-23.1.x

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 19:55:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5151" class=".btn">#5151</a>
            </td>
            <td>
                <b>
                    Schedule Goerli shanghaiTime and configure forkId for tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Announced here: https://github.com/ethereum/execution-specs/pull/724

~Still waiting for confirmation of the forkId hash.~

Marius confirmed:
> I can confirm 0xf9843abf with 1678832736

Sepolia change for comparison: https://github.com/hyperledger/besu/commit/54521591f4dc2b9f142172d60c7a362b83ba3d32

I _could_ update `ForkIdsNetworkConfigTest` but Goerli hasn't been kept up to date for that test since Istanbul. I checked code coverage and I don't believe that test is providing any extra value beyond what `ForkIdTest` is already doing. I would suggest we remove `ForkIdsNetworkConfigTest` and the unnecessary parts of `ForkIdTestUtil`. Would like some feedback from @jframe about that first though.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 20:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5146" class=".btn">#5146</a>
            </td>
            <td>
                <b>
                    Add an acceptance test to ensure eth_getBlockByNumber and eth_getBlockByHash return withdrawals correctly for shanghai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Fixes https://github.com/hyperledger/besu/issues/4808

I spent a good amount of time trying to add a test similar to https://github.com/hyperledger/besu/blob/main/ethereum/api/src/integration-test/java/org/hyperledger/besu/ethereum/api/jsonrpc/methods/fork/frontier/EthGetBlockByNumberIntegrationTest.java

...but was ultimately thwarted by some post-merge genesis protocol schedule issues. 

I think this AT-style is actually easier to understand and work with, and also tests the JSON serialization as a bonus.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 05:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5145" class=".btn">#5145</a>
            </td>
            <td>
                <b>
                    [MINOR] Add slf4j api so that acceptance tests work with using acctests.runBesuAsProcess = false
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 04:12:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5144" class=".btn">#5144</a>
            </td>
            <td>
                <b>
                    Upgrade Gradle to 8.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Upgrade Gradle to 8.0.1

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 05:47:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5143" class=".btn">#5143</a>
            </td>
            <td>
                <b>
                    Add Withdrawls execution tests to reference test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add Ethereum execution spec test to be generated and executed by reference tests gradle task. Add `https://github.com/ethereum/execution-spec-tests/releases` as gradle repository to easily download and cache the test specs. Update the reference test gradle file to generate the test Java classes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4934 
## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 07:35:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5142" class=".btn">#5142</a>
            </td>
            <td>
                <b>
                    Use binary search to eth_estimateGas more accurately
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">RPC</span>
            </td>
            <td>
                ## PR description

eth_estimateGas currently conservatively estimates gas this change will take that estimate and use it as a high bound and will use gasUsed as a lower bound to hone in on the most true gas limit required.

Outstanding Issues/questions

- The estimate comes back lower than geth, I suspect this is due to the protocol schedule being used in the acceptance tests.
- further optimise the binary search?
- ganache does a better job of getting an exact gas requirement with only a few runs https://github.com/trufflesuite/ganache-cli-archive/releases/tag/v6.4.2

## Fixed Issue(s)

fixes https://github.com/hyperledger/besu/issues/4244


## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 18:10:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5141" class=".btn">#5141</a>
            </td>
            <td>
                <b>
                    Withdrawals engine API ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Basic withdrawals acceptance tests using the engine API

Covers these test cases
* Sending a prepare payload with no (null) withdrawals after withdrawals timestamp
* Sending a prepare payload with withdrawals
* Retrieving the built block with withdrawals
* Executing and updating forkchoice
* Confirming the balance is incremented for the withdrawals address

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5078 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 06:10:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5140" class=".btn">#5140</a>
            </td>
            <td>
                <b>
                    Fix issues with RLPExceptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR fixes two issues with RLP encoding:

### 1- BlockBody

For the BlockBody RLP serialisation, when an empty body `[]` is sent, a breach of protocol is triggered and Besu disconnects the peer. That causes Besu to disconnect peers with a good reputation. This PR adds an option in the readFrom method to allow an empty BlockBody whenever a `[]` is found. The message will be verified later and marked as invalid anyway, but besu will not disconnect the peer.

### 2 -NewPooledTransactionHashesMessage

`NewPooledTransactionHashesMessage` on Eth/68 has an issue with the array of types (`byte`):

`[[type_0: B_1, type_1: B_1, ...], [size_0: B_4, size_1: B_4, ...], [hash_0: B_32, hash_1: B_32, ...]]`

The current implementation serializes it as:
```
[
      ["0x01","0x02"]
      ["0x00000001","0x00000002"],
      ["0x0000000000000000000000000000000000000000000000000000000000000001",
       "0x0000000000000000000000000000000000000000000000000000000000000002"]
]
```
The other clients send the first array of this message as one element instead of an array:
```
[
      ["0x0102"]
      ["0x00000002","0x00000003"],
      ["0x0000000000000000000000000000000000000000000000000000000000000002",
       "0x0000000000000000000000000000000000000000000000000000000000000003"]
]
```
This PR fixes the encoding to match the other client messages.

 see #5056

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 02:37:55 +0000 UTC
    </div>
</div>

