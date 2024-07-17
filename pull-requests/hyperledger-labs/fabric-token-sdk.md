---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Next commits
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
        Created At 2024-07-16 22:15:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    Updated FSC version
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
        Created At 2024-07-16 11:23:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/695" class=".btn">#695</a>
            </td>
            <td>
                <b>
                    Added traces
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
        Created At 2024-07-16 08:20:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/694" class=".btn">#694</a>
            </td>
            <td>
                <b>
                    optimized balance with 64 precision
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
        Created At 2024-07-16 06:35:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/693" class=".btn">#693</a>
            </td>
            <td>
                <b>
                    cache audit info
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
        Created At 2024-07-16 04:38:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    add config flag for retries for selectors
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
        Created At 2024-07-15 15:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Fix duration metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                * Added different implementations to fetch the tokens. Behind these implementations we implement optimizations on how to fetch the tokens. The lazy one queries the database every time. The eager one polls the database and returns the cached result. The mixed one first serves the cached result and then the lazy one. Further strategies can be implemented as: a. Return the cached result if it is fresh enough. b. Listen for DB inserts in the token table and update the cache.
* Minimized the information we fetched from the database to avoid spooling big byte arrays
* Permutating the tokens every selector takes to avoid racing for the same tokens in the same order
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 22:01:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    fix data race in local membership
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevent some data race for the function `GetDefaultIdentifier` (reading list of resolvers) when called from `mapStringToID`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 13:49:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    orion update
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
        Created At 2024-07-10 17:25:14 +0000 UTC
    </div>
</div>

