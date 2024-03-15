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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/477" class=".btn">#477</a>
            </td>
            <td>
                <b>
                    Fixes for making PDO work in SGX HW-mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR continues the work in #463 to enable tests in SGX HW-mode, and makes the following contributions.

1. this PR passes the `SGX_MODE` variable to the docker builds. This is necessary when we build the services. Also, since we set the relative env var in the docker file, the env var persists in the image, so later test containers run directly in HW mode.

2. This PR moves the enclave signing key to `/tmp/` to fix the build process. The reason is that `environment.sh` sets `PDO_SGX_KEY_ROOT` to a folder within the XFER folder, but the XFER is not available during a docker build (it's docker compose that later mounts that). This is a problem during the service build, because PDO uses that folder to store the enclave signing key. Since the key is ephemeral for now, this PR moves it in the temp folder.

3. This PR fixes the tests in HW mode by making docker compose mount the appropriate SGX-related volumes and devices on the host.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 19:58:59 +0000 UTC
    </div>
</div>

