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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/233" class=".btn">#233</a>
            </td>
            <td>
                <b>
                    set default value for osnadmin_feats_enabled as true
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

- New feature

#### Description
set default value for `osnadmin_feats_enabled` as `true`, was `false`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 13:37:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    channel participation apis - join orderer  via drill down
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature - adds new join osn to channel flows

#### Description
- Adds join orderer to channel via cluster drill down (this is a new modal)
   1. general join flow - from OS page -> can select join-channel button, then select existing OS to get config block, select channel name, select osn(s) to join
   2.  specific join flow - from OS page -> can select the channel, then select osn(s) to join

- changes create orderer flow - user must select if they want to use a system channel or not when creating a orderer 
   - (only applies if `osnadmin_feats_enabled` is enabled)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 20:52:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/231" class=".btn">#231</a>
            </td>
            <td>
                <b>
                    update license headers in all files
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
Looks like a big pr, but its just a license update we had to do.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 21:24:35 +0000 UTC
    </div>
</div>

