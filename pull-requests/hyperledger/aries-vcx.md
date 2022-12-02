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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Add ios legacy wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds building and release of ios wrapper ios_legacy, copied from 0.47.0 release (before https://github.com/hyperledger/aries-vcx/pull/663) was applied
- This legacy ios wrapper is added temporarily to make transition smoother and it's expected to be removed in soon future. The main wrapper is `wrappers/ios`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 11:38:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Release 0.49.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 10:52:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/681" class=".btn">#681</a>
            </td>
            <td>
                <b>
                    Release 0.48.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 09:44:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/680" class=".btn">#680</a>
            </td>
            <td>
                <b>
                    Drop actix dependency in 'messages' crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 23:20:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/676" class=".btn">#676</a>
            </td>
            <td>
                <b>
                    another agents no write routing_keys, in this case is none.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bugfix</span>
            </td>
            <td>
                when performing a test with acapy a routing_keys problem was discovered, it generates an empty ledger.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 19:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/675" class=".btn">#675</a>
            </td>
            <td>
                <b>
                    Implement a basic connection test using Actix framework
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">tests</span><span class="chip">agents</span>
            </td>
            <td>
                This was written purely to explore the Actix framework and its viability in aries-vcx integration tests.

As you can see, it can be used, but the benefits outside of perhaps saving a few lines per integration test are unclear. On the other hand, there are glaring drawbacks:
* async code in `handle` method [can't use](https://github.com/actix/actix/issues/308) (or at least trivially) the reference to `self` and thus a necessity for cloning in the handler, or
* having to clone the agent in the tests (since the `start()` method consumes the agent), or
* having to store handled messages in the agent itself (unlike when using a channel with a capacity).

In addition, it seems far from certain that actix would stay maintained for long. Here is a citation from the actix docs:
> Long ago, Actix Web was built on top of the actix actor framework. Now, Actix Web is largely unrelated to the actor framework and is built using a different system. Though actix is still maintained, its usefulness as a general tool is diminishing as the futures and async/await ecosystem matures. At this time, the use of actix is only required for WebSocket endpoints.

Again, this was just an exploration, so if you don't think the benefits outweigh the costs, feel free to close this PR.

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 15:42:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/673" class=".btn">#673</a>
            </td>
            <td>
                <b>
                    Create integration test on top of aries-vcx-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">tests</span>
            </td>
            <td>
                Create integration test on top of aries-vcx-agent
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 18:00:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/672" class=".btn">#672</a>
            </td>
            <td>
                <b>
                    Align service resolution on indy ledger with did:sov spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ase it does not find a search for service.

A new add_service_public method was added, which generates information in the ledger with this structure

    "endpoint": {
        "endpoint": "https://example.com",
        "types": [ "endpoint", "did-communication", "DIDComm"],
        "routingKeys": [ "did:key12345", "did:key12345" ]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 22:46:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    Implement Storage trait for agent's ObjectCache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">agents</span>
            </td>
            <td>
                Adds a Storage trait and implements it for Rust agent's ObjectCache. This may eventually allow for multiple storage implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 20:15:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/670" class=".btn">#670</a>
            </td>
            <td>
                <b>
                    Remove ios wrapper indysdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 16:20:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/668" class=".btn">#668</a>
            </td>
            <td>
                <b>
                    revealed parameter in prover building proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span>
            </td>
            <td>
                Signed-off-by: Pompeo Faruolo <pompeo.faruolo@etuitus.it>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 07:45:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    Validated some parameters passed as a JSON string.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove of the FFI layer also removed some validations of parameters passed as a JSON strings. This PR restore missed validations.

Signed-off-by: Artem Mironov <artem.mironov@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-27 21:14:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/666" class=".btn">#666</a>
            </td>
            <td>
                <b>
                    Set indy wallet master secret
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Set indy wallet master secret
master_secret parameter has been added to wallet config
Master secret is used in some methods where the wallet config is not there,
then has been added a global access to master secret of each wallet
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-27 05:52:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/665" class=".btn">#665</a>
            </td>
            <td>
                <b>
                    Generate node bindings using napi-rs - separate crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">wrappers</span>
            </td>
            <td>
                Based on approach taken by #661, but moving node API to a separate crate in order to minimize impact of NAPI boilerplate on libvcx.

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 14:28:06 +0000 UTC
    </div>
</div>

