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
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    Allow switching between return routing types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Short description of what this resolves:
This PR enables implementers to select different types of return routing. Before, the `return_routing` decorator was always set to `all` and could not be changed. Now, the default value is still `all`, but the value can be defined via a parameter of `SendReceiveAsync`.

#### Changes proposed in this pull request:

- Add parameter to `SendReceiveAsync` in `IMessageService.cs` and `DefaultMessageService.cs` which specifies the desired return_routing type

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 15:21:27 +0000 UTC
    </div>
</div>

