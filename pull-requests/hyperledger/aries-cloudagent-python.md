---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1641" class=".btn">#1641</a>
            </td>
            <td>
                <b>
                    Update include seed in wallet_create_did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: DaevMithran <daevmithran1999@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 08:51:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1638" class=".btn">#1638</a>
            </td>
            <td>
                <b>
                    Fix auto connection response not being properly mediated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Connection responses associated with an invite that was created with mediation were not properly reporting the mediators endpoint and keys when automatically sent after receiving a connection request. This PR fixes this issue and also does some minor code clean up.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 18:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1637" class=".btn">#1637</a>
            </td>
            <td>
                <b>
                    feat: query connections by their_public_did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now that `their_public_did` is saved as a tag (https://github.com/hyperledger/aries-cloudagent-python/pull/1543), we can use it to filter connections made with a specific public did.

This PR adds the filter option to the get all connections endpoint. Same as with #1453, this will only work for connections made after PR #1453 was merged or if the upgrade command has been run
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 10:01:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1633" class=".btn">#1633</a>
            </td>
            <td>
                <b>
                    Move database operations inside the session context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## What is this PR for?
- Error state saving was done when the session could be already disposed

Signed-off-by: Andraž Cuderman <andraz.cuderman@global.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 13:07:37 +0000 UTC
    </div>
</div>

