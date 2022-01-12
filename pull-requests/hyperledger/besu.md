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
                PR <a href="https://github.com/hyperledger/besu/pull/3269" class=".btn">#3269</a>
            </td>
            <td>
                <b>
                    Added integration test to ensure DevP2P-over-TLS can handle large messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TLS fragments large messages into 16KB records.
Actual fix was done in an earlier commit: https://github.com/hyperledger/besu/commit/f2f7ac9af1a52e04c422f5663063ad27aad35137

This fixes https://github.com/hyperledger/besu/issues/3254
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 04:53:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3266" class=".btn">#3266</a>
            </td>
            <td>
                <b>
                    Gas price too low warning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
When transactions are sent with a gasPrice below the minimum configured, a message alerting the user is only displayed when in TRACE mode.

## Fixed Issue(s)
Fixes #3211 

## Changelog
Changed logging for the gasPrice too low message from TRACE to WARN so the user will be alerted to this issue if it occurs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 10:52:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3265" class=".btn">#3265</a>
            </td>
            <td>
                <b>
                    Release 21.10.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update dependencies in preparation for release 21.10.7
Also JWT support for multiple algorithms as this overlapped with the vert.x upgrade

See #3229 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 07:44:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3263" class=".btn">#3263</a>
            </td>
            <td>
                <b>
                    Kubernetes 14
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Update kubernetes dependency - package rename mostly.
Also added additional licence alias for CDDL + GPLv2 with classpath extension
See #3229 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 00:47:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3261" class=".btn">#3261</a>
            </td>
            <td>
                <b>
                    Fast sync state error
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
Previously, fastSyncState.getPivotBlockHeader().get() is accessed before checking pivot block not present. Added fixes, needed to add the exit code but not able to understand.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #3227

## Changelog
Added the error message log if pivot block not present.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 17:04:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3260" class=".btn">#3260</a>
            </td>
            <td>
                <b>
                    We want to know how long it took to import blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 12:41:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3258" class=".btn">#3258</a>
            </td>
            <td>
                <b>
                    don't stuff hex into a decimal parser
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-08 01:04:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3257" class=".btn">#3257</a>
            </td>
            <td>
                <b>
                    Removed deprecated Orion classes
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

## Fixed Issue(s)
#3244 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 20:13:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3256" class=".btn">#3256</a>
            </td>
            <td>
                <b>
                    ETC Mystique hard fork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adds the blocks and the changes for the Mystique hard fork

## Fixed Issue(s)

Fixes #3255

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 17:13:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3253" class=".btn">#3253</a>
            </td>
            <td>
                <b>
                    Use out-of-the-box netty codecs to fix TLS P2P failing to process messages over a certain size (> TLS record limit of 16 KB)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Based on https://github.com/perusworld/besu/commit/06f94311d8196a35759ae5e647c282a2204e9dd9 but removed Protobufs

This will fix https://github.com/hyperledger/besu/issues/3254

Note, this supersedes https://github.com/hyperledger/besu/pull/3242
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 06:57:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3251" class=".btn">#3251</a>
            </td>
            <td>
                <b>
                    BFT header validation updated to support London hard fork EIP-1559
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

Added EIP-1559 support for BFT protocols. Block header validation rule GasLimitRangeAndDeltaValidationRule has been updated to include the market base fee. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes https://github.com/hyperledger/besu/issues/2714 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 05:39:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3250" class=".btn">#3250</a>
            </td>
            <td>
                <b>
                    Add upnp only for p2p nat method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add a nat method option that only enables upnp for p2p networking not RPC

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3021 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 04:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3249" class=".btn">#3249</a>
            </td>
            <td>
                <b>
                    Merge of main
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
merge main into merge branch


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 02:22:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3248" class=".btn">#3248</a>
            </td>
            <td>
                <b>
                    Fixes for kintsugi consensus errors
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
* ensure we validate block parameters before we optimistically return valid for block hash param
* address a corner case discovered in kintsugi where we refuse to import a block which has already finalized
* test coverage


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 02:18:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3247" class=".btn">#3247</a>
            </td>
            <td>
                <b>
                    update CHANGELOG.md for RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

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
        Created At 2022-01-06 17:36:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3246" class=".btn">#3246</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.1.0-RC3-SNAPSHOT
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
        Created At 2022-01-06 17:03:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3245" class=".btn">#3245</a>
            </td>
            <td>
                <b>
                    Release 22.1.0-RC2
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
        Created At 2022-01-06 16:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3243" class=".btn">#3243</a>
            </td>
            <td>
                <b>
                    assertj update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

dependency 'org.assertj:assertj-core:3.22.0'

See #3229 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 05:36:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3241" class=".btn">#3241</a>
            </td>
            <td>
                <b>
                    update web3j dependency versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Update to 5.0.0 where there's no breaking changes

Updating others from 4.8.9 to 5.0.0 (see previous commits on this PR) caused things to break. 

See #3229 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 03:30:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3240" class=".btn">#3240</a>
            </td>
            <td>
                <b>
                    remove old comment re bls12-381 version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The referenced issue has been fixed and bls12-381 has been updated
https://github.com/hyperledger/besu/issues/2668

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 03:18:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3238" class=".btn">#3238</a>
            </td>
            <td>
                <b>
                    Fix JSON syntax
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

just a trival fix, to avoid error messages in the IDE

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 15:33:01 +0000 UTC
    </div>
</div>

