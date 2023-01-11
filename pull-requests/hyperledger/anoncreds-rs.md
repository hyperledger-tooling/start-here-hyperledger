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
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    removed required prover_did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #52 

Implemented according to: https://github.com/hyperledger/anoncreds-spec/issues/107#issuecomment-1376698662

Also removed the dependency on `indy_utils::DidValue` which makes #40 a whole lot easier.

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 13:29:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    update revocation registry definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #22 

Where it was required, e.g. we pass it to Ursa, I used `ISSUANCE_BY_DEFAULT` which is a 0 or true.

@whalelephant could you also give this a review with regards to any revocation changes, I am not too familiar with the exact internals so just to be safe.

- removed the revocation registry config type
- removed V1 wrapper around revocation objects
- removed issuance by default reference

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 10:12:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    added schema attrNames validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 09:11:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Added `issuerId` to the `schema` and `cred_def` anoncreds objects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Partially closes #34 

- Adds `IssuerId` property to the `Schema` and `CredentialDefinition`.

This is reflects the PR for adding the `issuerId` to anoncreds objects.

(revocation needs to be done but is omitted here for conflicts with #37.

Signed-off-by: blu3beri <blu3beri@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 12:13:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Return NRP warning if presentation timestamp is outside of req interval
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #41 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 15:01:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Updated to correct openssl-src repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work funded by the Government of Ontario.

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 10:33:00 +0000 UTC
    </div>
</div>

