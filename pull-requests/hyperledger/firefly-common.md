---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    feat: Add mTLS configuration for ffresty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding the ability to supply a config to the ffresty client to setup TLS and mTLS.

**NOTE** This changes the interface of that init function to now return an error as well, so every consumer of this library and that client on update will need to handle that error. We could avoid doing this by allowing the user to provide a TLS Config as an argument but the pattern seems to be to provide viper config!

For testing I added a series of real and fake certificates and keys. I also explore standing up an mTLS mock server with the `httptest` but it proved cumbersome. I think validating that the correct certificates are added to the TLS Config should be good enough but happy to rectify
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 10:03:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    Add "networkName" and "published" to FFI fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These will be needed as part of https://github.com/hyperledger/firefly/issues/1220, based on its current trajectory. See notes there for an overview of plans and unanswered questions.

The argument could be made that these fields may or may not belong in the base `fftypes.FFI` struct, and that some of this info is metadata specific to the functionality in FireFly core, and that perhaps the FFI type should be wrapped there. That would generate more work, but I wasn't sure how "pure" we want to be about adding extra fields to this struct.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 21:03:21 +0000 UTC
    </div>
</div>

