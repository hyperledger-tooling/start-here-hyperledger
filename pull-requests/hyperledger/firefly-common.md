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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Add ability to selectively ignore adding a route into the OpenAPI document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow at the Route level to choose to add it to the OpenAPI generated or not
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 16:48:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    [ffapi] Support for Text and Binary Streams
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Motivation

I needed to ensure I was returning the correct `Content-Type` for my responses. Binary was supported but not plain text. And I wanted to have the OpenAPI accurately reflect the expected response `Content-Type`.

## Changes

- For routing / server - adds a new `StreamHandler` extension similar to the `JSONHandler` but with the expectation that an `io.ReadCloser` is returned. The route will be assumed to be streaming binary unless a `StreamOutputContentType` is specified.
- For OpenAPI generation - adds a new `OutputType` to determine if the default JSON helpers are used, or the stream helpers. Streams are assumed to always return `200 OK` with the `Content-Type` being customizable through the same `StreamOutputContentType`.

## TODOs
- [ ] confirm from maintainers this the right API we want for streams
- [ ] unit tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 13:29:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Do not lose calling context in the logger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The log lines that contain the `breq` are currently missing the `req` and `httpreq` context, as well as any other calling context on that. It looks like a straight typo, that we're overwriting the `rCtx` with the constructor context of the client.
```
[2024-02-08T18:43:49.638Z] DEBUG EVMConnectorBody: {....} httpreq=dJAh7YSk pid=1 req=7hvX9eW_
[2024-02-08T18:43:49.638Z] DEBUG ==> POST https:/.../ breq=6yjJwWIC pid=1 proto=ethereum
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 20:07:15 +0000 UTC
    </div>
</div>

