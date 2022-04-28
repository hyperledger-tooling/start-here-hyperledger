---
layout: default
title: firefly-sdk-nodejs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-sdk-nodejs
---

# firefly-sdk-nodejs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-sdk-nodejs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sdk-nodejs/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    [alpha-10] package.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 21:19:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sdk-nodejs/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Use npm publish action provided by GitHub
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 20:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sdk-nodejs/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Update schemas from FireFly v1.0.0-rc.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 14:59:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sdk-nodejs/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Extract and wrap FireFly error messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If an error reply from FireFly has the form `{"error": "Something bad"}`, extract only the error message from the JSON and throw it as a new `FireFlyError` type. If the error message cannot be parsed, use the whole body text.

See https://github.com/hyperledger/firefly/issues/753
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 16:42:24 +0000 UTC
    </div>
</div>

