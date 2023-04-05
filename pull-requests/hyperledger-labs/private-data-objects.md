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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/425" class=".btn">#425</a>
            </td>
            <td>
                <b>
                    Remove the gipsy interpreter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes all files, references and dependencies on Gipsy. 

While Scheme still seems like a fantastic language for building smart contracts (see DAML for another commercial example), it is far easier to write in Wasm in Wawaka. This just removes a lot of the old and mostly unmaintained code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:57:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/423" class=".btn">#423</a>
            </td>
            <td>
                <b>
                    Remove all remaining mentions and code related to AoT wasm contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR completely removes any remaining documentation and code related to supporting AoT compiled wasm contracts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 00:51:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    Clean up 18.04 references
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses #381 .

A couple of references still persist in the proxy yaml files.
As detailed in those comments, once we improve the proxy handling, those files should become obsolete and be removed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 18:36:42 +0000 UTC
    </div>
</div>

