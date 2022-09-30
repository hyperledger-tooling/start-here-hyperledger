---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/588" class=".btn">#588</a>
            </td>
            <td>
                <b>
                    Builder pattern in agency client configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                Allows constructing agency client more eloquently as

```let agency_client = AgencyClient::new().configure(&agency_client_config)?;```

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 10:39:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    Make vcx_issuer_send_credential return SM state number
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 19:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/585" class=".btn">#585</a>
            </td>
            <td>
                <b>
                    Add CONTRIBUTING.md file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 17:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/581" class=".btn">#581</a>
            </td>
            <td>
                <b>
                    Reorganize libindy module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                - rename `libindy` module to `indy` - better vocabulary to cover both libindy (well more accurately libvdrtools) and in upcoming future implementation using bcgov extracted libs
- `libindy/wallet.rs` and `libindy/utils/wallet.rs` are merged into `indy/wallet.rs`
- number of files pulled out of `libindy/utils/*.rs` to `indy/*.rs`
- `ledger.rs` and `pool.rs` reshuffled to `ledger/pool.rs` and `ledger/transactions.rs`
- `cache.rs` renamed to `wallet_non_secrets.rs`
- `crypto.rs` renamed to `signing.rs`
- `signus.rs` renamed to `keys.rs`
- `anoncreds.rs` was originally huge file - its content is now reshuffled to more appropriate files across `indy/`
- added submodule `credentials` to cover issuance and receiving credentials
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 11:46:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/580" class=".btn">#580</a>
            </td>
            <td>
                <b>
                    Remove pool handle from connection protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-25 17:28:07 +0000 UTC
    </div>
</div>

