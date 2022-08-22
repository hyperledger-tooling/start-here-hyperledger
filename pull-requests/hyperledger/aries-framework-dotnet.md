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
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    Integrate indy vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                #### Short description of what this resolves:
This adds a Hyperledger Indy-VDR integration for AF .NET. Interfaces were minimally adjusted to handle different pool and request handles.

#### Changes proposed in this pull request:

- Adds DefaultPoolServiceV2, DefaultLedgerServiceV2 and DefaultSingingService
- Indy-sdk types were redacted from the interfaces
- Builder extensions AddAriesFrameworkV2 will add the Indy-VDR compliant services
- Integration tests for LedgerService and SchemaService included

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 06:58:05 +0000 UTC
    </div>
</div>

