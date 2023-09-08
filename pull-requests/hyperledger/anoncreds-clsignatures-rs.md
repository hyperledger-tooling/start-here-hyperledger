---
layout: default
title: anoncreds-clsignatures-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-clsignatures-rs
---

# anoncreds-clsignatures-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-clsignatures-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Include blinded messages in check for missing attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow up to #21 

The checks during credential issuance are extended to:
1. Include blinded attributes when checking if all attributes are provided
2. Check that there is no overlap between the blinded attributes (the link secret) and the attributes provided by the issuer

The second fix highlighted an issue with many of the unit tests, where the issuer was providing the `master_secret` attribute, and these are now fixed.

Tested for compatibility with indy-credx and anoncreds-rs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 18:30:53 +0000 UTC
    </div>
</div>

