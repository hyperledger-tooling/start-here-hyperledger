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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    Upgrade docker images from 20.04 to 22.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Title mostly says it all.  Main trigger was that client docker image had too old a `cmake`  ("thanks" to a 1/16 change) to build contracts in `pdo-contracts`.  That said, 20.04 of course is also a bit dated and EOL if in a year.

Tested by running the usual `make test` here and by mounting `pdo-contracts` into a client container and then run `make test` in it (which admittedly initially failed in the inference tests but that was due to the guardian requiring an `apt install libgl1 libcudart11.0` to work properly!   After running that `make test` also worked for pdo-contracts => _Q: should we add these dependencies also to pdo_client.dockerfile?_)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 03:59:49 +0000 UTC
    </div>
</div>

