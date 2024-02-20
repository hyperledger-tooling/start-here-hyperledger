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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    fix: empty stream state on broadcast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a broadcast is attempted and the steam state hasn't been initialise it caused a nil pointer.

Two ways to solve this:
- If the stream state is nil, set an empty one as part of broadcast but that means no connections will receive those messages until that map updates 
- Wait for a least one connection on this stream to start and then start broadcasting. At least one connection will receive the messages for the stream whilst it's connected

I've gone for the latter one. We perform best-effort delivery for broadcast, so it could be argued to do the former, any thoughts appreciated! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 12:12:15 +0000 UTC
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

