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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    fix tails server for test net
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 09:09:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    allow tails server configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-05 08:58:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    remove uniresolver url and did prefix from bpa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Leftover work from the aca-py 0.7 migration. I did not want to change the chart for this, but micronaut has a special behavior that translates environment variables to system properties. So settings an environment variable like BPA_DID_PREFIX gets translated to/or behaves the same as -Dbpa.did.prefix Therefore I had to remove the uniresolver and prefix settings. Both are needed again in the future, but on the aca-py level. As the details are still somewhat in the working it is better to remove both properties anyway.

Signed-off-by: Philipp Etschel <philipp@etschel.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 12:49:56 +0000 UTC
    </div>
</div>

