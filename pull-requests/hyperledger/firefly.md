---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1331" class=".btn">#1331</a>
            </td>
            <td>
                <b>
                    Process batch of events from Blockchain connector, in a single DB TX
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                One of the outstanding observations from the performance testing in V1.2 was that we are performing a DB commit for each Blockchain event.

These are sequential on the single logical delivery thread from the blockchain connector (which currently is server-wide, although that should itself become namespace-wide).

This PR proposes that instead we update all the internal callback interfaces, to propagate the batch of events that come in over the wire from the connector, through to the event processor.

This means a few things handled in this PR:
1. Handling a batch that contains events of multiple types -  Batch Pin, Network Action, or custom Blockchain Event Listener
2. Handling a batch that needs different events dispatching to different namespaces
3. Continuing to handle old events that didn't come with a namespace at all (these are dispatched to all registered namespaces)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 05:48:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1330" class=".btn">#1330</a>
            </td>
            <td>
                <b>
                    feat: TLS Configs for Webhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sitting in draft as there is some more extend testing that needs to be done but this is the general idea I was going for. 

Have tested it e2e with a local server secured with mTLS and it works.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 16:37:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1329" class=".btn">#1329</a>
            </td>
            <td>
                <b>
                    Do not perform key resolution when looking up multiparty root org
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently whenever we look up root org details in multiparty mode, we are also performing key resolution on the org's default signing key every time. This is ~~only needed when we actually intend to use the org's key to sign something~~ 
 unnecessary, because in most instances we are only interested in the org name/DID. In the instances where the signing key is needed, it is separately resolved (so in these cases it is currently resolved twice).

I've adjusted all instances of the root org lookup to remove the signing key verification, and have adjusted the naming of methods to make it clearer when key resolution will occur.

Fixes #1328 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 20:53:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1327" class=".btn">#1327</a>
            </td>
            <td>
                <b>
                    Add unit test for "delete contract API" route
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
        Created At 2023-05-30 17:20:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1326" class=".btn">#1326</a>
            </td>
            <td>
                <b>
                    Perform nextpin calculations for both confirmed and rejected messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                Fixes #1324
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 17:19:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1325" class=".btn">#1325</a>
            </td>
            <td>
                <b>
                    docs: add mTLS section
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
        Created At 2023-05-26 16:12:14 +0000 UTC
    </div>
</div>

