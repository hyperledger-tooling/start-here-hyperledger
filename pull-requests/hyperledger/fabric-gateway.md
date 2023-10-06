---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    Remove support for Go 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the release of Go 1.21 in August 2023, Go 1.19 has not been a supported Go version.

Closes #615
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 23:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/640" class=".btn">#640</a>
            </td>
            <td>
                <b>
                    Update Gem dependencies
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
        Created At 2023-10-02 20:11:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/639" class=".btn">#639</a>
            </td>
            <td>
                <b>
                    Support ECMAScript explicit resource management in Node API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `[Symbol.dispose]()` implementation added to Gateway and CloseableAsyncIterable. For environments that support ECMAScript resource management (such as [TypeScript 5.2](https://devblogs.microsoft.com/typescript/announcing-typescript-5-2/#using-declarations-and-explicit-resource-management) and later), this allows the `using` keyword to be used to automatically close chaincode and block event iterables when they go out of scope instead of explcitly calling close with a try/finally block.

For example, this eventing code:

```typescript
const events = await network.getChaincodeEvents(chaincodeName, { startBlock: BigInt(101) });
try {
    for async (const event of events) {
        // Process event
    }
} finally {
    events.close();
}
```

Can be replaced with the following, where the clean-up carried out by calling `events.close()` is done automatically when the `events` variable goes out of scope:

```typescript
using events = await network.getChaincodeEvents(chaincodeName, { startBlock: BigInt(101) });
for async (const event of events) {
    // Process event
}
```

Closes #636
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-30 01:23:56 +0000 UTC
    </div>
</div>

