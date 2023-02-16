---
layout: default
title: anoncreds-spec
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-spec
---

# anoncreds-spec <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-spec){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    Schema version note
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding a note as discussed in #130 .
I've only updated `version` of schema. However `version` and `ver` also appear in Create Presentation Request as:
- `version` is a string set by the [verifier](https://hyperledger.github.io/anoncreds-spec/#term:verifier), the version of the [presentation request](https://hyperledger.github.io/anoncreds-spec/#term:presentation-request) 
- `ver` is an optional string, specifying the [presentation request](https://hyperledger.github.io/anoncreds-spec/#term:presentation-request) version.
If omitted, “1.0” is used by default.
“1.0” to use unqualified identifiers for restrictions
“2.0” to use fully qualified identifiers for restrictions

Having `version` and `ver` in the same object looks weird. Was this already discussed?


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 06:48:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    Correct the ANDs and ORs in presentation request restrictions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 16:30:36 +0000 UTC
    </div>
</div>

