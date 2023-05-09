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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    Set of proposed small enhancements to httpserver, WS support, and others
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Expose `WrapCorsIfEnabled` independent of `HTTPServer`
- Expose `CalcRequestTimeout` independent of `APIServer`
- Address feedback from improved linter - some of which highlighted genuine issues.
- Issue from linter: Fix recently added common `version.NewInfo` utility - was ignoring inputs
- Fix missing `global.` on API Server config descriptions, causing re-definition in other packages
- Update `github.com/getkin/kin-openapi` to `v0.116.0` and address code change this requires in swagger generator
- Provided `ReceiveExt` functionality on `wsclient` to allow `Reader` based streaming when receiving
  - An optional alternative to the whole `[]byte` payload being loaded into memory for each message
- Provided `DisableReconnect` option on `wsclient`
- Set read deadlines when heartbeating enabled, so if the backend connection fails the read doesn't hang indefinitely
  - Without this, if the context cancels, or the send thread otherwise errors without the receive loop getting a socket error, the receive loop never exits
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-07 16:40:12 +0000 UTC
    </div>
</div>

