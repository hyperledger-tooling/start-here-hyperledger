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
                PR <a href="https://github.com/hyperledger/firefly/pull/852" class=".btn">#852</a>
            </td>
            <td>
                <b>
                    Fix github.ref in prereleased action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-03 19:06:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/851" class=".btn">#851</a>
            </td>
            <td>
                <b>
                    Use API framework newly moved to cmomon with extension points
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In https://github.com/hyperledger/firefly-common/pull/16 the API framework was made general for re-use in other microservices.

Specifically [FFTM](https://github.com/hyperledger/firefly-transaction-manager), which needs REST APIs for subscriptions and event streams.

The Swagger has changed a tiny bit in this:
- Fixed a typo in a description
- The formatting of the default `request-timeout` header is now `2m0s` rather than `120s`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 20:17:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/850" class=".btn">#850</a>
            </td>
            <td>
                <b>
                    Remove unneeded BatchManager references
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
        Created At 2022-06-02 18:55:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/849" class=".btn">#849</a>
            </td>
            <td>
                <b>
                    Enhancements to migration/network version behavior
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Network version is loaded during blockchain plugin init, instead of lazily. This is (soon) going to be needed at manager initialization time, so might as well load it once upfront.

Since we currently have a single blockchain plugin that services all namespaces, any termination/migration event is recorded against ALL namespaces (rather than arbitrarily recording it against ff_system only).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 17:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/845" class=".btn">#845</a>
            </td>
            <td>
                <b>
                    Update dependency versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 17:43:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    Allow extra options to pass through to blockchain connectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the ability to pass additional options through to blockchain connectors. This is useful for controlling other parameters when submitting a blockchain transaction besides the specific arguments that a smart contract function takes. For example, this can now be used to set a custom gas price

<img width="2537" alt="Screen Shot 2022-05-31 at 11 39 25 AM" src="https://user-images.githubusercontent.com/2530008/171214094-4fb58412-eb32-4748-a223-5bd37d007be6.png">

Anywhere that a smart contract can be invoked or queried a new `options` JSON object (treated as a `map[string]interface{}` in Go) can be optionally specified. Any fields in this structure will be included in the request to the blockchain connector.

Overriding existing fields in the request is **not** allowed. For example, if using Ethconnect, the following request body would be rejected because `headers` is a field that FireFly itself needs to set:

```json
{
  "input": {
    "newValue": "x"
  },
  "options": {
    "headers": "not allowed"
  }
}
```
This would result in an HTTP 400 with an error message indicating which option was not allowed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 15:46:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/843" class=".btn">#843</a>
            </td>
            <td>
                <b>
                    Verify namespace for all broadcast/private message requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #817
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 14:45:58 +0000 UTC
    </div>
</div>

