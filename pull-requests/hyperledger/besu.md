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
                PR <a href="https://github.com/hyperledger/besu/pull/2295" class=".btn">#2295</a>
            </td>
            <td>
                <b>
                    Ts ats on XL executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run with parallelism 8 on XL executor

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 03:48:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2294" class=".btn">#2294</a>
            </td>
            <td>
                <b>
                    GoQuorum ATs: run the estimate gas test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Revert #2282 
Enabling one more passing GoQuorum AT 
See https://github.com/hyperledger/besu/pull/2282

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 00:54:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2292" class=".btn">#2292</a>
            </td>
            <td>
                <b>
                    EIP-1559 Transaction Pool Sorting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
fixes #2286

## Changelog
- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 22:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2289" class=".btn">#2289</a>
            </td>
            <td>
                <b>
                    EIP-3554: Difficulty Bomb Delay to December 1st 2021
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>


## PR description

implemented for london https://eips.ethereum.org/EIPS/eip-3554

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 17:29:29 +0000 UTC
    </div>
</div>

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

