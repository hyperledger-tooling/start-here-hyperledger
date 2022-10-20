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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/495" class=".btn">#495</a>
            </td>
            <td>
                <b>
                    Update Java gRPC dependency to match Go implementation
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
        Created At 2022-10-19 20:02:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    Update Node dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes a TypeScript version update, and matching the fabric-protos versions used by Go and Java implementations. Minor changes to test code are required to satisfy new ESLint Jest rules.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 19:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    Update Go gRPC dependency to address CVE-2022-32149
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
        Created At 2022-10-19 18:06:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Use nancy directly as a Go tool to avoid Docker dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initially the Docker approach was attractive as it kept a nice separation of the nancy environment used to do Go code vulnerability scans. The build uses lots of Go tools directly already so it seems simpler to do the same with nancy too. This should make it easier to use a local exclude file checked into the repository if necessary, make it easier to keep the nancy version up-to-date, and remove the need for Docker outside of the scenario tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 17:14:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Update Java dependencies to address CVE-2022-3171
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
        Created At 2022-10-14 19:43:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Ensure all vulnerability checks run regardless of failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Go scan uses two scanning tools and a failure of the first would stop the second running. Split them into separate Makefile targets and run them as a matrix with fail-fast disabled.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 17:25:32 +0000 UTC
    </div>
</div>

