---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5711" class=".btn">#5711</a>
            </td>
            <td>
                <b>
                    Return all not selected transactions, not only invalid ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 15:09:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5710" class=".btn">#5710</a>
            </td>
            <td>
                <b>
                    Updated from main, disposable pr.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 12:43:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5708" class=".btn">#5708</a>
            </td>
            <td>
                <b>
                    replace ArrayList with HashSet for rpcMethodExists check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
When executing the RpcMethod.rpcMethodExists(String rpcMethod) method, using HashSet instead of ArrayList provides a very very small performance improvement of a few nanoseconds. 😂😂


## Fixed Issue(s)
nothing
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-16 09:09:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5706" class=".btn">#5706</a>
            </td>
            <td>
                <b>
                    Append ABI-decoded revert reason to message field in error responses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Todo:

- [x] eth_call unit tests
- [x] eth_estimateGas unit tests
- [x] Changelog

This PR does the following:

- Adds a helper function to `JsonRpcErrorResponse` to decode revert reasons
- Adds a private member variable `reason` to `JsonRpcError` which can optionally be set
- Appends the `reason` to the response from `JsonRpcError.getMessage()` so that whenever the message for a JSON RPC error is retrieved, any reason that is set is included e.g. `Execution reverted: ERC20: transfer amount exceeds balance`

__Note__: this is proposed as a change to existing behaviour. I have assumed (rightly or wrongly) that existing applications will most likely use `startsWith("Execution reverted")` or other language equivalent, to parse error responses today. The fact that Quorum returns errors in this format (and that there isn't an option to exclude the decoded reason) suggests that any application not using `startsWith` semantics for error parsing is already brittle to different ethereum clients. It could be made configurable in Besu (perhaps with a `--exclude-decoded-reason` or similar option) but my personal view is to treat this as a fix to existing behaviour and document it in the changelog accordingly. I'm open to other opinions on this from reviewers.

Example error response before this PR:

```
{
    "jsonrpc": "2.0",
    "id": 1,
    "error": {
        "code": -32000,
        "message": "Execution reverted",
        "data": "0x08c379a00000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000002645524332303a207472616e7366657220616d6f756e7420657863656564732062616c616e63650000000000000000000000000000000000000000000000000000"
    }
}
```

Example error response with this PR:

```
{
    "jsonrpc": "2.0",
    "id": 1,
    "error": {
        "code": -32000,
        "message": "Execution reverted: ERC20: transfer amount exceeds balance",
        "data": "0x08c379a00000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000002645524332303a207472616e7366657220616d6f756e7420657863656564732062616c616e63650000000000000000000000000000000000000000000000000000"
    }
}
```

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/5705
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 09:19:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5704" class=".btn">#5704</a>
            </td>
            <td>
                <b>
                    switch RlpBlockImporter tests to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Migrate RlpBlockImporterTest from JUnit 4.0 to JUnit 5.0 #5571

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
#5571 
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 06:47:35 +0000 UTC
    </div>
</div>

