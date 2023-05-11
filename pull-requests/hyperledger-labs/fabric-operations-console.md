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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    fix the library name for the self signed tls renew
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
The auto renewal of the self signed tls cert code had some copy paste error in it, preventing it from working.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 16:13:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    fixes the toggle pending channel tiles button
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
Fixes the toggle pending channel tile button.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 20:43:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/469" class=".btn">#469</a>
            </td>
            <td>
                <b>
                    fix anchor peer error when joining peer to channel
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
When joining a peer to a channel (and the anchor peer toggle was enabled) it was failing to add a peer as an anchor peer to the channel.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 19:59:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    rebuild safelist during comp edits/fabric upgrades
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
- After upgrading a fabric node we need to rebuild the internal url safe list
- after editing a component, we should rebuild the internal url  safe list


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 18:29:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/467" class=".btn">#467</a>
            </td>
            <td>
                <b>
                    fix adding and removing of consortium members
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
This fixes adding and removing consortium members to the system channel of an ordering service.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 17:35:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    fix a few action buttons not rendering in modal + removed need for debug route
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
- Fixes a few of the action buttons in the Orderer modal not rendering (and also just not working at all!), preventing things like updating capabilities, and toggling maintenance mode.
- also we will now always show the `Open Channel Config` link in an orderer drill down. there's no longer a need to type out the `/debug/` route to activate this tool/link.
- also fixes the block parameter sliders (found in the orderer advanced configuration modal) not reflecting the current settings (they were always showing the default values console sets for an ordering service instead of the current value)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 19:59:18 +0000 UTC
    </div>
</div>

