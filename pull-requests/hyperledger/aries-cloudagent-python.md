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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1581" class=".btn">#1581</a>
            </td>
            <td>
                <b>
                    OOB connection_reuse webhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 23:53:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1576" class=".btn">#1576</a>
            </td>
            <td>
                <b>
                    Add fix for #1575 to allow OPTIONS method to work with x-api-key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow OPTIONS method used by browsers to implement CORS checks to be serviced without requiring the x-api-key to be present in the request.  Also added a test case for same.

Signed-off-by: john court <jcourt@anonyome.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 07:54:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    Allow public invites for alice/faber demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses https://github.com/hyperledger/aries-cloudagent-python/issues/1571

Note - added a `--reuse-connections` parameter to faber - this will trigger faber to use a public did in the didexchange connection (and alice will always "reuse connection" if possible) and the connection indeed gets reused, however right now there are no webhooks for the "reuse" messages so the alice/faber controllers are getting hung ...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 23:59:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    Updates for final Release 0.7.3
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
        Created At 2021-12-21 22:54:45 +0000 UTC
    </div>
</div>

