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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/326" class=".btn">#326</a>
            </td>
            <td>
                <b>
                    💥 Update, ForceUpdate: allow abortion through error return value (reverts #306)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In #306, we disabled update abortion under the assumption that there aren't many use cases for it.

Since then, we discovered that in two of our applications we were using this functionality (perun-credential-payment and perun-websocket-backend).

Hence, I propose to enable it again.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 11:14:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    Initialize wire encoding explicitly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR proposes to initialize the wire encoding explicitly when needed, instead of setting it via an implicit import. This allows a user to have a better understanding which component uses which encoding and when setting an encoding is not necessary (for example, in case of using a local bus).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 10:02:00 +0000 UTC
    </div>
</div>

