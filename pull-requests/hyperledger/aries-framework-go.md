---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3581" class=".btn">#3581</a>
            </td>
            <td>
                <b>
                    refactor: VC, VP, and supporting models moved into components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Verifiable Credentials and Presentation models are now in component/models/verifiable
- SD-JWT package is now in component/models/sdjwt
- move jsonld validator to component/models/ld
- Key fingerprint helpers and JOSE extensions moved to component/kmscrypto

All APIs in original afgo pkg/ folders can continue to be used, these now transparently refer/call the moved APIs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 20:18:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3580" class=".btn">#3580</a>
            </td>
            <td>
                <b>
                    chore: add CreateDisplayCredentialBytes
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
        Created At 2023-05-09 10:20:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3579" class=".btn">#3579</a>
            </td>
            <td>
                <b>
                    chore: add ValidateJSONLDMap
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
        Created At 2023-05-08 16:39:55 +0000 UTC
    </div>
</div>

