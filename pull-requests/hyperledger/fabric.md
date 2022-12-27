---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3882" class=".btn">#3882</a>
            </td>
            <td>
                <b>
                    Switch base docker image from golang-alpine to ubuntu:20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

This PR switches the Fabric base docker images from golang-alpine to ubuntu:20.04.  The upgrade is necessary as the golang-alpine libc runtimes (musl) are incompatible with the requirements on multi-arch runtimes. 

The motivations for this upgrade are described in detail in Discussion #3876 and comments in DRAFT PR #3877 


#### Additional details

- Discussion #3876 
- PR #3877  (DRAFT)


#### Related issues

- #2994
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 15:00:25 +0000 UTC
    </div>
</div>

