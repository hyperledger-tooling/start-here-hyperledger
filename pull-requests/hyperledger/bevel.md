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
                PR <a href="https://github.com/hyperledger/bevel/pull/2382" class=".btn">#2382</a>
            </td>
            <td>
                <b>
                    bug(r3cordaos) vault k8s release files not getting removed on reset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Fix**
- Doorman, NMS and notary vault k8s release files will be created under the org name folder, which is deleted on reset.
- Added missing variables in `setup vault kubernetes` task, in add-new-channel playbook.
- Removed service account and clusterolebinding checks. This fixes nms and notary vault k8 jobs getting skipped.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 08:17:05 +0000 UTC
    </div>
</div>

