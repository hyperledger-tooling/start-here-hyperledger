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
                    v1.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.5.1
                </span>
            </td>
            <td>
                v1.5.1 Release Notes - August 16, 2021
======================================

Improvements
------------

**FABC-931: Re-enroll with existing key even if certificate is expired**

As of Fabric CA v1.4.9 it is possible to reenroll and get a certificate using an existing
private/public key pair when passing --csr.keyrequest.reusekey to the Fabric CA
client re-enroll request. This is advantageous especially for TLS certs since it means an
orderer identity can get a certificate with updated expiration without the channel
configuration needing to be updated (as of Fabric v1.4.9 and v2.2.1 when TLS certs
are verified between channel members only the key is checked, the entire certificate
does not need to be identical). However, if the certificate is already expired,
Fabric CA has historically returned an error and did not allow the identity to
reenroll to receive a new certificate.
This improvement allows the client to re-enroll even if the current certificate is expired.
To use the improvement, start the Fabric CA with the configuration option ``ca.reenrollIgnoreCertExpiry``
set to ``true`` (or set environment variable FABRIC_CA_SERVER_CA_REENROLLIGNORECERTEXPIRY).
Alternatively, start the Fabric CA with flag ``--ca.reenrollignorecertexpiry``.

Fixes
-----
Release binaries for Linux and Windows that were corrupted in v1.5.0 have been fixed in v1.5.1.

Dependencies
------------

Fabric CA v1.5.1 has been tested with the following dependencies:
- Go 1.15.7
- Alpine 3.13 (for Docker images)


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

* a01d0ae681a3d71e7b812cd9c9e5ad852fcc7621 Build release artifacts on native platforms
* d6f546ba4b9f43fcf11bda0b8d0bc08912607563 Release commit for Fabric CA v1.5.1
* 71436f400465dcecc09abe0dd66e20830da77711 Add native target description in Makefile
* 9b0e156edd9b244254b0ffb5189e6aeaa9f51bea review comments
* 5c502ff88ba9ef3dedee4cc53ae06a240b4b6f28 Docs updates
* cb74047a1f8d0d4d86d83ecc24e0f96f11a1b647 Review comments and added an integration test
* ac256a9b5fe43f562fdb819b75f860ce80049909 Support ignoring certificate expiry for re-enrolls
* 385273877385b0cffbd9b1bb07245a722f4a9fea 521 is not supported anymore
* 2147670bd8b25199dfd897dbfbea5ac3fbbc6eba fixed 521 to 512 ecdsa algorithm
* 05fe243f24bfc761d3c075c4049b093ed7d270d8 fixed missed double quotation
<details><summary><b>See More</b></summary>

* 2f05c9a10dbe43344b11572ea612ed53d534b392 fixed a typo
* 0e750f79ac8ed92d4317879d3d5e339b8eaf3784 Enable arm64
* 9a9d6ff0a2d43aec1d97cea7b66676a9d31a345a Bump jinja2 from 2.10.1 to 2.11.3 in /docs
* c8d2ffb69208f64ada7ac90c23d856fd8a23a8c5 Update default branch to main
* 8ea82d3026af0358aadd1f08907d81a90c86501f Update Fabric CA Readme
* 7fd582b1363f6234c99e18b36ca0b6f9c5cb4f6e Update doc references for main branch
* 99187d5ba2ed394fa9cb07673f776e7deb0e6a54 Update CI to use main branch
* 7bb43f222167ba15d37cf1e6ca7e732ef7e0fcb6 Remove local copy of repolint.json
* f960dd479c830c16f39405d528cb1fddbb970b9d Prepare for next version Fabric CA v1.5.1
* 6e825cc1a71a2ed191f17182eef8e6888108a212 Add release Target to Release Pipeline
* fd12c1d23e6f033996ac64c7b7e963b0fe3b7e76 Change release pipeline service connection

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=39316&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-ca/releases/tag/v1.5.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-08-17 19:50:27 +0000 UTC
    </span>
</div>

