---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    Avoid bug in typescript-eslint@5.13.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pin to ~5.12.1 to avoid bug in v5.13.0 causing false positives in async Mocha tests.

https://github.com/typescript-eslint/typescript-eslint/issues/4609
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 15:57:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/554" class=".btn">#554</a>
            </td>
            <td>
                <b>
                    Fix environment variables to correctly data format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                process.env will implicitly convert the value to a string.
If an environment value is set as a boolean or number, the value
will be a string. This patch uses environment value from nconf.env
not process.env.

Signed-off-by: Nao Nishijima <nao.nishijima.xt@hitachi.com>
Reported-by: Shinsuke Hasegawa <shinsuke.hasegawa.fc@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 04:24:23 +0000 UTC
    </div>
</div>

