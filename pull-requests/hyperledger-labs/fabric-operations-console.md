---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/546" class=".btn">#546</a>
            </td>
            <td>
                <b>
                    add buttons to delete all components or the wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
Added a new delete-all-components button and a delete-wallet button to the settings page. they are hidden by default to prevent mishaps. they can be shown by adding `?debug=true` to the url when on the `/settings` page, like `/settings?debug=true`, 
- the delete-all-components button only appears to users w/ a `manager` role
- the delete-wallet button only appears to users w/ a `writer` role


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 17:31:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/545" class=".btn">#545</a>
            </td>
            <td>
                <b>
                    added release notes on missing tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
add to release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 13:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/544" class=".btn">#544</a>
            </td>
            <td>
                <b>
                    Fix drilldown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
From the channels page, and the channel details tab, when clicking an orderer node on the channel, the app will now correctly redirect the user to the drill down of that orderer.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 12:57:45 +0000 UTC
    </div>
</div>

