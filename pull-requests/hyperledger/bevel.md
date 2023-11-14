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
                PR <a href="https://github.com/hyperledger/bevel/pull/2428" class=".btn">#2428</a>
            </td>
            <td>
                <b>
                    update repo readme file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change log**
- New bevel overview image
- Removed contributor section
- Added more details in scope section 

TODO: Update the platform specific images
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 05:54:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2427" class=".btn">#2427</a>
            </td>
            <td>
                <b>
                    [r3-corda-ent)] fix chart name and linting issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**bug(r3-corda-ent): fix chart name and linting issue**

```
Fixed the chart name at following locations:
- Ansible role.
- Template file (.tpl) file.
- Helm Chart name itself.

Linting issue:
- Fixed for the "corda-ent-node" Helm chart.
```

fixes: quick-fixes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 13:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2426" class=".btn">#2426</a>
            </td>
            <td>
                <b>
                    hot fix: workflow dispatch options
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
        Created At 2023-11-08 20:38:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2423" class=".btn">#2423</a>
            </td>
            <td>
                <b>
                    update: chart name and version changes 
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
        Created At 2023-11-08 13:30:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2422" class=".btn">#2422</a>
            </td>
            <td>
                <b>
                    [fabric] Fix playbook add organization 2.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
Removed the platforms/hyperledger-fabric/configuration/roles/create/new_organization/syschannel_block role. Since this playbook is used to add a peer organization. To set up an orderer type organization, the add-orderer-organization.yaml playbook will be executed. Therefore it never runs.


fixes #2399
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 11:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2421" class=".btn">#2421</a>
            </td>
            <td>
                <b>
                    [shared] ensure elasticIp is available
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## **Commit to be reviewed**

---

### **bug(shared): ensure elasticIp is available**

- #### A when condition has been added to ensure that elasticIp is only fetched when it is actually available.

#### fixes: quick-fix
---
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 10:09:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2420" class=".btn">#2420</a>
            </td>
            <td>
                <b>
                    chart name refactoring
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
        Created At 2023-11-07 17:39:05 +0000 UTC
    </div>
</div>

