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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    retry for smart contract error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)


#### Description
<!--- Describe your changes in detail, including motivation. -->

retry for smart contract error


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 13:20:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/500" class=".btn">#500</a>
            </td>
            <td>
                <b>
                    if comp is migrated choose correct route when getting the component status
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
- if a component was migrated from an iks cluster, the component status requests were using the new style of "api url" instead of the legacy style. the new style will not work on a legacy migrated component. the result is the status icon of a component in that state never goes green.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 19:50:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/499" class=".btn">#499</a>
            </td>
            <td>
                <b>
                    if in read-only disable actions in the access tab
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
If the console is in read only mode, the access tab will no longer let you change the auth scheme, add/remove users, or add/remove api keys


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 14:09:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    update api doc link
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
- Update api key doc link on the migration info page


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 19:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)


#### Description
- lint fixes, set some data types, remove unused lib


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 19:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    clear session cache on logout/login
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
- when running multiple console instances, it was possible to have a stale session cache that would cause logout and login failures
- deletes browser session when a user role is changed (forcing the user to login again)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 18:33:54 +0000 UTC
    </div>
</div>

