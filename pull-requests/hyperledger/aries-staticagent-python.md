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

