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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/546" class=".btn">#546</a>
            </td>
            <td>
                <b>
                    Release 0.40.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 07:25:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/545" class=".btn">#545</a>
            </td>
            <td>
                <b>
                    Include ~timing decorator on presentation request messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - include `~timing` decorator on outgoing messages
- extract building aries messages to functions to test easier testing of what the messages we send looks like (eg. whether they include ~timing)
- some minor refactoring run into through out the process (eliminated `send_handshake_*` functions, created `protocols/oob` module)

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 21:38:30 +0000 UTC
    </div>
</div>

