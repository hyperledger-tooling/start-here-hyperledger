---
layout: default
title: fabric-config
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-config
---

# fabric-config <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-config){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-config/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    remove kafka and fix tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix
- Test update


#### Description

I removed Kafka as it is not supported as a consensus type, by mark as a deprecated Kafka's fields and functions. I also blocked the option to add configuration to an orderer with Kafka as a consensus type.
I fixed tests that had a bug and tests that need to fit to our new requirements.

#### Related issues

 issue #3513 in Fabric

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 13:12:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-config/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Added support to fabric smartbft protos.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: arkadi.piven@ibm.com

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix


#### Description

Add support to fabric smartbft protos parsing.

#### Related issues
Add support for "Orderers" and BFT "Options" parsing from binary to json. #57 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 11:19:37 +0000 UTC
    </div>
</div>

