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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    Fix ci: caching, mysql test build, nodejs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 22:14:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    Logging/adjust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                - lift log level to `info` for write/udpate/important-and-rare operations
- lift log level from `trace` to `debug` for potentially useful debugging operations
- simplified implementations of some of the`to_string` functions
- adjust log'error message content
- delete dead code
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 21:57:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    Expose verkey rotation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 20:22:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/477" class=".btn">#477</a>
            </td>
            <td>
                <b>
                    Npm/upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 19:10:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/476" class=".btn">#476</a>
            </td>
            <td>
                <b>
                    Try to fix intermittent testing fail in nodejs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 19:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/475" class=".btn">#475</a>
            </td>
            <td>
                <b>
                    Remove json log formatter, add color format, fix timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Change minute/second separator from `.` to `:`
- Add nanoseconds to timestamp
- Colorize log level by default
- Add `text_no_color` formatter which logs text without colorization
- Remove support for json log formatter - it wouldn't produce valid json logs if they contain non-ascii characters


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
                <span class="chip">enhancement</span><span class="chip">wrappers</span>
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

