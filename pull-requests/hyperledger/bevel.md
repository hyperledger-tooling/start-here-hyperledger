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
                PR <a href="https://github.com/hyperledger/bevel/pull/2192" class=".btn">#2192</a>
            </td>
            <td>
                <b>
                    [besu] fixed the helm ansible module for TLS cert creation using cert manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                changes:
Removed the helm module while creation of TLS cert by cert manager because we are deploying helm chart using shell module
changed the order of organization.issuer to check if it is defined/undefined and then to check the value if it is default/letsencrypt instead of first checking value and then checking if it is defined

Reviewers:
@suvajit-sarkar @sownak @jagpreetsinghsasan 

Fixes:
hotfix
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 11:31:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2190" class=".btn">#2190</a>
            </td>
            <td>
                <b>
                    [chore] Merge Develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                commit_title
   - Add
   - Fix
   - Update 

Fixes #issue_number

---
**Example (for reference only)**:   

feat(fabric): support for v2.2.3
  - Add platforms/hyperledger-fabric/charts/commit_chaincode chart
  - Add platforms/hyperledger-fabric/charts/approve_chaincode
  - Update platforms/hyperledger-fabric/configuration/deploy-network.yaml  

Fixes #000
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 16:01:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2189" class=".btn">#2189</a>
            </td>
            <td>
                <b>
                    [indy] change indy image names in code to match with ghcr.io
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                change indy image names in code to match with ghcr.io
   - Update indy image names

Fixes #2188 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 11:17:18 +0000 UTC
    </div>
</div>

