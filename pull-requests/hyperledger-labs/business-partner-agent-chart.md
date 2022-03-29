---
layout: default
title: business-partner-agent-chart
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent-chart
---

# business-partner-agent-chart <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent-chart){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Replace public DID when running init acapy container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tim Schlagenhaufer <tim.schlagenhaufer@bosch.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 14:37:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    compatibility fixes for 0.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                restores pre 0.11.0 behavior. meaning aca-py creates an own db called 'mywallet' on the server and the bpa uses the default db of the postgres user.

by setting:

_acapy.postgresql.database=""_
_bpa.config.pg.schema="bpa"_

both aca-py and the bpa will share the same database. this is needed in usecases where both instances should share a pre existing database.


Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 16:57:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Feature: inject existing database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It is now possible to inject a database name to aca-py. Like this it is possible to share a preexisting db between aca-py and bpa.

Warning this is not backwards compatible., If you upgrade to 0.11 your data will be lost. I will fix this with a later release, probably 0.11.1 If you do not want to loose data wait with the upgrade.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 16:12:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    support tls on all database connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - support TLS on the bpa connection string
- allow to set a database name on the bpa connection string
- allow to set a port on the bpa connection string
- default wallet type is now askar


Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 11:43:07 +0000 UTC
    </div>
</div>

