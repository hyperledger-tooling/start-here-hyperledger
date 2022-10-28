---
layout: default
title: yui-corda-ibc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-corda-ibc
---

# yui-corda-ibc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-corda-ibc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Relayer API server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - update `CommitmentProof` contents
    - `List<SerializedBytes<SignableData>>` is added
    - `FilteredTransaction` is used instead of `WireTransaction`
- introduce `IbcClientState`, in which a ClientState of any type (e.g. Corda or Fabric) is included
- fix grpc-adapter interfaces
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-28 01:07:48 +0000 UTC
    </div>
</div>

