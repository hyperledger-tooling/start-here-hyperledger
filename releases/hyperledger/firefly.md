---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.13.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.13.0
                </span>
            </td>
            <td>
                ## Summary
This is an important hardening release - while very little has changed on the surface, it includes a lot of significant rework to the core of FireFly, mostly to fix issues exposed by the performance testing in #316.

Breaking changes:
* The `token_pool_rejected` event was removed, along with the recently-added `contract_interface_rejected` and `contract_api_rejected` (only `message_rejected` will now be emitted for rejected definitions)
* The expected format of the FireFly contract address in the "instance" config entry for Ethereum blockchains has changed (see "Migrations" below)

Other major items included in this release:
* Support for running on ARM-based M1 processors
* Rewrite of the message batching and event aggregation logic inside FireFly, to fix numerous edge cases with lost or hung messages
* Hardening of operations and transactions to behave more consistently across all types
* Metrics reporting to [Prometheus](https://prometheus.io)
* Continued development to support [custom on-chain logic](https://github.com/hyperledger/firefly-fir/pull/2) (still in preview)

## Migrations
* The Ethereum plugin now expects just a contract address in the `instance` field of the FireFly core config file. The value should be a hex string (with the `0x` prefix) which is the Ethereum address of the FireFly smart contract. It is recommended to update any existing config file for this release, though this version will attempt to read values from existing configs and determine the contract address from the old value. Note: FireFly will not automatically update the config file as it treats it as read-only.

Here is an example of what your blockchain section should look like (your actual `instance` value will be a different hex string):
```
blockchain:
  type: ethereum
  ethereum:
    ethconnect:
      instance: 0x8707d1f1151220430fc8f89836b20bcf05d6eb41
```

## Updated Dependencies

* firefly-ethconnect [v3.1.3](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.3)
* firefly-fabconnect [v0.9.9](https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.9)
* firefly-dataexchange-https [v0.10.4](https://github.com/hyperledger/firefly-dataexchange-https/releases/tag/v0.10.4)
* firefly-tokens-erc20-erc721 [v0.1.5](https://github.com/hyperledger/firefly-tokens-erc20-erc721/releases/tag/v0.1.5)

## What's Changed
* Store all token transfer inputs on operation by @awrichar in https://github.com/hyperledger/firefly/pull/478
* Make the factories act like factories by @awrichar in https://github.com/hyperledger/firefly/pull/474
* Add missing test coverage in txcommon by @awrichar in https://github.com/hyperledger/firefly/pull/476
* Use PreFinalize/Finalize in all definition handlers by @awrichar in https://github.com/hyperledger/firefly/pull/475
* wsReader cannot rely on `testing.T` as it might extend past test scope by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/472
* Set default keepalive timeout to 5s on clients for Node.js connectors by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/470
* Address some inconsistencies in Operation behavior by @awrichar in https://github.com/hyperledger/firefly/pull/480
* Remove extra "rejected" events by @awrichar in https://github.com/hyperledger/firefly/pull/482
* Update aggregator batch processing to maintain in-memory pin state until OnFinalize by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/483
* Fix fabric event timestamp parsing by @jimthematrix in https://github.com/hyperledger/firefly/pull/491
* Fix Docker build on ARM by @nguyer in https://github.com/hyperledger/firefly/pull/473
* Add extra logging for message/event ids by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/488
* Pass arguments from Makefile to docker build script by @nguyer in https://github.com/hyperledger/firefly/pull/495
* Fix possibility for nil access in sendloop by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/486
* Fix group to be constant throughout test by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/490
* Compile directly with solc to avoid full Node.js npm install of Truffle by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/494
* Rewind when messages appear behind offset by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/496
* Pass requestId to DX and remove backend_id from Operation by @awrichar in https://github.com/hyperledger/firefly/pull/497
* Rename data exchange plugin to "ffdx" by @awrichar in https://github.com/hyperledger/firefly/pull/505
* Misc fixes for operations by @awrichar in https://github.com/hyperledger/firefly/pull/498
* Use inline ABI for all Ethconnect contract interactions by @nguyer in https://github.com/hyperledger/firefly/pull/502
* Prometheus metrics by @eberger727 in https://github.com/hyperledger/firefly/pull/503
* Re-work batch logic for simplicity, efficiency, and restart recovery by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/501
* Add "initEnabled" config to DX by @awrichar in https://github.com/hyperledger/firefly/pull/507
* Move insert of events to a special pre-commit phase of the DB transaction by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/510
* Flatten the DXInfo back to the orginal payload on the ffdx API to connectors by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/514
* Implement and use UpsertOptimization for groups by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/513
* Update components ready for v0.13.0 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/516
* Update EthConnect to 3.1.3 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/518
* [metrics-types] using fftypes in metrics manager by @eberger727 in https://github.com/hyperledger/firefly/pull/520
* Provide Migration / Registration / Debugging Utilities in Docker Image by @hfuss in https://github.com/hyperledger/firefly/pull/521
* go-migrate in Dockerfile by @hfuss in https://github.com/hyperledger/firefly/pull/524
* Fix pages build by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/526
* Use bash for variable expansion prior to make by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/528
* Allow building in docker by removing .git from .dockerignore by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/530


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.12.0...v0.13.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.13.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-02-15 00:22:09 +0000 UTC
    </span>
</div>

