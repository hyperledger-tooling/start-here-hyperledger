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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    Dashboard Update - more cards, get counts from backend.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

Refactor out a UX component for the cards, do some styling on different window sizes to keep text readable.
Get all counts (totals and "new" items) from backend for the dashboard. This will allow future enhancements to get counts for different periods, such as new items since yesterday (default) or last week or last month.



<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/577"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 02:34:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/576" class=".btn">#576</a>
            </td>
            <td>
                <b>
                    bugfix: proof template view/create pages not loading on refresh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When refreshing the proof template view & create pages manually, some fields were not being loaded due to the state/store variables being loaded asynchronously.  I corrected the code to accurately hook into the state lifecycle via the ```computed``` hook and provided a backed ```REST``` endpoint for getting a ```proof-template``` via an ID to make the endpoint fully CRUD.  

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/576"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 19:26:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/575" class=".btn">#575</a>
            </td>
            <td>
                <b>
                    Refactor 1 of Credential Management screen layout, prep for refactor 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is just an initial PR to remove the duplicated Schema/Cred Def management from Credential Management.

This was confusing users to the real purpose of the screen which is to Issue Credentials.
So, renaming titles to Issue Credentials, remove the schema table, and move the Issuance action of the screen to the top of the screen.

There will be a subsequent PR to finish of the refactor (rename VUE files and paths, add in more resource based labels/naming). Holding off for now as there is another big PR that will hit the same code; just making it easier for that merge.


Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/575"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 18:29:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/574" class=".btn">#574</a>
            </td>
            <td>
                <b>
                    Issue V2 Indy Credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently work in progress.

Issue and receive indy credentials via v2 api.

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/574"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 13:57:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/573" class=".btn">#573</a>
            </td>
            <td>
                <b>
                    these are only used by multi-sort, so remove those too.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                missed commit 

Signed-off-by: Jason Sy <jasyrotuck@gmail.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/573"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 20:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/572" class=".btn">#572</a>
            </td>
            <td>
                <b>
                    Update .gitignore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                errors merging in with bcgov.

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/572"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 19:08:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Ux/remove multi sort
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is confusing users, remove for now. 

It's easy to add later. 

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/571"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 19:04:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Ux/move did off dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The DID being the first thing users see confuses them as they don't know what it means. 

Moved it to the settings page for us.

New dashboard: 
![image](https://user-images.githubusercontent.com/5376854/129115131-178f63f6-c92a-4cc9-a2ff-a8acd68e70e0.png)

New settings page:
![image](https://user-images.githubusercontent.com/5376854/129115190-8ba6986f-7696-478d-8a04-494cc0e0dbd3.png)


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/570"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 23:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    Virtual Partner Name/Alias
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently when we add a new Partner the Partners name is always pre filled with the partners legal name (if set). This can cause confusion because like this the partners alias is always set as well. For example:

1. agent 1 adds a new partner with legal name foo
2. partner changes legal name to bar
3. agent 1 reloads partner, legal name changes to bar, display name stays foo

This is totally correct as this adheres to our partner name strategy, but it is very confusing to the user. So instead of using two way binding to set the alias I only set the placeholder like this,

<img width="721" alt="Screen Shot 2021-08-11 at 16 34 47" src="https://user-images.githubusercontent.com/13498217/129050143-c6d76c08-8f05-45dd-9c2c-3ad1452c5c61.png">

then the user can set a real alias if needed.

<img width="696" alt="Screen Shot 2021-08-11 at 16 34 56" src="https://user-images.githubusercontent.com/13498217/129050188-46935d9c-7408-4c0a-945d-2faf40de94cf.png">


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/569"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 14:36:08 +0000 UTC
    </div>
</div>

