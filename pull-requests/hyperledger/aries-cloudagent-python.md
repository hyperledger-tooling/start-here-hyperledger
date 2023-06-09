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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2255" class=".btn">#2255</a>
            </td>
            <td>
                <b>
                    Resolve definitions.py fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Include searching by the module base package when resolving plugin definitions location.

Fixes #2224 

This still depends on the module package names and file system paths matching up, which is not guaranteed. But without adding additional configuration in the plugin registry, I think this is all we can do.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 22:56:19 +0000 UTC
    </div>
</div>

