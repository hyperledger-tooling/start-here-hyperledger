---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1738" class=".btn">#1738</a>
            </td>
            <td>
                <b>
                    Documentation on existing language wrappers for aca-py
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I do not know if this is a complete list, but I think this might be useful information for anyone getting started on implementing their own controllers.

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 10:36:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1737" class=".btn">#1737</a>
            </td>
            <td>
                <b>
                    Feature: Add the ability to deny specific plugins from loading
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of #1734, I found that the Revocation Notification V2 code
failed to properly run due to the fact that the V1 code was deleting the
DB objects before V2 could get to it. @dbluhm and I decided that adding
an option to deny specific plugins from loading was one of the better
solutions to the problem.

Before the plugin has been initialized, any plugins listed within
`--deny-plugins` will be unregistered to prevent them from initializing
and potentially interferring with other plugins that have conflicts.

Signed-off-by: Colton Wolkins (Indicio work address) <colton@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 21:58:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1734" class=".btn">#1734</a>
            </td>
            <td>
                <b>
                    Feat/revocation notification v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements Revocation Notification V2, as described in https://github.com/hyperledger/aries-rfcs/pull/721. At this time, V1 takes precedence over V2 when a revocation occurs and V2 never gets fired off. After talking with @dbluhm, I plan to implement a config option to disable/exclude the loading of specific plugins so that, in terms of configuration, one can disable V1 notifications to allow V2 notifications to be triggered. Since Indy-Anoncreds are currently the only standard to be implemented at this time, there are a few hard coded values pointing to "indy-anoncreds" until such a time where a second credential revocation format needs to be implemented.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 14:33:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1729" class=".btn">#1729</a>
            </td>
            <td>
                <b>
                    feat: allow querying default mediator from base wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 16:57:10 +0000 UTC
    </div>
</div>

