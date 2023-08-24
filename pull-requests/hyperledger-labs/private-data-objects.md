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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/446" class=".btn">#446</a>
            </td>
            <td>
                <b>
                    Legitimately handle versions for packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We have not been very good about version updates. By default the version is extracted from the VERSION file but this requires an explicit commit to update.

This change uses the most recent annotated version tag to determine the major and minor numbers and the commit count to determine that patch number. Future versions should be annotatively tagged as 'vM.N.0'.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 00:20:31 +0000 UTC
    </div>
</div>

