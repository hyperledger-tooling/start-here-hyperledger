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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    Handle valid invitation type (didcomm)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `https://didcomm.org/connections/1.0/invitation` is a valid invitation type, so let's handle the current case and this value.
IBM had generated a connection invitation with the didcomm format and we couldn't connect, so we needed to update our invitation parser class.

We can generate invitations with the same `@type` by starting the agent with `--emit-new-didcomm-prefix` option.

fixes #620

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/623"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 18:04:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    Import Error Message - show backend message.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                400 was being handled in the frontend to always mean one error (Schema exists), but that hid other types of errors so message was misleading.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/621"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 00:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    ternary instead of pipe
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Sy <jasyrotuck@gmail.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/619"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 22:41:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    Expert Mode - Issue Credential from CSV
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow user to copy/paste, type or upload a CSV file and load the credential data (first row only).
Further enhancement to the Expert Mode Load Credential data.
As noted by @etschelp, this is just a basic first step and we should further enhance for multi-credential load etc.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/618"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 22:38:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Expert Mode - Issue Credential from JSON
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">frontend</span>
            </td>
            <td>
                Allow user to copy/paste, type or upload a JSON file and load the credential data.
Fix bug from Credential Management when you cancel Issue Credential and re-open form, the cred def wasn't loading.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

![Screen Shot 2021-09-14 at 3 36 50 PM](https://user-images.githubusercontent.com/39388115/133343781-c1aaa943-72a0-4002-972f-d950f5562436.png)


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/617"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 22:47:34 +0000 UTC
    </div>
</div>

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

