---
layout: default
title: did-webs-resolver
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/did-webs-resolver
---

# did-webs-resolver <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/did-webs-resolver){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Feat/regex port and tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Will move from draft once Markus' changes have been merged.
updated regex to have optional port and path. also added some regex unit tests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 01:18:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Transform to/from did:web document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With this change, the DID document on the server is transformed to a did:web DID document (to be compatible with the did:web method), and when resolving it, it is transformed back to a did:webs DID document.

See corresponding spec change: https://github.com/trustoverip/tswg-did-method-webs-specification/pull/40
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 22:31:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Fix base_url
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
        Created At 2023-10-05 11:17:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Add support for --metadata in did webs resolve
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
        Created At 2023-10-05 10:43:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Add "versionId" DID document metadata property
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See spec support for "versionId" DID document metadata property: https://github.com/trustoverip/tswg-did-method-webs-specification/pull/49
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 10:28:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Add support for JsonWebKey and ConditionalProof2022
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements changes in https://github.com/trustoverip/tswg-did-method-webs-specification/pull/39 and https://github.com/trustoverip/tswg-did-method-webs-specification/pull/41
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 10:04:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Add py-multibase dependency.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It looks like https://github.com/hyperledger-labs/did-webs-resolver/commit/2263a3ecb3652e4a884a3cc91623d51c8dbabab0 removed the "py-multibase" dependency, but it's needed in https://github.com/hyperledger-labs/did-webs-resolver/blob/main/src/dkr/core/didding.py#L11 (at least for now).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 19:31:55 +0000 UTC
    </div>
</div>

