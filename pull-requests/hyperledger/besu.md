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
                PR <a href="https://github.com/hyperledger/besu/pull/2284" class=".btn">#2284</a>
            </td>
            <td>
                <b>
                    refactor: expose EnodeUrl to plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couldn't figure out a nice way of not having EnodeURLImpl.

If we kept it as EnodeURL we could add static imports in for things like `fromURI` but the problem is they are mostly used as method references. So you can either have method references with the class name or lambdas with a static import! 

I think it's the least worse option at the moment.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 08:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2283" class=".btn">#2283</a>
            </td>
            <td>
                <b>
                    refactor: EeaSendRawTransaction isolate send raw on/off chain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor EeaSendRawTransaction so to allow further extension and isolate responsibilities
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 07:24:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2282" class=".btn">#2282</a>
            </td>
            <td>
                <b>
                    Modify Gas estimation logic for GoQuorum mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If in GoQuorum privacy mode, use a fully filled data field to get max value for gas estimation.

This doesn't make the GQ AT pass. 
They get 21000 + 64 * 68 (homestead)
With this we get 21000 + 64 * 16 (latest ie istanbul)


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 00:55:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2281" class=".btn">#2281</a>
            </td>
            <td>
                <b>
                    try to use the hostName property from log4j2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
This adds the ability to default to the `hostName` property, filled by log4j2, before we default to sending localhost.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 19:20:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2278" class=".btn">#2278</a>
            </td>
            <td>
                <b>
                    Stabilize eth/65
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's been stable for a while now, time to clean up the code surrounding it.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 14:55:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2277" class=".btn">#2277</a>
            </td>
            <td>
                <b>
                    Remove EIP1559 flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 14:01:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2276" class=".btn">#2276</a>
            </td>
            <td>
                <b>
                    Support qbft encoding of extra data in the operator generate-blockchain subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Frame <jasonwframe@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Support qbft encoding of extra data in the operator generate-blockchain subcommand

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2049

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 06:14:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2275" class=".btn">#2275</a>
            </td>
            <td>
                <b>
                    support qbft encoding of extra data in the rlp encode subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Frame <jasonwframe@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
support qbft encoding of extra data in the rlp encode subcommand

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2049 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 03:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2274" class=".btn">#2274</a>
            </td>
            <td>
                <b>
                    [MINOR] update deprecated calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

recursive comparison 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 01:19:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2273" class=".btn">#2273</a>
            </td>
            <td>
                <b>
                    Ignore SECP256R1 tests for now
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ignore these tests for now as the static reference to the signatureAlgorithm breaks other tests.

See #2267 

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 22:07:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2270" class=".btn">#2270</a>
            </td>
            <td>
                <b>
                    Update reference tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Update reference tests to this version https://github.com/ethereum/tests/commit/bb662629b6da3a4ebea3f7cebf02d6c4870c2871

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 14:00:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2265" class=".btn">#2265</a>
            </td>
            <td>
                <b>
                    Qbft invalid timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Fix error where we get an invalid header timestamp occasionally. This seems to be due slight deviation from the block period. It's not likely we can ever get the timing exact as we need determine the delay before scheduling the block expiry event so there can be a very small discrepancy.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2241 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 03:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2264" class=".btn">#2264</a>
            </td>
            <td>
                <b>
                    [MINOR] Allowlist comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                updated comment in test

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 02:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2262" class=".btn">#2262</a>
            </td>
            <td>
                <b>
                    Entropy aargh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                file:/dev/urandom

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 23:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2261" class=".btn">#2261</a>
            </td>
            <td>
                <b>
                    Bonsai trie : clone updater during persist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 12:53:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2259" class=".btn">#2259</a>
            </td>
            <td>
                <b>
                    Rayonism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
 merge master into rayonism


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:47:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2258" class=".btn">#2258</a>
            </td>
            <td>
                <b>
                    Revert "fix newblock transaction decoding RPC"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/besu#2256.  revert so Proto can get cred for his commit :)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:43:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2257" class=".btn">#2257</a>
            </td>
            <td>
                <b>
                    rayonism: fix newblock transaction decoding RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)

Previous `consensus_newBlock` (for the Merge prototype) was expecting full transactions, but the beacon node sends opaque transactions, and so blocks with a transaction would fail and cause the besu node to fail to sync the chain.

This mirrors the encoding code (stream tx list, map from hex and decoding instead of encoding and to hex, collect in list), and wraps it with some logging and error handling just in case. Tested this on a local merge testnet with all consensus and execution clients mining on top of the blocks, no errors.

<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
  - Small fix in experimental fork of besu, no new features, not updating changelog.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2256" class=".btn">#2256</a>
            </td>
            <td>
                <b>
                    fix newblock transaction decoding RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
fix consensus_newBlock transaction decoding

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:26:29 +0000 UTC
    </div>
</div>

