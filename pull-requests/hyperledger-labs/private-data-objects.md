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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    Significant update to build and install process for ccf ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several parts of this commit:

1.  Move the ccf python scripts into their own directory and package them into an installable python wheel file; this should lay the structural foundation for supporting our own version of the CCF python client (which is not included in more recent versions of CCF).
2. Canonicalize argument handling for the ccf python scripts; this moves all argument processing (including the common handling of creating the CCF client) into a single routine. All CCF python files should share the same structure and command line API.
3. Split the build of the CCF ledger components into two pieces. The first piece builds and installs the python packages. Since these utilities are useful on any PDO node (client, service, ccf ledger), they can now be installed independently from the pdo tp. The second piece is the PDO TP itself which need only be installed on ccf ledger nodes.
4. In order to package the ccf scripts in a wheel, copy the basic functions of the python.cmake macros from the pdo-contracts repository. Some modifications needed to be made (assumptions about directory structures are different) but the essence is the same. Also made some modifications to the project variables cmake library in order to generate the version number is a macro that can be used for naming the wheel files.

I would strongly recommend we merge this prior to merging #467 . The changes here should make processing command line arguments consistently and installing the policy registration scripts much easier. @prakashngit I can help modify your PR. 

Note that this PR addresses some of the issues brought up in #469 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 18:54:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    Simplify build and install for CCF
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several changes to improve the performance (and remove dependencies) for CCF startup. Many of the changes are centered in the ccf Makefile to separate the creation of the ccf clients (like the ping test, ledger authority retrieval and policy scripts that might reasonably be executed from anywhere) from the environment needed for a ccf service node (the script to start a ccf network).

The big win from the separation is that we can remove dependency on the sandbox script & pre-install all of the python package dependencies independently from the execution of the ccf nodes. The result is that the ledger containers start in a couple seconds instead of several minutes.

Note that a future PR will package the ccf client scripts separately and install them with other PDO packages so they are available on all PDO installations.

@bvavala your review is requested because the second commit adds the code to copy the member keys into the
ledger key directory. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 23:13:15 +0000 UTC
    </div>
</div>

