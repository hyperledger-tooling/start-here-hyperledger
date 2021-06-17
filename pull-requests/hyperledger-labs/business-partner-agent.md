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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/487" class=".btn">#487</a>
            </td>
            <td>
                <b>
                    fix echo
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
        Created At 2021-06-15 10:32:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    fix explanation
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
        Created At 2021-06-15 10:22:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    add terminal
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
        Created At 2021-06-15 10:10:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    wait a little for DB
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
        Created At 2021-06-15 09:26:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/483" class=".btn">#483</a>
            </td>
            <td>
                <b>
                    fix gitpod did reg
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
        Created At 2021-06-15 09:01:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/481" class=".btn">#481</a>
            </td>
            <td>
                <b>
                    fix startup
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
        Created At 2021-06-14 23:46:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    Feature/proof request rejection problem report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">frontend</span>
            </td>
            <td>
                ThreadId wasn't being saved properly by the initiator, the event handler by the VERIFIER wasn't working. 
If there is a problemReport, show the user an icon with the message as a tooltip.

Also added debug port for second BPA in local-network docker-compose.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 22:53:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    fix .env
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
        Created At 2021-06-14 22:25:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    add startup tasks
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
        Created At 2021-06-14 22:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/477" class=".btn">#477</a>
            </td>
            <td>
                <b>
                    Customized UX
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use configuration values to update the look and feel of the application.

Add in BC Gov branding (could be used by others), adjusts the UX to have a business logo on Top Right Hand side, can override the style of Title (add the BPA Name before page/screen title). Change the layout of the navigation (put logout at bottom, put Settings at bottom, hide About). Can override the favicon.

Colors are configurable and will set the vuetify light theme.

Will have a [related PR](https://github.com/hyperledger-labs/business-partner-agent-chart/pull/15) for the helm charts to load ux like we do schemas for each deployment.

I have removed any changes to text via configuration. We had discussed that custom text changes should be handled when we do internationalization.

Also, note that the `main.js` the configuration is loaded synchronously before loading `App.vue`, we need the configuration data to be fully loaded first.

### BCGov Branded  (loaded to Openshift via Helm charts)
![Screen Shot 2021-06-14 at 2 14 28 PM](https://user-images.githubusercontent.com/39388115/121961004-b2a68280-cd1b-11eb-8622-a5e83396a9d5.png)

### Default branding (loaded to Openshift via Helm charts)
![Screen Shot 2021-06-14 at 2 14 41 PM](https://user-images.githubusercontent.com/39388115/121961115-d964b900-cd1b-11eb-821d-1933a5943600.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 21:22:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/475" class=".btn">#475</a>
            </td>
            <td>
                <b>
                    Add release drafter
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
        Created At 2021-06-14 08:38:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/474" class=".btn">#474</a>
            </td>
            <td>
                <b>
                    Add release drafter
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
        Created At 2021-06-14 06:51:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/473" class=".btn">#473</a>
            </td>
            <td>
                <b>
                    Add basic gitpod config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Bernhardt <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 06:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    Feature/simple rules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://hackmd.io/2m16i56sTtmYi9tVuklVVw?view
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 15:28:15 +0000 UTC
    </div>
</div>

