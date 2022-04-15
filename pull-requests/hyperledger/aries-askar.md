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
                PR <a href="https://github.com/hyperledger/aries-askar/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    Reliability improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fix intermittent Not Found error when repeatedly updating existing rows (Postgres / Sqlite)
- Fix occasional memory access errors when using the Python wrapper
- Add unit tests for contention between transactions
- Add connection options for Sqlite backend (locking mode, journal mode, synchronized flag)
- Update to sqlx 0.5.12
- Update version to 0.2.5

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 00:11:29 +0000 UTC
    </div>
</div>

