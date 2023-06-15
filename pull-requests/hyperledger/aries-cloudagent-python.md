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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2268" class=".btn">#2268</a>
            </td>
            <td>
                <b>
                    Create .readthedocs.yaml file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add readthedocs YAML file as required by RTD.  Per this [blog post](https://blog.readthedocs.com/migrate-configuration-v2/), this file is now required for publishing the type of documentation we generate to the RTD sites. For those not aware, here is the link to the RTD site for ACA-Py -- https://aries-cloud-agent-python.readthedocs.io

Here is the link to the version of the docs generated from this branch with this new file: https://aries-cloud-agent-python.readthedocs.io/en/swcurran-add-rtd/. LGTM!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 23:43:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2267" class=".btn">#2267</a>
            </td>
            <td>
                <b>
                    Add devcontainer for ACA-Py
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addressing an issue where it is difficult to get set up to debug and begin coding by adding a devcontainer.

See Issue #2251 - this is only one small part of developer documentation. I wanted this out for feedback while we identify other areas of concern.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 23:36:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2265" class=".btn">#2265</a>
            </td>
            <td>
                <b>
                    Allow awaiting in verification key strategy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #2235 has just been merged, but I realized that having a non-async function could be too restrictive. For example, accessing storage with the current function's signature is hard. 

This PR fixes this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 14:08:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2263" class=".btn">#2263</a>
            </td>
            <td>
                <b>
                    Propose adding Jason Sherman usingtechnology as a Maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 22:37:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2262" class=".btn">#2262</a>
            </td>
            <td>
                <b>
                    feat(did creation route): reject unregistered did methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change a small oversight in did creation admin route:

* Missing `method` parameter will default to `sov`
* Unknown (ie: not registed in `DIDMethods`) methods will be rejected
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 10:39:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2261" class=".btn">#2261</a>
            </td>
            <td>
                <b>
                    Assign ~thread.thid with thread_id value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The previous assignment used a value from a field that had not been assigned yet. So, use the correct `thread_id` value for the `thid`.

Fixes #2259 

The fix originally discussed in #2259 is too aggressive and after reviewing the code it is clear that there can be empty `~thread` and they are expected to be dealt with by the receiver.  In this case, we were attempting to set the `thid` but just using an unassigned value.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 00:07:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2260" class=".btn">#2260</a>
            </td>
            <td>
                <b>
                    Release 0.8.2-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 18:24:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2258" class=".btn">#2258</a>
            </td>
            <td>
                <b>
                    Updating Maintainers list to be accurate and using the TOC format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 17:14:56 +0000 UTC
    </div>
</div>

