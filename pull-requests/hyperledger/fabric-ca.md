---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/410" class=".btn">#410</a>
            </td>
            <td>
                <b>
                    handling `setLogLevel` error of `ConfigInit` if both `debug` flag and `loglevel` are set
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description
Either `debug` flag or a valid `loglevel` string is expected to be set to determine the log level of application.
When both are set, `setLogLevel` method returns an error which is handled in `ConfigInit`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-30 17:41:46 +0000 UTC
    </div>
</div>

