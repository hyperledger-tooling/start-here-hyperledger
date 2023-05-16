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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3586" class=".btn">#3586</a>
            </td>
            <td>
                <b>
                    perf: reuse same gjson parser
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
        Created At 2023-05-15 11:07:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3585" class=".btn">#3585</a>
            </td>
            <td>
                <b>
                    feat: Revert feat: support for optional field in presexch (#3582)
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
        Created At 2023-05-10 13:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3582" class=".btn">#3582</a>
            </td>
            <td>
                <b>
                    feat: support for optional field in presexch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Support for optional field in presexch.


**Summary:**
Extended PresentationDefinition JSON Schema V1 with field `optional` and `contains`
This filed is already exist in the [relevant struct](https://github.com/hyperledger/aries-framework-go/blob/main/pkg/doc/presexch/definition.go#L181), but wasn't a part of the Schema.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 07:16:48 +0000 UTC
    </div>
</div>

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

