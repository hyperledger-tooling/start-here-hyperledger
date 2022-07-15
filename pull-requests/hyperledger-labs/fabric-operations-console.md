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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    update osn feature to false by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description
<!--- Describe your changes in detail, including motivation. -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 16:00:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    fix orderer detail crash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- Bug fix


#### Description
orderer details crashes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 15:39:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    404 when joining channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- Bug fix

#### Description
when joining channel from an orderer cluster, if there are two nodes (one consenter and one follower) and if the follower happens to be the first one, there is a 404. Try getting the channel config block from consenter.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 21:39:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    Unable to join channel from another orderer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- Bug fix
#### Description
Use correct identity for pulling blocks from orderer


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 21:01:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    fix empty channel list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- Bug fix


#### Description
Channel list is empty when there are channels with empty OrdererAddresses


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 15:58:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    updated release notes
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
- Documentation update

#### Description
release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 20:37:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    improve system channel readme
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

- Documentation update

#### Description
Added a `Console differences with no system channel` section


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 20:28:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    add error msg when there are 0 channels for join
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
Added error message when doing a osn admin join and there are no channels to use.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 19:36:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    remove auto restart when editing specific fields
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
The operator will take care of restarting the component when the admin_certs field is edited. This PR removes the restart from console.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 18:59:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    Various system channel fixes
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
- toggle create wizard steps based on systemless status if the drop down selection changes
- add consenter warning to create wizard summary when 0 consenters are found/selected
- fix importing of  asystemless ordering clusters from json
- hide the unjoin channel button on ordering clusters w/system channel (it won't work)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 18:53:59 +0000 UTC
    </div>
</div>

