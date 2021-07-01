---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/520" class=".btn">#520</a>
            </td>
            <td>
                <b>
                    Fix/null schema attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A schema config is linked to a credential definition and/or a trusted issuer. We had a startup job that deleted the default (read only) schemas on each startup regardless of any linked objects. As there were no db constraints child objects were referencing none existing objects resulting in joins without a result. I removed the read only attributes and added constraints. Schemas are only added if they do not exist already, and it is not possible to delete a schema if it is still referenced somewhere.


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/520"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 11:07:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/519" class=".btn">#519</a>
            </td>
            <td>
                <b>
                    Update milestones.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/519"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 08:00:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/516" class=".btn">#516</a>
            </td>
            <td>
                <b>
                    auto generate milestone  document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/516"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 06:57:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/513" class=".btn">#513</a>
            </td>
            <td>
                <b>
                    fixEnvVars
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/513"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 12:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/512" class=".btn">#512</a>
            </td>
            <td>
                <b>
                    Tune gitpod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/512"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 08:24:53 +0000 UTC
    </div>
</div>

