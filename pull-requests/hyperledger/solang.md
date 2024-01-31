---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1621" class=".btn">#1621</a>
            </td>
            <td>
                <b>
                    Fix fresh clippy lints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 09:56:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1620" class=".btn">#1620</a>
            </td>
            <td>
                <b>
                    Polkadot: Implement `caller_is_root` runtime API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recent versions of the contracts pallet expose a runtime API for contracts to check whether their caller is of root origin. The PR exposes this API as a builtin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 09:09:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1619" class=".btn">#1619</a>
            </td>
            <td>
                <b>
                    feat(parser): exclude build.rs, include auto-generated parser on crates.io
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Helps with compile times by removing dependency on lalrpop and build script when using `solang-parser` from crates.io. Downside is this is 2MB in tree, but this shouldn't be that big of a deal.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 15:37:30 +0000 UTC
    </div>
</div>

