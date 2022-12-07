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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Release 0.50.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 09:35:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Release 0.49.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 18:13:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Fix legacy wrapper ios release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 16:01:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Replace failure crate with thiserror
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span><span class="chip">agents</span><span class="chip">dependencies</span>
            </td>
            <td>
                Replaces the dependency on outdated `failure` crate with the dependency on `thiserror` in `messages`, `aries-vcx-agent`, `aries-vcx` and `libvcx`. Although our entire approach to logging needs to be reconsidered, removing a dependency on an unmaintained crate is likely not a step in the wrong direction.

It seems that we have to temporarily give up backtrace in libvcx errors stored in `CURRENT_ERROR_C_JSON` until `error_generic_member_access` is [stabilized](https://github.com/rust-lang/rust/issues/99301) since `thiserror` makes use of [unstable](https://doc.rust-lang.org/std/error/trait.Error.html#method.provide) `provide()` method to the error type in order to capture and share `std::backtrace::Backtrace`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 21:57:10 +0000 UTC
    </div>
</div>

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
                    Handle did:sov service omitting routing_keys attribute
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

