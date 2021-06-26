---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Better error message for missing mspid connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When mspid is missing in connection yaml , the sdk gives a slightly misleading error message - "No client organization defined in the config" (which implies client.org is not been defined in connection.yaml) . We can give a better  error message to imply that mspid is missing - No mspid defined in the config for Org1

-------------------example wrong config-----------
name: voterNet-investorOrg
version: 1.0.0
client:
  organization: investorOrg
  connection:
    timeout:
      peer:
        endorser: '300'
organizations:
  investorOrg:    (mspid missing)
    peers:
    - peer0.investorOrg.voternet.com
    certificateAuthorities:
    - ca.investorOrg.voternet.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-26 12:30:26 +0000 UTC
    </div>
</div>

