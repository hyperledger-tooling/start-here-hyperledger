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
                PR <a href="https://github.com/hyperledger/bevel/pull/1940" class=".btn">#1940</a>
            </td>
            <td>
                <b>
                    [fabric] Multiple operations fix after ansible decoupling changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- **Add peer to org:** https://github.com/hyperledger/bevel/pull/1940/commits/aef4ecde31a4d52c80f5e15b7e16b9965541c18e https://github.com/hyperledger/bevel/commit/d928beedde25ebf74bda46776453f643af2b240f
    - `platforms/hyperledger-fabric/configuration/add-peer.yaml`: "create/crypto/peer" role was no more available & replaced
    - `platforms/hyperledger-fabric/charts/catools/templates/configmap.yaml`: store-vault-peer.sh logic fix: If peer status is not "new" or "", then move on to next peer.
    - `platforms/hyperledger-fabric/configuration/roles/create/ca-tools/peer/tasks/main.yaml`:  The export syntax: 
    `export VARIABLE=$VALUE` does not seem to work in the sh used in bevel. Instead two line approach works `VARIABLE=$VALUE; export VARIABLE`. Ref: [Link](https://stackoverflow.com/questions/7328223/unix-export-command)
    
- **Add raft orderer to org:** https://github.com/hyperledger/bevel/pull/1940/commits/97394ca400b89330dba2b8f8de95eb883aee5a51
    - `platforms/hyperledger-fabric/configuration/add-orderer.yaml`: "create/crypto/orderer" role was no more available & replaced
    - `platforms/hyperledger-fabric/configuration/roles/create/ca-tools/orderer/tasks/main.yaml`: Export syntax change
    
- **Removing org:** https://github.com/hyperledger/bevel/pull/1940/commits/e7951c5dd49445cd87d49a2d45e5be0cc1b4d1ac
    - `platforms/hyperledger-fabric/configuration/roles/setup/config_block/sign_and_update/tasks/main.yaml`: Changed condition to also involve the org being deleted to sign the config update block. 
    In a 3 org setup `{supplychain (orderer), carrier, manufacturer}`, removing one of the peer orgs lead to error indicating channel update policy not being met. Making the above change fixes this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 08:35:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1938" class=".btn">#1938</a>
            </td>
            <td>
                <b>
                    [fabric ] update flux to flux v2 setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Update the setup flux role to setup flux-v2
  - Installs flux cli
  - In case the git protocol is ssh, it updates the git host
  - Bootstraps the flux (this creates the flux namespace as well)
- Update reset network of fabric to uninstall flux
  - Added task to delete the flux manifest on reset of network
 

- **The installations are idempotent in itself so don't require checks before installation**
- **Ensure to use ecdsa for ssh key**

 

**Reviewed by**
@sownak 

 

**Linked issue**
#1898

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 07:57:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1936" class=".btn">#1936</a>
            </td>
            <td>
                <b>
                    [fabric] add-organization file fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Fix configuration/add-organization.yaml
- Update charts/invoke_chaincode/templates/invoke_chaincode.yaml

 

**Reviewed by**
@suvajit-sarkar
@jagpreetsinghsasan 

 

**Linked issue**
#1932 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 06:28:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1935" class=".btn">#1935</a>
            </td>
            <td>
                <b>
                    develop merge to flux-v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 06:15:59 +0000 UTC
    </div>
</div>

