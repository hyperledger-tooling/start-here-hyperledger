---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Add intermediate headers support for update-client and refactor chain and prover interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - refactor some interfaces
  - LightClient: remove unnecessary methods and clarify method names(especially clarify on finalisation for header)
  - ChainI/ProverI: introduce QueryContext that keeps proof height and wraps `context.Context`
- fix https://github.com/hyperledger-labs/yui-relayer/issues/82
- [reorder proof generation and header setup](https://github.com/hyperledger-labs/yui-relayer/pull/83/commits/f3e3d308e42f5e7e3ef23f63e7eb98b6147f27ef)
  - it allows to remove unnecessary sync steps during packet relay with LCP
  - ref. https://github.com/datachainlab/lcp/pull/55
- [remove 'I' suffix from interface names](https://github.com/hyperledger-labs/yui-relayer/pull/83/commits/07ad300cb601f5d4268ef3c11061cdb0f53e8191)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 09:14:43 +0000 UTC
    </div>
</div>

