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
                PR <a href="https://github.com/hyperledger/aries-askar/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    chore: update version to 0.3.0 dev
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Need to wait with releasing until #177 is merged

@andrewwhitehead  @berendsliedrecht @genaris all good to make a first 0.3.0 dev release?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 13:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Add method to ping store sessions; verify profile existence when opening a session
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #163 

For Postgres, this also ensures that a profile cannot be removed while there is an active transaction against it.

Includes a fix for the persistent test failure copying a Store instance on Windows.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 22:42:05 +0000 UTC
    </div>
</div>

