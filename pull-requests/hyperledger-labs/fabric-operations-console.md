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

