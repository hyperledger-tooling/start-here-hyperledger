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
                    Destroys cluster environment when a test fails
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

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 09:02:16 +0000 UTC
    </div>
</div>

