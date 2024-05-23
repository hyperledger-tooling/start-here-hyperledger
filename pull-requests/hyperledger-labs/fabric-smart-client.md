---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/574" class=".btn">#574</a>
            </td>
            <td>
                <b>
                    Cache fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses two issues detected by the integration tests of Token SDK:
* When two nodes try to set the state at the same time, one gets a duplicate error and doesn't update the vault. Then we don't fail, because we know that another process has updated it, but the txidstore cache remains with the same previous value. Now we invalidate the cache and fetch the new value.
* When multiple replicas are trying to commit the same TX and rewrite the same keys, we get a deadlock error from the DB. Now we retry every time we get a deadlock error until the operation is successful. This means that either the other writes have failed so we can write the new values, or the other writes were successful so we update the state (using the same values).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 06:45:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/573" class=".btn">#573</a>
            </td>
            <td>
                <b>
                    remove default resolver, register the node id itself so we don't need…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … the alias.

This PR attempts to solve two things:

1. The default resolver, which was registered with the node id and the grpc address, was causing unpredictable behaviour with the new websockets communication method (the default resolver is selected instead of the correct one - even though the grpc address is empty).
2. It was necessary to list the resolver id as 'alias' in the configuration, even though it's not really an alias if it's the same id. The code in this PR binds the node id to itself, so it's not necessary anymore to do that.

For the first one, I'm not sure if this code was still in use in some way. For the second, binding the id to itself looks a bit odd, and there might be cleaner solutions available that I'm not aware of. Would like to get some feedback before 'undrafting' it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-17 15:24:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/572" class=".btn">#572</a>
            </td>
            <td>
                <b>
                    Move Mathilde to Emeritus
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
        Created At 2024-05-17 12:29:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Replace deprecated logging param in nwo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, NWO uses the deprecated --logging-level param when invoking the peer cli. This commit replaces this param with FABRIC_LOGGING_SPEC env variable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-17 12:06:01 +0000 UTC
    </div>
</div>

