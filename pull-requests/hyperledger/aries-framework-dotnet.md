---
layout: default
title: aries-framework-dotnet
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-dotnet
---

# aries-framework-dotnet <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-dotnet){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Allow arbitrary mime types for credential attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Short description of what this resolves:

Currently, in order to add support for new mime types in credential attributes one has to adjust the framework and add the wanted mime type. This PR proposes the option to allow any arbitrary mime types by removing the validation check of mime types.

#### Changes proposed in this pull request:

- Removes strict validation of credential attribute mime types in order to enable arbitrary mime types

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-14 14:37:56 +0000 UTC
    </div>
</div>

