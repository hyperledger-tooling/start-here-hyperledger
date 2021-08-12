---
layout: default
title: firefly-ethconnect
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/firefly-ethconnect/issues/133" class=".btn">133</a>
            </td>
            <td>
                <b>
                    Arg packing for an empty slice actually returns an array
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                When packing the args for a `bytes` value that should be converted to a slice, one path actually returns a 0-length array instead of a slice, which results in the error reported for the "data" parameter here:
```
[2021-07-30T17:40:03.403Z] DEBUG Parsing args for function: function foo3(address[] to, bytes data) returns()
[2021-07-30T17:40:03.403Z] DEBUG Arg 0 requiredType: address[]
[2021-07-30T17:40:03.403Z] DEBUG Arg 0 value: [0xE57D3Fc7774DC54F1C1D618196FB4aFB933CE613] (type=[]common.Address)
[2021-07-30T17:40:03.403Z] DEBUG Arg 1 requiredType: bytes
[2021-07-30T17:40:03.403Z] DEBUG Arg 1 value: [] (type=[0]uint8)
[2021-07-30T17:40:03.403Z] ERROR Attempted to pack args [[0xE57D3Fc7774DC54F1C1D618196FB4aFB933CE613] []]: Packing arguments for method 'foo3': abi: cannot use array as type slice as argument
```

See here:
https://github.com/hyperledger-labs/firefly-ethconnect/blob/d7fd3fd213c85d164e9a610708ec912a55175969/internal/eth/txn.go#L623
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 18:31:01 +0000 UTC
    </div>
</div>

