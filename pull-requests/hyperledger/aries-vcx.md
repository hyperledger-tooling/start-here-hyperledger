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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/475" class=".btn">#475</a>
            </td>
            <td>
                <b>
                    Fix json log formatter, fix timestamp format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add missing quotes around `message` field for json log formatter
- Change minute/second separator from `.` to `:`
- Add nanoseconds to timestamp
- Colorize log level by default
- Add `text_no_color` formatter which logs text without colorization

Example JSON:
```
{"timestamp":"2022-04-24 18:11:03.320649000","level":"TRACE","filename":"aries_vcx/src/settings.rs","message":"clear_config >>>"}
```
Example text:
```
2022-04-24 18:16.50.179280000|TRACE|aries_vcx::settings           |          aries_vcx/src/settings.rs:166 | clear_config >>>
```


Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-24 16:14:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/474" class=".btn">#474</a>
            </td>
            <td>
                <b>
                    Build separate libvcx image of smaller size for release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - decreases size of released libvcx image by 75%; 2gb -> 500mb

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 22:32:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/473" class=".btn">#473</a>
            </td>
            <td>
                <b>
                    Async vdr-tools API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 13:22:19 +0000 UTC
    </div>
</div>

