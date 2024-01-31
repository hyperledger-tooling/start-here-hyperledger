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
                PR <a href="https://github.com/hyperledger/fabric/pull/4652" class=".btn">#4652</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.6 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.21.6.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 16:00:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4651" class=".btn">#4651</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.6 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.21.6

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 15:42:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4650" class=".btn">#4650</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.21.6

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 15:36:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4649" class=".btn">#4649</a>
            </td>
            <td>
                <b>
                    Update github actions to use Node 20 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - actions/setup-go@v5
- actions/checkout@v4

Need to ensure checkout is done before setup-go for cache to work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 14:29:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4648" class=".btn">#4648</a>
            </td>
            <td>
                <b>
                    Update github actions to use Node 20 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - actions/setup-go@v5
- actions/checkout@v4

Need to ensure checkout is done before setup-go for cache to work.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 14:24:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4647" class=".btn">#4647</a>
            </td>
            <td>
                <b>
                    Patch gnark-crypto and github.com/sirupsen/logrus.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dependencies that need upgrades.

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

These dependencies need some love. They are not transitive dependencies, so they end up getting left behind in typical updates. Trust me, they need to be bumped.

#### Additional details

N/A

#### Related issues

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 22:50:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4644" class=".btn">#4644</a>
            </td>
            <td>
                <b>
                    change smartbft chain log message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Log message update

#### Description

This PR aims to fix a log message that includes the channel name twice. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 14:32:55 +0000 UTC
    </div>
</div>

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

