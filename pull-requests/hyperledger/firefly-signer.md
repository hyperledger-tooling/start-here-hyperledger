---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    fix: check dynamic type for tuple before decoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes https://github.com/hyperledger/firefly/issues/1323


# Context behind the fix

I took a a look at this issue and turns out that when a Solidity struct is encoded in RLP and the type in the ABI is a tuple the resulting RLP doesn't have a variable ABI length block.

For the struct in Solidity contract:
```
    struct AccountBalance {
      address account;
      uint balance;
    }
```
We get the RLP
```
000000000000000000000000d2d8a61d774f552301d71aa99a78aff2e4765ca7 // address value
000000000000000000000000000000000000000000000000000000000000007b // balance value
```

After chatting with @peterbroadhurst  we determined based on the spec what a dynamic tuple means. A tuple is dynamic if any of its elements are dynamic! In this case the tuple isn't since `address` and `uint` are not dynamic.
![image (1)](https://github.com/hyperledger/firefly-signer/assets/30461857/6b39551d-8280-4901-b2a1-dd1da694d087)

The code was always treating a TupleComponent when decoding as dynamic and decoding the ABI length. The fix is to check if the Tuple is dynamic and if so decode the ABI length, or just walk through the bytes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 12:53:15 +0000 UTC
    </div>
</div>

