---
layout: default
title: firefly-cli
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Improve ganache healthcheck and shorten timeouts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds an extra step to the ganache healthcheck, using `grep` to make sure that we actually get an HTTP upgrade response for the websocket. The previous code just assumed that if it didn't exit immediately that it was successful, which is not always a safe assumption. This also allows us to shorten the timeouts a bit, which should shave a few seconds off the stack startup time.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 13:40:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    Add healthcheck for ganache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should ensure the correct startup order for dependencies, should fix https://github.com/hyperledger-labs/firefly-cli/issues/35
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 19:09:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Suggested improvements for local dev
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Exposes ports for all services, to aid running of firefly outside of compose
  - Fixes IPFS which was exposing port `5000` rather than `5001`
  - Avoids port `6000` which Chrome does not like querying (for when `/webui` is enabled for IPFS)
  - Allows commandline options `-p` and `-s` to configure the base ports
     - FireFly base port - default 5000 with increment of 1 for each member (5000,5001,5002 etc.)
     - Service base port - default 5100 with increment of 100 for each member (5100, 5200, 5300 etc.)
- Allows `docker pull` to be disabled during `ff start`, for developers with locally built images
  - `ff start -n mystack`
  - Will update the e2e test to use this
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 02:41:17 +0000 UTC
    </div>
</div>

