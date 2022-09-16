---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3374" class=".btn">#3374</a>
            </td>
            <td>
                <b>
                    fix: Docker warning when using frapsoft/openssl on arm64 system
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolved a warning from Docker that would get printed when running the generate-test-keys Makefile target on an arm64 system. The warning from Docker alerts you that the image for frapsoft/openssl is for amd64, which doesn't match the system you're on (when using an arm64-based OS). To resolve the warning, you have to either use an image that matches the system architecture, or explicitly state the platform using the --platform flag. In this case, there is only an amd64 version of frapsoft/openssl, so I added the explicit flag to resolve the warning. I also added a TODO for us to find an arm64 alternative in the future (although the amd64 version of frapsoft/openssl does seem to work fine on arm64 Mac OS currently, presumably due to Apple's Rosetta translation layer or some other emulation layer).

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 20:44:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3372" class=".btn">#3372</a>
            </td>
            <td>
                <b>
                    feat: Validate did configuration for did and domain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Parse and validate DID configuration bytes.
Search through domain linkage credential(s) for specified did and domain. 
Validate domain linkage credential for Linked Data (JWT validation will be handled in different issue).

Closes #3371

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 19:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3369" class=".btn">#3369</a>
            </td>
            <td>
                <b>
                    refactor: Add handling inbound problem report messages inside legacy-connection protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Problem report inside legacy connection

**Summary:**
- Add handling problem report messages inside protocol
-  Cover with unit tests


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 06:57:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3368" class=".btn">#3368</a>
            </td>
            <td>
                <b>
                    feat: fix format filtering in pEx V2 for JWTVCs, and add bdd tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - also fix an issue with initializing sdk agents, when old clients
  still exist under the same name
- also rename wallet-jsonld bdd tests since they aren't jsonld-only

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 22:24:32 +0000 UTC
    </div>
</div>

