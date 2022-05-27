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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/218" class=".btn">#218</a>
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
Added release notes for 1.0.3-11


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 17:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    add a restart progress bar when changing settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvements to settings panel

#### Description
- added progress bar to indicate the server restart is still in progress when saving new settings
- allow user to select a log level without selecting the log-to-file option
- sync the tooltip min/max text for the inactivity time on the settings panel to match the values in the validator


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 21:43:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    add option to create system channel-less orderers
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
- Added ability to create orderers w/o a system channel. it is selectable via a checkbox. requires deployer to be present and the feature flag `osnadmin_feats_enabled` to be true.
   - note if this is selected channel participation APIs must be used to create application channels


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 20:37:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    allow edit-settings api to use default password
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
For automation purposes it would be nice if the console settings can be edited using the default password. This PR does that.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 18:31:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    add support for stitch to decode utf8 characters - input
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

- Improvement 

#### Description
Add support for decoding utf8 characters in fabric transaction  * inputs *.  Similar to https://github.com/hyperledger-labs/fabric-operations-console/pull/210

fixes https://github.com/hyperledger-labs/fabric-operations-console/issues/198


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 13:15:23 +0000 UTC
    </div>
</div>

