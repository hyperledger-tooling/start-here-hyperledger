---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Refactor Fetch SQL queries in Postgres backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An attempt at some optimizations on the `FETCH_QUERY` and `FETCH_QUERY_UPDATE` Postgres queries.

Opening as a draft PR while I work on figuring out a way to benchmark the updated queries.

According to GPT:
> The refactored versions with the LEFT JOIN and GROUP BY clauses, as well as the use of CTEs are likely to be more efficient in terms of performance, especially when dealing with large datasets. It allows for a more optimized approach to data retrieval, particularly when combining information from multiple tables.

Please be as pedantic as possible (`-Wclippy::pedantic -Wclippy::nursery`).

Related to #195 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 09:21:06 +0000 UTC
    </div>
</div>

