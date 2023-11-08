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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2419" class=".btn">#2419</a>
            </td>
            <td>
                <b>
                    New Document Restructure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Base theme changed along with light/dark toggle
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 11:21:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2418" class=".btn">#2418</a>
            </td>
            <td>
                <b>
                    feat(shared): Implement GitHub Spellcheck and grammar linting for Pull request.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
This pull request implements the GitHub Spellcheck feature to automatically check the spelling and grammar in commit messages for all Pull Requests (PRs).

Changes Made:
- Added GitHub Spellcheck and grammar linting integration to the repository
- Configured the spellcheck tool to check commit messages in PRs
- Configured the language tool for grammar linting.

Fixes: #2327
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 08:59:30 +0000 UTC
    </div>
</div>

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

