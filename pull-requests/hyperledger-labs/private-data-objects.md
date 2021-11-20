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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    add to wawaka native functions to verify sgx attestation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Add native functions to Wawaka that allow for a report to be verified. This means that we can write contracts that establish an attested connection to services hosted in other enclaves. For example, we should be able to build a secure channel to a service hosted in Gramine.

A couple other cleanups where necessary to make this work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 23:27:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    Updates to cmake files and wawaka benchmarks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces two main updates:
- Bump the minimum required cmake version to 3.10 throughout the CMakeLists.txt files in the codebase (cmake 3.10 is the default in Ubuntu 18.04)
- Update the wawaka benchmarks to build with clang-wasi 

This PR supersedes #334 .


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 22:52:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    Fix secp256k1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The build fails due to a recent update to the secp256k1 API which is used for Sawtooth.
We stick for now to the original old version.

Signed-off-by: Bruno Vavala <bruno.vavala@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 00:56:12 +0000 UTC
    </div>
</div>

