---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Fabric CLI changes for asset-exchange using Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes:

- user registration/enrollment using go-sdk
- 'fabric-cli user add ' command in go-cli
- Minor typos in docs and in fabric-cli for node
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 19:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    Github Workflows for Unit and Integration Tests; Added local-docker page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added workflow for all Go unit tests.
2. Added workflow for node sdk unit tests.
3. Added workflow for corda interop app unit tests.
4. Added workflow for Locally built weaver components (host deployment): end-to-end data transfer test.
5. Added workflow for Imported Dockerized Weaver Components: end-to-end data transfer test.
6. Added workflow for end-to-end asset-exchange (fabric-fabric) test.

Fix:
Fabric driver build error fix.

Update:
1. Modified Dockerfiles and makefiles to build docker images locally.
2. Added docs page for `setup-local-docker`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 21:11:46 +0000 UTC
    </div>
</div>

