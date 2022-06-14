---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Add namespace information, batch event delivery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Add namespace to all subscriptions and events**

The /init and /activatepool APIs now accept a namespace, which will
be incorporated into the subscription names on ethconnect, and will
be unpacked and returned on all websocket events.

The field is mandatory on /activatepool (therefore requires a new
version of FireFly) but optional on /init (so older CLIs that attempt
/init will not be broken). Newer FireFly versions should also perform
/init once for each namespace utilizing this token connector.

Going forward, all ethconnect subscription names  will have a prefix
of "fft:" so they can more easily be recognized. This prefix can also
be versioned in the future if further subscription changes are needed.

Existing subscriptions will continue to function, but to avoid issues
when adding new subscriptions, the following migration steps are highly
recommended after upgrading the token connector:
- Stop the token connector and FireFly
- On ethconnect, remove all token subscriptions not starting with "fft:"
- Start the token connector and FireFly
- For every pool in FireFly that was created with an explicit address
  (rather than via the token factory), manually invoke /activatepool on
  the connector with the proper namespace and pool locator, and verify
  new subscriptions are created

---

**Add 'batch' event to deliver many events at once**

Fixes https://github.com/hyperledger/firefly-tokens-erc20-erc721/issues/52

Requires a new version of FireFly that understands this event.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 16:20:16 +0000 UTC
    </div>
</div>

