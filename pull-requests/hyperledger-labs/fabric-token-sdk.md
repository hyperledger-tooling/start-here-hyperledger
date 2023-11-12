---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/516" class=".btn">#516</a>
            </td>
            <td>
                <b>
                    store mine key in tokenstore instead of processor directly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moving the storage of the mine key to the TokenStore makes the code more flexible to change; now the processor only uses the TokenStore for any storage instead of using the rwSet directly. An implementation of the TokenStore interface would be independent of the processor to decide how to store tokens and lookup values.

Note that the code assumes that tokens stored via `StoreFabToken` are always 'mine'. If that's not true we could change the signature of the method to add a boolean flag for 'mine'.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-12 15:05:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/515" class=".btn">#515</a>
            </td>
            <td>
                <b>
                    enhance VerifyCertifications to return processed certifications
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
        Created At 2023-11-09 10:25:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/513" class=".btn">#513</a>
            </td>
            <td>
                <b>
                    add sql database driver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a SQL driver for the ttxdb database.

Still in draft until:
- Include code for validation records
- Confirmation about expected functionality of Sender/Recipient wallet queries
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 13:09:40 +0000 UTC
    </div>
</div>

