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
                    v1.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.5.4
                </span>
            </td>
            <td>
                v1.5.4 Release Notes - June 17, 2022
====================================

Release v1.5.4 updates Fabric CA to use https://github.com/IBM/idemix for the Identity Mixer implementation,
making it possible to issue credentials using various Identity Mixer curves.
The Identity Mixer curve can be configured in the Fabric CA server and client configuration yaml file:

```
# Specifies the Elliptic Curve used by Identity Mixer.
# It can be any of: {"amcl.Fp256bn", "gurvy.Bn254", "amcl.Fp256Miraclbn"}.
# If unspecified, it defaults to 'amcl.Fp256bn'.
curve: amcl.Fp256bn
```

Dependencies
------------

Fabric CA v1.5.4 has been tested with the following dependencies:
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

* 076f37bb68814b8dc4464d768b4263045ff32bc0 Release commit for v1.5.4
* 60ae815406b0b143859530999555e3a272ba9929 Run "go mod tidy" (#301)
* 9dbdf809e832b8b81dc1e95b4bda85c2c497fb71 Bump Alpine to 3.16 (#300)
* a0ab17964d1dd4e3fded074b9af1ec5222b1284f Update vendor for sys/unix
* e45e34725c62ed9f5a4bfa1b962846b3c9d46068 Update Fabric CA Readme (#296)
* dd6a104ff856a0dc2e5ac2bdceb321d6914cf70c Bump Go to 1.18.2 (#294)
* 78e1f1adad257e8bd7e5454d29d328cb757532b1 Make idemix use Mathlib instead of AMCL directly
* 6a9e85f9ee4079f295b0c9e19624076a5a59f742 Nominate Josh and Mark as maintainers
* 7405422b689940643e613eaf3045020b4a1e7b30 Add OpenAPI Documentation 
* 2e79a3e704f501a536748540e1e0776a6ed2e541 Fix swagger issues
<details><summary><b>See More</b></summary>

* 90e53e33661c36735708408c27a4054c57c754fa Wrong path
* d0e0abab810ba27c3be77ba1b25aa320eda03968 Minor type
* c6bbc4b865d87c28205c81776ddbde96b9db2507 test: use `T.TempDir` to create temporary test directory
* 8b815daa5620516fd5ff0bd58d35e802cc468f24 Prepare for v1.5.4 release
* e960bb96bd23febfa38178aa8f512bd33c4a2c45 Cleanup maintainers list

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=53830&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-ca/releases/tag/v1.5.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-17 16:29:22 +0000 UTC
    </span>
</div>

