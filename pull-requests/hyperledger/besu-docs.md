---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1509" class=".btn">#1509</a>
            </td>
            <td>
                <b>
                    Document RPC authentication JWT algorithm option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When [generating a keypair for JWT public key authentication](https://besu.hyperledger.org/public-networks/how-to/use-besu-api/authenticate#jwt-public-key-authentication), if you use a different method than `RS256` to generate such keypair, especially if you use a `ESXXX` method, you also need to specify such method in the command line options. Otherwise you'll face a `java.security.InvalidKeyException: Invalid RSA public key` exception when running `besu`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-11 23:45:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1508" class=".btn">#1508</a>
            </td>
            <td>
                <b>
                    Add sequenced synonym for legacy txpool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add `sequenced` synonym for `legacy` non-layered transaction pool, and remove deprecation warnings for non-layered transaction pool. Fixes #1470.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 23:23:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1507" class=".btn">#1507</a>
            </td>
            <td>
                <b>
                    Add Joan as docs maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds Joan Edwards (@joaniefromtheblock) to the list of Besu docs maintainers. She has authored the following PRs:

- #1485 
- #1486 
- #1490 
- #1501 
- #1504 
- #1502 
- #1503 

You can see [her current list of PRs](https://github.com/hyperledger/besu-docs/pulls?q=is%3Apr+author%3Ajoaniefromtheblock+).

> Note: This PR also moves Mike Sanko to emeritus status.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 19:43:26 +0000 UTC
    </div>
</div>

