---
layout: default
title: mirbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/mirbft
---

# mirbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/mirbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Bug in CommitLogEntry hashing, view change
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A direct pointer to a CommitLogEntry was used in a HashOrigin
when requesting to hash the former. When the HashResult arrived,
the digest was added to the CommitLogEntry concurrently with the
HashRequest (pointing to the CommitLogEntry) being intercepted
and stored, resulting in a data race. Now the preliminary
CommitLogEntry (that is missing the hash) is stored locally by
the ISS protocol in a map and only the map's key (the
corresponding sequence number) is used as HashOrigin.

Signed-off-by: Matej Pavlovic <matopavlovic@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 17:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    PBFT good-case sub-protocol
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
        Created At 2022-03-09 10:16:11 +0000 UTC
    </div>
</div>

