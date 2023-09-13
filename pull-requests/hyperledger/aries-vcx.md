---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/975" class=".btn">#975</a>
            </td>
            <td>
                <b>
                    Remove `tokio`, `android_logger` deps from agency_client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - removes tokio dependency at cost of one test (very low value)
- also removed unused `android_logger` dependency
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 18:34:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/974" class=".btn">#974</a>
            </td>
            <td>
                <b>
                    Eradicate mediated connection from issuance and presentation integration tests, part 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Continuation of #967.

* Completely removes usage of `MediatedConnection` and `agency_client` from any and all integration tests.
* Removes legacy agency tests.
* MySQL tests are preserved, where keypair generation is used to test MySQL connection.
* Redundant `integration_tests` and `tests` modules were removed.
* Alice and Faber were significantly pruned, where the plan is to replace them with a singular test agent impl.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 18:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/972" class=".btn">#972</a>
            </td>
            <td>
                <b>
                    Feature/msg builders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces message builders through the `typed-builder` crate. The builder are based on the typestate pattern, but the crate is (at least advertised) to be fully compatible/replaceable by the `derive-builder` trait, which is using runtime construction of the type and allows for more flexibility (like passing builders around).

The `typestate` vs `runtime construction` decision will essentially depend on whether consumers want/need to build messages themselves and how convoluted these processes usually get. We don't really have to decide now, but it's a good thing to consider in the future.

For consistency reasons even some single fielded protocol specific messages contents implement builders, so that it is convenient, uniform and easy to know how one would go about composing a message.

There are some inner types which also implement the builders, yet for some types it is indeed quite the overkill (like `CredentialPreview`). I might revisit such types and just implement plain old `new()` constructors.

Another change that this PR brings is a uniformization of the `Invitation` message from the `Connection` protocol, so that the same decorators are used regardless of invitation type. The rationale is that it's much easier to reason with the invitation this way and since the protocol is old and won't be suffering changes it should be fine to simply deal with it like this.

Also, this addresses #949 .

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 12:08:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/971" class=".btn">#971</a>
            </td>
            <td>
                <b>
                    fix android compilation by providing libzmq to be dynamically linked
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify scripts to enable dynamic linking with libzmq by default on android
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 03:42:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/970" class=".btn">#970</a>
            </td>
            <td>
                <b>
                    Uniffi simple message relay
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
        Created At 2023-09-07 18:56:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/969" class=".btn">#969</a>
            </td>
            <td>
                <b>
                    Fix genesis file URL in vdrproxy config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                Tests using vdrproxy started failing as the URL used to fetch the genesis file was recently invalidated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 08:01:16 +0000 UTC
    </div>
</div>

