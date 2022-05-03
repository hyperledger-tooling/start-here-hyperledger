---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Point ERC20/ERC721 connector at deployed contract address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This includes multiple changes to how the `docker-compose.yml` file is handled:

* `docker-compose.yml` has moved back up to the root directory of the stack (instead of being placed in "init" and "runtime" subfolders). A simple migration check will copy it out of "runtime" into the parent folder if needed.
* The `docker-compose.yml` file will now be rewritten after first-time setup is complete. This allows it to pick up on new things such as deployed contracts. It is notated at the top with comments indicating it is a generated file and should not be edited.
* For overriding Docker configuration values, users are now directed to edit a `docker-compose.override.yml` file, as [supported by docker-compose](https://docs.docker.com/compose/extends).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 16:50:17 +0000 UTC
    </div>
</div>

