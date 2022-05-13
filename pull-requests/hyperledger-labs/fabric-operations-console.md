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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    allow zero length admin array for org
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Historically Fabric required admin certs for an organization... somewhere around 1.4 when Node OU was introduced, admin certs in the orgs were no longer required. Adjusting the code to accommodate that

https://github.com/hyperledger-labs/fabric-operations-console/issues/203


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 22:55:16 +0000 UTC
    </div>
</div>

