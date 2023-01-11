---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Fixed minor issues with the build pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #115 

- Switched back to static libraries as there were some small issues with the dynamic libraries. We should change it in the future, but for now this will work (it is just a bit more megabytes that have to be downloaded).
- tested here https://www.npmjs.com/search?q=indy-vdr-test
- Supersedes #127 

Work funded by the Government of Ontario.

Signed-off-by: blu3beri <blu3beri@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-07 19:57:45 +0000 UTC
    </div>
</div>

