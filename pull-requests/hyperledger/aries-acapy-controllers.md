---
layout: default
title: aries-acapy-controllers
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-controllers
---

# aries-acapy-controllers <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-controllers){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Git ignore node modules built in Traction demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Traction demo runs an `npm install` so we should gitignore any node modules in this repo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 22:43:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Readme steps for local tunnel for Traction demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Traction Demo steps in the readme will not work for running locally unless there's a way to expose the localhost.

Adding instructions here to use Localtunnel, which is very simple to set up and start https://theboroer.github.io/localtunnel-www/

Could use ngrok or other things, but Node/npm is required to start the Traction demo app supplied so it's easy to use Localtunnel in that case. We could also have a dockerfile that starts up everything, but a user would of course need Docker as well for that, so not sure if it's any simpler in that case. Could think of as a future step.

I tested these instructions and it worked a couple times for me on my Windows machine at home at least. Went through connection/issue/pres-req/revoke to my BC Wallet, using Sandbox. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 22:37:14 +0000 UTC
    </div>
</div>

