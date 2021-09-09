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
                    v1.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.5.2
                </span>
            </td>
            <td>
                v1.5.2 Release Notes - September 8, 2021
========================================

Release v1.5.2 updates Fabric CA to be compatible with Go 1.16.7.

Dependencies
------------

Fabric CA v1.5.2 has been tested with the following dependencies:
- Go 1.16.7
- Alpine 3.14 (for Docker images)


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

* 17b4d1a448bd25bbfe805427367fc3e2bf3a4db2 Release commit for v1.5.2.
* f242447365027d06010b49a2fb89fe383165fcf7 Update alpine to 3.14
* 073587e5682b8999d8ff43d0bc327bed94e3128d Update Go to 1.16.7
* 7026aeee0b8e46d29432df586c8e53f4bdd9d92b Prepare for next release v1.5.2
* f9889d4171431ee63919bba7fe1c3b0e299c6f2f Bump Debian
* 916d684b536bf19b8897ba597b81c7355d6c852a Update CI Pool Image

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40704&view=logs).
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-ca/releases/tag/v1.5.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-09-09 19:07:44 +0000 UTC
    </span>
</div>

