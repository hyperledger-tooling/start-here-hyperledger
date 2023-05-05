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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    fix safe URL vaildation for legacy field "caport"
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
The safe-url validation code was not working correctly if the legacy field `caport` was used. This only effects the `/v2/` APIs.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 21:04:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    fixes orderer details panel not loading b/c bad id
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
Fixed the id error on the orderer details page.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 16:49:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/463" class=".btn">#463</a>
            </td>
            <td>
                <b>
                    sync component data after fabric upgrade
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
When upgrading fabric, new features might become available. we need to sync the component data after a fabric upgrade.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 20:23:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    fix doc links for different console builds
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
- Fix links to console documentation that were dependent on what type of console build it was.
- removed some dead code


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 20:14:05 +0000 UTC
    </div>
</div>

