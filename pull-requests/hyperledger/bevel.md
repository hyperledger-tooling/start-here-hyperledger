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
                PR <a href="https://github.com/hyperledger/bevel/pull/2415" class=".btn">#2415</a>
            </td>
            <td>
                <b>
                    [fabric] Fix playbook add organization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1.Added /setup/scripts role in playbook
2.Fixed undefined variables
3.FIxed creation of configtx.yaml

Modifications
-----------------------
platforms/hyperledger-fabric/configuration/add-organization.yaml 
platforms/hyperledger-fabric/configuration/roles/create/configtx/templates/configtxOrderer_default.tpl 
platforms/hyperledger-fabric/configuration/roles/k8_component/templates/existing_peer_cli.tpl

fixes #2412

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 10:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2414" class=".btn">#2414</a>
            </td>
            <td>
                <b>
                    update release_chart workflow and roadmap
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
        Created At 2023-11-06 09:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2413" class=".btn">#2413</a>
            </td>
            <td>
                <b>
                    [substrate] replace ansible roles readme with inline code comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(substrate): replace ansible roles readme with inline code comments**

```
This PR enhances the readability and understanding of our roles by adding comment messages throughout the code.

Changes:
- Added clear and concise comment messages in ansible roles.
- Maintained proper code indentation for increased code reliability.
- Removed the roles' Readme.md if it existed.
```

fixes #2326
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 11:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2411" class=".btn">#2411</a>
            </td>
            <td>
                <b>
                    [indy] replace ansible roles readme with inline code comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(indy): replace ansible roles readme with inline code comments**

```
This PR enhances the readability and understanding of our roles by adding comment messages throughout the code.

Changes:
- Added clear and concise comment messages in ansible roles.
- Maintained proper code indentation for increased code reliability.
- Removed the roles' Readme.md if it existed.
```

fixes #2326
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 10:01:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2410" class=".btn">#2410</a>
            </td>
            <td>
                <b>
                    upgrade(hyperledger-indy): ambassador to ambassador edge stack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR will provide the support of using latest ambassador edge-stack

changes:
• Updated all services to use the latest Ambassador Edge Stack routing rules.

fixes https://github.com/hyperledger/bevel/issues/2359
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 19:23:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2409" class=".btn">#2409</a>
            </td>
            <td>
                <b>
                    [shared] flux installation bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------

1. flux installation based on the context specified at org level.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 17:32:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2408" class=".btn">#2408</a>
            </td>
            <td>
                <b>
                    [fabric] replace ansible roles readme with inline code comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---
**feat(fabric): replace ansible roles readme with inline code comments**

```
This PR enhances the readability and understanding of our roles by adding comment messages throughout the code.

Changes:
- Added clear and concise comment messages in ansible roles.
- Maintained proper code indentation for increased code reliability.
- Removed the roles' Readme.md if it existed.

Additional changes:
- Deleted storageclass ansible role as we already migrated it to the shared platform.

```
fixes #2326
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 12:32:51 +0000 UTC
    </div>
</div>

