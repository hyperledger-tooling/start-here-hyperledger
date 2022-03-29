---
layout: default
title: minbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minbft
---

# minbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minbft/pull/246" class=".btn">#246</a>
            </td>
            <td>
                <b>
                    Semi-automated view-change test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request resolves #243.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 20:21:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minbft/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    Fix generation of duplicate Prepare messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request fixes a bug that caused generation of duplicate Prepare messages when transitioning into a new active new.

Related to #243, #176 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 12:53:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minbft/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Fix handling messages embedded into own generated messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request fixes a bug in handling of own generated messages. A replica could skip handling some of the messages it has generated shortly before resetting its message log and replacing it with a newly generated ViewChange or NewView message.

Relates to #176.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 20:26:06 +0000 UTC
    </div>
</div>

