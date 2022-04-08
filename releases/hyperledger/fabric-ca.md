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
                    v1.5.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.5.3
                </span>
            </td>
            <td>
                v1.5.3 Release Notes - April 7, 2022
====================================

Release v1.5.3 updates Fabric CA to be compatible with Go 1.17.8.

Additionally, packages that shifted from exported to unexported in v1.5.0 are now exported again.

Dependencies
------------

Fabric CA v1.5.3 has been tested with the following dependencies:
- Go 1.17.8
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

* 2061c8df7eda8516ea64a37471797852c92c2e61 Release commit for v1.5.3
* 8651918aea1b83bd7c64ddd943af5b62d29efc86 Undo breaking changes to exported packages
* c025d5ea5243d74d919df2d442975bd60386c37c Bump Go to 1.17.8
* 077518e71fb25b6beca91aca804997ebfafc0b36 Fix FVT intermediateca test
* 655a0f97c76b61c72e89a5669ad4cee58ad27262 Remove redundant assignment
* bb858908d0356edb678ee2be1ca8345f24d641d0 Bump fvt mysql to 0.8.22-1
* 62026907484c33f3ba599a283ebbccc54043882f Make server config.go and serverconfig.rst consistent
* 4c5d2ef98f6109ecceaa02e7b04aebe02fdff86f Fixes for CA deployment guide
* fc42d91b57b2f425b4985babfee8969e841572b7 fix expired root.pem certificate - was breaking 8-10 unit test cases
* 19cdbf5d1396dca57acdf378ae1964190c262ea7 Prepare for next release v1.5.3

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=50654&view=logs).
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-ca/releases/tag/v1.5.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-07 21:40:50 +0000 UTC
    </span>
</div>

