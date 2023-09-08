---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    fix(js): bump patched ref-napi/ffi-napi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the issue with types that appeared in https://github.com/hyperledger/aries-askar/pull/170#issuecomment-1708337866, here we update patched `ref-napi` and `ffi-napi` to embed their own types instead of using the ones from the original ones.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 20:43:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Make zeroize not used with `no-default-features`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #241 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 07:25:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    Simplify create_credential parameters and remove RevocationRegistryId
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As far as I understand, there's no such thing as a RevocationRegistryId, since RevocationRegistryDefinitionId covers that usage (for example, see within the Credential structure). Looking at the unit tests they seem to have been used interchangeably. If anything, I think there would need to be a RevocationStatusListId instead. So this PR removes RevocationRegistryId and just uses RevocationRegistryDefinitionId in its place.

When issuing via `create_credential`, the revocation registry definition ID can be taken from the status list object.

The Python wrapper is updated, but I haven't looked at updating the JS wrappers yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 19:21:36 +0000 UTC
    </div>
</div>

