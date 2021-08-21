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
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    Add an "id" parameter to SendMessageWithID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Given the method naming, it feels more intuitive to pass this in (rather
than requiring the sender to set it on a nested field before invoking).

Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 21:06:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/160" class=".btn">#160</a>
            </td>
            <td>
                <b>
                    Make sync-async helpers less specific to messaging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changeset simplifies the `inflightRequest` interface and adds 3 new generic constructs:
* `inflightResponse`
* `requestType`
* `requestSender`

The core helpers of sync-async (`sendAndWait` and `eventCallback`) now deal with these generic types and perform much less messaging-specific inspection of the requests and responses. There are clearer extension points for new request-response flows that may or may not relate to messaging at all.

The end goal is that this will make it easier to wrap tokens (and other future operations) in sync-async handlers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 15:09:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/158" class=".btn">#158</a>
            </td>
            <td>
                <b>
                    Add config infrastructure for arrays of config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hopefully the test makes it clear how this works.

Had to jump through a couple of hoops in the `viper` API to allow defaults to work correctly, but per the test it should be all good now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 21:51:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    bump ui to v0.2.2
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
        Created At 2021-08-17 20:44:12 +0000 UTC
    </div>
</div>

