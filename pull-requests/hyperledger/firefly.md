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

