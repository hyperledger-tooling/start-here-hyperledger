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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1514" class=".btn">#1514</a>
            </td>
            <td>
                <b>
                    Document profile files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document `--profile` CLI option and add how-to page on using profile files. Slight updates to the "Use a configuration file" page. Fixes #1512.

Previews:
- `--profile` documentation: https://besu-docs-qvq914ru4-hyperledger.vercel.app/development/public-networks/reference/cli/options#profile
- Use a configuration file: https://besu-docs-qvq914ru4-hyperledger.vercel.app/development/public-networks/how-to/use-configuration-file
- Use a profile file: https://besu-docs-qvq914ru4-hyperledger.vercel.app/development/public-networks/how-to/use-configuration-file/profile-file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 07:43:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1513" class=".btn">#1513</a>
            </td>
            <td>
                <b>
                    Fix example for rpc-http-cors-origins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor fix for `--rpc-http-cors-origins` example with better formatting.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 06:05:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1511" class=".btn">#1511</a>
            </td>
            <td>
                <b>
                    Add deprecation note
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1506 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 21:11:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1510" class=".btn">#1510</a>
            </td>
            <td>
                <b>
                    Update storage amount
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1482 


Updating doc to reflect new numbers detailed in [this doc](https://docs.google.com/document/d/1ykIANeVOh9E95-l-ZQU1L6QkyXwpaBcXhPEr7w3xuSs/edit#heading=h.vcpe6a3o9ru9). 

Should Checkpoint values also be added to this table?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 19:20:49 +0000 UTC
    </div>
</div>

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

