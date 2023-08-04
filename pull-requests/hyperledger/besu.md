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
                PR <a href="https://github.com/hyperledger/besu/pull/5752" class=".btn">#5752</a>
            </td>
            <td>
                <b>
                    [WIP] Rebase current EIP-6110 prototype to Cancun
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
This is to rebase the existed implementation of EIP-6110 from Shanghai to Cancun. As well, it updates the implementation according to the latest Engine API [specification](https://github.com/ethereum/execution-apis/blob/main/src/engine/experimental/eip6110.md).
Changes include:

- [ ] Remove 6110 related changes from `engine_newPayloadV2` and `engine_getPayloadV2`
- [ ] Rename `deposits` to `depositReceipts` in `EnginePayloadParameter`
- [ ] Introduce `engine_newPayloadV6110` and `engine_getPayloadV6110` that are based on `engine_newPayloadV3` and `engine_getPayloadV3`
- [ ] Revamp the existed 6110 acceptance test

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 08:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5750" class=".btn">#5750</a>
            </td>
            <td>
                <b>
                     23.7.1-RC burn in
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
RC burn-in release of 23.7.1:
 * cherry pick of #5734 performance regression fix
 * changelog revision to reflect 23.7.0 not released
 * change rev to 23.7.1-RC


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 20:41:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5749" class=".btn">#5749</a>
            </td>
            <td>
                <b>
                    Update native libraries
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

Use the 0.8.0 version of native libraries, which uses better names for automatic modules for JPMS.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 18:23:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5748" class=".btn">#5748</a>
            </td>
            <td>
                <b>
                    Force the use of jdk18 version of Bouncy Castle library
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
This avoid that any dependency can include the jdk15 version in the distribution.

Implement the solution described here https://docs.gradle.org/7.6/userguide/dependency_capability_conflict.html

Had to inline the `xor` function since it is now deprecated in newer versions of Bouncy Castle.



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 14:26:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5746" class=".btn">#5746</a>
            </td>
            <td>
                <b>
                    Uniform the way fee market is used in ProtocolSpecBuilder
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

Looking at `MainnetProtocolSpecs` I found that the fee market is passed in different way to objects that require it, while the intended way is to set it via `ProcotocolSpecBuilder::feeMarket` and the pass it via builders to object that require it, so we are sure that always the same fee market is used in that milestone definition, so this PR removes any set of the fee market that does not follow the said approach.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 14:14:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5745" class=".btn">#5745</a>
            </td>
            <td>
                <b>
                    Migrate to blobGas in execution-spec-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Execution-spec-tests migrated from DataGas to BlobGas and checks for its inclusion in tests now. Add needed support.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 06:36:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5743" class=".btn">#5743</a>
            </td>
            <td>
                <b>
                    fix: Move maintainers to emeritus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose moving maintainers @mark-terry and @wcgcyx to Emeritus status, pursuant to the inactivity clause. These maintainers have had no activity since January 2023.

We very much appreciate their contributions, but moving their status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If any of these maintainers express in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.

I propose this vote remain open until either both maintainers mentioned above confirm on this PR their acceptance of this change, OR an absolute majority of active maintainers votes for the same outcome, OR until two weeks has passed, after which a voting majority will determine the outcome (with a tie resulting in no change).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 02:41:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5742" class=".btn">#5742</a>
            </td>
            <td>
                <b>
                    added worldview service to plugin api
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

Add a new `WorldViewService` which allows to get any account of the world state.

## Fixed Issue(s)
fixes #5740 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 21:48:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5741" class=".btn">#5741</a>
            </td>
            <td>
                <b>
                    Added traceContextEnter & traceContextExit
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

The `OperationTracer` is extended by the new methods:

* `traceContextEnter`: called before switching to a new context
* `traceContextExit`: called after leaving the context

## Fixed Issue(s)
fixes #5728 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 21:43:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5734" class=".btn">#5734</a>
            </td>
            <td>
                <b>
                    Address import performance issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Address a performance regression observed in import testing -
* ensure we are on a single tuweni version
* factor out an unneeded concatenate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 14:02:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5733" class=".btn">#5733</a>
            </td>
            <td>
                <b>
                    Reference tests 12.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update Reference Tests to 12.3
* fix decoding error
* add ignored field
* update module

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 02:36:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5732" class=".btn">#5732</a>
            </td>
            <td>
                <b>
                    Add missing methods to transaction interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Missing methods which exist in the transaction class, but not the interface were added. This required the creation of a `AccessListEntry` interface in `org.hyperledger.besu.datatypes` and it's use in all the places that have used the class directly before.

## Fixed Issue(s)
fixes #5731
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-30 16:54:57 +0000 UTC
    </div>
</div>

