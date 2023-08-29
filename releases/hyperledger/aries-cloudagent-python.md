---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.10.1
                </span>
            </td>
            <td>
                Release 0.10.1 contains a breaking change, an important fix for a regression introduced in 0.8.2 that impacts certain deployments, and a number of fixes and updates. Included in the updates is a significant internal reorganization of the DID and connection management code that was done to enable more flexible uses of different DID Methods, such as being able to use did:web DIDs for DIDComm messaging connections. The work also paves the way for coming updates related to support for did:peer DIDs for DIDComm. For details on the change see https://github.com/hyperledger/aries-cloudagent-python/pull/2409, which includes some of the best pull request documentation ever created.

Release 0.10.1 has the same contents as 0.10.0. An error on PyPi prevented the 0.10.0 release from being properly uploaded because of an existing file of the same name. We immediately released 0.10.1 as a replacement.

The regression fix is for ACA-Py deployments that use multi-use invitations but do NOT use the --auto-accept-connection-requests flag/processing. A change in [0.8.2](https://github.com/hyperledger/aries-cloudagent-python/blob/main/CHANGELOG.md#082) (PR https://github.com/hyperledger/aries-cloudagent-python/pull/2223) suppressed an extra webhook event firing during the processing after receiving a connection request. An unexpected side effect of that change was that the subsequent webhook event also did not fire, and as a result, the controller did not get any event signalling a new connection request had been received via the multi-use invitation. The update in this release ensures the proper event fires and the controller receives the webhook.

See below for the breaking changes and the [CHANGELOG](https://github.com/hyperledger/aries-cloudagent-python/blob/main/CHANGELOG.md#0101) for a categorized list of the pull requests included in this release.

Updates in the CI/CD area include adding the publishing of a nightly container image that includes any changes in the main branch since the last nightly was published. This allows getting the "latest and greatest" code via a container image vs. having to install ACA-Py from the repository. In addition, Snyk scanning was added to the CI pipeline, and Indy SDK tests were removed from the pipeline.

0.10.1 Breaking Changes
https://github.com/hyperledger/aries-cloudagent-python/pull/2352 is a breaking change related to the storage of presentation exchange records in ACA-Py. In previous releases, presentation exchange protocol state data records were retained in ACA-Py secure storage after the completion of protocol instances. With this release the default behavior changes to deleting those records by default, unless the ----preserve-exchange-records flag is set in the configuration. This extends the use of that flag that previously applied only to issue credential records. The extension matches the initial intention of the flag--that it cover both issue credential and present proof exchanges. The "best practices" for ACA-Py is that the controller (business logic) store any long-lasting business information needed for the service that is using the Aries Agent, and ACA-Py storage should be used only for data necessary for the operation of the agent. In particular, protocol state data should be held in ACA-Py only as long as the protocol is running (as it is needed by ACA-Py), and once a protocol instance completes, the controller should extract and store the business information from the protocol state before it is deleted from ACA-Py storage.

## What's Changed
* Add workaround for ARM based macs by @finnformica in https://github.com/hyperledger/aries-cloudagent-python/pull/2313
* chore(deps): Bump certifi from 2023.5.7 to 2023.7.22 in /demo/playground/scripts by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2354
* Extend `--preserve-exchange-records` to include Presentation Exchange. by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2352
* Corrected typo on mediator invitation configuration argument by @jorgefl0 in https://github.com/hyperledger/aries-cloudagent-python/pull/2365
* Fix empty ServiceDecorator in OobRecord causing 422 Unprocessable Entity Error by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2362
* Correct the response type in `send_rev_reg_def` by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2355
* fix: additional tweaks for did:web and other methods as public DIDs by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2392
* fix: keylist update response race condition by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2391
* Feat: Support Selectable Write Ledger by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2339
* fix: outbound send status missing on path by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2393
* Multitenant check endorser_info before saving by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2395
* Chore: fix marshmallow warnings by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2398
* Upgrade pre-commit and flake8 dependencies; fix flake8 warnings by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2399
* feat: add DID Exchange specific problem reports and reject endpoint by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2394
* Fix: Ensure event/webhook is emitted for multi-use invitations by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2413
* 0.10.0-rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2414
* fix: ensure request matches offer, if sent by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2341
* Remove Indy tests from workflows by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2415
* Enable Snyk scanning by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/2418
* feat: add legacy peer did resolver by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2404
* Issue #2250 Nightly publish workflow by @Gavinok in https://github.com/hyperledger/aries-cloudagent-python/pull/2421
* Don't run Snyk on forks by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/2429
* Fix for nightly tests failing on Python 3.10 by @Gavinok in https://github.com/hyperledger/aries-cloudagent-python/pull/2435
* feat: resolve connection targets and permit connecting via public DID by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2409
* 0.10.0-rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2442
* fix: more doc corrections by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2446
* Add symlink to /home/indy/.indy_client for backwards compatibility by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2443
* fix: ignore duplicate record errors on add key by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2447
* 0.10.0-rc2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2448
* fix: handle stored afgo and findy docs in corrections by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2450
* chore: relax connections filter DID format by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2451
* 0.10.0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2452
* 0.10.1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2454

## New Contributors
* @finnformica made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2313
* @jorgefl0 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2365
* @Gavinok made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2421

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.9.0...0.10.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.10.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-29 15:41:29 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.10.0
                </span>
            </td>
            <td>
                Release 0.10.1 has the same contents as 0.10.0. An error on PyPi prevented the 0.10.0 release from being properly uploaded because of an existing file of the same name. We immediately released 0.10.1 as a replacement.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.10.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-29 14:09:56 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.10.0-rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.10.0-rc2
                </span>
            </td>
            <td>
                Release 0.10.0 contains a breaking change, an important fix for a regression introduced in 0.8.2 that impacts certain deployments, and a number of fixes and updates. Included in the updates is a significant internal reorganization of the DID and connection management code that was done to enable more flexible uses of different DID Methods, such as being able to use did:web DIDs for DIDComm messaging connections. The work also paves the way for coming updates related to support for did:peer DIDs for DIDComm. For details on the change see [PR #2409](https://github.com/hyperledger/aries-cloudagent-python/pull/2409), which includes some of the best pull request documentation ever created.

The regression fix is for ACA-Py deployments that use multi-use invitations but do NOT use the --auto-accept-connection-requests flag/processing. A change in [0.8.2](https://github.com/hyperledger/aries-cloudagent-python/blob/0.10.0-rc2/CHANGELOG.md#082) (PR [#2223](https://github.com/hyperledger/aries-cloudagent-python/pull/2223)) suppressed an extra webhook event firing during the processing after receiving a connection request. An unexpected side effect of that change was that the subsequent webhook event also did not fire, and as a result, the controller did not get any event signalling a new connection request had been received via the multi-use invitation. The update in this release ensures the proper event fires and the controller receives the webhook.

See below for the breaking changes and the [CHANGELOG file](https://github.com/hyperledger/aries-cloudagent-python/blob/0.10.0-rc2/CHANGELOG.md) for a categorized list of the pull requests included in this release.

Updates in the CI/CD area include adding the publishing of a nightly container image that includes any changes in the main branch since the last nightly was published. This allows getting the "latest and greatest" code via a container image vs. having to install ACA-Py from the repository. In addition, Snyk scanning was added to the CI pipeline, and Indy SDK tests were removed from the pipeline.

## 0.10.1 Breaking Changes

[#2352](https://github.com/hyperledger/aries-cloudagent-python/pull/2352) is a breaking change related to the storage of presentation exchange records in ACA-Py. In previous releases, presentation exchange protocol state data records were retained in ACA-Py secure storage after the completion of protocol instances. With this release the default behavior changes to deleting those records by default, unless the ----preserve-exchange-records flag is set in the configuration. This extends the use of that flag that previously applied only to issue credential records. The extension matches the initial intention of the flag--that it cover both issue credential and present proof exchanges. The "best practices" for ACA-Py is that the controller (business logic) store any long-lasting business information needed for the service that is using the Aries Agent, and ACA-Py storage should be used only for data necessary for the operation of the agent. In particular, protocol state data should be held in ACA-Py only as long as the protocol is running (as it is needed by ACA-Py), and once a protocol instance completes, the controller should extract and store the business information from the protocol state before it is deleted from ACA-Py storage.

## What's Changed
* Add workaround for ARM based macs by @finnformica in https://github.com/hyperledger/aries-cloudagent-python/pull/2313
* chore(deps): Bump certifi from 2023.5.7 to 2023.7.22 in /demo/playground/scripts by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2354
* Extend `--preserve-exchange-records` to include Presentation Exchange. by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2352
* Corrected typo on mediator invitation configuration argument by @jorgefl0 in https://github.com/hyperledger/aries-cloudagent-python/pull/2365
* Fix empty ServiceDecorator in OobRecord causing 422 Unprocessable Entity Error by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2362
* Correct the response type in `send_rev_reg_def` by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2355
* fix: additional tweaks for did:web and other methods as public DIDs by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2392
* fix: keylist update response race condition by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2391
* Feat: Support Selectable Write Ledger by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2339
* fix: outbound send status missing on path by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2393
* Multitenant check endorser_info before saving by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2395
* Chore: fix marshmallow warnings by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2398
* Upgrade pre-commit and flake8 dependencies; fix flake8 warnings by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2399
* feat: add DID Exchange specific problem reports and reject endpoint by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2394
* Fix: Ensure event/webhook is emitted for multi-use invitations by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2413
* 0.10.0-rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2414
* fix: ensure request matches offer, if sent by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2341
* Remove Indy tests from workflows by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2415
* Enable Snyk scanning by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/2418
* feat: add legacy peer did resolver by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2404
* Issue #2250 Nightly publish workflow by @Gavinok in https://github.com/hyperledger/aries-cloudagent-python/pull/2421
* Don't run Snyk on forks by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/2429
* Fix for nightly tests failing on Python 3.10 by @Gavinok in https://github.com/hyperledger/aries-cloudagent-python/pull/2435
* feat: resolve connection targets and permit connecting via public DID by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2409
* 0.10.0-rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2442
* fix: more doc corrections by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2446
* Add symlink to /home/indy/.indy_client for backwards compatibility by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2443
* fix: ignore duplicate record errors on add key by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2447
* 0.10.0-rc2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2448

## New Contributors
* @finnformica made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2313
* @jorgefl0 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2365
* @Gavinok made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2421

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.9.0...0.10.0-rc2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.10.0-rc2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-25 22:04:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.10.0-rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.10.0-rc1
                </span>
            </td>
            <td>
                Release 0.10.0 contains a breaking change, an important fix for a regression introduced in 0.8.2 that impacts certain deployments, and a number of fixes and updates. Included in the updates is a significant internal reorganization of the DID and connection management code that was done to enable more flexible uses of different DID Methods, such as being able to use did:web DIDs for DIDComm messaging connections. The work also paves the way for coming updates related to support for did:peer DIDs for DIDComm. For details on the change see [PR #2409](https://github.com/hyperledger/aries-cloudagent-python/pull/2409), which includes some of the best pull request documentation ever created.

The regression fix is for ACA-Py deployments that use multi-use invitations but do NOT use the --auto-accept-connection-requests flag/processing. A change in [0.8.2](https://vscode-remote+ssh-002dremote-002bx-002ecloudcompass-002eca.vscode-resource.vscode-cdn.net/home/swcur/repos/aries-cloudagent-python/CHANGELOG.md#082) (PR [#2223](https://github.com/hyperledger/aries-cloudagent-python/pull/2223)) suppressed an extra webhook event firing during the processing after receiving a connection request. An unexpected side effect of that change was that the subsequent webhook event also did not fire, and as a result, the controller did not get any event signalling a new connection request had been received via the multi-use invitation. The update in this release ensures the proper event fires and the controller receives the webhook.

See below for the breaking changes and the [CHANGELOG file](/CHANGELOG.md) for a categorized list of the pull requests included in this release.

Updates in the CI/CD area include adding the publishing of a nightly container image that includes any changes in the main branch since the last nightly was published. This allows uses the "latest and greatest" code via a container image vs. having to install ACA-Py from the repository. In addition, Snyk scanning was added to the CI pipeline, and Indy SDK tests were removed from the pipeline.

## 0.10.0 Breaking Changes

[#2352](https://github.com/hyperledger/aries-cloudagent-python/pull/2352) is a breaking change related to the storage of presentation exchange records in ACA-Py. In previous releases, presentation exchange protocol state data records were retained in ACA-Py secure storage after the completion of protocol instances. With this release the default behavior changes to deleting those records by default, unless the ----preserve-exchange-records flag is set in the configuration. This extends the use of that flag that previously applied only to issue credential records. The extension matches the initial intention of the flag--that it cover both issue credential and present proof exchanges. The "best practices" for ACA-Py is that the controller (business logic) store any long-lasting business information needed for the service that is using the Aries Agent, and ACA-Py storage should be used only for data necessary for the operation of the agent. In particular, protocol state data should be held in ACA-Py only as long as the protocol is running (as it is needed by ACA-Py), and once a protocol instance completes, the controller should extract and store the business information from the protocol state before it is deleted from ACA-Py storage.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.10.0-rc1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-24 01:40:57 +0000 UTC
    </span>
</div>

