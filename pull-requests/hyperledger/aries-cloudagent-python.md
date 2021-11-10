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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1484" class=".btn">#1484</a>
            </td>
            <td>
                <b>
                    Clarify instructions in Acme Controller Workshop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1477 

Signed-off-by: Elias Strehle <elias@circulartree.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 09:38:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1483" class=".btn">#1483</a>
            </td>
            <td>
                <b>
                    fix: create static doc use empty endpoint if None
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This enables us to use the undelivered queue with static connections by not specifying the endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 19:58:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1476" class=".btn">#1476</a>
            </td>
            <td>
                <b>
                    fix: use named tuple instead of dataclass in mediation invite store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dataclass wasn't added until python 3.7 and we're on 3.6. Not sure how this wasn't failing tests :thinking: we must have a backport package installed in the base image or similar but at any rate, I'm hopeful this will resolve issues @swcurran raised in #1473 for this module's doc generation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 20:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1475" class=".btn">#1475</a>
            </td>
            <td>
                <b>
                    Update credential and proof mappings to allow negative encoded values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

See issue https://github.com/hyperledger/aries-cloudagent-python/issues/1462

@jsyro
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 18:13:53 +0000 UTC
    </div>
</div>

