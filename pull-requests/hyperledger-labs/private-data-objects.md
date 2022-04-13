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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    Create key/value store for client use
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Implement python client support for building key value stores
    
In order to share large data structures with a contract, this commit implements support for python to create and send encrypted key value stores.
    
A test script & contract are included to demonstrate how to pass a key value store as a parameter to a contract.

This includes a number of other bug fixes:
* fixes the wawaka system test execution in run-tests.sh
* adds a blockstore "head" operation that returns all metadata
* adds support for replication parameters in pdo-shell
* updates block-store-manager configuration handling
* allow the key prefix in wawaka to be empty
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 23:31:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/370" class=".btn">#370</a>
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
                This PR introduces changes to upgrade CCF version used for PDO-TP from 0.11.7 to 1.0.19.  A few points to note:

1. CCF Base installation process is different for 1.0.19 (wrt 0.11.7) if one is installing CCF on a bare metal. (without docker) (deb vs tar files). CCF documentation https://microsoft.github.io/CCF/release/1.x/build_apps/install_bin.html should act as your guide. PDO TP Installation expects Ubuntu 20.04.

2. PDO clients no longer need to install CCF Base. Python client package is installed via pip. The client package is tested only on Ubuntu 20.04.

3. CCF user keys are no longer required by PDO clients. PDO clients will instead use one-way TLS. PDO TP now implements a custom authentication policy to permit anonymous PDO clients submit unauthenticated transactions. 

4. PDO-dev docker image uses Ubuntu 20.04 as the base.

5. PDO signing keys while using CCF based PDO TP will now use SECP384R1 as the ECDSA curve. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 00:59:23 +0000 UTC
    </div>
</div>

