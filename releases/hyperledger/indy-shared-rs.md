---
layout: default
title: indy-shared-rs
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/indy-shared-rs
---

# indy-shared-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-shared-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    indy-credx 1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0
                </span>
            </td>
            <td>
                This release switches the backend for `indy-credx` from `ursa` (which is now archived) to the new `anoncreds-clsignatures` package.

There are relatively minor breaking changes to the API:

- MasterSecret is renamed to LinkSecret.
- Creating a revocable credential no longer requires a tails file.
- Updating a revocation registry requires the credential definition and revocation private key, instead of the tails file.

There are also important security fixes:

- For issuers, new revocation registries must be created due to changes to the tails file contents. Credentials should be re-issued.
- For provers, the proof of non-revocation has been updated. This means that verifiers that have not been upgraded will not be able to verify the new proof.
- For verifiers, a new FFI method is added to verify either the older non-revocation proof format or the new proof format. This is only added to allow for a more gradual upgrade of the ecosystem, and will be removed in version 0.5.

Performance is generally improved, especially for operations such as creating a new revocation registry.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/indy-shared-rs/releases/tag/v1.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-07-12 00:15:53 +0000 UTC
    </span>
</div>

