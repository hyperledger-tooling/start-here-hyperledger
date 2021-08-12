---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Add support for creating token pools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial support for tokens by plugging in an instance of https://github.com/hyperledger-labs/firefly-tokens-erc1155.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 19:15:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/153" class=".btn">#153</a>
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
                I was missing the `@` characters on the GitHub IDs previously :(
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 18:25:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Provide a blocking mode for async msgs, and add more intuitive POST routes returning types not messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements #112 

- Does _lots_ of dependency work to allow the sync-async bridge to be callable from broadcast/privatemessaging/networkmap
  - Adds a `syshandlers` package for the system event handlers that we previously bundled into `events`
  - Adds a `sysmessaging` that abstracts broadcast/private sends, and reply exchanges
  - Updates the orchestrator initialixation order to manage passing things between the internal components
- Deprecates all the old routes
- Adds new routes that:
  - Are all grouped on the path with the resources they create
  - Consistently return the object type that is the input
  - Have a `?confirm` option to block until the confirmation event arrives (or a 500 on the case it's rejected)
- Leaves the old routes there functioning exactly as today
  - Gives time for the CLI setup, and other consumers to move to the new routes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 02:50:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    bump ui to v0.2.0
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
        Created At 2021-08-06 18:10:59 +0000 UTC
    </div>
</div>

