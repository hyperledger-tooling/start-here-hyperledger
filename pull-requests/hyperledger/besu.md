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
                PR <a href="https://github.com/hyperledger/besu/pull/2381" class=".btn">#2381</a>
            </td>
            <td>
                <b>
                    CI: use med executor for more steps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Use medium executor where xl not needed.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 02:20:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2380" class=".btn">#2380</a>
            </td>
            <td>
                <b>
                    eth_getCode: add support for GoQuorum private tx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Attempt to retrieve from GoQuorum private state first, otherwise get from public state as before.

I have tested this by:
Node1 deploys a contract, private for Node4. Nodes 1 and 4 can get the code; Nodes 2 and 3 do not. getCode for public tx works as before (all nodes get the right value). Attempting to getCode for non-existent address gives 0x.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 01:57:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2379" class=".btn">#2379</a>
            </td>
            <td>
                <b>
                    QBFT to use fixed IBFT mixhash value for headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Use the fixed IBFT mixedHash value in QBFT as this is what is being done in Quorum.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 01:20:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2377" class=".btn">#2377</a>
            </td>
            <td>
                <b>
                    Hook up an empty plugin for future unrestricted privacy encryption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Placeholder for `UnrestrictedPayloadEncryptionProvider` to be able to add future methods.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 14:00:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2376" class=".btn">#2376</a>
            </td>
            <td>
                <b>
                    Upgrade to Apache Tuweni 2.0
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
This is a test PR against Apache Tuweni's latest release candidate version 2.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 06:14:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2375" class=".btn">#2375</a>
            </td>
            <td>
                <b>
                    Fix flaky OpenTelemetry acceptance test
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
Fixes a flaky acceptance test checking OpenTelemetry traces are reported.

## Fixed Issue(s)
Fixes #2299

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 05:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2374" class=".btn">#2374</a>
            </td>
            <td>
                <b>
                    1559 blockchain reftests
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
* change transaction pool behavior to not reject transactions based on chain head's baseFee
* add short form of Wei for maxFeePerGas and maxPriorityFeePerGas
* ~~address edge case of allowable maximum delta gasLimit per block~~
* update reference tests module to latest

This pr gets besu passing all of the London blockchain tests using the retesteth engine.  There will be a follow up pr to address issues the few remaining GeneralStateTests failures for Berlin and London

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #2350 for London Blockchain tests

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 02:48:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2372" class=".btn">#2372</a>
            </td>
            <td>
                <b>
                    test fix fastsync bonsai
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
        Created At 2021-06-03 10:35:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2368" class=".btn">#2368</a>
            </td>
            <td>
                <b>
                    add effectiveGasPrice to TransasctionReceipt 
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
Implementation of json-rpc spec change from https://github.com/ethereum/eth1.0-specs/pull/206

DO NOT MERGE until the json-rpc spec PR is merged

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2364 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 05:25:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2366" class=".btn">#2366</a>
            </td>
            <td>
                <b>
                    Fixes for 1559 retesteth behaviors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

quick pr to unblock retesteth testing, remove aleut and calaveras from retesteth chain genesis.  

Aleut config was an artifact from when we did not have London configs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 22:48:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2365" class=".btn">#2365</a>
            </td>
            <td>
                <b>
                    eth66
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
        Created At 2021-06-02 20:56:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2363" class=".btn">#2363</a>
            </td>
            <td>
                <b>
                    [Cleanup] Remove Gas Budget Calculator
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
Since there are no separate gas budgets for eip-1559 and non-eip-1559 txs. We can return to the simpler method of just comparing against the gas limit.

This is a non-functional change.
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 15:31:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2361" class=".btn">#2361</a>
            </td>
            <td>
                <b>
                    ci/cd: Require Quorum Acceptance Tests to pass
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ricardo Silva <ricardo.silva@consensys.net>

### Summary

As the work is done for the privacy interop, we remove now the ignore of the results so if it fails, it breaks the build.

## Changes

* Removed `|| true` to make the job fail if the tests fail.
* Make the publish of docker images depend on the Quorum AT.
* Add the `nosupport` tag as privacy polishing to be done later.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 10:32:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2360" class=".btn">#2360</a>
            </td>
            <td>
                <b>
                    pending tx logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add trace logging for pending transactions behavior.

fixes #2353 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 21:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2359" class=".btn">#2359</a>
            </td>
            <td>
                <b>
                    Remove Separation of EIP-1559 and pre-EIP-1559 Gas Tracking
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
The segregated tracking was used in an older version of the spec but not anymore.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 20:33:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2347" class=".btn">#2347</a>
            </td>
            <td>
                <b>
                    update CHANGELOG for 21.1.7 release
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

update CHANGELOG for 21.1.7 release


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 16:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2346" class=".btn">#2346</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.1.8-SNAPSHOT
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
        Created At 2021-06-01 15:47:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2345" class=".btn">#2345</a>
            </td>
            <td>
                <b>
                    Release 21.1.7
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
        Created At 2021-06-01 15:28:57 +0000 UTC
    </div>
</div>

