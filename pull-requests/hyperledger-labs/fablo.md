---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    Set version 1.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 13:44:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/458" class=".btn">#458</a>
            </td>
            <td>
                <b>
                    Update publish CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 13:40:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    Fix: Support Channel-Specific Chaincode Directories to Prevent Duplicate Docker Mounts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: updated fablo.sh to support channel-name/chaincode-name directory structure for Docker mounts

- Modify `executeOnFabloDocker` function to dynamically create Docker volume mounts for each chaincode based on the channel-name/chaincode-name directory structure.
- This change resolves the issue of duplicate Docker mount errors when multiple chaincodes are defined for the same network.


Fixes: #346 #228 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-22 12:10:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    Create ARCHITECTURE.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 09:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    Drop the yarn installation support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #451 

I have dropped the yarn installation, I am not sure about the nvm, I think will need that cause we are installing node js using nvm,I need slight clarification on this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 05:10:18 +0000 UTC
    </div>
</div>

