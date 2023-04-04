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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Expose the mock provider for other packages to use in tests
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
        Created At 2023-03-30 08:26:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    Add `APIServer` utility, `showconf` Cobra command, and debug server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                More items that can become common and avoid boilerplate in microservices built on this framework:
- A fully fledged `APIServer` that gives an opinionated way to run an API Server
   - Builds on the `httpserver` and `ffapi.Route`/`ffapi.Handler` framework making some opinionated decisions
   - Uses generics to allow you to pass through a single `manager` instance, or generate a context struct for each request
   - Includes metrics using the new metrics utilities recently added to common
- Cobra command for `showconfig` that you can just add to your root command
- Function to run the debug server with consistent config

Example of the code needed now to create an API Server:
https://github.com/hyperledger/firefly-common/blob/e6af84602ced0f11c35c2e8efbbd2ef287e2d702/pkg/ffapi/apiserver_test.go#L99-L113
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 08:27:37 +0000 UTC
    </div>
</div>

