---
layout: default
title: firefly-tokens-erc1155
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc1155
---

# firefly-tokens-erc1155 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc1155){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Rsjx version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not sure why we didn't see this in the Github actions builds, but after building API calls are failing due to the below stack.
See https://github.com/hyperledger/firefly/pull/215#issuecomment-940150647

This is due to a move in rxjs 7 that deprecated `toPromise`, and you should explicitly now use `lastValueOf`.
However, in my VSCode I did find the automatic type casting was a faff, and I had to make some more tweaks.

```
�[34;1mtokens_0_1        |�[0m �[32m[Nest] 17  - �[39m10/11/2021, 3:52:08 PM �[32m    LOG�[39m �[38;5;3m[RequestLogging] �[39m�[32mPOST /api/v1/init�[39m
�[34;1mtokens_0_1        |�[0m �[31m[Nest] 17  - �[39m10/11/2021, 3:52:08 PM �[31m  ERROR�[39m �[38;5;3m[ExceptionsHandler] �[39m�[31mrxjs_1.lastValueFrom is not a function�[39m
�[34;1mtokens_0_1        |�[0m TypeError: rxjs_1.lastValueFrom is not a function
�[34;1mtokens_0_1        |�[0m     at RouterResponseController.transformToResult (/root/node_modules/@nestjs/core/router/router-response-controller.js:32:27)
�[34;1mtokens_0_1        |�[0m     at /root/node_modules/@nestjs/core/router/router-execution-context.js:173:52
�[34;1mtokens_0_1        |�[0m     at /root/node_modules/@nestjs/core/router/router-execution-context.js:47:19
�[34;1mtokens_0_1        |�[0m     at processTicksAndRejections (internal/process/task_queues.js:95:5)
�[34;1mtokens_0_1        |�[0m     at async /root/node_modules/@nestjs/core/router/router-proxy.js:9:17
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 16:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Use strings to pass all values, as they are uint256
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update passing of int256 values to base10 strings
  - Per https://github.com/hyperledger/firefly/pull/215#issuecomment-939998082
- Update dependencies to pick up security fixes 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 15:14:34 +0000 UTC
    </div>
</div>

