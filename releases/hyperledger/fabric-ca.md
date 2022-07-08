---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.5.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.5.5
                </span>
            </td>
            <td>
                v1.5.5 Release Notes - July 8, 2022
===================================

v1.5.5 is a maintenance release, providing updates for the following issues in the Fabric CA:

- Closes [Issue #305](https://github.com/hyperledger/fabric-ca/issues/305) : Issue with re-enrolling certificates

Dependencies
------------

Fabric CA v1.5.5 has been tested with the following dependencies:
- Go 1.18.2
- Alpine 3.16 (for Docker images)

Changes, Known Issues, and Workarounds
--------------------------------------

None.

Known Vulnerabilities
---------------------
- FABC-174 Commands can be manipulated to delete identities or affiliations

  This vulnerability can be resolved in one of two ways:

    1) Use HTTPS (TLS) so that the authorization header is not in clear text.

    2) The token generation/authentication mechanism was improved to optionally prevent
       token reuse. As of v1.4 a more secure token can be used by setting environment variable:

  FABRIC_CA_SERVER_COMPATIBILITY_MODE_V1_3=false

  However, it cannot be set to false until all clients have
  been updated to generate the more secure token and tolerate
  FABRIC_CA_SERVER_COMPATIBILITY_MODE_V1_3=false.
  The Fabric CA client has been updated in v1.4 to generate the more secure token.
  The Fabric SDKs will be updated by v2.0 timeframe to generate the more secure token,
  at which time the default for Fabric CA server will change to:
  FABRIC_CA_SERVER_COMPATIBILITY_MODE_V1_3=false

Resolved Vulnerabilities
------------------------
None.


## Changes:

* 9d2a31238d9204b1093bb770daaf79b834e18397 Release commit for v1.5.5
* 1f16304be0a3ed6ba5a5ae1dde7ae2df0ae839df Revert "Idemix MSP Folder Structure incompatible with what Fabric expects #303"
* 98dfc86c8586fa986be99c3fcdcd83f65301f3c6 Revert "fixup! Idemix MSP Folder Structure incompatible with what Fabric expects #303"
* f2fed4ddf529997bab850735f53bcc27fbc6bb68 Revert "create idemix `user` folder under root folder"
* 65315b2ed52cef4e0c82b2d5b40f3dda0c3319ef Revert "fixup! create idemix `user` folder under root folder"
* fac0ce6496ed4478f950389f2da09a91c49e18c8 Revert "fixup! create idemix `user` folder under root folder"
* 77c54da58aaf85c3f6a71f8af968ffb01431aefb fixup! create idemix `user` folder under root folder
* dfd29fe02e1e3cdb18b157dafc70e1df4040c048 fixup! create idemix `user` folder under root folder
* 0fcf897b4f57cfc774ebe5d5e75e75e89582429d create idemix `user` folder under root folder
* 29e083ecab02634beea6e9500ea4d86be3fa21a5 fixup! Idemix MSP Folder Structure incompatible with what Fabric expects #303
<details><summary><b>See More</b></summary>

* acea74626c69f180dd60e67f35c0d2aa0e3d6394 Idemix MSP Folder Structure incompatible with what Fabric expects #303
* 3be7a152bfb879e58b58f1bb53769519ddc00334 Correct handling of CA VerifyOptions (#306)

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=54593&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-ca/releases/tag/v1.5.5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-07-08 09:07:56 +0000 UTC
    </span>
</div>

