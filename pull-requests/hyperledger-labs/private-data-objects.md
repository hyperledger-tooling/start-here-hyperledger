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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/460" class=".btn">#460</a>
            </td>
            <td>
                <b>
                    Update package dependencies: WAMR, WASI SDK, and parson
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is not quite as simple as expected. With our
default configuration (LIBC on, WASI off) there are a couple errors in WAMR. Namely that os_is_handle_valid is not defined in sgx-platform.c and there is an include of libc_errno.h that appears to be outside the check for WASI includes.

Changes were made to work around these problems. Namely we explicitly include the libc header & source. And we add a file that defines the missing function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 19:18:03 +0000 UTC
    </div>
</div>

