---
layout: default
title: web3j
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/web3j
---

# web3j <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/web3j){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2042" class=".btn">#2042</a>
            </td>
            <td>
                <b>
                    fix encodePacked DynamicBytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
**fix encodePacked DynamicBytes**

*In solidity, abi.encodePacked function is used to pack the given parameters into a **tightly packed byte array without inserting length information.** This function is commonly used for creating hashes or signatures of data in Solidity contracts, **It does not align the data to 32 bytes like abi.encode**.*

```
//  ethers   ^6.10.0
import {AbiCoder, ethers} from "ethers";
let packed = ethers.solidityPacked(["bytes", "bytes"], ["0x12", "0x12"])
console.log(packed)  //0x1212
```
### Where should the reviewer start?

1. TypeEncoder#encodePacked
2. DefaultFunctionEncoderTest#testEncodeConstructorPacked_multipleParameters
3. TypeEncoderPackedTest#testDynamicBytesEncodePacked

### Why is it needed?

**fix encodePacked DynamicBytes**   -> solidity bytes

## Checklist

- [ ] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [ ] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 13:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2039" class=".btn">#2039</a>
            </td>
            <td>
                <b>
                    Add contributor call details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
*required*

### Where should the reviewer start?
*required*

### Why is it needed?
*required*

## Checklist

- [ ] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [ ] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 18:32:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2037" class=".btn">#2037</a>
            </td>
            <td>
                <b>
                    web3j release fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
*required*

### Where should the reviewer start?
*required*

### Why is it needed?
*required*

## Checklist

- [x] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 08:30:37 +0000 UTC
    </div>
</div>

