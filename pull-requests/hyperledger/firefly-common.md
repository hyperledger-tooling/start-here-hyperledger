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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    Add support for passing custom HTTP headers through
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for two new features that can be used in FireFly core and other microservices.

- A header named `X-FireFlyRequestID` can be set on HTTP requests and the service will use that as the internal request ID, rather than a generated short ID. The request ID is now also propagated to other FFResty client requests so it can be used as a trace ID through several services.
- Support for passing custom HTTP request headers through. A set of header names can be provided in the `ffapi.HandlerFactory` called `PassthroughHeaders`. In FireFly core, these are specified under the `api` config section. These headers will be put onto the request context.
- If an FFResty client is configured with `passthroughHeadersEnabled: true` in its config section, it will set any headers that have been packed into the context on the new request that it builds
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 21:03:15 +0000 UTC
    </div>
</div>

