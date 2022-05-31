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
                PR <a href="https://github.com/hyperledger/bevel/pull/1959" class=".btn">#1959</a>
            </td>
            <td>
                <b>
                    [fabric] Fix for helm operator to fetch chart from private git repo using https
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This resolves the issue of bevel network failing with private git repositories. 

**Reason for the failures:** 
- flux-helm-operator wasn't configured used/configured correctly with git credentials. So, it was not able to fetch the charts from the private git repo as defined under the `chart:`  section of the value file. 

**Fix:**
- Create a kubernetes secret which has the git credentials stored inside the variables: `username` and `password` (within each of the organization namespaces respectively)
- Add `secretRef:` field in the value files and refer the above mentioned secret.

**Doc Reference:** https://fluxcd.io/legacy/helm-operator/helmrelease-guide/chart-sources/#https

Signed-off-by: Prasanth Sundaravelu <prasanth.s@spydra.app>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 15:50:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1958" class=".btn">#1958</a>
            </td>
            <td>
                <b>
                    [chore]Develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add
- Fix
- Update

 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 11:15:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1957" class=".btn">#1957</a>
            </td>
            <td>
                <b>
                    [chore] updated package-lock.json file for corda images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Update package-lock.json file for networkmap website

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 03:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1956" class=".btn">#1956</a>
            </td>
            <td>
                <b>
                    [fabric]  Add orderer/peer update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**

- Update platforms/hyperledger-fabric/configuration/add-orderer.yaml and platforms/hyperledger-fabric/configuration/add-peer.yaml: 

 

**Reviewed by**
@suvajit-sarkar
@jagpreetsinghsasan

 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 15:54:35 +0000 UTC
    </div>
</div>

