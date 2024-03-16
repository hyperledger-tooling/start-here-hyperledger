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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    Make SGX registration a bit more robust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Handle missing SGX verification status CONFIGURATION_AND_SW_HARDENING_NEEDED
* Honor PDO_LOG_LEVEL in registration script

Note this is tested on top if (2024-03-15) version of PR #477, so for now still "inherits" also Bruno's commit from that PR.  Once PR#477 is closed i will rebase this one and  "undraft" it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 18:00:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    Provide PDO_SOURCE_ROOT default for docker to allow zero-config build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor change to allow docker builds out-of-the-box without any configuration/environment variable definition.  This default for PDO_SOURCE_ROOT also hides an error for undefined `PDO_SOURCE_ROOT` which is _very_ unintuitive to figure out if you haven't run into this issue beforehand.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 01:42:45 +0000 UTC
    </div>
</div>

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

2. This PR fixes the tests in HW mode by making docker compose mount the appropriate SGX-related volumes and devices on the host.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 19:58:59 +0000 UTC
    </div>
</div>

