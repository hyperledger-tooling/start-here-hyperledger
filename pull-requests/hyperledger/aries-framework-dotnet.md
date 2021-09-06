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
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Improve Dispatch Error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Short description of what this resolves:
Improves error message to include the endpointUri

#### Changes proposed in this pull request:

Change to line 47 only:
From:
ErrorCode.A2AMessageTransmissionError, $"Failed to send A2A message with an HTTP status code of {response.StatusCode} and content {responseBody}");
To:
`ErrorCode.A2AMessageTransmissionError, $"Dispatch Failure. Endpoint:{endpointUri} Status: {response.StatusCode} Content: {responseBody}");`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 13:43:40 +0000 UTC
    </div>
</div>

