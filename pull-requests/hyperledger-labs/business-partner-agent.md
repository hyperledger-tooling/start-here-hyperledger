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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/506" class=".btn">#506</a>
            </td>
            <td>
                <b>
                    clean install required
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
        Created At 2021-06-22 06:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/504" class=".btn">#504</a>
            </td>
            <td>
                <b>
                    remove liveness probe
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
        Created At 2021-06-21 14:13:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/503" class=".btn">#503</a>
            </td>
            <td>
                <b>
                    frank-bee/issue482
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #482

Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 11:53:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    do not use relative paths
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
        Created At 2021-06-20 19:23:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/501" class=".btn">#501</a>
            </td>
            <td>
                <b>
                    Typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 19:26:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/500" class=".btn">#500</a>
            </td>
            <td>
                <b>
                    fix gitpod docu
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
        Created At 2021-06-18 18:58:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/499" class=".btn">#499</a>
            </td>
            <td>
                <b>
                    Gitpod fully configured
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
        Created At 2021-06-18 15:12:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    configure branches and so on
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
        Created At 2021-06-18 08:57:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    Standardize secondary buttons (text, outlined),
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">frontend</span>
            </td>
            <td>
                Try for only one Primary per section/form.

For BC Gov our [secondary buttons](https://developer.gov.bc.ca/Design-System/Secondary-Button) are supposed to be outlined and text. So if there are no objections, I'd like to put this in place. It is much easier to set on the VUE components themselves than to attempt via SASS overrides or CSS.

We may want to set a specific secondary color for our default theme. The default color is `#424242` which may be too dark?
For our BC theme, we are setting secondary = primary. This shouldn't be a problem until we use secondary for another purpose.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

### Default Look and Feel
![Screen Shot 2021-06-16 at 4 53 08 PM](https://user-images.githubusercontent.com/39388115/122310354-056f6e00-cec5-11eb-8ebc-9fe879e00bf6.png)


### BC Gov Look and Feel
![Screen Shot 2021-06-16 at 4 52 00 PM](https://user-images.githubusercontent.com/39388115/122310118-7a8e7380-cec4-11eb-8114-aa5cbe8b582b.png)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 00:04:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    Tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Will implement #491 

Todo
- [ ] Fix Join
- [ ] Update tags of partners. UI is ready. Backend needs some more work.
- [ ] Init tags by config file similar to schemas
- [ ] Sensible error message if user wants to delete a tag that has been assigned to a partner
- [x] Add tags to partner list

Maybe in another Issue/PR
- [ ] Update name of tags in UI
- [ ] Provide a hard delete that will delete  the tag from all partners as well
- [ ]  Add a tag to an invitation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 15:48:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    remove leftovers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix link to issues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 13:16:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    fix link to issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 09:42:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Adding GLN as another Identifier along side the LEI, DUNS, etc. IDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sebastian Schmittner <sebastian.schmittner@eecc.de>

I have tested this change by building and running a container using https://github.com/hyperledger-labs/business-partner-agent/blob/master/scripts/docker-compose.dev.yml build. The new GLN appears in the public profile just as the other IDs. Generic handling of the id types in the backend makes this change almost trivial. :+1:
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 09:12:28 +0000 UTC
    </div>
</div>

