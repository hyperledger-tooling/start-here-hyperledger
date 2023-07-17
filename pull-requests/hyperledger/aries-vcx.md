---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    Cleanup/constant
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 Remove unused constants
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 15:00:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/897" class=".btn">#897</a>
            </td>
            <td>
                <b>
                    Refactor dealing with tails_dir in tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor tests (way of creating tails directory)
- Clear up confusion calling variables `tails_file` what actually is `tails_directory`
- Remove duplicated method for creating tmp directories and files

CI: 
- Small adjustment, when building android docker image, in case of cache miss, do not try to load up `main` branch revision of that image (this is happening to optimize CI in order to reuse some docker layers)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 14:39:48 +0000 UTC
    </div>
</div>

