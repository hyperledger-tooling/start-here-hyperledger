---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    Remove Azure Pipeline artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With the addition of Github Actions, the old Azure Pipeline CI artifacts can now be removed.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 16:10:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    Fix the build : renew expired test TLS certificates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the build: 

This PR renews a couple of integration test suite certificates, which had expired.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 02:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    Build release packages for arm64 CLI binaries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature

#### Description

- Generates arm64 CLI binaries for linux and darwin.

#### Additional details

This PR compiles sqlite3 using CGO on the various platforms.  

#### Related issues

- https://github.com/hyperledger/fabric/issues/2994


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 20:40:32 +0000 UTC
    </div>
</div>

