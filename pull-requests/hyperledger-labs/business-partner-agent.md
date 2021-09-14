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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    formatting for nev header image with max dimensions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With custom navigation header image provided. 

![Screenshot_20210913_164016](https://user-images.githubusercontent.com/5376854/133170841-3b7ddb94-5602-4efe-b7ee-7b2be9fe2db1.png)

With default flag set. 

![Screenshot_20210913_164832](https://user-images.githubusercontent.com/5376854/133171464-b6123d32-256e-42e2-9b20-0a780ce54e10.png)

Some formatting/prettier automatic changes. 


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/615"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 23:57:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/614" class=".btn">#614</a>
            </td>
            <td>
                <b>
                    Show Partner and Cred. Def on Credential Data Form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Put common logic for select lists (Partner and Cred Def) into $store.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/614"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 23:11:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    Label updates (Issue Credential -> Credential Definition).
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add some sorting on the issue credential screen, allow issue credential without all fields entered.
Previously, ALL fields were required which means you need data for every field which may not be true.
Adding sort of schema attributes when we fetch the BPA Schema model, allows for consistent rendering of the attribute order (alphabetical)

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/613"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 15:45:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    Cred Def - make Tag required (help with our display of cred defs).
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">frontend</span>
            </td>
            <td>
                Add some cleanup/reset to Cred Def and Trusted issuer components when closing Schema form.

The issue was strictly for our frontend. When we have a list of credential definitions to choose from (for issuing), if there was no Tag set, then the display is like `Schema Name (version) - `, and it should be `Schema Name (version) - Tag`.

I also did a check and returned a nicer error if you attempt to save the same tag (for a given schema) twice.

Did a little clean up on Credential Definitions and Trusted Issuers components, so when you close the Manage Schema form, those components will reset (currently would leave half-edited fields in place with whatever text hadn't been saved).

**NOTE:** I've put in a very temporary "hack" related to issue 611, just adding the referent id to the matching credential list labels so you can select from all the matches.  This does NOT actually fix the issue, I think it's a bigger refactoring/fix required.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/612"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 17:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    Axios Error Message Fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add in an axios error handler method that parses out the user friendly message that the backend has set.
The delete was ok, just that the useful message that we send from the backend is never surfaced to the frontend.


Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

fixes #609 

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/610"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 22:07:37 +0000 UTC
    </div>
</div>

