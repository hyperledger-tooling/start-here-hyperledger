---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4641" class=".btn">#4641</a>
            </td>
            <td>
                <b>
                    Update github actions to use Node 20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - actions/setup-go@v5
- actions/checkout@v4

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 14:20:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4640" class=".btn">#4640</a>
            </td>
            <td>
                <b>
                    Throttle greedy clients in orderer Broadcast API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit implements a shared rate limiter for connections authenticated with mutual TLS. The throttling and rate limiting is applied at both the Authority Key Identifier and Subject Key Identifier level, which guarantees no single organization or client can bombard the orderer with endless transactions on the expense of others.

The effective rate is divided across all clients and orgs for a time period specified by InactivityTimeout.

By default this feature is turned off.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-28 23:23:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4639" class=".btn">#4639</a>
            </td>
            <td>
                <b>
                    BFT chain test: update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

This PR includes rebasing and updates to the BFT chain unit tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-28 21:26:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4638" class=".btn">#4638</a>
            </td>
            <td>
                <b>
                    update the following actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <img width="961" alt="Снимок экрана 2024-01-29 в 00 02 10" src="https://github.com/hyperledger/fabric/assets/7284783/1732ca21-a39a-4dc6-bdf6-1558d1f46d0e">

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-28 21:03:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4637" class=".btn">#4637</a>
            </td>
            <td>
                <b>
                    BFT synchronizer in orderer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature
- Improvement (improvement to code, performance, etc)

#### Description

Create a BFT synchronizer for the smartbft chain


#### Related issues

#4566 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-28 16:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4636" class=".btn">#4636</a>
            </td>
            <td>
                <b>
                    Upgrade Docker Dependency to v20.10.27.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Move `github.com/docker/docker` to v20.10.27.

#### Additional details

This may be the last commit to v2.2, but it's definitely a good one.

#### Related issues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 19:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4635" class=".btn">#4635</a>
            </td>
            <td>
                <b>
                    docs: fix grammer for ledger docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Fix grammer for ledger docs.

#### Additional details

NA
#### Related issues

NA


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 17:04:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4634" class=".btn">#4634</a>
            </td>
            <td>
                <b>
                    Re-add the RSA definitions to BCCSP - RSA implementation additional c…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BCCSP supported RSA in version 1.4. The Fabric CA is currently using the Fabric 1.4 dependency. It is necessary to move Fabric CA off of Fabric 1.4 dependencies since they are no longer maintained. Fabric 2.X does not support RSA, however the CA still needs to support RSA for any older but not expired certificates that may be in use by older netwo

Github:
https://github.com/hyperledger/fabric/issues/4625


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 23:27:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4632" class=".btn">#4632</a>
            </td>
            <td>
                <b>
                    Fix docs that link to .md files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docs should link to the .html file rather than the .md file in order to get resolved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 22:38:35 +0000 UTC
    </div>
</div>

