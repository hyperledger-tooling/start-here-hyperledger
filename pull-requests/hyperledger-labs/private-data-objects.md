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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    Remove templates & make IAS certificate generation more robust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace the template expansion that is causing periodic file corruption errors with a more resilient method for downloading the IAS certificate. This approach removes the template completely and uses a file system move to atomically update the certificate
file.

Also uses the cmake clean to remove any generated files. We were leaving extra files in the common directory tree.

This should be an addition to PR #457 to add one more level of resilience. 

If you are running in HW mode inside a firewall that does not correctly proxy the IAS certificates URL, there is a new environment variable PDO_FORCE_IAS_PROXY that can be set to "true" to force use of the configured proxy (that is,
it overrides NO_PROXY).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 16:36:56 +0000 UTC
    </div>
</div>

