---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2047" class=".btn">#2047</a>
            </td>
            <td>
                <b>
                    [fabric] Fix multiple orderers - Develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add the following fields in the network.yaml:
   *`network.consensus` 
   *`network.channels[*].orderer.name` (is a list)
   *`network.organizations[*].orderer_org` (This field should only be added in peer organizations. Indicate from which 
     organization takes the orderers)

- Update create/configtx and ca-tools roles to perform deployments with multiple orderer organizations
- Update documentation and network-schema.json

 

**Reviewed by**
@suvajit-sarkar @jagpreetsinghsasan @sownak 

 

**Linked issue**
#2038 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-24 10:04:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2046" class=".btn">#2046</a>
            </td>
            <td>
                <b>
                    [fabric] Fix getting orderer certs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Fix issues related to helmrelease deletion
- Issues for copying orderer certs locally
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 14:56:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2045" class=".btn">#2045</a>
            </td>
            <td>
                <b>
                    [shared]: Updated ambassador CRDs API version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: adityajoshi12 <adityaprakashjoshi1@gmail.com>

**Changelog**

- Updated ambassador proxy CRDs from `v1beta1` to `v1`

 

**Reviewed by**

 

**Linked issue**
#2044

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 06:25:09 +0000 UTC
    </div>
</div>

