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
                PR <a href="https://github.com/hyperledger/fabric/pull/4328" class=".btn">#4328</a>
            </td>
            <td>
                <b>
                    fix: missing tag for make docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Fix missing tag for `make docker`
#### Type of change

- Bug fix

#### Description

When `make docker` make file is miss the tag. So, `make docker-tag-latest` and `make docker-tag-stable` will not work

#### Additional details

Reproduce: run `make docker-tag-latest` or `make docker-tag-stable` after run `make docker`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 14:24:34 +0000 UTC
    </div>
</div>

