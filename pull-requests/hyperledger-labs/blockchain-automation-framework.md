---
layout: default
title: blockchain-automation-framework
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-automation-framework
---

# blockchain-automation-framework <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-automation-framework){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1702" class=".btn">#1702</a>
            </td>
            <td>
                <b>
                    update compatibility table and NPM prerequisite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add NPM prerequisite section
- Update compatibility table 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 06:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1701" class=".btn">#1701</a>
            </td>
            <td>
                <b>
                    [shared] k8s context. allow context name different than cluster name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Fix query to get k8s server name from config file


 

**Reviewed by**
@pppazos 

 

**Linked issue**
#1697

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 16:13:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1700" class=".btn">#1700</a>
            </td>
            <td>
                <b>
                    release 0.10.0 code merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**

https://github.com/hyperledger-labs/blockchain-automation-framework/releases

 

**Reviewed by**
@sownak @jagpreetsinghsasan @alvaropicazo 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 08:41:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1699" class=".btn">#1699</a>
            </td>
            <td>
                <b>
                    [shared] merged code for release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Added main branch commits and resolved conflict  

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 07:46:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1698" class=".btn">#1698</a>
            </td>
            <td>
                <b>
                    [quorum] Vault engine integration for tessera node keys generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: alvaropicazo <alvaro.picazo.haase@accenture.com>

**Changelog**
- Added inegration of vault engine for generating tessera node keys (public and private keys)
- Fixed paths and small bugs on some chart / template files
- Updated roles for checking the key paths due to the changes that the integration of the engine
 

**Reviewed by**
@sownak 
@suvajit-sarkar 

 

**Linked issue**
#1551

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 07:39:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1696" class=".btn">#1696</a>
            </td>
            <td>
                <b>
                    [fabric] Addition of custom user certificate generation and management using fabric-ca
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add

- Addition of new playbook user-certificate.yaml
- New create roles addition
- network-user-certificate sample addition

**Reviewed by**
@arsulegai 

 

**Linked issue**
#1184 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 08:08:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1695" class=".btn">#1695</a>
            </td>
            <td>
                <b>
                    [besu] added clique consensus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: roshan13046 <roshanpk.raut@gmail.com>

**Changelog**
- Added a new role for the clique consensus to generate a clique genesis file
- Updated deploy-network to include the option for generating crypto for the clique network and to deploy nodes for Clique consensus




 

**Reviewed by**
@sownak 
 

**Linked issue**
#510 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 15:13:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1693" class=".btn">#1693</a>
            </td>
            <td>
                <b>
                    [fabric] Operations console
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add helmchart for Fabric operations console
- Rename ca-server to more appropriate generate_cacerts
- Add support for grpcws for peer and orderer charts
- Add support for Operations API (non TLS) for ca, peer and orderer charts
- Add playbook to deploy operations console and generate json files

 
**Linked issue**
Resolves #1610 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 13:44:46 +0000 UTC
    </div>
</div>

