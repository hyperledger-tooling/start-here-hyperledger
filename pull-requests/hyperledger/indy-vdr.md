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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    integrate indy utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Integrated txn_signature into indy-vdr
- Added base64 and base58 inside the package
- Removed features from indy-utils

## Question

Do we want to just implement all the functionality, from `indy-utils` inside `indy-vdr` and reimplement this in `anoncreds` (There should not be a lot of code reimplemented inside anoncreds as most of it, if not all, will be stripped out)? 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 13:53:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/125" class=".btn">#125</a>
            </td>
            <td>
                <b>
                    build(android): add CI/CD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work funded by the Government of Ontario.

Signed-off-by: blu3beri <blu3beri@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 15:10:04 +0000 UTC
    </div>
</div>

