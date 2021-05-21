---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    Update crate dependencies to latest solana_rbpf and more
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 10:50:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    Upgrade to tower-lsp 0.14 and tokio 1.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Changed

* Upgrade to `tower-lsp` 0.14.0 ([release notes](https://github.com/ebkalderon/tower-lsp/releases/tag/v0.14.0)).
* Upgrade to `tokio` 1.6 (single-threaded flavor, like before).

### Fixed

* Use async-aware `tokio::sync::Mutex` instead of `std::sync::Mutex` in order to avoid stalling the executor.

### Removed

* Remove redundant direct dependency on `lsp-types`, since it's already re-exported by `tower-lsp`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 01:38:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/418" class=".btn">#418</a>
            </td>
            <td>
                <b>
                    Solana contract instantiation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-16 15:25:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    Update integration tests to latest Solana/Burrow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-16 08:25:18 +0000 UTC
    </div>
</div>

