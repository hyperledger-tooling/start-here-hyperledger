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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    fix(js): free native strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not completely sure if it's the right approach (especially in react-native) but here is a simple attempt to free strings automatically in JS wrappers before returning to the caller, as discussed in https://github.com/hyperledger/anoncreds-rs/issues/236. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 01:23:51 +0000 UTC
    </div>
</div>

