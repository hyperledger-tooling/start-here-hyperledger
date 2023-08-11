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
                PR <a href="https://github.com/hyperledger/firefly/pull/1388" class=".btn">#1388</a>
            </td>
            <td>
                <b>
                    Use separate event stream per namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR resolves https://github.com/hyperledger/firefly/issues/1381

Because we are moving from a single event stream to one per namespace, existing subscriptions will be recreated and events will be replayed on a new event stream the first time a FireFly Core node starts with these changes. Otherwise there is no user impacting change in this PR.

Event streams now follow the format `<plugin_topic_name>/<namespace_name>`. For example, event stream for the `default` namespace with a plugin topic of `0` would now be: `0/default`.

There is still outstanding work to do in the tokens plugin and tokens connectors, but I'm splitting those out into separate PRs. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 20:53:53 +0000 UTC
    </div>
</div>

