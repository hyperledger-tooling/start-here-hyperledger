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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    orderer associate admin identity label update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: selvaprakash92 <selvaprakash92@gmail.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
<!--- Describe your changes in detail, including motivation. -->

orderer associate admin identity label update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 14:28:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    always add the selected cluster nodes for joinflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

- always add the drill down cluster nodes to the join-orderer-to-channel flow, b/c these nodes should always be valid options.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 19:55:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    fix the orderer/cluster select options in join wiz
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
- the node options listed during a  systemless-channel orderer join were not as lax as they should be. this pr allows selecting nodes from any cluster that has the same MSP. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 19:48:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    list each cluster once in pending channel tile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
A pending channel tile was listing the cluster names once per node, which is redundant. This only lists the cluster names once.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 13:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    configblock changes in console
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- adds the ability to archive console config blocks, which will hide them from the channels tab
  - this is done with a new field. `visibility`
  - existing config blocks that do not have a `visibility` field will default to `inbox` which means they are visible
- the get-all-config-blocks api can now specify a `visibility` query param of `all`, `inbox`, or `archive`
  -  it defaults to `inbox`
- once an orderer joins a pending channel we will now archive a config block instead of deleting it
- during the join orderer flow if we are unable to pull a config block from an orderer we will direct the user to the channels tab if one of the blocks looks like a possible match. the user can join the orderer by selecting the archived config block tile and then following the normal join process.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 19:09:35 +0000 UTC
    </div>
</div>

