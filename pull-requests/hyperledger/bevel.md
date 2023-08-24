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
                PR <a href="https://github.com/hyperledger/bevel/pull/2351" class=".btn">#2351</a>
            </td>
            <td>
                <b>
                    feat(shared): Simplifying storage class creation with helm module 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request addresses to refactor the current implementation of creating helm releases using GitOps to a more flexible approach by leveraging the ansible helm module and moving the creation of storage class roles to a share folder.

The six platforms that have been modified to make them compatible with the shared "storage class" charts and roles are:
   • Hyperledger-Besu
   • Hyperledger-Fabric
   • R3-corda
   • R3-corda-Ent
   • Quorum
   • Hyperledger- Indy

Changes Made:

Instead of using gitOps to create helm release, used helm module from ansible by creating jinja(j2) template. Moved the creation of storage class roles to a shared folder to use them across all the platforms.

Fixes: #2306
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 15:05:34 +0000 UTC
    </div>
</div>

