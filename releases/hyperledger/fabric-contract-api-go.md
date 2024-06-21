---
layout: default
title: fabric-contract-api-go
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric-contract-api-go
---

# fabric-contract-api-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-contract-api-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0
                </span>
            </td>
            <td>
                ## v2 Release Notes
The v2 release is functionally equivalent to the v1 release. The primary difference is the use of the [current Go API for protocol buffers](https://go.dev/blog/protobuf-apiv2) in place of the original (deprecated) API. The v2 implementation retains wire-level compatibility with Fabric but does include the following breaking changes:

- Chaincode implementations that make direct use of `github.com/hyperledger/fabric-protos-go` will experience protocol buffer namespace conflicts (as described in https://protobuf.dev/reference/go/faq/). Any use of **fabric-protos-go** must be replaced by `github.com/hyperledger/fabric-protos-go-apiv2`.
- In order to avoid an indirect dependency on **fabric-protos-go**, chaincode implementations that make use of `github.com/hyperledger/fabric-chaincode-go` must instead use `github.com/hyperledger/fabric-chaincode-go/v2`.

## What's Changed
* Update dependencies to address GO-2024-2687 by @bestbeforetoday in https://github.com/hyperledger/fabric-contract-api-go/pull/129
* v2 implementation based on fabric-chaincode-go/v2 by @bestbeforetoday in https://github.com/hyperledger/fabric-contract-api-go/pull/137

## New Contributors
* @benjsmi made their first contribution in https://github.com/hyperledger/fabric-contract-api-go/pull/133

**Full Changelog**: https://github.com/hyperledger/fabric-contract-api-go/compare/v1.2.2...v2.0.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-contract-api-go/releases/tag/v2.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-20 23:10:55 +0000 UTC
    </span>
</div>

