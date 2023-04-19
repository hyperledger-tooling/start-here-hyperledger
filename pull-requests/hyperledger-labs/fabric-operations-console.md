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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    improve doc on audit logs and changing settings
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
Update markdown docs on the how to enable/disable activity tracker logs and added some lines about the basic console setting APIs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 17:11:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    Toggle between to sho/hide archived pending channels
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature

#### Description

There already exists a query parameter that will show archived pending channel tiles under the orderer section of the channels tab but the only way to do this was by putting in the query, `?visibility=all`, into the address bar. 

Added a button on the orderer channels section of the channels page to toggle between showing and hiding the channels:

![Screenshot 2023-04-17 at 17 41 54](https://user-images.githubusercontent.com/44674616/232557100-2147cb8c-8097-4204-a5d4-b767502d71e2.png)
![Screenshot 2023-04-17 at 17 42 05](https://user-images.githubusercontent.com/44674616/232557106-e0ee06ff-696a-467b-9d44-2a1f6acfecec.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 16:59:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    change proxy route cor settings
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
Security improvement, by not accepting all http methods these "proxy" routes will no longer reply with CORS '*'.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 18:04:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/452" class=".btn">#452</a>
            </td>
            <td>
                <b>
                    bump node to 18 in dockerfile & add tag to image
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
- change node 16 to 18 in dockerfile
- adds our git tag to docker image tag


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 16:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    limit length of text in channel tile
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
 - cuts off the orderer names on channel tiles if they are over 42 characters. Full names can still be viewed in the table layout.
 - updates release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 16:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/449" class=".btn">#449</a>
            </td>
            <td>
                <b>
                    fix associate orderer modal regression
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
Fixes the associate identity with orderer modal bug introduced in build -40. The identity drop down was not loading.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 14:39:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    decompress component docs during migration to edit
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
During migration the  component documents need to be decompressed so we can actually edit the docs. New fields get added.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 22:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/447" class=".btn">#447</a>
            </td>
            <td>
                <b>
                    Fix NodeRestApi lib performance
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
More speed/network improvements to minimize requests made by the front end.
- removed the function that calls the get-ALL-component-details api over and over for 1 component
- hooked up the skip cache param in more places
- can now filter multiple node types at once, so you don't have to call get-all-components multiple times when multiple component types are requested
- now absorbs any deployer error if the API asks for `deployment_attrs` on a component, but it was unable to get them, AND cached responses were not allowed (the error is still logged, but the api no longer returns a error response w/503 code)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 19:31:29 +0000 UTC
    </div>
</div>

