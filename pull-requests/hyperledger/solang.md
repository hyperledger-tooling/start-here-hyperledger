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

