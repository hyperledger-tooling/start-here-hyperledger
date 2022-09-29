---
layout: default
title: minifabric
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minifabric
---

# minifabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minifabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/357" class=".btn">#357</a>
            </td>
            <td>
                <b>
                    Added deploynodes operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                User can now deploy nodes with a new deploynodes operation. The user must first place their node manifest files into the vars/nodespecs directory before deploying. The operation will search for CA manifest files and deploy those first before deploying the other nodes. 

Also adds missing help messages for deployoperator operation and --target-environment option. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 00:37:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/356" class=".btn">#356</a>
            </td>
            <td>
                <b>
                    Error fix for older versions missing TARGET_ENV in its envsettings file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sets TARGET_ENV to DOCKER when TARGET_ENV is not set from envsettings.

Because Ansible extra variables have the highest precedence and cannot be overwritten, we name the extra var (TARGET_ENVIRONMENT) differently than our local var (TARGET_ENV) so that we are able to change the value of our local var later if necessary. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 19:22:21 +0000 UTC
    </div>
</div>

