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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    Simplify build with different curve
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The build with a different curve was optimized for the crypto library, but not for the common library and the rest -- thanks @prakashngit for spotting the issue and brainstorm a possible solution.
The main issue stems from putting the compile-time define in the crypto header.
As there are included by several (and probably all of the) PDO components, many cmake files have to be modified and also the `setup.py` which takes care of the python wrappers.

This PR removes the define from the headers.
Most importantly, it moves the default constructor using it from the headers to the respective cpp files.
As a result, the define is only used in cpp files and it can be easily set in the crypto cmake file.
This additionally allows to specify an exported global variable to pick the default value from the environment.
Finally, this seamlessly works with the python wrappers since the headers do not contain the define, and the crypto library (used by the python wrappers) is linked using the proper pre-compiled cpp static crypto library.

Signed-off-by: Bruno Vavala <bruno.vavala@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 06:18:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    Introduce client support key/value stores to enable large parameter passing to contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Implements support for python clients to build encrypted key/value stores. Among the uses, the key/value store enables large parameters to be passed to contracts. 

A number of other small improvements are included such as support for replication parameters in the pdo-shell. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 21:30:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Blockstore and configuration updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                PR includes two commits. 

The first makes the configuration globally accessible. A PDO client builds the configuration from files & command line switches and then pushes it into the global configuration. Services like the block store, file lookup, and replication manager can use it. Several strange defaults have been replaced with references to the global configuration.

The second commit moves the block store manager out of the storage service so that it can be used more generally. Specifically, the file system-based cache used by the client has been replaced with a cache based on the block store manager. This should simplify the process of managing the cache *as a cache*. Replaced several constants (that were overriding configuration file settings) with calls to the configuration manager. Generalized the block store to block store synchronization to make it easier to move blocks between various servers (may want to look at simplifying the replication service with this). The local block store cache will also simplify development of the client-side kv store management.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 16:52:12 +0000 UTC
    </div>
</div>

