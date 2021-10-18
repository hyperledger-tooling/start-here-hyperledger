---
layout: default
title: aries-staticagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-staticagent-python
---

# aries-staticagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-staticagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Add get_nowait and return messages in queue on flush
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
        Created At 2021-10-17 19:13:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    chore: bump version for 0.9.0-pre4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 01:29:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    fix: export new components from package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 01:24:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    feat: add helper for extracting recipients from packed message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 01:19:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Refine awaiting messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Having never been completely satisfied with the previous mechanism, this refactor seeks to simplify and solidify the message awaiting functionality of the static agent library. Rather than creating and tracking individual futures, these changes implement a new dispatcher that queues messages and provides a simple interface for retrieving messages from this queue. This dispatcher is temporarily installed using the `Connection.queue` context manager. On exit from the context, any messages that were received while queuing and not explicitly retrieved are passed to the main dispatcher for routing to handlers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 03:00:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    feat: better typing on ModuleRouter.__call__ using @overload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 11:24:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    Simplify Dispatcher
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an internal change to Dispatchers to remove some superfluous classes and simplify the interface used by Connection.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 10:54:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Further simplify module routing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed PartialType
- ModuleRouter.__init__() accepts a ProtocolIdentifier
- Modules now must define protocol as a string

BREAKING CHANGE: Modules must define protocol as a string and ModuleRouter must accept a protocol identifier

These changes remove a significant amount of "magic" for the sake of simplicity.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 19:00:32 +0000 UTC
    </div>
</div>

