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
                PR <a href="https://github.com/hyperledger/bevel/pull/1962" class=".btn">#1962</a>
            </td>
            <td>
                <b>
                    [chore] merge develop on feature/flux-v2
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
        Created At 2022-05-31 13:03:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1961" class=".btn">#1961</a>
            </td>
            <td>
                <b>
                    [indy] update image pull policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

- Update image pull policy to IfNotPresent


 

**Linked issue**
#1885 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 12:47:35 +0000 UTC
    </div>
</div>

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

