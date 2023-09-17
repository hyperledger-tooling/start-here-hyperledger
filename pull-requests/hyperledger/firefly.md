---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1402" class=".btn">#1402</a>
            </td>
            <td>
                <b>
                    Tezos plugin support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An additional FF core plugin with Tezos chain support, which utilizes recently created tezos connector.
https://github.com/hyperledger/firefly-tezosconnect
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 15:18:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1401" class=".btn">#1401</a>
            </td>
            <td>
                <b>
                    Fix SQL migration conflict and coverage gaps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We had two PRs get merged separately that used the same migration number. This PR also fixes two small gaps in unit test coverage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 20:04:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1400" class=".btn">#1400</a>
            </td>
            <td>
                <b>
                    Enhance OpenAPI interface, for namespace-local APIs, and extra routing options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently each namespace has it's own API, but you cannot get an OpenAPI/Swagger definition scoped just to that namespace.

This PR proposes an enhance OpenAPI / Swagger UI interface at the Namespace level, which allows an API to be generated that only contains the API at that level.

It also provides extra dynamic header support for the external URL that an individual namespace has been exposed on, such that the namespace local API can be exposed on a mapped URL/Host.

Depends on https://github.com/hyperledger/firefly-common/pull/97

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 00:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1399" class=".btn">#1399</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add OpenSSF Best Practices badge
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 20:01:52 +0000 UTC
    </div>
</div>

