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
                PR <a href="https://github.com/hyperledger/firefly/pull/1391" class=".btn">#1391</a>
            </td>
            <td>
                <b>
                    Enrich events for contract deploy success/failure
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
        Created At 2023-08-21 18:58:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1389" class=".btn">#1389</a>
            </td>
            <td>
                <b>
                    Two functions with the same param types, but different names, cannot share a cache entry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Issue

If you invoke a Method FFI to FireFly with one set of parameter names like:

- `myfunc(uint256 var1, address var2)`

Then you invoke another function with an identical ABI, but different parameter names like:

- `myfunc(uint256 _var1, address _var2)`

Then you will see the following error from EVMConnect, with valid inputs:

`FF10111: Error from ethereum connector: FF22034: Unable to parse input of type <nil>`

This is because the cache we use to avoid expensive JSON Schema compilation, uses a cache key that does not factor in the names of the parameters.

However, when we look at the input JSON Object to extract the parameters in order to pass them into EVMConnect, we need to know the exact parameter names.

### Fix

This PR proposes including all parameter names from the FFI in the calculation of the cache key.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 18:44:44 +0000 UTC
    </div>
</div>

