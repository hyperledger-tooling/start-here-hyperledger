---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/808" class=".btn">#808</a>
            </td>
            <td>
                <b>
                    unit tests for credential_schema::Schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixes #775 
- added tests for the functions `to_string_versioned`, `from_string_versioned`, `get_schema_id` 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 12:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/806" class=".btn">#806</a>
            </td>
            <td>
                <b>
                    Move post_message to shared_vcx  #772
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue #772 - Move out post_message to shared_vcx

Move the code to shared_vcx instead
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 10:36:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    Release 0.54.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 06:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    Regression: Fix dependency tree when using aries_vcx_core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                apologies, I should have manually checked this when approving the core PR.

But since the aries_vcx_core crate was being pulled in without opting out of default features, this means that the aries_vcx crate now has no way to opt-out of depending on vdrtools.

This fix addresses that regression whilst keeping vdrtools as the default flag (should not affect consumers who are happy with the default vdrtools flag)


I also fix some of regressions in certain indy elements which should remain to be hidden behind the vdrtools.

also added a CI step to check the aries_vcx compiles with some of the common feature flags
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 22:15:51 +0000 UTC
    </div>
</div>

