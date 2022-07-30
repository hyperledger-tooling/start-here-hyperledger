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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Join Channel Step 2 Next button validation
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

Join Channel Step 2 Next button validation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 15:04:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    use "bulk_add_components" for a systemless append
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
The systemless orderer append flow should use the `bulk_add_components` logic when onboarding and parsing deployer's create-orderer response. This is b/c deployer responds with an array of components and not an object for this route.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 13:50:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Generate Genesis Page Style updates
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

- UI alignment fix


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 15:06:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    fix route and body for appending to systemless os
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
Fixes the route and body to use for the request to append a new orderer node to an os without a system channel.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 14:23:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Fix join orderer text alignment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Modem [nikhil.modem@ibm.com](mailto:nikhil.modem@ibm.com)

#### Type of change

- Bug fix
 
#### Description

- Imported the new joinOSNChanelModal scss to app.scss so that styles are actually applied now.
- Removed the corresponding styles from the channelModal scss file.
- Fixed the alignment of the name of the node and the checkbox to be inline.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 10:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    show success toast msg when orderer joins channel
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

- Improvement (improvement to code, performance, etc)

#### Description
Adds a toast message after a orderer successfully joins the channel using the channel participation apis.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 20:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    fix update channel wizard launch
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
The update channel wizard button was launching the create channel wizard.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 20:29:54 +0000 UTC
    </div>
</div>

