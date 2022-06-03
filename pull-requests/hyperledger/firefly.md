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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    Move /admin/api to /spi and PUT->PATCH
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                > Leaving this as a draft until the updates to FFTM are complete, because otherwise early adopters trying out the feature will not have a functioning combination.

- [x] Rename the `/admin/api/v1` API to `/spi/v1`
- [x] `PUT`s change to `PATCH`s, because there are race conditions between delete/update that mean PUT semantics wouldn't be safe without optimistic concurrency locking
- [x] Make sure all APIs FFTM needs to function are on this API, so it doesn't need to use two
  - [x] `GET` `/spi/v1/operations`
  - [x] `GET` `/spi/v1/operations/{ns}/{opid}`
  - [x] `PATCH` `/spi/v1/operations/{ns}/{opid}`
  - [x] `GET` `/spi/v1/namespaces`
  - [x] `GET` `/spi/v1/namespaces/{ns}`
- [x]  Continue to allow FFTM to use cross-namespace calls on the internal API
- [x] Add namespaces to the API that FFTM has

> Previously we discussed additional changes, to allow event listeners hosted in FFTM to be stateless - and avoid the
> need to have a REST API + LevelDB in FFTM to manage listeners/checkpoints. This worked out to be too complex
> to change right now. Specifically because:
> 1. BatchPin is not tracked as a listener
> 2. Token connectors use the APIs of EthConnect today to directly create event streams

Note thread in discord: https://discord.com/channels/905194001349627914/979733575496790086
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 23:24:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/841" class=".btn">#841</a>
            </td>
            <td>
                <b>
                    fabconnect async calls + setting broadcast/private message header types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span><span class="chip">backport-complete</span>
            </td>
            <td>
                This PR adds two changes included in future release `1.0.2` into upstream firefly.

https://github.com/hyperledger/firefly/pull/838
https://github.com/hyperledger/firefly/pull/836

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 20:48:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/839" class=".btn">#839</a>
            </td>
            <td>
                <b>
                    Disable external link checking when building docs, due to unreliable external servers
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
        Created At 2022-05-27 18:23:58 +0000 UTC
    </div>
</div>

