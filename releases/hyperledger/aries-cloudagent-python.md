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

