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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/489" class=".btn">#489</a>
            </td>
            <td>
                <b>
                    use absolute paths for logout/login links
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
- changes the logout/login links from a url + path, to just an absolute path. more robust this way


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 19:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    fix the deployer sync timing
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
- fixes the component data sync with deployer, now waits for the deployer changes to write to the db before rebuilding the url safelist


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 19:46:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/487" class=".btn">#487</a>
            </td>
            <td>
                <b>
                    Fix button size
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
Fixes the width of the button container to match the side panel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 20:07:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    fixes passport setup during oauth switching
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
- fixes the passport strategy setup after switching to oauth, it needed a delay to wait for the effect
- fixes oauth setup when console has multiple instances running


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 14:13:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    update passport strats for oauth on a auth change
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

- need to update passport strategies when the auth scheme is changed



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 19:54:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    fix orderer node options in consenter input
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
- when editing a channel, the add/remove consenter part was not showing all the orderer nodes as options


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 19:31:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/483" class=".btn">#483</a>
            </td>
            <td>
                <b>
                    fix component dropdown option bug
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
- fixes the bug where it doesn't render the selected option in a fabric component dropdown input 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 18:03:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    remove sensitive fields from a CA response
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
 - removes the sensitive field `datasource` from component API responses (applies to CA components)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 19:34:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/481" class=".btn">#481</a>
            </td>
            <td>
                <b>
                    add comments & check orderer ver around CP feat
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
added comments and check orderer version to show/hide channel participation content


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 19:26:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    fix the oauth login revert logic
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
- fixes the oauth login timer, it will now clear after the first successful login by a manager

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 17:16:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    Fix input option bug and table bug
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
- fixes dropdown menus not showing the selected value
- fixes mutli select table errors which were creating a blank page


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 17:15:17 +0000 UTC
    </div>
</div>

