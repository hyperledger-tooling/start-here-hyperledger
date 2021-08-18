---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    Fix: Cannot launch chaincode in nano bash in Linux
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CHAINCODEADDRESS is set to host.docker.internal which is
only available in MAC and Windows environments.
For that reason, it cannot launch chaincode on Linux.
This PR sets CHAINCODEADDRESS to 127.0.0.1 instead of
host.docker.internal.

Signed-off-by: Nao Nishijima <nao.nishijima.xt@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 06:56:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/467" class=".btn">#467</a>
            </td>
            <td>
                <b>
                    Fixed state deserialize which is an uint enum in contract definition.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Luciano da Silva Ribas <luciano.ribas+git@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 18:06:48 +0000 UTC
    </div>
</div>

