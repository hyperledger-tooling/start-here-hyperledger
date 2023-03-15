---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Use latest Go release for Go vulnerability scan
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Go version cached by actions/setup-go sometimes lags several days behind a Go patch release. This can cause vulnerabilities in Go standard libraries to be flagged that are already resolved in the latest Go patch release.

The Go vulnerability scan has been failing for a week due to a vulnerability that is already fixed in the latest Go patch release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 00:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/568" class=".btn">#568</a>
            </td>
            <td>
                <b>
                    Build refactor for performance and clarity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use Junit5 platform runner for Cucumber tests, avoiding dependency on Junit4.
- Allow Java unit tests to be (optionally) skipped when running scenario tests.
- Split build into unit and scenario test jobs for each language, running in parallel.
- Run all Go lint checks in a single job to reduce the required number of build runners.
- Use Junit5 tree reporter plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 10:24:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    Improve golangci-lint performance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - For local runs, use binary instead of Docker image.
- For CI, use GitHub Action.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 17:38:01 +0000 UTC
    </div>
</div>

