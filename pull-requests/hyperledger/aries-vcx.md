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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/579" class=".btn">#579</a>
            </td>
            <td>
                <b>
                    Proof presentation/always ack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 10:44:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/578" class=".btn">#578</a>
            </td>
            <td>
                <b>
                    Refactor/ci workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span><span class="chip">ci</span>
            </td>
            <td>
                Depends on #575 

Target: run all Rust tests under 30 mins.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 16:51:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    Separate messages module into a crate
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
        Created At 2022-09-21 07:56:03 +0000 UTC
    </div>
</div>

