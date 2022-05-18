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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    add support for stitch to decode utf8 characters
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
Add support for decoding utf8 characters in fabric transaction outputs.  Specifically the read/write set from a transaction will now display correctly * **if** * utf8 characters were used.

fixes https://github.com/hyperledger-labs/fabric-operations-console/issues/198


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 17:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    Added more logging around login for Saas and Software scenarios
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ketul Shah <shah.ketul@ibm.com>

#### Type of change
- Test update

#### Description
Added more logging around login for Saas and Software scenarios for pipeline troubleshooting
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 15:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    Update safelist comp update
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
Same fix as https://github.com/hyperledger-labs/fabric-operations-console/pull/205 but this PR fixes the update component api.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 14:47:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    add query param to login link from logout panel
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

After a logout there is a log back in link. Sometimes this link fails to send the user to the login page. It spins. This pr attempts to fix that by making the link a un-cachable link.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 15:14:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    Added check for IBM Cloud login - w3id login
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ketul Shah <shah.ketul@ibm.com>

#### Type of change
- Test update

#### Description
Added check for IBM Cloud login - w3id login
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 15:00:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    rebuild safelist when validating create-peer api
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
When creating a component the hostname safelist will be recalculated before API validation. 

This will fix the problem when a user creates a peer and the hostname of the CA for the peer's enrollment is not known to all instances of the console.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 18:09:29 +0000 UTC
    </div>
</div>

