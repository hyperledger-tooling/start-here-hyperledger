---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    fix(js): integer list struct types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Another issue found during testing credential revocation in AFJ: remove pointer for integer arrays
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 21:59:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    fix(js): revocation status list typo and optional timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some things I found while digging a bit with revocation status lists in JavaScript.

Also, maybe more for a discussion or separate issue, but I find a bit odd to have both `updateTimestamp()` and `update()` methods in `RevocationStatusList` class from JS API. It could be more straightforward to just have `update()` and, if the only defined parameter is the timestamp, it can call `anoncreds.updateRevocationStatusListTimestampOnly`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 18:23:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    chore: cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed some of the unused delta related code
- Moved the revocation registry to its own file
- Some other minor fixes that do not change the functionality directly

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 07:35:45 +0000 UTC
    </div>
</div>

