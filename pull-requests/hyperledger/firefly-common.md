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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Add config option to provide a regex to decide status code that can be retried
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add an option so that a regex can be used to determine which error status code should be retried to avoid unnecessary retries causing further delay and traffic.

There is already an `OnCheckRetry` function available for the developer using the library to support this feature. However this feature seems to be a standard configuration that would benefit all consumers. So I'm proposing to add it to this common lib.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 15:15:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Update MAINTAINERS.md and CODEOWNERS
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
        Created At 2023-09-13 18:21:42 +0000 UTC
    </div>
</div>

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

