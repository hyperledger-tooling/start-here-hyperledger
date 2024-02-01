---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    Speed up docker (re-)build by caching pip cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With warm pip-caches this did reduce docker build time on my laptop in WSL by more than half ...

BTW: mounting a pip-cache volume (`docker run -v $(DOCKER_DIR)/cache/pip:/project/pdo/.cache/pip ...`) also sped up ever more greatly testing of inference contract given the homogenously sized tensorflow packages ... 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 01:33:38 +0000 UTC
    </div>
</div>

