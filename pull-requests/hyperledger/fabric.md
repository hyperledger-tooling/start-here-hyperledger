---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3530" class=".btn">#3530</a>
            </td>
            <td>
                <b>
                    Insecure TLS Configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Insecure TLS Configuration

Signed-off-by: Bhaskar <ram@hacker.ind.in>

#### Type of change

Insecure TLS configuration is found to be in use. MaxVersion is set to a deprecated SSL/TLS version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-17 07:49:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3526" class=".btn">#3526</a>
            </td>
            <td>
                <b>
                    Update link to Toturial in Style Guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexander Zemtsov <a.zemtsov@gmail.com>

#### Type of change

Documentation update

#### Description

Style Guide describes how to write tutorials. And it has a link to the document which is supposed to be a tutorial example (./private-data/private-data.html). But it is not a tutorial. This commit updates the link. Now it aims to Using Private Data in Fabric tutorial.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 10:48:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3525" class=".btn">#3525</a>
            </td>
            <td>
                <b>
                    Extra checks for invalid args in gateway api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Additional argument validation and consistently use getters to safely traverse proto structures.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 10:10:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3522" class=".btn">#3522</a>
            </td>
            <td>
                <b>
                    Update fabric-chaincode-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Latest version includes purge private data support

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 15:08:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3521" class=".btn">#3521</a>
            </td>
            <td>
                <b>
                    WIP: Orderer v3: Kafka integration tests cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Clean up kafka related infrastructure from integration tests.

#### Additional details

#### Related issues

Epic: #3511 
Issue: #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 14:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3520" class=".btn">#3520</a>
            </td>
            <td>
                <b>
                    WIP: Orderer v3: disable kafka and remove integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: Icba69b9e104377337adefc466745ad5548b4fbab

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

- Disable kafka in server/main by not creating the kafka consenter.

- Remove kafka specific integration tests.

- Move consensus migration tests to raft (solo to raft).

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

Issue: #3513 
Epic: #3511 

#### Release Note
The kafka consensus protocol is no longer supported.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-10 13:31:20 +0000 UTC
    </div>
</div>

