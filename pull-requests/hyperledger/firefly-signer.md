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
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Fix oneOf FFI param schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After attempting to update FireFly Core to use the new version of this library, I realized the `oneOf` wasn't implemented quite correctly, given the JSON Schema library that we're using here. This PR corrects that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 15:36:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Add function for decoding event ABI data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds an `Entry. DecodeEventData` function that takes a `topics` array, plus `data` bytes, and decodes into a value tree.

Also updates a bit of spelling for consistency.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 21:12:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Proposal to standardize elementary type info in the abi package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Here's my proposal for how to address my suggestion in https://github.com/hyperledger/firefly-signer/pull/9#discussion_r905462373

Note I filled in the gap on the floating point input, with a `oneOf` there, and this means the test fails due to `number` being missing from: https://github.com/hyperledger/firefly-common/blob/7f6b2eaf8066c146f377864981e92ea9e1f43903/pkg/fftypes/ffi_param_validator.go#L54-L58

> PR submitted here for common: https://github.com/hyperledger/firefly-common/pull/21
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 22:34:38 +0000 UTC
    </div>
</div>

