---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    Destroys cluster environment when a test fails and avoid locking forever when waiting for a server after killing it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solves #428 

This commit adds a `destroyClusterEnv()` method that closes all the nodes that were started and removes the environment directory.
Each test, calls `defer destroyClusterEnv(t, env)` right after the environment is created to make sure it will be destroyed
even in the case of test failure.

It also adds timeout when waiting for a server in `(s *Server) shutdown()`.

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 09:02:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    acl on Provenance data queries
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
        Created At 2022-06-28 10:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/427" class=".btn">#427</a>
            </td>
            <td>
                <b>
                    provenance acl: for operations APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Operations such as reads, writes, and deleted
performed by an user can be retrieved either by
the respective user or by the admin only.

Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 10:03:48 +0000 UTC
    </div>
</div>

