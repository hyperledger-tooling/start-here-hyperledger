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

