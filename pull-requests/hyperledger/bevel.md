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
                PR <a href="https://github.com/hyperledger/bevel/pull/2014" class=".btn">#2014</a>
            </td>
            <td>
                <b>
                    mixed-org fixes base code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Fix platforms/hyperledger-fabric/configuration/roles/helm_component/templates/ca-mixed.tpl. The secretRef field has been removed, because it causes the error shown in the following image.
<img width="678" alt="https-error in ca" src="https://user-images.githubusercontent.com/83813093/185910473-413b8121-671a-4b23-9917-b57826105261.png">

- Update platforms/hyperledger-fabric/configuration/roles/create/configtx/templates/configtxOrderer_default.tpl. The value of the BlockValidation field has been modified because it produced an error in the approvechaincode job.
 


 

**Reviewed by**
@suvajit-sarkar @jagpreetsinghsasan 

 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 11:31:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2013" class=".btn">#2013</a>
            </td>
            <td>
                <b>
                    [docs] inclusive language changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add inclusive language changes

 

**Linked issue**
#1948 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 10:10:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2012" class=".btn">#2012</a>
            </td>
            <td>
                <b>
                    mixed-org fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 09:41:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2011" class=".btn">#2011</a>
            </td>
            <td>
                <b>
                    Mixed org fixes and schema updated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Fix mixed org vault policy
- Update default policies

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 11:48:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2010" class=".btn">#2010</a>
            </td>
            <td>
                <b>
                    [fabric] feature: orderer & peer in same org.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add Fabric platforms code for mixed org feature to support orderer and peer in same org.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 16:14:51 +0000 UTC
    </div>
</div>

