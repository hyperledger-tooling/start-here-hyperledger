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
                PR <a href="https://github.com/hyperledger/bevel/pull/2045" class=".btn">#2045</a>
            </td>
            <td>
                <b>
                    updated ambassador CRDs API version
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2043" class=".btn">#2043</a>
            </td>
            <td>
                <b>
                    [fabric] Multiple chaincode option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add nested task in chaincode operations to allow multiple chaincode installation in one go
- Update docs and sample yamls with chaincode section and channel section changes 

 

**Reviewed by**
@jagpreetsinghsasan 

 

**Linked issue**
#1224 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-12 07:58:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2042" class=".btn">#2042</a>
            </td>
            <td>
                <b>
                    [fabric] One CA tools deployment per organization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**

- Update ca-tools role to combine into a single role.
- Update create/users
- Update catools chart

-  Add priority variable in network.yaml to ensure correct order of creation of cryptographic materials.
   This variable has two possible values:
   *high: indicates that this organization has orderer services, on which other organizations depend and must be executed first.
   *standard: for organizations that only have peers and need orderer certificates already created

The modifications have been tested for the following network.yaml configurations:
* A single mixed type organization
* A mixed type organization and a peer type organization
* An orderer type organization and a peer type organization
The add_peer operation has also been tested.

 

**Reviewed by**
@suvajit-sarkar @jagpreetsinghsasan @sownak 

 

**Linked issue**
#1874 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 13:58:23 +0000 UTC
    </div>
</div>

