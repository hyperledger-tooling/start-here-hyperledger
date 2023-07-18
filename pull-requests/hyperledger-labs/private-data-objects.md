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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/445" class=".btn">#445</a>
            </td>
            <td>
                <b>
                    DRAFT: Update handling of client extensions and plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Plugins in the PDO shell have been fairly complicated to implement. This is the first step in a process to convert plugins and client functionality in general to a more portable and hopefully easier approach.

The gist is that every command is implemented as a class derived from a common base class that provides implementations of interactive display methods. Commands are grouped into families such as all the commands for interacting with contracts are a part of the contract command family.

This approach makes it relatively easy to write the client functionality one time and make it easily available through the pdo-shell, a command line bash shell, and through Python scripts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 03:51:13 +0000 UTC
    </div>
</div>

