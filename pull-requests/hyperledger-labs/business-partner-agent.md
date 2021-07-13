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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/541" class=".btn">#541</a>
            </td>
            <td>
                <b>
                    Add Endorser support to BPA agents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for the aca-py endorser protocols.

First step - configure each BPA as an Endorser or Author (or neither/both), and allow users to flag partners as an Endorser (for Authors) or Author (for Endorsers) (uses connection "tags").

Work in progress, obviously, but opening a PR for visibility.


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/541"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 21:35:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/540" class=".btn">#540</a>
            </td>
            <td>
                <b>
                    aca-py rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/540"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 08:32:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/539" class=".btn">#539</a>
            </td>
            <td>
                <b>
                    WIP for interested readers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Open points:
- currently there is one RequestedAttributes per Attribute, should be grouped.
- relation between a put PresentProofRequest and the used ProofTemplate has to be persisted.
- further tests.


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/539"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 07:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/538" class=".btn">#538</a>
            </td>
            <td>
                <b>
                    fix endorser related methods after aca-py0.7.0rc0 changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/538"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 15:36:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/536" class=".btn">#536</a>
            </td>
            <td>
                <b>
                    Check if tails is configured
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/536"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 16:20:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/535" class=".btn">#535</a>
            </td>
            <td>
                <b>
                    Use did exchange protocol for all connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Switched all connection related methods to did exchange. Like this it is possible to send the agents public did with the connection request. The opposite BPA now resolves the public profile if it finds a public did in the connection event. To use this functionality I also upgraded aca-py to 0.7-rc1. Also I fixed the partner naming strategy that the following order is used: alias, legal name, label. The alias is the value set by the user. The legal name is resolved from the public profile, the label is the label set by aca-py.

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/535"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 14:48:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/534" class=".btn">#534</a>
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
                

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/534"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 10:40:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/533" class=".btn">#533</a>
            </td>
            <td>
                <b>
                    update milestone docu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/533"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 10:31:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/532" class=".btn">#532</a>
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
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/532"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 09:56:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/531" class=".btn">#531</a>
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
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/531"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 09:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/529" class=".btn">#529</a>
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
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/529"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 09:43:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/528" class=".btn">#528</a>
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
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/528"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 09:41:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    Fix did doc web
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger-labs/business-partner-agent/issues/445

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/527"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 13:03:41 +0000 UTC
    </div>
</div>

