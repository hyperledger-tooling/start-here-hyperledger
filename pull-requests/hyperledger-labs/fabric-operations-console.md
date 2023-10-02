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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/534" class=".btn">#534</a>
            </td>
            <td>
                <b>
                    Updating ginkgo to version v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description
Upgrading ginkgo framework to V2 version

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 18:10:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/533" class=".btn">#533</a>
            </td>
            <td>
                <b>
                    Mustgather Inactive - setbackoff added in startGather
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
<!--- Describe your changes in detail, including motivation. -->
This pull request involves the addition of the setbackoff in the startgather method for Mustgather component to ensure that the mustgather button does not time out , if the action is not started  

#### Reviewer
@dshuffma-ibm 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 07:42:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/532" class=".btn">#532</a>
            </td>
            <td>
                <b>
                    fix error msg when changing channel capabilities
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
- Prevents the error when trying to change channel capabilities from v1.4 to v2, when peers/orderers have a fabric version that starts with `v`, like `v2.5.4` instead of `2.5.4`
- formats the fabric version in some error messages to a standard
- Prevents the error when trying to change channel capabilities from v1.4 to v2, when peers/orderers do not have a known fabric version


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 17:32:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/531" class=".btn">#531</a>
            </td>
            <td>
                <b>
                    edit csp headers to remove medallia sources
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
Removed csp header sources that we no longer use.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 13:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/530" class=".btn">#530</a>
            </td>
            <td>
                <b>
                    Openapi file cleanup
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
- lots of openapi edits/cleanup (api and field descriptions & summary improvements)
  - there are no actual api spec changes
- adds a couple more openapi validation steps to our automation (github actions)
- updates js-yaml to v4, and uses the new `load` method instead of `safeLoad`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 17:55:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/529" class=".btn">#529</a>
            </td>
            <td>
                <b>
                    bump release note
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
update release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 14:22:28 +0000 UTC
    </div>
</div>

