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
                PR <a href="https://github.com/hyperledger/firefly/pull/975" class=".btn">#975</a>
            </td>
            <td>
                <b>
                    Adjust defaults for all cache items that don't expose a Size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Caches may be limited on size (if the items advertise their Size) or on
number of items. Since most cached items do not expose a Size, the limit
should be set on number of items alone.

Picked numbers pretty much at random, so I'm open to feedback if they
should be higher or lower, or if any of these items should get a Size method
to do size estimation.

I've tagged with "migration_consideration" since I have renamed a few
config keys, but I don't think they're widely used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 19:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/974" class=".btn">#974</a>
            </td>
            <td>
                <b>
                    Leverage transaction cache in a few more places
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
        Created At 2022-08-17 18:33:36 +0000 UTC
    </div>
</div>

