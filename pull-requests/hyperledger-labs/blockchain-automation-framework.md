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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1745" class=".btn">#1745</a>
            </td>
            <td>
                <b>
                    [fabric] Fix usage of roottoken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add delete/k8s_secrets role
- Fix root-token usage
- Fix usage of reviewe-role for the vault-kubernetes job

 

**Reviewed by**
@jagpreetsinghsasan @suvajit-sarkar 

 

**Linked issue**
Resolves #1730 #1638 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 15:10:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1742" class=".btn">#1742</a>
            </td>
            <td>
                <b>
                    [ci skip] Added gateway chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add gateway chart

 

**Reviewed by**
@sownak @jagpreetsinghsasan 

 

**Linked issue**
#1507 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 11:46:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1741" class=".btn">#1741</a>
            </td>
            <td>
                <b>
                    [skip ci] Added auth chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add helm chart for auth service
- Update pki job to create auth trust store

**TODO**
Creds for the crypto materials needs to fetch vault and replaced
JWT creation can be moved to PKI job

 

**Reviewed by**
@sownak @jagpreetsinghsasan 

 

**Linked issue**
#1506 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 05:56:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1740" class=".btn">#1740</a>
            </td>
            <td>
                <b>
                    [corda-ent] created ansible roles for the CENM Auth service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Added an ansible role for the Auth service and an Auth tpl file for its automation
- Updated the Ansible setup/cenm role to include a task for the deployment of the Auth service

 

**Reviewed by**
@suvajit-sarkar @sownak 

 

**Linked issue**
#1726 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 11:10:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1739" class=".btn">#1739</a>
            </td>
            <td>
                <b>
                    [quorum] Fixed raft errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Fix generic RAFT errors


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 17:25:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1737" class=".btn">#1737</a>
            </td>
            <td>
                <b>
                    [corda-ent] Added the helm chart and dockerfile for CENM Zone service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: surabhi-dudhediya <surabhi.dudhediya@accenture.com>

**Changelog**
- Add helm chart and dockerfile for CENM Zone service

**Reviewed by**
@suvajit-sarkar @jagpreetsinghsasan @sownak 

 

**Linked issue**
#1735 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 11:24:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1736" class=".btn">#1736</a>
            </td>
            <td>
                <b>
                    [quorum] Added new tables for sql db tessera
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: alvaropicazo <alvaro.picazo.haase@accenture.com>

**Changelog**
- Added new tables creation which fix some sql tables missing errors logs in tessera node chart

**Linked issue**
#1551 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 17:00:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1733" class=".btn">#1733</a>
            </td>
            <td>
                <b>
                    [shared] Fixed docs formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sownak Roy <sownak.roy@accenture.com>

**Changelog**
- Fix formatting error for docs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 17:00:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1732" class=".btn">#1732</a>
            </td>
            <td>
                <b>
                    [shared] Fix docutils so readthedocs don't fail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Fix readthedocs build
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 16:44:01 +0000 UTC
    </div>
</div>

