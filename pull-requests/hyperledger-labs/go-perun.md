---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    [backend/eth/ch] Test (To|From)EthState encoding.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing-only</span>
            </td>
            <td>
                - Cover `ToEthState` and `FromEthState` with unit a test

Closes #226
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 14:30:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    [sim] Use all bytes for Addr.String()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing-only</span>
            </td>
            <td>
                - Don't discard bytes anymore when encoding a sim address.  

Closes #261
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 13:47:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Context check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                - Introduces `wire.NewRelayNeverForget()` to remove a context check error
- Fixes one contextcheck error and removes a `nolint:staticcheck`
- Enables contextcheck for non-testing code

The remaining linter warnings in the CI need to be discussed.  
As far as i understand this, it wants us to introduce a context in `Client.Handle` and pass it down to the handlers, aka `handleChannelUpdate`.  
Currently the timeout for the handlers are derived from `client.Ctx` so there could be requests which run until the client is closed.  
We could add some timeouts like `channelUpdateTimeout` akin to `virtualFundingTimeout` and use them in `client.Handle`.  

What do you think?  
@matthiasgeihs 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 13:03:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Rename Address.Equals to Equal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactor</span>
            </td>
            <td>
                Closes #253 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 15:54:12 +0000 UTC
    </div>
</div>

