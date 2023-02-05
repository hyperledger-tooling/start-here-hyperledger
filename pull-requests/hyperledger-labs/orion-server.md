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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    Avoid instantiating the default marshaller before each use
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fix typo in class name

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 10:25:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Go 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">security</span>
            </td>
            <td>
                Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 08:22:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Allow issuing cert with URI instead of IP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                This is used by Orion's benchmark to issue certificates for the servers.

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 13:50:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Use lock-free map for LevelDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span>
            </td>
            <td>
                - Replacing map with sync.Map
- Caching DB snapshot after commit to avoid creating a snapshot for each Get operation
- Modifying cache to return byte array to avoid code duplication
- Remove Db lock because levelDB is already protected
- Reduce code duplication in Open()

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 14:58:42 +0000 UTC
    </div>
</div>

