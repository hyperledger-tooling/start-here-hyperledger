---
layout: default
title: fabric-gateway-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway-java
---

# fabric-gateway-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    Add pointer to Fabric Gateway client API for Fabric v2.4
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
        Created At 2022-02-08 18:24:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Close InputStream on Wallet.get() (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of e50a619ada02d5434c3fbfae539f123e509fa8e9 from main branch.

The Wallet get() method did not close the InputStream returned by the WalletStore. For store implementations backed by persistent storage, such as FileSystemWalletStore, this was a resource leak.

Updated dependency versions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 17:23:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Close InputStream on Wallet.get()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Wallet get() method did not close the InputStream returned by the WalletStore. For store implementations backed by persistent storage, such as FileSystemWalletStore, this was a resource leak.

Wrote and then removed a unit test for close of the InputStream since a Mockito spy of the InputStream broke the JSON parsing only when run with Java 17. Updated dependencies in an unsuccessful attempt to resolve Java 17 mocking issues.

Closes #97
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 12:41:34 +0000 UTC
    </div>
</div>

