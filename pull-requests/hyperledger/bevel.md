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
                PR <a href="https://github.com/hyperledger/bevel/pull/2109" class=".btn">#2109</a>
            </td>
            <td>
                <b>
                    [besu] ability to pass custom chain ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Added the feature to pass custom chain ID in the besu network. The default value for the chainID is `2018`
- Updated the required playbooks to accept custom chain ID 

chainID can be passed as
```
network:
   config:
     chain_id: 2018
```
 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#2105 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 17:08:19 +0000 UTC
    </div>
</div>

