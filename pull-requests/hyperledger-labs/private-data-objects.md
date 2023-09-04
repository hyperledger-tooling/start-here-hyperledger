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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/449" class=".btn">#449</a>
            </td>
            <td>
                <b>
                    fix broken twisted dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Twisted has a dependency on zope-interface. The path to zope-interface appears to have changed (it is now zope.interface). The failed dependencies causes the build to fail. This removes the dependencies from the sservice, pservice, and eservice python packages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 22:42:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    DRAFT: Update for OpenSSL 3.x, SGXSSL/SGXSDK 2.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a draft. The docker updates are not complete in part because the OpenSSL 3.x support in SGXSSL is not complete.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 15:44:07 +0000 UTC
    </div>
</div>

