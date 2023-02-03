---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2109" class=".btn">#2109</a>
            </td>
            <td>
                <b>
                    Update dockerfiles to use python 3.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Per comments in https://github.com/hyperledger/aries-cloudagent-python/pull/2105
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 19:41:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2105" class=".btn">#2105</a>
            </td>
            <td>
                <b>
                    Updating base images from slim-buster to slim-bullseye
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Creating this PR to update the base docker images from `slim-buster` to `slim-bullseye` version as the slim-buster image is reported to have known vulnerabilities identified by scanning tools like Snyk and Qualys. This relates to #2087 where this is discussed.

Signed-off-by: pradeepp88 <pradeep.prakasam@ontario.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 21:17:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2103" class=".btn">#2103</a>
            </td>
            <td>
                <b>
                    Delete tail files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Creating this PR to add an endpoint to delete the tails file based on cred_def_id or rev_reg_id under revocation protocol. This is done to clean up the local tails file after uploading it to tails server. Looking for the feedback from the community.
-Signed off by: ramreddychalla94 <ram.challa@ontario.ca>
-Funded by the Ontario Government

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 18:29:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2099" class=".btn">#2099</a>
            </td>
            <td>
                <b>
                    fix: fix connection timing bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an interesting bug that occurs under load in aca-py. It appears that on receive connection for a multi-use invitation, that we copy the object. The problem is for a short time the original search that takes places to find the multi-use invitation matches both the original and the copy. If this occurs, Aca-Py throws an un-caught error indicating that two connections records for the invitation were found. By setting Request on the clone object, this condition is avoided.

Signed-off-by: Kim Ebert <kim@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 18:32:45 +0000 UTC
    </div>
</div>

