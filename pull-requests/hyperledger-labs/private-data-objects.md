---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/373" class=".btn">#373</a>
            </td>
            <td>
                <b>
                    Ccf upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces the following changes:

1. CCF version upgrade from 0.11.7 to 1.0.19.
2. PDO installation changes for Ubuntu version upgrade from 18.04 to 20.04. After this PR, 18.04 is no longer supported for PDO. As part of this, stock tinyscheme is now installed via apt install. 

A few points regarding CCF version upgrade:

1. CCF Base installation process is different for 1.0.19 (wrt 0.11.7) if one is installing CCF on a bare metal. (without docker) (deb vs tar files). CCF documentation https://microsoft.github.io/CCF/release/1.x/build_apps/install_bin.html should act as your guide. 

2. PDO clients no longer need to install CCF Base. Python client package is installed via pip. 

3. CCF user keys are no longer required by PDO clients. PDO clients will instead use one-way TLS. PDO TP now implements a custom authentication policy to permit anonymous PDO clients submit unauthenticated transactions.

4. PDO signing keys while using CCF based PDO TP will now use SECP384R1 as the ECDSA curve.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-18 04:02:48 +0000 UTC
    </div>
</div>

