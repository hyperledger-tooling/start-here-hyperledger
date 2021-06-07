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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1505" class=".btn">#1505</a>
            </td>
            <td>
                <b>
                    [besu] Adding new validator node to existing network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Signed-off-by: alvaropicazo <alvaro.picazo.haase@accenture.com>

**Changelog**
- Added validator_node role for creating new enode, certs and doing the voting process by existing validator nodes
- Fixed create/ambassador nested_main condition
- Updated docs for new role

 

**Reviewed by**
@jagpreetsinghsasan 
@suvajit-sarkar

 

**Linked issue**
#1494 

**Screenshots**

![Capture1](https://user-images.githubusercontent.com/76157062/121003315-b1aaa980-c78d-11eb-923c-586ff8aff580.PNG)

Helm releases files are updated correctly with all the static nodes
![Capture2](https://user-images.githubusercontent.com/76157062/121003380-c1c28900-c78d-11eb-8e28-9a7bca041af0.PNG)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 10:44:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1504" class=".btn">#1504</a>
            </td>
            <td>
                <b>
                    [corda-ent] remove ambassador license
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- remove ambassador license
- Update jenkinsfile for corda-ent


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 10:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1503" class=".btn">#1503</a>
            </td>
            <td>
                <b>
                    [shared] Changed default namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: angelaalagbe <angela.alagbe@accenture.com>

**Changelog**
- Updated default namespace to component_ns

 

**Reviewed by**
@suvajit-sarkar @sownak 

 

**Linked issue**
#1491 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 11:32:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1502" class=".btn">#1502</a>
            </td>
            <td>
                <b>
                    [docs] Using GitHub API icons for roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Removed roadmap icons from _static folder
- Update roadmap icons to use github icons url 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 08:14:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1501" class=".btn">#1501</a>
            </td>
            <td>
                <b>
                    [corda-ent] certificates for ambassador
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- in cenm (idman, network, notaries) trust tls root ca in cenm organization
- in nodes (include idman and network crts in corda truststore)
- k8s tls secrets created in the org namespace


**Reviewed by**
@sownak 
@suvajit-sarkar 

 

**Linked issue**
#996 #1462 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 13:37:12 +0000 UTC
    </div>
</div>

