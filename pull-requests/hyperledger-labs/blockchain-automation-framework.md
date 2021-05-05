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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1441" class=".btn">#1441</a>
            </td>
            <td>
                <b>
                    create namespace for flux deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jose <pppazos@gmail.com>

**Changelog**
- Add namespace for flux  named as flux-<environment>
- Create flux inside new namespace
- Delete namespace on reset playbooks for all networks

 

**Reviewed by**


 

**Linked issue**
1292

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 12:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1439" class=".btn">#1439</a>
            </td>
            <td>
                <b>
                    [shared] changes for ssh only git
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Use only SSH for gitops and well as ansible controller
- Update molecule tests to run on Kubernetes 1.16 and Vault 1.7.0

**Linked issue**
resolves #876 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 14:56:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1438" class=".btn">#1438</a>
            </td>
            <td>
                <b>
                    [corda-ent] ambassadorv2 upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sownak.roy <sownak.roy@accenture.com>

Ambassador V2 changes for corda enterprise
 

**Linked issue**
Resolves #1287 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 09:43:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    [ fabric ]bug resolve for removeOrg in DR scenario
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kumar, D. bd <d.bd.kumar@accenture.com>

- Fix bug removing an org in DR

 

**Reviewed by**
@alvaropicazo 

 

**Linked issue**
#1408 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 08:51:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1436" class=".btn">#1436</a>
            </td>
            <td>
                <b>
                    latest develop to feature merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                latest develop to feature merge
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 17:58:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1435" class=".btn">#1435</a>
            </td>
            <td>
                <b>
                    [corda] fix networkmap frontend for Opensource Corda
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix networkmap frontend
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 17:38:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1434" class=".btn">#1434</a>
            </td>
            <td>
                <b>
                    [fabric] Updated condition for not creating a channel when adding a new peer t…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …o an existing creator org

Signed-off-by: alvaropicazo <alvaro.picazo.haase@accenture.com>

**Changelog**
- Fix condition when adding a new peer to an existing creator org, for not running the create channel task as it is not wanted in that case. Now it will only be run if the participant.type is a creator AND the org_status is not defined or it is new.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 14:08:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1433" class=".btn">#1433</a>
            </td>
            <td>
                <b>
                    Updated Roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Update roadmap

 

**Reviewed by**
@sownak 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 09:51:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1432" class=".btn">#1432</a>
            </td>
            <td>
                <b>
                    added default molecule tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Added molecule test for default scenario

 

**Reviewed by**
@suvajit-sarkar @deepakkumardbd @jagpreetsinghsasan 

 

**Linked issue**
#718 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 09:47:51 +0000 UTC
    </div>
</div>

