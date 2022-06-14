---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    SPI updates for new alpha
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updates FFTM images to work with new alpha
- Updates FireFly Signer image to latest release
- Adds an `spi` config section for the new SPI, which supersedes the Admin API
  - Note the old `admin` config section is not removed, as the FireFly CLI needs to generate config that works for the V1.0.x stream still, and without this section the admin API would be turned off in V1.0.x

With this the instructions in https://gist.github.com/peterbroadhurst/63b147c679f76d485523650e76796009 can be executed successfully (instructions updated to use the `alpha` channel, rather than source builds).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 21:47:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    Use firefly-signer for wallet creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the dependence on the `geth account import` command to perform the keystore v3 wallet encryption, and uses the `firefly-signer` library for that. This should speed up first time startup and new account creation.

I needed to re-arrange a couple of the steps around account creation, but I think the end result is better, deferring more of the specifics to the blockchain-provider implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 17:57:03 +0000 UTC
    </div>
</div>

