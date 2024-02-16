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

I needed to ensure I was returning the correct `Content-Type` for my responses. Binary was supported but not plain text. And I wanted to have the OpenAPI accurately reflect the expected response `Content-Type` and allow for greater future customization.

## Changes

- For routing / server - adds a new `StreamHandler` extension similar to the `JSONHandler` but with the expectation that an `io.ReadCloser` is returned. The route handler will continue to assume it is streaming binary unless a `Content-Type` header is already specified.
- For OpenAPI generation - adds a new `CustomResponseRefs` to allow for adding custom responses for either streams or JSON. 

## TODOs
- [x] confirm from maintainers this the right API we want for streams
- [ ] unit tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 13:29:25 +0000 UTC
    </div>
</div>

