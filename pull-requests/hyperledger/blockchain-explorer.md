---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    Fix ill-formed response by /api/peersStatus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After setting up explorer, I was getting this error when switching to the 'Network' Tab of the client view.
![image](https://user-images.githubusercontent.com/16841301/166065469-5a58dad7-b622-4f96-80b5-486fe4190a98.png)

Found out it was coming from Peer.js
![image](https://user-images.githubusercontent.com/16841301/166065519-1c2d8c55-7d1f-4c05-84a0-8056db7e1020.png)

Upon further investigation I found that the client would sometimes receive ill-formed json responses.
![image](https://user-images.githubusercontent.com/16841301/166065627-661f4827-c260-44d5-a018-2ea1a28cffab.png)

Then I checked the request 
![image](https://user-images.githubusercontent.com/16841301/166065779-fb32cd91-0c6b-4047-bce9-28f6681a5fbd.png)

After going through the api, I found out that for some cases [Proxy::getPeersStatus()](https://github.com/hyperledger/blockchain-explorer/blob/3950864ac4027374a664e327be5e98966dc34699/app/platform/fabric/Proxy.ts#L108) would return ill-formed JSON.

I have changed a few lines to cover those situations.

Signed-off-by: kaushikkumarbora <kaushikkumarbora@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 20:41:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    Update CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 21:47:11 +0000 UTC
    </div>
</div>

