---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Allow for local override of contract families to be built
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                By default, all contract families are built. Tests will be run from all families.

This update supports a local cmake file (Local.cmake) that will allow for local overrides of variables. In particular, this is useful to set the new CMake variable CONTRACT_FAMILIES to just the subset that you want to build.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 00:11:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Updated Jupyter notebooks for exchange family 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Significant update for the Jupyter notebooks in the exchange contract family. Notebooks added for creating and importing orders, for interacting with an issuer as an account holder, and for kick starting the factories there is a new index file.

To make all this work, this update adds an experimental file format for sharing contract information. The file uses the python zip library (distributed with python) to package the PDO files and the context files. 

Updated from earlier draft PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 21:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Fix a problem with cleaning python egg directories
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix a bug in the python cmake library that resulted in just the exchange folder being cleaned correctly.

Mea culpa.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 23:36:37 +0000 UTC
    </div>
</div>

