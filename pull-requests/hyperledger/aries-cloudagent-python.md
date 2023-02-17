---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2127" class=".btn">#2127</a>
            </td>
            <td>
                <b>
                    OpenAPI validation fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed when generating some Typescript types that the top level OpenAPI spec (Swagger 2.0 is the version) has some quick validation errors to fix. Checked against [editor.swagger.io](https://editor.swagger.io/) or other tools to call https://validator.swagger.io/

(I'm not actually using this openAPI json for generation, using the actual generated Swagger spec from a acapy + plugins deployment, but came across this while looking)

![image](https://user-images.githubusercontent.com/17445138/219472523-97c156d6-e91d-4222-a043-6d88bcf3eb02.png)


* **should have required property 'url'**
There is a externalDocs reference in /resolver that lacks a URL.
I'm not really sure about the resolver functionality so correct me if I'm wrong about using the following URL...
https://github.com/hyperledger/aries-rfcs/tree/fa4b1947c6077168d2c69f45ed6bee2bb1eae4c8/features/0124-did-resolution-protocol

* **should NOT have additional properties** (description)
A couple of the parameters have descriptions in the param, then an additional description in the `items` array, which is not supported by the spec.
Removed those, as they are unsupported, and seem redundant with the parameter description as well?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 19:56:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2125" class=".btn">#2125</a>
            </td>
            <td>
                <b>
                    Temporarily disable multi-architecture image builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Temporarily disable multi-architecture image builds until the required dependencies publish compatible packages.
- Details here; https://github.com/hyperledger/aries-cloudagent-python/issues/2124

- Add support for defining the image platforms when running the image publishing workflows manually.
- Add support for building off a git ref when running the image publishing workflows manually.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 16:32:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2123" class=".btn">#2123</a>
            </td>
            <td>
                <b>
                    Fix ACA-py image builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Ensure the final images install ACA-py from the wheel rather than from PyPI.
- Resolves #2121 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 23:04:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2122" class=".btn">#2122</a>
            </td>
            <td>
                <b>
                    Update some of the demo Readme and Endorser instructions
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
        Created At 2023-02-14 22:29:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2120" class=".btn">#2120</a>
            </td>
            <td>
                <b>
                    Update demo to issue multiple credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

@swcurran / @shaangill025  this adds an option to the demo ("1m") to issue multiple creds, in either indy or json-ld format.

It includes all creds in one offer, rather than the verbose request/response protocol.

Let me know if there are other additions to the demo you would like.

(There is also a new integration test - it doesn't work yet but @swcurran said last week to not worry about integration tests yet ...)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 18:39:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2117" class=".btn">#2117</a>
            </td>
            <td>
                <b>
                    Fix publish workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Trigger when releases and prereleases are published.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-11 13:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2116" class=".btn">#2116</a>
            </td>
            <td>
                <b>
                    Fix multi-use invitation performance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Multiuse invitation performance degrades over time. By adding state into the tag names, performance doesn't degrade over time while using multi-use invitations.

This breaks backwards compatibility, but while load testing it can be seen that performance no longer degrades when using a multi-use invitation. Previously, only 1600 connections could be established while load testing, and on a second run is reduced to 300. After the modification, the load testing exceeded 2400 connections and the testing client machine ran out of ram for clients.

This shows a clear improvement in performance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-11 00:37:00 +0000 UTC
    </div>
</div>

