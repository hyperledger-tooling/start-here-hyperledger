---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Remove redundant `admin` global variable from NetEmissionsTokenNetwork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The NetEmissionsTokensNetwork contract inherits the AccessControl library, which uses the role `DEFAULT_ADMIN_ROLE`. The modifier `onlyAdmin()` uses this and `DEFAULT_ADMIN_ROLE` is used elsewhere in the contract. This commit removes the redundant `admin` variable which is never used after initializing the contract to save on storage/deployment cost.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 00:09:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    Mentorship postgres
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Created api server. Need to add CI api server test now
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 15:18:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/568" class=".btn">#568</a>
            </td>
            <td>
                <b>
                    Added documentation for Bevel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 16:30:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    get code up to date
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 15:32:42 +0000 UTC
    </div>
</div>

