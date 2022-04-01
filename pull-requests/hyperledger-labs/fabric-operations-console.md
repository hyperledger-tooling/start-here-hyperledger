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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    fix channel nodes
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

Clicking on the info for channel (under orderer drill down) shows nodes where the channel got removed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 20:03:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    update release notes
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
- added release notes
- (back) sync translation file


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 20:23:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/174" class=".btn">#174</a>
            </td>
            <td>
                <b>
                    validate CA enrollment host during create peer/os
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

- Improvement (safety)

#### Description
- will reject apis to create a peer or orderer using an unknown CA hostname. 
  - failures generate: `The parameter 'crypto.enrollment.ca.host' was not found in the list of known hostnames. Import the CA using this hostname or use a hostname that is already known.`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 19:45:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    Tweak pass submit button
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
- The reset password modal was allowing a user to click submit even if there were password strength errors.  The password was still being rejected, but disabling the submit button is the desired behavior.
- Adds release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 18:32:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    adds a feature flag for osnadmin
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

- Improvement / Bug Fix


#### Description
- added feature flag `osnadmin_feats_enabled` to enable channel participation features which use the fabric osnadmin endpoint
- fixed system channel detection in orderer panel
- add description for all feature flags!


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:13:41 +0000 UTC
    </div>
</div>

