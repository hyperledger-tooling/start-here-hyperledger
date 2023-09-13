---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Update Swagger UI and provide dynamic hostname support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Tidies up the OpenAPI generator code in `ffapi`
- Upgrades Swagger UI to V5
- Exposes on the `ffapi.APIServer` on `/api/openapi.yaml` as well as `/api/openapi.json`
- Allows an option for dynamically determining the public hostname from the request
   - For scenarios where there is complex API Gateway infrastructure in front of the FireFly server, that needs to propagate the external protocol/hostname/path via Header on each request

Note there are breaking API changes for any package that is directly using the SwaggerUIHTML function, which to my knowledge is only FireFly Core (where I'm working on a corresponding change).

There shouldn't be any breaking changes for consumers just using `ffapi.APIServer` to expose their routes as REST.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 20:21:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Improve mapping of errors on HTTP responses, and log stacks with debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The use of string parsing could be improved, especially as it doesn't work in cases where the `i18n` framework is used with custom non-`FF` prefixes (which we support).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 22:51:31 +0000 UTC
    </div>
</div>

