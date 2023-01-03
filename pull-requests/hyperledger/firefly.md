---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1125" class=".btn">#1125</a>
            </td>
            <td>
                <b>
                    Custom errors support in FFI contract invocations and queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For a test solidity contract that declares custom errors like the following :

```
pragma solidity ^0.8.0;

error CustomError1(uint256 x, uint256 y);
error CustomError2(string x);

contract SimpleStorage {
    uint256 storedData;

    function set(uint256 x) public {
        if (x == 0) {
            revert CustomError1({x: x, y: x});
        }
        if (x == 1) {
            revert CustomError2({x: "This is a custom error"});
        }
        require(x > 2, "Can not equal to 2");
        storedData = x;
    }
}
```

Use the `POST /contracts/interfaces/generate` endpoint to generate the corresponding FFI:

```
{
    "namespace": "default",
    "name": "simple-storage-custom-errors",
    "description": "simple-storage-custom-errors",
    "version": "1.0.0",
    "methods": [
        {
            "name": "set",
            "pathname": "",
            "description": "",
            "params": [
                {
                    "name": "x",
                    "schema": {
                        "oneOf": [
                            {
                                "type": "string"
                            },
                            {
                                "type": "integer"
                            }
                        ],
                        "details": {
                            "type": "uint256",
                            "internalType": "uint256"
                        },
                        "description": "An integer. You are recommended to use a JSON string. A JSON number can be used for values up to the safe maximum."
                    }
                }
            ],
            "returns": [],
            "details": {
                "stateMutability": "nonpayable"
            }
        }
    ],
    "errors": [
        {
            "signature": "",
            "name": "CustomError1",
            "description": "",
            "params": [
                {
                    "name": "x",
                    "schema": {
                        "oneOf": [
                            {
                                "type": "string"
                            },
                            {
                                "type": "integer"
                            }
                        ],
                        "details": {
                            "type": "uint256",
                            "internalType": "uint256"
                        },
                        "description": "An integer. You are recommended to use a JSON string. A JSON number can be used for values up to the safe maximum."
                    }
                },
                {
                    "name": "y",
                    "schema": {
                        "oneOf": [
                            {
                                "type": "string"
                            },
                            {
                                "type": "integer"
                            }
                        ],
                        "details": {
                            "type": "uint256",
                            "internalType": "uint256"
                        },
                        "description": "An integer. You are recommended to use a JSON string. A JSON number can be used for values up to the safe maximum."
                    }
                }
            ]
        }
    ]
}
```

Then when invoking the generated API:

##  matching custom error
```
curl --location --request POST 'http://127.0.0.1:5000/api/v1/namespaces/default/apis/simple-storage/invoke/set' \
--header 'Content-Type: application/json' \
--data-raw '{
  "input": {
    "x": 0
  }
}'
```

response:
```
{
    "error": "FF10111: Error from ethereum connector: FF23021: EVM reverted: CustomError1(\"0\", \"0\")"
}
```

## no matching custom error (raw error data returned):
```
curl --location --request POST 'http://127.0.0.1:5000/api/v1/namespaces/default/apis/simple-storage/invoke/set' \
--header 'Content-Type: application/json' \
--data-raw '{
  "input": {
    "x": 1
  }
}'
```

response:
```
{
    "error": "FF10111: Error from ethereum connector: FF23022: EVM reverted: 0x60b7d47e0000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000001654686973206973206120637573746f6d206572726f7200000000000000000000"
}
```

## regular error from the require()
```
curl --location --request POST 'http://127.0.0.1:5000/api/v1/namespaces/default/apis/simple-storage/invoke/set' \
--header 'Content-Type: application/json' \
--data-raw '{
  "input": {
    "x": 2
  }
}'
```

response:
```
{
    "error": "FF10111: Error from ethereum connector: FF23021: EVM reverted: Can not equal to 2"
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-01 21:48:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1124" class=".btn">#1124</a>
            </td>
            <td>
                <b>
                    Minor cleanup in token pool event processing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After > 1 year, I think we can remove the special handling for this long-deprecated migration path around pre-0.11.0 token pools.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-30 15:10:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1123" class=".btn">#1123</a>
            </td>
            <td>
                <b>
                    Add ability to bind a contract interface to a token pool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16).
Depends on https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/104.

_Discussion about the overall architecture/usefulness of this proposed feature should be directed to [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16), while discussion here should focus on specific technical details of the current proposed approach._

This demonstrates a thin thread whereby FireFly can provide ABI details to a token connector, making it easier for the token connector to know the shape of the underlying contract it is dealing with (vs. having to probe/guess at the methods available).

With this change and the corresponding token connector changes, I was able to generate a custom ERC721 with auto-indexing via https://wizard.openzeppelin.com (a variant never previously supported) and successfully mint tokens.

**Outstanding Problems/Questions**
1. ABI format should not be assumed - it should either be configured in the token plugin configuration, or should be queried somehow from the token connector.
2. When creating a token pool, we should probably allow passing the interface by name/version in addition to by ID (similar to the flow when creating contract APIs).
3. We likely want a handshake protocol between FireFly and the token connector in order to prune down the ABI methods it cares about, rather than passing them all on every HTTP request (even a simple contract ABI may be 3KB or more, while a single method definition is around 150 bytes).
4. When ABI format is needed by the token connector, perhaps FireFly should store the converted method definitions rather than converting on demand before every operation.

**Other Misc Notes**
* This feature is only useful to users who have significant knowledge of the underlying token contract that sits on the other side of their token connector.
* It's likely to be most useful when creating a pool against a pre-deployed contract - ie when passing `config.address`. Worth mentioning that FireFly doesn't really "know" you can create pools against pre-deployed contracts (as `config` is opaque), but it's up to the user to understand the combination of features that are useful here.
* Theoretically you could create a factory contract that deploys custom ERC20/ERC721 instances, and then you'd need to pass `interface` on every pool creation even while relying on the factory sitting on the other side of the token connector to do the deploy. Seems like a less useful combo, but calling it out here for completeness.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-28 21:38:00 +0000 UTC
    </div>
</div>

