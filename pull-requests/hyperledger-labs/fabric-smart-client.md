---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    fabric2.5, go1.20, and more...
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                This PR updates FSC to use Fabric 2.5.0 and go1.20.
In addition, it brings also the following improvements:
- `nwo/common/runner`: fix that prevented the check of the exit code
- `nwo/fabric/topology`: fix orderer address, add extra params to the topology
- `nwo/fsc`: fix tracing and metrics address, adjust topology
- `fabric/core/generic/committer`: don't parse events if a transaction has been already processed in the past.
- `fabric/core/msp/idemix`: support for BLS12_377_GURVY
- `fabric/core/vault/`: refactor the package to export more fields and allow extensions
- `fabric/core`: use RWSetLoader wherever possible
- `view/services/db`: introduce support for `TransactionalVersionedPersistence`. Only badger driver supports it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 07:36:51 +0000 UTC
    </div>
</div>

